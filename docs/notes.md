\newpage


# CPU information

-   `lscpu` &rarr; human readable version of `less /proc/cpuinfo`

-   check if turbo is enabled

```shell
grep flags /proc/cpuinfo | grep -q " ida " && echo Turbo mode is on || echo Turbo mode is off
```


# Benchmarks

-   `yes` &rarr; output a string repeatedly until killed
-   [memhog.c](resources/memhog.c) &rarr; in [numactl](http://developer.amd.com/wordpress/media/2012/10/LibNUMA-WP-fv1.pdf) (**memory-bound**)
    
    Ex.: called with `memhog -r1000 1G` allocates 1G of memory and write 0xff in each byte &times; 8
    
    Result: `memhog -r1000 1G 99.07s user 2.54s system 99% cpu 1:41.95 total`


## Binding one task to a single CPU

-   In shell: `taskset`
-   In C: `sched_setaffinity`

Example script:

```bash
#!/bin/bash
taskset --cpu-list 2 memhog -r20 1G &
MEMHOG_PID=$! # last background process pid
sleep 1
taskset --pid --cpu-list 3 $MEMHOG_PID
```


## Monitoring performance


### Performance counters

*Definition:* Performance counters are CPU hardware registers that count hardware events such as instructions executed, cache-misses suffered, or branches mispredicted. They form a basis for profiling applications to trace dynamic control flow and identify hotspots ([perf wiki](https://perf.wiki.kernel.org/index.php/Main_Page)).

-   perf list: events list
-   perf record: record events for later reporting
-   perf report: break down events by process, function, etc.
-   perf annotate: annotate assembly or source code with event counts
-   perf top: see live event count
-   perf bench: run different kernel microbenchmarks
-   perf stat: obtain event counts
    -   `perf stat -a -I1000 --per-socket -e power/energy-pkg/` &rarr; shows power drained per second (-I1000 = 1000 millisec). Launch it and then start a benchmark. Tested with `yes > /dev/null`: 1-2 Joule &rarr; 6-7 Joule

```shell
perf list | grep msr
```

    msr/aperf/                                         [Kernel PMU event]
    msr/irperf/                                        [Kernel PMU event]
    msr/mperf/                                         [Kernel PMU event]
    msr/tsc/                                           [Kernel PMU event]


### Performance counter (advanced) and MSR reading

*[turbostat](resources/turbostat.c)*: reads Intel CPU&rsquo;s stats


### MSR

Available trace points: `/sys/kernel/debug/tracing/events/msr/`

```shell
ls -l /sys/kernel/debug/tracing/events/msr/
```

    total 0
    -rw-r--r-- 1 root root 0 Jun 22 09:17 enable
    -rw-r--r-- 1 root root 0 Jun 22 09:17 filter
    drwxr-xr-x 2 root root 0 Jun 22 09:17 rdpmc
    drwxr-xr-x 2 root root 0 Jun 22 09:17 read_msr
    drwxr-xr-x 2 root root 0 Jun 22 09:17 write_msr

Trace MSR reads:

-   read\_msr
    -   msr: MSR number
    -   val: Value written
    -   failed: 1 if the access failed, otherwise 0

Trace MSR writes:

-   write\_msr
    -   msr: MSR number
    -   val: Value written
    -   failed: 1 if the access failed, otherwise 0

Intel&rsquo;s documentation on package level thermal management [here](docs/Intel64 and IA-32 Architectures Software Developers Manual Volume 3B System Programming Guide, Part 2.pdf).

Passive cooling (frequency throttling) should be driven by measuring (a) the core and package temperatures, or (b) only the package temperature. If measured package temperature led the power management agent to choose which core to execute passive cooling, then all cores need to execute passive cooling. Core temperature is measured using the IA32\_THERMAL\_STATUS and IA32\_THERMAL\_INTERRUPT MSRs. The exact implementation details depend on the platform firmware and possible solutions include defining two different thermal zones (one for core temperature and passive cooling and the other for package temperature and active cooling).

1.  rdmsr/wrmsr

    *[rdmsr](resources/msr-tools/rdmsr.c)*: is a tool used for reading a CPU&rsquo;s machine specific registers (MSR), [man page](https://manpages.ubuntu.com/manpages/hirsute/en/man1/rdmsr.1.html).
    
    ```shell
    rdmsr -h
    ```

2.  HWP

    -   intel foss driver code [here](https://code.woboq.org/linux/linux/drivers/cpufreq/intel_pstate.c.html#intel_pstate_request_control_from_smm)
    -   [Cutress, Ian: The Intel Skylake Mobile and Desktop Launch, with Architecture Analysis (2015)](https://www.anandtech.com/show/9582/intel-skylake-mobile-desktop-launch-architecture-analysis/7)
    -   [Howse, Brett: Examining Intel’s New Speed Shift Tech on Skylake: More Responsive Processors](https://www.anandtech.com/show/9751/examining-intel-skylake-speed-shift-more-responsive-processors)
    -   [Intel: Intel 64 and IA-32 Architectures Software Developer’s Manual, Vol 3, chap. 14, sec. 4](https://software.intel.com/en-us/articles/intel-sdm) (vedere: PPERF, Productive Performance)
    -   <https://beta.suse.com/private/ggherdovich/sugov/sugov-2020-paper.pdf>
    -   [cpufreq](https://beta.suse.com/private/ggherdovich/cpufreq/x86-cpufreq.png) discusso anche [qua](https://www.youtube.com/watch?v=OPWoj_xgkBA)
    -   [vulnerabilites](docs/vulnerabilites.pdf)


### C-states

C-State residencies are collected from hardware and/or the operating system (OS). For systems that collect OS C-State residencies, CPU C-states are core power states requested by the Operating System Directed Power Management (OSPM) infrastructure that define the degree to which the processor is &ldquo;idle&rdquo;. For systems that collect hardware C-State residencies, CPU C-States are obtained by reading the processor’s MSRs which count the actual time spent in each C-State. C-States range from C0 to Cn. C0 indicates an active state. All other C-states (C1-Cn) represent idle sleep states where the processor clock is inactive (cannot execute instructions) and different parts of the processor are powered down. As the C-States get deeper, the exit latency duration becomes longer (the time to transition to C0) and the power savings becomes greater.

`cat /sys/module/intel_idle/parameters/max_cstate` max allowed C-states for a CPU


### P-states

-   [Intel&rsquo;s manual on P-states (APERF, MPERF)](docs/Intel64 and IA-32 Architectures Software Developers Manual Volume 3B System Programming Guide, Part 2.pdf)
-   [HWP](docs/Intel64 and IA-32 Architectures Software Developers Manual Volume 3B System Programming Guide, Part 2.pdf)


### C-states VS P-states

C-states are idle states and P-states are operational states. This difference, though obvious once you know, can be initially confusing.

With the exception of C0, where the CPU is active and busy doing something, a C-state is an idle state. Since an idle CPU isn&rsquo;t doing anything (i.e. any useful work), why not shut it down? No one is going to notice since there&rsquo;s no one using it. (Letting a CPU run at full bore when idle is like driving in circles very fast; all you&rsquo;re doing is going nowhere quickly.)

A P-state is an operational state, meaning that the core / processor can be doing useful work in any P-state. The most obvious example is when your laptop is using a low power profile and operating on battery. The OS will lower the C0 operating frequency and voltage, i.e. enter a higher P-state. Reducing the operating frequency reduces the speed at which the processor operates, and so the energy usage per second (i.e. power). Reducing the voltage decreases the leakage current from the CPU&rsquo;s transistors, making the processor more energy efficient resulting in further gains. The net result is a significant reduction in the energy usage per second of the processor. On the flip side, an application will take longer to run. This may or may not be a problem from a power perspective. I&rsquo;ll talk about this issue in some depth in a later blog.

\newline

C-states and P-states are also orthogonal. This is a fancy mathematical term meaning that each can vary independently of the other. This doesn&rsquo;t mean that in the higher C-states, the voltage doesn&rsquo;t change. It only means that when you resume C0, you go back to the operating frequency and voltage defined by that P-state.

The intel\_pstate driver running in one of the active modes doesn&rsquo;t allow you to set a particular frequency directly (cpupower frequency-set -f), but you can change the maximum and minimum frequencies the driver is allowed to set as follows:

With cpupower you can use:

`cpupower frequency-set -u 3000mhz`

&#x2026; to set the maximum frequency for all cores. To set minimum frequency you can use

`cpupower frequency-set -d 3000mhz`


# Tracing

-   [Tracing](https://www.kernel.org/doc/html/latest/trace/index.html)
-   [Tracepoint](https://www.kernel.org/doc/html/latest/trace/events.html)

![img](/home/fedeztk/UNI/project/tesi/resources/Linux_tracing_architecture.png)

-   Tracing events &rarr; `less /sys/kernel/debug/tracing/available_events` or `trace-cmd report --events`
-   Useful events:
    -   `sched:sched_migrate_task`: migrazione
    -   `sched:sched_switch`: context switch (ci dice quando il processo è lanciato sulla CPU)
    -   `sched:sched_wakeup`: processo esce da wait queue ed entra in runqueue
    -   `sched:sched_process_exec`: eseguita una exec
    -   `sched:sched_process_exit`: eseguita una exit
    -   `sched:sched_process_fork`: una fork
    -   `sched:sched_process_wait`: una wait
    -   `power:cpu_frequency`: invocato sia da schedutil che da ondemand ad ogni richiesta di cambio di clock
    -   `power:cpu_idle`: quando si chiede di cambiare stato alla CPU da running a idle (e viceversa)
-   Tracing file system is under `/sys/kernel/debug/tracing`
-   [Filter](https://www.kernel.org/doc/html/latest/trace/events.html#event-filtering) tracing fields in order to avoid useless (and big) data
-   `echo "event_x" >> /sys/kernel/debug/tracing/set_event` &rarr; add event x to tracing
-   `echo "!event_x" >> /sys/kernel/debug/tracing/set_event` &rarr; remove event x from tracing

Common run in [tracing#]:

```bash
echo 0 > tracing_on
echo function_graph > current_tracer
echo 1 > tracing_on; run_test; echo 0 > tracing_on
```


## Alternative tracing viewer

-   `trace-cmd` Ex: `trace-cmd record -e sched_switch sleep 1` &rarr; memorizza tutti i context switch (marcati dall&rsquo;evento `sched_switch`) in un secondo. Questa esecuzione comporta la creazione di un file trace.dat che può essere letta con trace-cmd report.

As trace-cmd is a front end to Ftrace, the arguments of record reflect some of the features of Ftrace. The -e option enables an event. The argument following the -e can be an event name, event subsystem name, or the special name all. The all name will make trace-cmd enable all events that the system supports. If a subsystem name is specified, then all events under that subsystem will be enabled during the trace. For example, specifying sched will enable all the events within the sched subsystem.

Ftrace also has special plugin tracers that do not simply trace specific events. These tracers include the function, function graph, and latency tracers. Through the debugfs tracing directory, these plugins are enabled by echoing the type of tracer into the current\_tracer file. With trace-cmd record, they are enabled with the -p option. Using the tracer plugin name as the argument for -p enables that plugin.

The -l option is the same as echoing its argument into set\_ftrace\_filter, and the -n option is the same as echoing its argument into set\_ftrace\_notrace.

`trace-cmd reset` disable all tracing events. `trace-cmd extract -o kernel-buf.dat` extract tracing events in kernel-buf.dat file (it can be used after the Ftrace tracer has been started manually through the Ftrace pseudo file system).


## Tracing in C

[In-kernel trace event API](https://www.kernel.org/doc/html/latest/trace/events.html#in-kernel-trace-event-api)


# Scheduler

-   [The Linux Scheduler](https://static.linaro.org/connect/bkk19/presentations/bkk19-tr03.pdf) (slide)
-   [Fixing CPU\_IDLE](https://lwn.net/Articles/805317/) (LWN, scheduler classes/policies)


## Scheduler classes


### **STOP**

The Stop scheduling class is a special class that is used internally by the kernel. It doesn&rsquo;t implement any scheduling policy and no user task ever gets scheduled with it. The Stop class is, instead, a mechanism to force a CPU to stop running everything else and perform a specific task. As this is the highest-priority class, it can preempt everything else and nothing ever preempts it. It is used by one CPU to stop another in order to run a specific function, so it is only available on SMP systems. The Stop class creates a single, per-CPU kernel thread (or kthread) named migration/N, where N is the CPU number. This class is used by the kernel for task migration, CPU hotplug, RCU, ftrace, clock events, and more.


### **DEADLINE**

The Deadline scheduling class implements a single scheduling policy, SCHED\_DEADLINE, and it handles the highest-priority user tasks in the system. It is used for tasks with hard deadlines, like video encoding and decoding. The task with the earliest deadline is served first under this policy. The policy of a task can be set to SCHED\_DEADLINE using the sched\_setattr() system call by passing three parameters: the run time, deadline, and period. To ensure deadline-scheduling guarantees, the kernel must prevent situations where the current set of SCHED\_DEADLINE threads is not schedulable within the given constraints. The kernel thus performs an admittance test when setting or changing SCHED\_DEADLINE policy and attributes. This admission test calculates whether the change can be successfully scheduled; if not, sched\_setattr() fails with the error EBUSY.


### **RT (REALTIME)**

The POSIX realtime (or RT) scheduling class comes after the deadline class and is used for short, latency-sensitive tasks, like IRQ threads. This is a fixed-priority class that schedules higher-priority tasks before lower-priority tasks. It implements two scheduling policies: SCHED\_FIFO and SCHED\_RR. In SCHED\_FIFO, a task runs until it relinquishes the CPU, either because it blocks for a resource or it has completed its execution. In SCHED\_RR (round-robin), a task will run for the maximum time slice; if the task doesn&rsquo;t block before the end of its time slice, the scheduler will put it at the end of the round-robin queue of tasks with the same priority and select the next task to run. The priority of the tasks under the realtime policies range from 1 (low) to 99 (high).


### **CFS (completely fair scheduling)**

The CFS (completely fair scheduling) class hosts most of the user tasks; it implements three scheduling policies: SCHED\_NORMAL, SCHED\_BATCH, and SCHED\_IDLE. A task under any of these policies gets a chance to run only if no other tasks are enqueued in the deadline or realtime classes (though by default the scheduler reserves 5% of the CPU for CFS tasks regardless). The scheduler tracks the virtual runtime (vruntime) for all tasks, runnable and blocked. The lower a task&rsquo;s vruntime, the more deserving the task is for time on the processor. CFS accordingly moves low-vruntime tasks toward the front of the scheduling queue.

The priority of a task is calculated by adding 120 to its nice value, which ranges from -20 to +19. The priority of the task is used to set the weight of the task, which in turn affects the vruntime of the task; the lower the nice value, the higher the priority. The task&rsquo;s weight will thus be higher, and its vruntime will increase more slowly as the task runs.

The SCHED\_NORMAL policy (called SCHED\_OTHER in user space) is used for most of the tasks that run in a Linux environment, like the shell. The SCHED\_BATCH policy is used for batch processing by non-interactive tasks — tasks that should run uninterrupted for a period of time and hence are normally scheduled only after finishing all the SCHED\_NORMAL activity. The SCHED\_IDLE policy is designed for the lowest-priority tasks in the system; these tasks get a chance to run only if there is nothing else to run. Though, in practice, even in the presence of other SCHED\_NORMAL tasks a SCHED\_IDLE task will get some time to run (around 1.4% for a task with a nice value of zero). This policy isn&rsquo;t widely used currently and efforts are being made to improve how it works.


### **IDLE**

Last is the Idle scheduling class (which should not be confused with the SCHED\_IDLE scheduling policy). This is the lowest-priority scheduling class; like the Stop class, it doesn&rsquo;t manage any user tasks and so doesn&rsquo;t implement a policy. It only keeps a single per-CPU kthread which is named swapper/N, where N is the CPU number. These kthreads are also called the &ldquo;idle threads&rdquo; and aren&rsquo;t visible to user space. These threads are responsible for saving system power by putting the CPUs into deep idle states when there is no work to do.


# Systemtap

-   [opensuse docs](https://doc.opensuse.org/documentation/leap/tuning/html/book-sle-tuning/cha-tuning-systemtap.html#sec-tuning-systemtap-setup)
-   [arch docs](https://wiki.archlinux.org/index.php/SystemTap)
-   [lang manual](https://sourceware.org/systemtap/langref/)
-   [script example](https://www.sourceware.org/systemtap/examples/)
-   [monitor of userspace function](https://stackoverflow.com/questions/46783960/systemtap-simple-userspace-example-function-tracing-ubuntu)
-   `man: stap, staprun, stapprobes, stapfuncs`


## Tracepoint

This family of probe points hooks to static probing tracepoints inserted into the kernel or kernel modules. As with marker probes, these tracepoints are special macro calls inserted by kernel developers to make probing faster and more reliable than with DWARF-based probes. DWARF debugging information is not required to probe tracepoints. Tracepoints have more strongly-typed parameters than marker probes.

Tracepoint probes begin with kernel. The next part names the tracepoint itself: trace(&ldquo;name&rdquo;). The tracepoint name string, which can contain wildcard characters, is matched against the names defined by the kernel developers in the tracepoint header files.

The handler associated with a tracepoint-based probe can read the optional parameters specified at the macro call site. These parameters are named according to the declaration by the tracepoint author. For example, the tracepoint probe kernel.trace(&ldquo;sched\_switch&rdquo;) provides the parameters $rq, $prev, and $next. If the parameter is a complex type such as a struct pointer, then a script can access fields with the same syntax as DWARF $target variables. Tracepoint parameters cannot be modified; however, in guru mode a script can modify fields of parameters.

The name of the tracepoint is available in `$$name`, and a string of name=value pairs for all parameters of the tracepoint is available in `$$vars` or `$$parms`.


## Useful stap commands

List probe points that matches

```shell
stap -L 'kernel.trace("power:*")'
stap -L 'kernel.trace("sched:*")'
stap -L 'kernel.trace("percpu:*")'
stap -L 'kernel.trace("*msr*")'
man -k "function::*"
man -k "probe::*"
```

    std::__detail::_Mod_range_hashing (3) - Default range hashing function: use d...
    Alien::Build::Plugin::Probe::CBuilder (3pm) - Probe for system libraries by g...
    Alien::Build::Plugin::Probe::CommandLine (3pm) - Probe for tools or commands ...
    Alien::Build::Plugin::Probe::Vcpkg (3pm) - Probe for system libraries using V...


## Stap tapset

```c
tid()              // The id of the current thread.
pid()              // The process (task group) id of the current thread.
uid()              // The id of the current user.
execname()         // The name of the current process.
cpu()              // The current cpu number.
gettimeofday_s()   // Number of seconds since epoch.
get_cycles()       // Snapshot of hardware cycle counter.
pp()               // A string describing the probe point being currently handled.
ppfunc()           // If known, the the function name in which this probe was placed.
$$vars             // If available, a listing of all local variables in scope.
print_backtrace()  // If possible, print a kernel backtrace.
print_ubacktrace() // If possible, print a user-space backtrace.
```

-   [all stap functions](https://sourceware.org/systemtap/tapsets/)


# Off Topic


## Bash

-   $1, $2, $3, &#x2026; are the positional parameters.
-   &ldquo;$@&rdquo; is an array-like construct of all positional parameters, {$1, $2, $3 &#x2026;}.
-   &ldquo;$\*&rdquo; is the IFS expansion of all positional parameters, $1 $2 $3 &#x2026;.
-   $# is the number of positional parameters.
-   $- current options set for the shell.
-   $$ pid of the current shell (not subshell).
-   $\_ most recent parameter (or the abs path of the command to start the current shell immediately after startup).
-   $IFS is the (input) field separator.
-   $? is the most recent foreground pipeline exit status.
-   $! is the PID of the most recent background command.
-   $0 is the name of the shell or shell script.


## C/Kernel utils

-   [kernel api](https://www.kernel.org/doc/htmldocs/kernel-api/)
-   `loff_t` = `long long int *`
-   print of ssize\_t:
    
    ```c
    size_t x = ...;
    ssize_t y = ...;
    printf("%zu\n", x); // prints as unsigned decimal
    printf("%zx\n", x); // prints as hex
    printf("%zd\n", y); // prints as signed decimal
    ```
-   Read/write in kernel
    
    ```c
    // Read the file from the kernel space.
    ssize_t kernel_read(struct file *file, void *buf,
                        size_t count, loff_t *pos);
    
    // Write the file from the kernel space.
    ssize_t kernel_write(struct file *file, const void *buf,
                         size_t count, loff_t *pos);
    ```


### Can I use library functions in the kernel ?

System libraries (such as glibc, libreadline, libproplist, whatever) that are typically available to userspace programmers are unavailable to kernel programmers. When a process is being loaded the loader will automatically load any dependent libraries into the address space of the process. None of this mechanism is available to kernel programmers: forget about ISO C libraries, the only things available is what is already implemented (and exported) in the kernel and what you can implement yourself.

Note that it is possible to &ldquo;convert&rdquo; libraries to work in the kernel; however, they won&rsquo;t fit well, the process is tedious and error-prone, and there might be significant problems with stack handling (the kernel is limited to a small amount of stack space, while userspace programs don&rsquo;t have this limitation) causing random memory corruption.

Many of the commonly requested functions have already been implemented in the kernel, sometimes in &ldquo;lightweight&rdquo; versions that aren&rsquo;t as featureful as their userland counterparts. Be sure to grep the headers for any functions you might be able to use before writing your own version from scratch. Some of the most commonly used ones are in include/linux/string.h.

Whenever you feel you need a library function, you should consider your design, and ask yourself if you could move some or all the code into user-space instead.

[coding in the kernel](https://www.kernel.org/doc/html/v4.17/process/4.Coding.html)


## Interesting resources

-   [BCC](https://github.com/iovisor/bcc)
