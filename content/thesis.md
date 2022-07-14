---
title: "Thesis"
date: 2022-07-14T16:25:11+02:00
draft: false
---

##  A study of Intel’s Speed Shift power management technology

PDF available [here](/thesis.pdf)

## Abstract
In modern processor design, lowering the energy consumption is of paramount importance. In PCs as well as in data centers, the CPU is the component consuming the most energy. Intel, from the Skylake processor generation and on, developed a hardware micro-controller, which is responsible for keeping the operating frequency at its optimal value, maximizing the performance per Watt. The logic behind such a microcontroller, however, is not disclosed. Hence the operating system and the HW controller may set contradictory operating points, leading then to performance degradation.

In this work, we investigate non-documented features of the frequency scaling policy of Intel's Skylake processors, known as Intel Speed Shift or Hardware-Controlled Performance State (HWP).

In our experiments, we investigated the response of the frequency controller in response to known workload patterns. A few characteristics were detected, analyzed and explained. Others are left as future work.
