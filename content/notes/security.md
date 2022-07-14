---
title: "Comptia Security+"
date: 2022-07-14T15:21:59+02:00
draft: false
toc: true
---

> Study group videos [here](https://www.youtube.com/playlist?list=PLG49S3nxzAnnjucQ18QzbCrv-er2zH7d9)  



# Attacks, Threats, and Vulnerabilities 24%



## Compare and contrast different types of social engineering techniques



### Phishing

~ social engineering with a touch of spoofing (email, text, etc)  

-   check the URL!
-   <span class="underline">usually</span> something wrong (spelling, font, graphics)

1.  Tricks

    -   typosquatting  
        -   <https://bancasampaolo.com>
        -   prepending: <https://bbancasanpaolo.com>
    -   pretexting  
        -   lying to get information (eg. we&rsquo;re calling from Visa regarging&#x2026;)

2.  Pharming

    -   poisoned DNS server or client vulnerabilities
    -   everybody will be automatically redirected to the attacker&rsquo;s web sites
    -   combined with phishing:  
        -   pharming: harvest large groups of people
        -   phishing: collect access credentials
    -   **difficult** for anti-malware and peple to detect
    -   relatively rare

3.  Vishing (voice phishing)

    -   spoofed phone number

4.  Smishing (sms phishing)

    -   forwards links or ask for personal information

5.  Finding the best spot to phish - Spear phishing

    -   targeted to specific people
    -   spear phishing the CEO is &ldquo;whaling&rdquo;  
        -   possible great catch
    -   eg social networks, corporate web sites
    -   where you work
    -   where you bank
    -   recent financial transactions
    -   family and friends



### Impersonation

-   usually start with pretext, an actor and a story
-   often with vishing
-   psychological techniques
-   examples:  
    1.  Hello sir, my name is Wendy and I’m from Microsoft Windows. This is an urgent check up call for your computer as we have found several problems with it.
    2.  Voice mail: This is an enforcement action executed by the US Treasury intending your serious attention.
    3.  Congratulations on your excellent payment history! You now qualify for 0% interest rates on all of your credit card accounts.

1.  Plan

    1.  pretend to be someone else
    2.  use of those details from reconnaissance
    3.  person high in rank
    4.  throw tons of technical details
    5.  be a buddy

2.  identity fraud

    -   bank fraud
    -   credit card fraud
    -   loan fraud
    -   government/tax fraud

3.  Protection

    -   never volunteer information
    -   don&rsquo;t disclose personal details
    -   always verify identity (through third parties)
    -   encourage verification



### Dumpster diving

-   mobile garbage bin
-   important information thrown out with trash
-   gather details
-   timing is important

1.  Protection

    -   secure garbage (locking key)
    -   burn documents



### Shoulder surfing

-   access to important information
-   curiosity, industrial espionage, competitive advantage
-   surprisingly easy  
    -   coffee
    -   airport
-   webcam, binoculars, office

1.  Protection

    -   control your input
    -   use privacy filters
    -   keep your monitor out of sight



### Hoaxes

-   hoax: a threat that doesn&rsquo;t exist
-   still consume a lot of resources
-   often an email or social
-   some hoaxes will take your money  
    -   by maxing you eg buying a gift card
-   equally time wasting as a &ldquo;real&rdquo; virus

1.  Protection

    -   consider the source
    -   cross reference
    -   check spam filter is operating
    -   if it sounds too good to be true



### Watering hole attack

-   if you have a secure network the attacker may go to a third party that you visit: the watering hole
-   infect also your network
-   where your users are visiting

1.  Protection

    -   defense-in-depth
    -   firewall and IPS
    -   anti virus - anti malware



### Spam

Unsolicited messages  

-   email, forums
-   spam over instant messaging (SPIM)

Various content  

-   commercial advertising
-   non commercial
-   phishing attempts

Significant technology issue  

-   managing the spam
-   security
-   resource utilisation

1.  Protection

    -   Mail gateway in front on the internal mail server
    -   Identitying spam  
        -   allowed list: only from trusted sender
        -   SMTP standards checking: block anything that doesn&rsquo;t follow RFC standard
        -   rDNS: block email where the sender&rsquo;s domain doesn&rsquo;t match the IP address
        -   tarpitting: intentionally slow down the server conversation
        -   recipient filtering: block email not addressed to a valid recipient email address



### Influence campaigns

-   hacking public opinion
-   nation-state actors
-   advertising is an option
-   enabled through social media
-   cyberwarfare: military strategy (not a new concept)  
    -   influencing foreign elections
    -   fake news

1.  Process

    1.  create fake users
    2.  create content
    3.  post on social medias
    4.  amplify message
    5.  real users share the message
    6.  mass media picks up the story



### Other social engineering attacks

1.  Tailgating

    Use an authorized person to gain unauthorized access to a building  
    
    -   blend in with clothing
    -   most security stops at the border

2.  Protection

    -   policy for visitors (eg badges)
    -   one scan one person
    -   access control vestibule / airlock
    -   don&rsquo;t be afraid to ask

3.  Invoice scam

    1.  starts with a bit os spear phishing
    2.  attacker sends a face invoice
    3.  from a spoofed address of the CEO
    4.  might also include links to pay

4.  Credential harvesting

    -   also called password harvesting
    -   there are a lot of stored credentials in the computer
    -   a program need to run on your local machine (eg malicious docx document)
    -   everything may happen in the background



### Principles of social engineering

-   constantly changing
-   may involve multiple people
-   may be in person or electronic
-   Principles:  
    1.  authority
    2.  intimidation
    3.  consensus / social proof
    4.  scarcity
    5.  urgency
    6.  familiarity / liking
    7.  trust



## Given a scenario, analyze potential indicators to determine the type of attack



### An overview of malware

-   malicious software
-   gather information (keystroke)
-   participate in a group (botnet)
-   show you advertising
-   viruses and worm (pay for decryption)

Malware types and method:  

1.  Viruses
2.  Crypto-malware
3.  Ransomware
4.  Worms
5.  Trojan Horse
6.  Rootkit
7.  Keylogger
8.  Adware/Spyware
9.  Botnet

1.  How you get malware

    1.  A worm takes advantage of a vulnerability
    2.  Installs malware that includes a remote access backdoor
    3.  Bot may be installed later
    
    Your computer must run a program  
    
    -   Email link - Don’t click links
    -   Web page pop-up
    -   Drive-by download
    -   Worm
    
    Your computer is vulnerable  
    
    -   Operating system - Keep your OS updated!
    -   Applications - Check with the publisher



### Viruses and Worms

-   Malware that can reproduce itself  
    -   it needs you to execute a program
-   Reproduces through file systems or the network  
    -   Just running a program can spread a virus
-   May or may not cause problems  
    -   Some viruses are invisible, some are annoying
-   Anti-virus is very common  
    -   Thousands of new viruses every week
    -   Is your signature file updated?

1.  Virus types

    -   Program viruses  
        -   it’s part of the application
    -   Boot sector viruses  
        -   Who needs an OS?
    -   Script viruses  
        -   Operating system and browser-based
    -   Macro viruses  
        -   Common in Microsoft Office
    -   Fileless viruses  
        -   Does a good job of avoiding  
            -   anti-virus detection
        -   Operates in memory  
            -   But never installed in a file or application

2.  Worms

    Malware that self-     replicates  
    
    -   Doesn’t need you to do anything
    -   Uses the network as a transmission medium
    -   Self-propagates and spreads quickly
    
    Worms are pretty bad things  
    
    -   Can take over many systems very quickly
    
    Firewalls and IDS/IPS can mitigate many worm infestations  
    
    -   Doesn’t help much once the worm gets inside



### Ransomware and Crypto- malware

1.  Ransomware

    Personal data  
    
    -   Family pictures and videos
    -   Important documents
    
    Organization data  
    
    -   Planning documents
    -   Employee personally identifiable information (PlI)
    -   Financial information
    -   Company private data
    
    How much is it worth?  
    
    -   There’s a number
    
    The bad guys want your money  
    
    -   They’ll take your computer in the meantime
    
    May be a fake ransom  
    
    -   Locks your computer “by the police”
    
    The ransom may be avoided  
    
    -   A security professional may be able
    
    to remove these kinds of malware  

2.  Crypto- malware

    A newer generation of ransomware  
    
    -   Your data is unavailable until you provide cash
    
    Malware encrypts your data files  
    
    -   Pictures, documents, music, movies, etc.
    -   Your OS remains available
    -   They want you running, but not working
    
    You must pay the bad guys to obtain the decryption key  
    
    -   Untraceable payment system
    -   An unfortunate use of public-key cryptography

3.  Protection

    Always have a backup  
    
    -   An offline backup, ideally
    
    Keep your operating system up to date  
    
    -   Patch those vulnerabilities
    
    Keep your applications up to date  
    
    -   Security patches
    
    Keep your anti- virus/anti-malware signatures up to date  
    
    -   New attacks every hour
    
    Keep everything up to date  



### Trojan and RATs

Used by the Greeks to capture Troy from the Trojans  

-   A digital wooden horse

Software that pretends to be something else  

-   So It can conquer your computer
-   Doesn’t really care much about replicating

Circumvents your existing security  

-   Anti-virus may catch it when it runs
-   The better Trojans are built to avoid and disable AV

Once it’s inside it has free reign  

-   And it may open the gates for other programs

1.  Potentially unwanted program (PUP)

    Identified by anti-virus/anti-malware  
    
    -   Potentially undesirable software
    -   Often installed along with other software
    
    Overly aggressive browser toolbar  
    A backup utility that displays ads ER  
    Browser search engine hijacker  

2.  Backdoors

    Why go through normal authentication methods?  
    
    -   Just walk in the back door
    
    Often placed on your computer through malware  
    
    -   Some malware software can take advantage of backdoors created by other malware
    
    Some software includes a backdoor (oops)  
    
    -   Old Linux kernel included a backdoor
    -   Bad software can have a backdoor as part of the app

3.  Remote access trojans (RATs)

    Remote Administration Tool  
    
    -   The ultimate backdoor
    -   Administrative control of a device
    
    Malware installs the server/service/host  
    
    -   Bad guys connect with the client software
    
    Control a device  
    
    -   Key logging
    -   Screen recording /screenshots
    -   Copy files
    -   Embed more malware

4.  Protection

    Don’t run unknown software  
    
    -   Consider the consequences
    
    Keep anti-virus/anti-malware signatures updated  
    
    -   There are always new attacks
    
    Always have a backup  
    
    -   You may need to quickly recover



### Rootkits

Originally a Unix technique  

-   The “root” in rootkit

Modifies core system files  

-   Part of the kernel

Can be invisible to the operating system  

-   Won’t see it in Task Manager

Also invisible to traditional anti-virus utilities  

-   If you can’t see it, you can’t stop it

1.  Kernel drivers

    Zeus/Zbot malware  
    
    -   Famous for cleaning out bank accounts
    
    Now combined with Necurs rootkit  
    
    -   Necurs is a kernel-level driver
    
    Necurs makes sure you can’t delete Zbot  
    
    -   Access denied
    
    Trying to stop the Windows process?  
    
    -   Error terminating process: Access denied

2.  Finding and removing rootkits

    Look for the unusual  
    
    -   Anti-malware scans
    
    Use a remover specific to the rootkit  
    
    -   Usually built after the rootkit is discovered
    
    Secure boot with UEFI  
    
    -   Security in the BIOS
    -   won&rsquo;t boot if kernel is modified



### Spyware

Your computer is one big advertisement  

-   Pop-ups with pop-ups

May cause performance issues  

-   Especially over the network

Installed accidentally  

-   May be included with other software

Be careful of software that claims to remove adware  

-   Especially if you learned about it from a pop-up

Malware that spies on you  

-   Advertising, identity theft, affiliate fraud

Can trick you into installing  

-   Peer to peer, fake security software

Browser monitoring  

-   Capture surfing habits W

Keyloggers  

-   Capture every keystroke  
    -   Send it back to the mother ship

1.  Why is there so much spyware and adware?

    Money  
    
    -   Your eyeballs are incredibly valuable
    -   Your computer time and bandwidth is incredibly valuable
    -   Your bank account is incredibly valuable  
        -   Yes, even your bank account

2.  Protection

    Maintain your anti-virus / anti-malware  
    
    -   Always have the latest signatures
    
    Always know what you’re installing  
    
    -   And watch your options during the installation
    
    Where’s your backup?  
    
    -   You might need it someday
    -   Cleaning adware isn’t easy
    
    Run some scans  
    
    -   eg Malwarebytes



### Bots and botnets

Robots  
Once your machine is infected, it becomes a bot  

-   You may not even know

How does it get on your computer?  

-   Trojan Horse (I just saw a funny video of you! Click here.) Or You run a program or click an ad you THOUGHT was legit, but&#x2026;
-   OS or application vulnerability

A day in the life of a bot  

-   Sit around. Check in with the Command and Control (C&C) server. Wait for instructions.

1.  Botnets

    A group of bots working together  
    
    -   Nothing good can come from this
    
    Distributed Denial of service (DDoS)  
    
    -   The power of many
    
    Relay spam, proxy network traffic, distributed computing tasks  
    Botnets are for sale  
    
    -   Rent time from the bad guys
    -   Not a long-term business proposition

2.  Protection

    Prevent the initial infection  
    
    -   OS and application patches
    -   Anti-virus/anti-malware and updated signatures
    
    Identify an existing infection  
    
    -   On-demand scans
    -   Network monitoring
    
    Prevent command and control (C&C)  
    
    -   Block at the firewall
    -   Identify at the workstation with a host-based firewall or host-based IPS



### Logic bombs

Waits for a predefined event  

-   Often left by someone with grudge

Time bomb  

-   Time or date

User event  

-   Logic bomb

Difficult to identify  

-   Difficult to recover if it goes off

1.  Protection

    Difficult to recognize  
    
    -   Each is unique
    -   No predefined signatures
    
    Process and procedures  
    
    -   Formal change control
    
    Electronic monitoring  
    
    -   Alert on changes
    -   Host-based intrusion detection, Tripwire, etc.
    
    Constant auditing  
    
    -   An administrator can circumvent existing systems



### Password attacks

1.  Plaintext/unencrypted passwords

    Some applications store passwords “in the clear”  
    
    -   No encryption. You can read the stored password.
    -   This is rare, thankfully
    
    Do not store passwords as plaintext  
    
    -   Anyone with access to the password file or database has every credential
    
    What to do if your application saves passwords as plaintext:  
    
    -   Get a better application

2.  Hashing a password

    Hashes represent data as a fixed-length string of text  
    
    -   A message digest, or “fingerprint”
    
    Will not have a collision (hopefully)  
    
    -   Different inputs will not have the same hash
    
    One-way trip  
    
    -   Impossible to recover the original message from the digest
    -   A common way to store passwords

3.  Password file

    Different across operating systems and applications  
    
    -   Different hash algorithms

4.  Spraying attack

    Try to login with an incorrect password  
    
    -   Eventually you&rsquo;re locked out
    
    There are some common passwords  
    
    -   <https://en.wikipedia.org/wiki/List_of_the_most_common_passwords>
    
    Attack an account with the top three (or more) passwords  
    
    -   If they don’t work, move to the next account
    -   No lockouts, no alarms, no alerts

5.  Brute force

    Try every possible password combination until the a hash is matched  
    This might take some time  
    
    -   A strong hashing algorithm slows things down
    
    Brute force attacks - Online  
    
    -   Keep trying the login process
    -   Very slow
    -   Most accounts will lockout after a number of failed attempts
    
    Brute force the hash - Offline  
    
    -   Obtain the list of users and hashes
    -   Calculate a password hash, compare it to a stored hash
    -   Large computational resource requirement

6.  Dictionary attacks

    Use a dictionary to find common words  
    
    -   Passwords are created by humans
    
    Many common wordlists available on the ‘net  
    
    -   Some are customized by language or line of work
    
    The password crackers can substitute letters  
    
    -   p&sswOrd
    
    This takes time  
    
    -   Distributed cracking and GPU cracking is common
    
    Discover passwords for common words  
    
    -   This won’t discover random character passwords

7.  Rainbow tables

    An optimized, pre-built set of hashes  
    
    -   Saves time and storage space
    -   Doesn’t need to contain every hash
    -   Contains pre-calculated hash chains
    
    Remarkable speed increase  
    
    -   Especially with longer password lengths
    
    Need different tables for different hashing methods  
    
    -   Windows is different than MySQL

8.  Adding some salt

    -   Salt:Random data added to a password when hashing
    
    Every user gets their own random salt  
    
    -   The salt is commonly stored with the password
    
    Rainbow tables won’t work with salted hashes  
    
    -   Additional random value added to the original password
    
    This slows things down the brute force process  
    
    -   It doesn’t completely stop the reverse engineering (maybe they know the implementation of the salt)
    
    Each user gets a different random hash  
    
    -   The same password creates a different hash



### Physical attacks

1.  Malicious USB cable

    It looks like a normal USB cable  
    
    -   It has additional electronics inside
    
    Operating system identifies it as a HID  
    
    -   Human Interface Device
    -   It looks like you’ve connected a keyboard or mouse
    -   A keyboard doesn’t need extra rights or permissions
    
    Once connected, the cable takes over  
    
    -   Downloads and installs malicious software
    
    Don’t just plug in any USB cable  
    
    -   Always use trusted hardware

2.  Malicious USB cable

    Free USB flash drive!  
    
    -   Plug it in and see what’s on it
    -   That’s a bad idea
    
    Older operating systems would automatically run files  
    
    -   This has now been disabled or removed by default
    
    Could still act as a HID (Human Interface Device) / Keyboard  
    
    -   Start a command prompt and type anything without your intervention

3.  Malicious USB cable

    Attackers can load malware in documents  
    
    -   PDF files, spreadsheets
    
    Can be configured as a boot device  
    
    -   Infect the computer after a reboot
    
    Acts as an Ethernet adapter  
    
    -   Redirects or modifies Internet traffic requests
    -   Acts as a wireless gateway for other devices
    
    Never connect an untrusted USB device  

4.  Skimming

    Stealing credit card information, usually during a normal transaction  
    
    -   Copy data from the magnetic stripe:
    
    Card number, expiration date, card holder’s name  
    ATM skimming  
    
    -   Includes a small camera to also watch for your PIN
    
    Attackers use the card information for other financial transactions  
    
    -   Fraud is the responsibility of the seller
    
    Always check before using card readers  

5.  Card cloning

    Get card details from a skimmer  
    
    -   The clone needs an original
    
    Create a duplicate of a card  
    
    -   Looks and feels like the original
    -   Often includes the printed CVC (Card Validation Code)
    
    Can only be used with magnetic stripe cards  
    
    -   The chip can’t be cloned
    
    Cloned gift cards are common  
    
    -   A magnetic stripe technology



### Adversarial Artificial Intelligence

1.  Machine learning

    Our computers are getting smarter  
    
    -   They identify patterns in data and improve their predictions
    
    This requires a lot of training data  
    
    -   Face recognition requires analyzing a lot of faces
    -   Driving a car requires a lot of road time
    
    In use every day  
    
    -   Stop spam
    -   Recommend products from an online retailer
    -   What movie would you like to see? This one.
    -   Prevent car accidents

2.  Poisoning the training data

    Confuse the artificial intelligence (Al)  
    
    -   Attackers send modified training data that causes the Al to behave incorrectly
    
    Microsoft Al chatter bot named Tay  
    (Thinking About You)  
    
    -   Joins Twitter on March 23, 2016
    -   Designed to learn by interacting with Twitter users
    -   Microsoft didn’t program in anti-offensive behavior
    -   Tay quickly became racist, sexist, and inappropriate

3.  Evasion attacks

    The Al is only as good as the training  
    
    -   Attackers find the holes and limitations
    
    An Al that knows what spam looks like  
    can be fooled by a different approach  
    
    -   Change the number of good and bad words in the message
    
    An Al that uses real-world information can release confidential information  
    
    -   Trained with data that includes social security numbers
    -   Al can be fooled into revealing those numbers

4.  Securing the learning algorithm

    Check the training data  
    
    -   Cross check and veritfy
    
    Constantly retrain with new data  
    
    -   More data
    -   Better data
    
    Train the Al with possible poisoning  
    
    -   What would the attacker try to do?



### Supply chain attack

1.  Supply chain

    The chain contains many moving parts  
    
    -   Raw materials, suppliers, manufacturers, distributors, customers, consumers
    
    Attackers can infect any step along the way  
    
    -   Infect different parts of the chain without suspicion
    -   People trust their suppliers
    
    One exploit can infect the entire chain  
    
    -   There’s a lot at stake

2.  Supply chain security

    Can you trust your new server/router/switch/firewall/software?  
    
    -   Supply chain cyber security
    
    Use a small supplier base  
    
    -   Tighter control of vendors
    
    Strict controls over policies and procedures  
    
    -   Ensure proper security is in place
    
    Security should be part of the overall design  
    
    -   There’s a limit to trust



### Cloud based vs on-Premise attacks

Two categories for IT security  

-   The on-premises data is more secure!
-   The cloud-based data is more secure!

Cloud-based security is centralized and costs less  

-   No dedicated hardware, no data center to secure
-   A third-party handles everything

On-premises puts the security burden on the client  

-   Data center security and infrastructure costs

Attackers want your data  

-   They don’t care where it is

1.  On-premises

    Customize your security posture  
    
    -   Full control when everything is in-house
    
    On-site IT team can manage security better  
    
    -   The local team can ensure everything is secure
    -   A local team can be expensive and difficult to staff
    
    Local team maintains uptime and availability  
    
    -   System checks can occur at any time
    -   No phone call for support
    
    Security changes can take time  
    
    -   New equipment, configurations, and additional costs

2.  Cloud

    Data Is In a secure environment  
    
    -   No physical access to the data center
    -   Third-party may have access to the data
    
    Cloud providers are managing large-scale security  
    
    -   Automated signature and security updates
    -   Users must follow security best-practices
    
    Limited downtime  
    
    -   Extensive fault-tolerance and 24/7/365 monitoring
    
    Scalable security options  
    
    -   One-click security deployments
    -   This may not be as customizable as necessary



### Cryptographyc attacks

You’&rsquo;ve encrypted data and sent it to another person  

-   Is it really secure?
-   How do you know?

The bad guy doesn’t have the combination (the key)  

-   So they break the safe (the cryptography)

Finding ways to undo the security  

-   There are many potential cryptographic shortcomings
-   The problem is often the implementation

1.  Birthday attack

    In a classroom of 23 students, what is the  
    chance of two students sharing a birthday?  
    
    -   About 50%
    -   For a class of 30, the chance is about 70%
    
    In the digital world, this is a hash collision  
    
    -   A hash collision is the same hash value for two different plaintexts
    -   Find a collision through brute force
    
    The attacker will generate multiple versions of plaintext to match the hashes  
    
    -   Protect yourself with a large hash output size

2.  Collisions

    Hash digests are supposed to be unique  
    
    -   Different input data should never create the same hash
    
    MDS5 hash  
    
    -   Message Digest Algorithm 5
    -   First published in April 1992
    -   Collisions identified in 1996
    
    December 2008: Researchers created CA certificate that appeared legitimate when MD5 is checked  
    
    -   Built other certificates that appeared to be legit and issued by RapidSSL

3.  Downgrade attack

    Instead of using perfectly good encryption, use something that’s not so great  
    
    -   Force the systems to downgrade their security
    
    2014 - TLS vulnerability  
    POODLE (Padding Oracle On  
    Downgraded Legacy Encryption)  
    
    -   On-path attack
    -   Forces clients to fallback to SSL 3.0
    -   SSL 3.0 has significant cryptographic vulnerabilities
    -   Because of POODLE, modern browsers won’t fallback to SSL 3.0



### Privilege escalation

Gain higher-level access to a system  

-   Exploit a vulnerability
-   Might be a bug or design flaw

Higher-level access means more capabilities  

-   This commonly is the highest-level access
-   This is obviously a concern

These are high-priority vulnerability patches  

-   You want to get these holes closed very quickly
-   Any user can be an administrator

Horizontal privilege escalation  

-   User A can access user B resources

1.  Protection

    Patch quickly  
    
    -   Fix the vulnerability
    
    Updated anti-virus/anti-malware software  
    
    -   Block known vulnerabilities
    
    Data Execution Prevention  
    
    -   Only data in executable areas can run
    
    Address space layout randomization  
    
    -   Prevent a buffer overrun at a known memory address



## Given a scenario, analyze potential indicators associated with application attacks



### Cross-site Scripting (XSS)

Originally called cross-site because of browser security flaws  

-   Information from one site could be shared with another

One of the most common web application development errors  

-   Takes advantage of the trust a user has for a site
-   Complex and varied

Malware that uses JavaScript  

-   Do you allow scripts? Me too.

Tokens **should** expire  

1.  Non persistent (reflected) XSS attack

    Web site allows scripts to run in user input  
    
    -   Search box is a common source
    
    Attacker emails a link that takes advantage of this vulnerability  
    
    -   Runs a script that sends credentials/session IDs/cookies to the attacker
    
    Script embedded in URL executes in the victim’s browser  
    
    -   As if it came from the server
    
    Attacker uses credentials/session IDs/cookies to steal victim’s information without their knowledge  
    
    -   Very sneaky

2.  Persistent (stored) XSS attack

    Attacker posts a message to a social network  
    
    -   Includes the malicious payload
    
    It’s now “persistent”  
    
    -   Everyone gets the payload
    
    No specific target  
    
    -   All viewers to the page
    
    For social networking, this can spread quickly  
    
    -   Everyone who views the message can have it posted to their page  
        -   Where someone else can view it and propagate it further&#x2026;

3.  Protection

    Be careful when clicking untrusted links  
    
    -   Never blindly click in your email inbox. Never.
    
    Consider disabling JavaScript  
    
    -   Or control with an extension
    -   This offers limited protection
    
    Keep your browser and applications updated  
    
    -   Avoid the nasty browser vulnerabilities
    
    Validate input  
    
    -   Don’t allow users to add their own scripts to an input field



### Injection attacks

1.  Code injection

    Code injection: Adding your own information into a data stream  
    Enabled because of bad programming  
    
    -   The application should properly handle input and output
    
    So many different data types  
    
    -   HTML, SQL, XML, LDAP, etc.

2.  SQL injection

    SQL - Structured Query Language  
    
    -   The most common relational database management system language

3.  XML injection and LDAP injection

    XML - Extensible Markup Language  
    
    -   A set of rules for data transfer and storage
    
    XML injection  
    
    -   Modifying XML requests - a good application will validate
    
    LDAP - Lightweight Directory Access Protocol  
    
    -   Created by the telephone companies
    -   Now used by almost everyone
    
    LDAP injection  
    
    -   Modify LDAP requests to manipulate application results

4.  DLL injection

    Dynamic-Link Library  
    
    -   A Windows library containing code and data
    -   Many applications can use this library
    
    Inject a DLL and have an application run a program  
    
    -   Runs as part of the target process



### Buffers overflows

Overwriting a buffer of memory  

-   Spills over into other memory areas

Developers need to perform bounds checking  

-   The attackers spend a lot of time looking for openings

Not a simple exploit  

-   Takes time to avoid crashing things
-   Takes time to make it do what you want

A really useful buffer overflow is repeatable  

-   Which means that a system can be compromised



### Replay attacks

Useful information is transmitted over the network  

-   A crafty hacker will take advantage of this

Need access to the raw network data  

-   Network tap, ARP poisoning, Malware on the victim computer

The gathered information may help the attacker  

-   Replay the data to appear as someone else

This is not an on-path attack  

-   The actual replay doesn’t require the original workstation
-   eg: pass the hash  
    Avoid this type of replay attack with a salt or encryption  
    Use a session ID with the password hash to create a unique authentication hash each time  
    1.  Attacker captures authentication (Username and hashed password)
    2.  Attacker sends his own authentication request using the previously captured information
    3.  Username and hash match a valid account - attacker gains access

1.  Browser cookies and session IDs

    Cookies: Information stored on your computer by the browser  
    Used for tracking, personalization, session management  
    
    -   Not executable, not generally a security risk  
        -   Unless someone gets access to them
    
    Could be considered be a privacy risk  
    
    -   Lots of personal data in there
    
    Session IDs are often stored in the cookie  
    
    -   Maintains sessions across multiple browser sessions

2.  Session hijacking (sidejacking)

    the attacker gains access of the session ID  
    Use an **encrypted** protocol  
    
    1.  Header manipulation
    
        Information gathering  
        
        -   Wireshark, Kismet
        
        Exploits  
        
        -   Cross-site scripting
        
        Modify headers  
        
        -   Tamper, Firesheep, Scapy
        
        Modify cookies  
        
        -   Cookies Manager+ (Firefox add-on)

3.  Protection

    Encrypt end-to-end  
    
    -   They can’t capture your session ID if they can’t see it
    -   Additional load on the web server (HTTPS)
    -   Firefox extension: HTTPS Everywhere, Force-TLS
    -   Many sites are now HTTPS-only
    
    Encrypt end-to-somewhere  
    
    -   At least avoid capture over
    
    a local wireless network  
    
    -   Still in-the-clear for part of the journey
    -   Personal VPN (OpenVPN, VyprVPN, etc.)



### Request forgeries

Cross-site requests are common and legitimate  

-   You visit ProfessorMesser.com
-   Your browser loads text from the ProfessorMesser.com server
-   Your browser loads a video from YouTube
-   Your browser loads pictures from Instagram

HTML on ProfessorMesser.com directs requests from your browser  

-   This is normal and expected

1.  The client and the server

    Website pages consist of client-side code and server-side code  
    
    -   Many moving parts
    
    Client side  
    
    -   Renders the page on the screen
    -   HTML, JavaScript
    
    Server side  
    
    -   Performs requests from the client
    -   HTML, PHP X
    -   Transfer money from one account to another
    -   Post a video on YouTube

2.  Cross-site request forgery

    One-click attack, session riding  
    
    -   XSRF, CSRF (sea surf)
    
    Takes advantage of the trust that a web application has for the user  
    
    -   The web site trusts your browser
    -   Requests are made without your consent or your knowledge
    -   Attacker posts a Facebook status on your account
    
    Significant web application development oversight  
    
    -   The application should have anti-forgery techniques added
    -   Usually a cryptographic token to prevent a forgery
    -   Attacker creates a funds transfer request
    -   Request is sent as a hyperlink to a user who may already be logged into the bank web site
    -   Visitor clicks the link and unknowingly sends the transfer request to the bank web site
    -   Bank validates the transfer &rsquo;and sends the visitor’s funds to the attacker

3.  Server-side request forgery (SSRF)

    Attacker finds a vulnerable web application  
    
    -   Sends requests to a web server
    -   Web server performs the request on behalf of the attacker
    
    Caused by bad programming  
    
    -   Never trust the user input
    -   Server should validate the input and the responses
    -   These are rare, but can be critical vulnerabilities
    -   how  
        1.  Attacker sends a request that controls a web application
        2.  Web server sends request to another service, such as cloud file storage
        3.  Cloud storage sends response to Web Server
        4.  Web Server forwards response to attacker



### Driver manipulation

1.  Malware hide-and-go-seek

    Traditional anti-virus is very good at identifying known attacks  
    
    -   Checks the signature
    -   Block anything that matches
    
    There are still ways to infect and hide  
    
    -   It’s a constant war
    -   Zero-day attacks, new attack types, etc.

2.  Drivers are powerful

    The interaction between the hardware and your operating system  
    
    -   They are often trusted
    -   Great opportunity for security issues
    
    May 2016 - HP Audio Drivers  
    
    -   Conexant audio chips
    -   Driver installation includes audio control software
    -   Debugging feature enables a keylogger
    
    Hardware interactions contain sensitive information  
    
    -   Video, keyboard, mouse

3.  Shimming

    Filling in the space between two objects  
    
    -   A middleman
    
    Windows includes it’s own shim  
    
    -   Backwards compatibility with previous Windows versions
    -   Application Compatibility Shim Cache
    
    Malware authors write their own shims  
    
    -   Get around security (like UAC)
    
    January 2015 Microsoft vulnerability  
    
    -   Elevates privilege

4.  Refactoring

    Metamorphic malware  
    
    -   A different program each time it’s downloaded
    
    Make it appear different each time  
    
    -   Add NOP instructions
    -   Loops, pointless code strings
    
    Can intelligently redesign itself  
    
    -   Reorder functions
    -   Modify the application flow
    -   Reorder code and insert unused data types
    
    Difficult to match with signature-based detection  
    
    -   Use a layered approach



### SSL stripping

Combines an on-path attack with a downgrade attack  

-   Difficult to implement, but big returns for the attacker

Attacker must sit in the middle of the conversation  

-   Must modify data between the victim and web server
-   Proxy server, ARP spoofing, rogue Wi-Fi hotspot, etc.

Victim does not see any significant problem  

-   Except the browser page isn’t encrypted
-   Strips the S away from HTTPS

This is a client and server problem  

-   Works on SSL and TLS
-   how: On-path attack Rewrites URLs HTTP/HTTPS

1.  Protection

    Avoid non encrypted communication (stick to HTTPS)  



### Race conditions

A programming conundrum  

-   Sometimes, things happen at the same time
-   This can be bad if you’ve not planned for it

Time-of-check to time-of-use attack (TOCTOU)  

-   Check the system
-   When do you use the results of your last check?
-   Something might happen between the check and the use



### Other applications attacks

1.  Memory vulnerabilities

    Manipulating memory can be advantageous (eg. for DOS)  
    
    -   Relatively difficult to accomplish
    
    Memory leak  
    
    -   Unused memory is not properly released
    -   Begins to slowly grow in size
    -   Eventually uses all available memory
    -   System crashes
    -   NULL Pointer dereference  
        -   Programming technique that references a portion of memory
        -   What happens if that reference points to nothing?
        -   Application crash, debug information displayed, DoS
    -   Integer overflow  
        -   Large number into a smaller sized space
        -   Where does the extra number go?
        -   You shouldn’t be able to manipulate memory this way

2.  Directory traversal

    Directory traversal / path traversal  
    
    -   Read files from a web server that are outside of the website’s file directory
    -   Users shouldn’t be able to browse the Windows folder
    
    Web server software vulnerability  
    
    -   Won’t stop users from browsing past the web server root
    
    Web application code vulnerability  
    
    -   Take advantage of badly written code
    
    `http://www.example.com/show.asp?view=../../Windows/system.ini HTTP/1l.1`  

3.  Improper error handling

    Errors happen  
    
    -   And you should probably know about it
    
    Messages should be just informational enough  
    
    -   Avoid too much detail
    -   Network information
    -   Memory dump
    -   Stack traces
    -   Database dumps
    
    This is an easy one to find and fix  
    
    -   A development best-practice

4.  Improper input handling

    Many applications accept user input  
    
    -   We put data in, we get data back
    
    All input should be considered malicious  
    
    -   Check everything. Trust nobody.
    
    Allowing invalid input can be devastating  
    
    -   SQL injections, buffer overflows, denial of service, etc.
    
    It takes a lot of work to find input that can be used maliciously  
    
    -   But they will find it

5.  API attacks

    API - Application Programming Interface  
    Attackers look for vulnerabilities in this new communication path  
    
    -   Exposing sensitive data, DoS, intercepted communication, privileged access

6.  Resource exhaustion

    A specialized DoS (Denial of Service) attack  
    
    -   May only require one device and low bandwidths
    
    ZIP bomb  
    
    -   A 42 kilobyte .zip compressed file
    -   Uncompresses to 4.5 petabytes (4,500 terabytes)
    -   Anti-virus will identify these
    
    DHCP starvation  
    
    -   Attacker floods a network with IP address requests
    -   MAC address changes each time
    -   DHCP server eventually runs out of addresses
    -   Switch configurations can rate limit DHCP requests



## Given a scenario, analyze potential indicators associated with network attacks



### Rogue Access Points and Evil Twins

1.  Rogue access points

    An unauthorized wireless access point  
    
    -   May be added by an employee or an attacker
    -   Not necessarily malicious
    -   A significant potential backdoor
    
    Very easy to plug in a wireless AP  
    
    -   Or enable wireless sharing.in your OS
    
    Schedule a periodic survey  
    
    -   Walk around your building/campus
    -   Use third-party tools / WAFi Pineapple
    
    Consider using 802.1X (Network Access Control)  
    
    -   You must authenticate, regardless of the connection type

2.  Wireless evil twins

    Looks legitimate, but actually malicious  
    
    -   The wireless version of phishing
    
    Configure an access point to look like an existing network  
    
    -   Same (or similar) SSID and security settings/captive portal
    
    Overpower the existing access points  
    
    -   May not require the same physical location
    
    WiFi hotspots (and users) are easy to fool  
    
    -   And they’re wide open
    
    You encrypt your communication, right?  
    
    -   Use HTTPS and a VPN



### Bluejacking and Bluesnarfing

1.  Bluejacking

    Sending of unsolicited messages to another device via Bluetooth  
    
    -   No mobile carrier required!
    
    Typical functional distance is about 10 meters  
    
    -   More or less, depending on antenna and interference
    
    Bluejack with an address book object  
    
    -   Instead of contact name, write a message  
        -   “You are Bluejacked!”
    -   “You are Bluejacked! Add to contacts?”
    
    Third-party software may also be used  
    
    -   Blooover, Bluesniff
    
    Low priority, only messages  

2.  Bluesnarfing

    Access a Bluetooth-enabled device and transfer data  
    
    -   Contact list, calendar, email, pictures, video, etc.
    
    First major security weakness in Bluetooth  
    
    -   Marcel Holtmann in September 2003 and
    
    Adam Laurie in November 2003  
    
    -   This weakness was patched
    
    Serious security issue  
    
    -   If you know the file, you can download it without authentication



### Wireless Disassociation Attacks

Surfing along on your wireless network  

-   And then you’re not

And then it happens again  

-   And again

You may not be able to stop it  

-   There’s (almost) nothing you can do
-   Time to get a long patch cable

Wireless deauthentication  

-   A significant wireless denial of service (DoS) attack

1.  802.11 management frames

    802.11 wireless includes a number of management  
    
    -   Frames that make everything work
    -   You never see them
    
    Important for the operation of 802.11 wireless  
    
    -   How to find access points, manage QoS, associate/disassociate with an access point, etc.
    
    Original wireless standards did not add protection for management frames  
    
    -   Sent in the clear
    -   No authentication or validation

2.  Protection

    IEEE has already addressed the problem YA  
    
    -   802.11w - July 2014
    
    Some of the important management frames are encrypted  
    
    -   Disassociate, deauthenticate, channel switch announcements, etc.
    
    Not everything is encrypted  
    
    -   Beacons, probes, authentication, association
    
    802.11w is required for 802.11ac compliance  
    
    -   This will roll out going forward



### Wireless jamming

Many different types  

-   Constant, random bits / Constant, legitimate frames
-   Data sent at random times - random data and legitimate frames
-   Reactive jamming - only when someone else tries to communicate

Needs to be somewhere close  

-   Difficult to be effective from a distance

Time to go fox hunting  

-   You’ll need the right equipment to hunt down the jam
-   Directional antenna, attenuator

1.  Radio frequency (RF) jamming

    Denial of Service  
    
    -   Prevent wireless communication
    
    Transmit interfering wireless signals  
    
    -   Decrease the sighal-to-noise ratio at the receiving device
    -   The receiving device can’t hear the good signal
    
    Sometimes it’s not intentional  
    
    -   Interference, not jamming
    -   Microwave oven, fluorescent lights
    
    Jamming is intentional  
    
    -   Someone wants your network to not work



### RFID and NFC Attacks

RFID (Radio-frequency identification) is everywhere  

-   Access badges
-   Inventory/Assembly line tracking
-   Pet/Animal identification
-   Anything that needs to be tracked

Radar technology  

-   Radio energy transmitted to the tag
-   RF powers the tag, ID is transmitted back
-   Bidirectional communication
-   Some tag formats can be active/powered

1.  RFID attacks

    Data capture  
    
    -   View communication
    -   Replay attack
    
    Spoof the reader  
    
    -   Write your own data to the tag
    
    Denial of service  
    
    -   Signal jamming
    
    Decrypt communication  
    
    -   Many default keys are on Google

2.  Near field communication (NFC)

    Two-way wireless communication  
    
    -   Builds on RFID, which is mostly one-way
    
    Payment systems  
    
    -   Many options available
    
    Bootstrap for other wireless  
    
    -   NFC helps with Bluetooth pairing
    
    Access token, identity “card”  
    
    -   Short range with encryption support
    
    1.  NFC security concerns
    
        Remote capture  
        
        -   It’s a wireless network
        -   10 meters for active devices
        
        Frequency jamming  
        
        -   Denial of service
        
        Relay / Replay attack  
        
        -   On-path attack
        
        Loss of RFC device control  
        
        -   Stolen/lost phone



### Randomizing Cryptography

Cryptography without randomization  

-   similar to the original data

1.  Cryptographic nonce

    Arbitrary number  
    
    -   Used once
    -   “For the nonce” - For the time being
    
    A random or pseudo-random number  
    
    -   Something that can’t be reasonably guessed
    -   Can also be a counter
    
    Use a nonce during the login process  
    
    -   Server gives you a honce
    -   Calculate your password hash using the nonce
    -   Each password hash sent to the host will be different, so a replay won’t work
    
    A type of nonce (initialization vector - IV)  
    
    -   Used for randomizing an encryption scheme
    -   The more random the better
    
    Used in encryption ciphers, WEP, and some SSL implementations  

2.  Salt

    A nonce most commonly associated with password randomization  
    
    -   Make the password hash unpredictable
    
    Password storage should always be salted  
    
    -   Each user gets a different salt



### On-path Attacks

How can an attacker watch without you knowing?  

-   Formerly known as man-in-the-middle

Redirects your traffic  

-   Then passes it on to the destination
-   You never know your traffic was redirected

ARP poisoning  

-   On-path attack on the local IP subnet
-   ARP has no security
-   poisons the ARP cache

1.  On-path browser attacks

    What if the middleman was on the same computer as the victim?  
    
    -   Malware/Trojan does all of the proxy work
    -   Formerly known as man-in-the-browser
    
    Huge advantages for the attackers  
    
    -   Relatively easy to proxy encrypted traffic
    -   Everything looks normal to the victim
    
    The malware in your browser waits for you to login to your bank ‘  
    
    -   And cleans you out



### MAC Flooding and Cloning

The MAC ADDRESS: Ethernet Media Access Control address  

-   The “physical” address of a network adapter
-   Unique to a device

48 bits / 6 bytes long  

-   Displayed in hexadecimal
-   the first 3 bytes are the Organizationally Unique |dentifier (OUI) (the manufacturer)
-   the last 3 bytes are the Network Interface Controller-Specific (the serial number)

1.  LAN switching

    Forward or drop frames  
    
    -   Based on the destination MAC address
    
    Gather a constantly updating list of MAC addresses  
    
    -   Builds the list based on the source MAC address of incoming traffic
    -   These age out periodically, often in 5 minutes
    
    Maintain a loop-free environment  
    
    -   Using Spanning Tree Protocol (STP)

2.  Learning the MACs

    Switches examine incoming traffic  
    
    -   Makes a note of the source MAC address
    
    Adds unknown MAC addresses to the MAC address table  
    
    -   Sets the output interface to the received interface (frame switching)

3.  MAC flooding

    The MAC table is only so big  
    Attacker starts sending traffic with different source MAC addresses  
    
    -   Force out the legitimate MAC addresses
    
    The table fills up  
    
    -   Switch begins flooding traffic to all interfaces
    
    This effectively turns the switch into a hub  
    
    -   All traffic is transmitted to all interfaces
    -   No interruption in traffic flows
    
    Attacker can easily capture all network traffic!  
    Flooding can be restricted in the switch’s port security settings  

4.  MAC cloning / MAC spoofing

    An attacker changes their MAC address to match the MAC address of an existing device  
    
    -   A clone / a spoof
    
    Circumvent filters  
    
    -   Wireless or wired MAC filters
    -   ldentify a valid MAC address and copy it
    
    Create a DoS  
    
    -   Disrupt communication to the legitimate MAC
    
    Easily manipulated through software  
    
    -   Usually a device driver option



### DNS attacks

1.  DNS poisoning / DNS spoofing

    Modify the DNS server  
    
    -   Requires some crafty hacking
    
    Modify the client host file  
    
    -   The host file takes precedent over DNS queries
    
    Send a fake response to a valid DNS request  
    
    -   Requires a redirection of the original request or the resulting response

2.  DNS hijacking

    Get access to the domain registration, and you have control where the traffic flows  
    
    -   You don’t need to touch the actual servers
    -   Determines the DNS names and DNS IP addresses
    
    Many ways to get into the account  
    
    -   Brute force
    -   Social engineer the password
    -   Gain access to the email address that manages the account
    -   The usual things

3.  URL hijacking

    Make money from your mistakes  
    
    -   There’s a lot of advertising on the ‘net
    
    Sell the badly spelled domain to the actual owner  
    
    -   Sell a mistake
    
    Redirect to a competitor  
    
    -   Not as common, legal issues
    
    Phishing site  
    
    -   Looks like the real site, please login
    
    Infect with a drive-by download  
    
    -   You’ve got malware!
    
    1.  Types of URL hijacking
    
        Typosquatting / brandjacking  
        
        -   Take advantage of poor spelling
        
        Outright misspelling  
        
        -   professormesser.com VS. professormessor.com
        
        A typing error  
        
        -   professormeser.com
        
        A different phrase  
        
        -   professormessers.com
        
        Different top-level domain  
        
        -   professormesser.org

4.  Domain reputation

    The Internet is tracking your security posture  
    
    -   They know when things go sideways
    
    Email reputation  
    
    -   Suspicious activity
    -   Malware originating from the IP address
    
    A bad reputation can cause email delivery to fail  
    
    -   Email rejection or simply dropped
    
    Check with the email or service provider to check the reputation  
    
    -   Follow their instructions to remediate
    
    Infected systems are noticed by the search engines  
    
    -   Your domain can be flagged or removed
    
    Users will avoid the site  
    
    -   Sales will drop
    -   Users will avoid your brand
    
    Malware might be removed quickly  
    
    -   Recovery takes much longer



### Denial of Service

Force a service to fail  

-   Overload the service

Take advantage of a design failure or vulnerability  

-   Keep your systems patched!

Cause a system to be unavailable  

-   Competitive advantage

Create a smokescreen for some other exploit  

-   Precursor to a DNS spoofing attack

Doesn’t have to be complicated  

-   Turn off the power

1.  A &ldquo;friendly&rdquo; DoS

    Unintentional DoSing  
    
    -   It’s not always a ne’er-do-well
    
    Network DoS  
    
    -   Layer 2 loop without STP
    
    Bandwidth DoS  
    
    -   Downloading multi-gigabyte Linux distributions over a DSL line
    
    The water line breaks  
    
    -   Get a good shop vacuum

2.  Distributed Denial of Service (DDoS)

    Launch an army of computers to bring down a service  
    
    -   Use all the bandwidth or resources - traffic spike
    
    This is why the attackers have botnets  
    
    -   Thousands or millions of computers at your command
    -   At its peak, Zeus botnet infected over 3.6 million PCs
    -   Coordinated attack
    
    Asymmetric threat  
    
    -   The attacker may have fewer resources than the victim

3.  DDoS amplification

    Turn your small attack into a big attack  
    
    -   Often reflected off another device or service
    
    An increasingly common network DDoS technique  
    
    -   Turn Internet services against the victim
    
    Uses protocols with little (if any)  
    authentication or checks  
    
    -   NTP, DNS, ICMP .
    -   A common example of protocol abuse
    -   eg: DNS amplification DDoS

4.  Application DoS

    Make the application break or work harder  
    
    -   Increase downtime and costs
    
    Fill the disk space 3  
    
    -   A 42 kilobyte .zip compressed file
    -   Uncompresses to 4.5 petabytes (4,500 terabytes)
    -   Anti-virus will identify these
    
    Overuse a measured cloud resource  
    
    -   More CPU/memory/network is more money
    
    Increase the cloud server response time  
    
    -   Victim deploys a new application instance
    -   Repeat

5.  Operational Technology (OT) DoS

    The hardware and software for industrial equipment  
    
    -   Electric grids, traffic control, manufacturing plants, etc.
    
    This is more than a web server failing  
    
    -   Power grid drops offline
    -   All traffic lights are green
    -   Manufacturing plant shuts down
    
    Requires a different approach  
    
    -   A much more critical security posture



### Malicious scripts

1.  Scripting and automation

    Automate tasks  
    
    -   You don’t have to be there
    -   Solve problems in your sleep
    -   Monitor and resolve problems before they happen
    
    The need for speed  
    
    -   The script is as fast as the computer
    -   No typing or delays
    -   No human error
    
    Automate the attack  
    
    -   The hacker is on borrowed time

2.  Windows PowerShell

    Command line for system administrators  
    
    -   .ps1 file extension
    -   Included with Windows 8/8.1 and 10
    
    Extend command-line functions  
    
    -   Uses cmdlets (command-lets)
    -   PowerShell scripts and functions
    -   Standalone executables
    
    Attack Windows systems  
    
    -   System administration
    -   Active Domain administration
    -   File share access

3.  Python

    General-purpose scripting language  
    
    -   .py file extension
    
    Popular in many technologies  
    
    -   Broad appeal and support
    
    Commonly used for cloud orchestration  
    
    -   Create and tear down application instances
    
    Attack the infrastructure  
    
    -   Routers, servers, switches

4.  Shell script

    Scripting the Unix/Linux shell  
    
    -   Automate and extend the command line
    -   Bash, Bourne, Korn, C
    
    Starts with a shebang or hash-bang #!  
    
    -   Often has a .sh file extension
    
    Attack the Linux/Unix environment  
    
    -   Web, database, virtualization servers
    
    Control the OS from the command line  
    
    -   Malware has a lot of options

5.  Macros

    Automate functions within an application  
    
    -   Or operating system
    
    Designed to make the application easier to use  
    
    -   Can often create security vulnerabilities
    
    Attackers create automated exploits  
    
    -   They just need the user to open the file
    -   Prompts to run the macro

6.  Visual Basic for Applications (VBA)

    Automates Processes within Windows applications  
    
    -   Common in Microsoft Office
    
    A powerful programming language  
    
    -   Interacts with the operating system
    
    CVE-2010-0815 / MS10-031  
    
    -   VVBA does not properly search for ActiveX controls in a document
    -   Run arbitrary code embedded in a document
    -   Easy to infect a computer



## Explain different threat actors, vectors, and intelligence sources



### Threat Actors

The entity responsible for an event that has an impact on the safety of another entity  

-   Also called a malicious actor

Broad scope of actors  

-   And motivations vary widely

Advanced Persistent Threat (APT)  

-   Attackers are in the network and undetected
-   2018 Firekye report:  
    -   Americas: 71 days,
    -   EMEA: 177 days,
    -   APAC: 204 days

1.  Insiders

    More than just passwords on sticky notes  
    
    -   Some insiders are out for no good
    
    Sophistication may not be advanced, but the insider has institutional knowledge  
    
    -   Attacks can be directed at vulnerable systems
    -   The insider knows what to hit
    
    Extensive resources  
    
    -   Eating away from the inside

2.  Nation states

    Governments  
    
    -   National security, job security
    -   Always an external entity
    
    Highest sophistication  
    
    -   Mlilitary control, utilities, financial control
    -   United States and Israel destroyed 1,000 nuclear centrifuges with the Stuxnet worm
    
    Constant attacks, massive resources  
    
    -   Commonly an Advanced Persistent Threat (APT)

3.  Hacktivist

    A hacker with a purpose  
    
    -   Social change or a political agenda
    -   Often an external entity
    
    Can be remarkably sophisticated  
    
    -   Very specific hacks
    -   DoS, web site defacing, release of private documents, etc.
    
    Funding is limited  
    
    -   Some organizations have fundraising options

4.  Script kiddies

    Runs pre-made scripts without any knowledge of what’s really happening  
    
    -   Not necessarily a youngster
    
    Can be internal or external  
    
    -   But usually external
    
    Not very sophisticated  
    No formal funding  
    
    -   Looking for low hanging fruit
    
    Motivated by the hunt  
    
    -   Working the ego, trying to make a name

5.  Organized crime

    Professional criminals  
    
    -   Motivated by money
    -   Almost always an external entity
    
    Very sophisticated  
    
    -   Best hacking money can buy
    
    Crime that&rsquo;s organized  
    
    -   One person hacks, one person manages the exploits, another person sells the data, another handles customer support
    
    Lots of capital to fund hacking efforts  

6.  Hackers

    Experts with technology  
    
    -   Often driven by money, power, and ego
    
    Authorized  
    
    -   An ethical hacker with good intentions
    -   And permission to hack
    
    Unauthorized  
    
    -   Malicious
    -   Violates security for personal gain
    
    Semi-authorized  
    
    -   Finds a vulnerability
    -   Doesn’t use it

7.  Shadow IT

    Going rogue  
    
    -   Working around the internal IT organization
    
    Information Technology can put up roadblocks  
    
    -   Shadow IT is unencumbered
    -   Use the cloud
    -   Might also be able to innovate
    
    Not always a good thing  
    
    -   Wasted time and money
    -   Security risks
    -   Compliance issues
    -   Dysfunctional organization

8.  Competitors

    Many different motivations  
    
    -   DoS, espionage, harm reputation
    
    High level of sophistication  
    
    -   Based on some significant funding
    -   The competitive upside is huge (and very unethical)
    
    Many different intents  
    
    -   Shut down your competitor during an event
    -   Steal customer lists
    -   Corrupt manufacturing databases
    -   Take financial information



### Attack Vectors

A method used by the attacker  

-   Gain access or infect to the target

A lot of work goes into finding vulnerabilities in these vectors  

-   Some are more vulnerable than others

IT security professional spend their career watching these vectors  

-   Closing up existing vectors
-   Finding new ones

1.  Direct access attack vectors

    There’s a reason we lock the data center  
    
    -   Physical access to a system is a significant attack vector
    
    Modify the operating system  
    
    -   Reset the administrator password in a few minutes
    
    Attach a keylogger  
    
    -   Collect usernames and passwords
    
    Transfer files  
    
    -   Take it with you
    
    Denial of service  
    
    -   This power cable is in the way

2.  Wireless attack vectors

    Default login credentials  
    
    -   Modify the access point configuration
    
    Rogue access point  
    
    -   A less-secure entry point to the network
    
    Evil twin  
    
    -   Attacker collects authentication details
    -   On-path attacks
    
    Protocol vulnerabilities  
    
    -   2017 - WPA2 Key Reinstallation Attack (KRACK)
    -   Older encryption protocols (WEP, WPA)

3.  Email attack vectors

    One of the biggest (and most successful) attack vectors  
    
    -   Everyone has email
    
    Phishing attacks  
    
    -   People want to click links
    
    Deliver the malware to the user ..  
    
    -   Attach it to the message
    
    Social engineering attacks  
    
    -   Invoice scam

4.  Supply chain attack vectors

    Tamper with the underlying infrastructure  
    
    -   Or manufacturing process
    
    Gain access to a network using a vendor  
    
    -   2013 Target credit card breach
    
    Malware can modify the manufacturing process  
    
    -   2010 - Stuxnet disrupts Iran’s uranium enrichment program
    
    Counterfeit networking equipment  
    
    -   Install backdoors, substandard performance and availability
    -   2020 - Fake Cisco Catalyst 2960-X and WS-2960X-48TS-L

5.  Social media attack vectors

    Attackers thank you for putting your personal information online  
    
    -   Where you are and when
    -   Vacation pictures are especially telling
    
    User profiling (eg for MFA or pwd reset)  
    
    -   Where were you born?
    -   What is the name of your school mascot?
    
    Fake friends are fake  
    
    -   The inner circle can provide additional information

6.  Removable media attack vectors

    Get around the firewall  
    
    -   The USB interface
    
    Malicious software on USB flash drives  
    
    -   Infect air gapped networks
    -   Industrial systems, high-security services
    
    USB devices can act as keyboards  
    
    -   Hacker on a chip
    
    Data exfiltration  
    
    -   Terabytes of data walk out the door
    -   Zero bandwidth used

7.  Cloud attack vectors

    Publicly-facing applications and services  
    
    -   Mistakes are made all the time
    
    Security misconfigurations  
    
    -   Data permissions and public data stores
    
    Brute force attacks  
    
    -   Or phish the users of the cloud service
    
    Orchestration attacks  
    
    -   Make the cloud build new application instances
    
    Denial of service  
    
    -   Disable the cloud services for everyone



### Threat Intelligence

Research the threats  

-   And the threat actors

Data is everywhere  

-   Hacker group profiles, tools used by the attackers, and much more

Make decisions based on this intelligence  

-   Invest in the best prevention

Used by researchers, security operations teams, and others  

1.  Open-source intelligence (OSINT)

    Open-source  
    
    -   Publicly available sources
    -   A good place to start
    
    Internet  
    
    -   Discussion groups, social media
    
    Government data  
    
    -   Mostly public hearings, reports, websites, etc.
    
    Commercial data  
    
    -   Maps, financial reports, databases

2.  Closed/proprietary intelligence

    Someone else has already compiled the threat information  
    
    -   You can buy it
    
    Threat intelligence services  
    
    -   Threat analytics
    -   Correlation across different data sources
    
    Constant threat monitoring  
    
    -   ldentify new threats
    -   Create automated prevention workflows

3.  Vulnerability databases

    Researchers find vulnerabilities  
    
    -   Everyone needs to know about them
    
    Common Vulnerabilities and Exposures (CVE)  
    
    -   A community managed list of vulnerabilities
    -   Sponsored by the U.S. Department of Homeland Security (DHS) and Cybersecurity and Infrastructure Security Agency (CISA)
    
    U.S. National Vulnerability Database (NVD)  
    
    -   A summary of CVEs
    -   Also sponsored by DHS and CISA - <https://nvd.nist.gov/>
    
    NVD provides additional details over the CVE list  
    
    -   Patch availability and severity scoring

4.  Public/private information-sharing centers

    Public threat intelligence  
    
    -   Often classified information
    
    Private threat intelligence  
    
    -   Private companies have extensive resources
    
    Need to share critical security details  
    
    -   Real-time, high-quality cyber threat information sharing
    
    Cyber Threat Alliance (CTA)  
    
    -   Members upload specifically formatted threat intelligence
    -   CTA scores each submission and validates across other submissions
    -   Other members can extract the validated data

5.  Automated indicator sharing (AlS)

    Intelligence industry needs a standard way to share important threat data  
    
    -   Share information freely
    
    Structured Threat Information eXpression (STIX)  
    
    -   Describes cyber threat information
    -   Includes motivations, abilities, capabilities, and response information
    
    Trusted Automated eXchange of Indicator Information (TAXII)  
    
    -   Securely shares STIX data

6.  Dark web Intelligence

    Dark web  
    
    -   Overlay networks that use the Internet
    -   Requires specific software and configurations to access
    
    Hacking groups and services  
    
    -   Activities
    -   Tools and techniques
    -   Credit card sales
    -   Accounts and passwords
    
    Monitor forums for activity  
    
    -   Company names, executive names

7.  Indicators of compromise (I0C)

    An event that indicates an intrusion  
    
    -   Confidence is high
    -   He’s calling from inside the house
    
    Indicators  
    
    -   Unusual amount of network activity
    -   Change to file hash values
    -   Irregular international traffic
    -   Changes to DNS data
    -   Uncommon login patterns
    -   Spikes of read requests to certain files

8.  Predictive analysis

    Analyze large amounts of data very quickly  
    
    -   Find suspicious patterns
    -   Big data used for cybersecurity
    
    Identify behaviors  
    
    -   DNS queries, traffic patterns, location data
    -   An early-warning system
    
    Often combined with machine learning  
    
    -   Less emphasis on signatures

9.  Threat maps

    Identify attacks and trends  
    
    -   View worldwide perspective

10. File/code repositories

    See what the hackers are building  
    
    -   Public code repositories
    -   GitHub
    
    See what people are accidentally releasing  
    
    -   Private code can often be published publicly
    
    Attackers are always  
    looking for this code  
    
    -   Potential exploits exist
    -   Content for phishing attacks



### Threat Research

Know your enemy  

-   And their tools of war

A never-ending process  

-   The field is constantly moving and changing

Information from many different places  

-   You can’t rely on a single source

1.  Vendor websites

    Vendors and manufacturers  
    
    -   They wrote the software
    
    They know when problems are announced  
    
    -   Most vendors are involved in the disclosure process
    -   They know their product better than anyone
    
    They react when surprises happen  
    
    -   Scrambling after a zero-day announcement
    -   Mitigating and support options

2.  Vulnerability feeds

    Automated vulnerability notifications  
    
    -   National Vulnerability Database (<https://nvd.nist.gov>)
    -   CVE Data Feeds (<https://cve.mitre.org>)
    
    Third-    party feeds  
    
    -   Additional vulnerability coverage
    
    Roll-    up to a vulnerability management system  
    
    -   Coverage across teams
    -   Consolidated view of security issues

3.  Conferences

    Watch and learn  
    
    -   An early warning of things to come
    
    Researchers  
    
    -   New DDoS methods
    -   Intelligence gathering
    -   Hacking the latest technologies
    
    Stories from the trenches  
    
    -   Fighting and recovering from attacks
    -   New methods to protect your data
    
    Building relationships  
    
    -   Forge alliances

4.  Academic journals

    Research from academic professionals  
    
    -   Cutting edge security analysis
    
    Evaluations of existing security technologies  
    
    -   Keeping up with the latest attack methods
    
    Detailed post mortem  
    
    -   Tear apart the latest malware and see what makes it tick
    
    Extremely detailed information  
    
    -   Break apart topics into their smaller pieces

5.  Request for comments (RFC)

    Published by the Internet Society (ISOC)  
    
    -   Often written by the Internet Engineering Task Force (IETF)
    -   Internet Society description is RFC 1602
    
    Not all RFCs are standards documents  
    
    -   Experimental, Best Current Practice, Standard Track, and Historic
    
    Many informational RFCs analyze threats  
    
    -   RFC 3833 - Threat Analysis of the Domain Name System
    -   RFC 7624 - Confidentiality in the Face of Pervasive Surveillance: A Threat Model and Problem Statement

6.  Local industry groups

    A gathering of local peers  
    
    -   Shared industry and technology
    -   Geographical presence
    
    Associations  
    
    -   Information Systems Security Association,
    
    Network Professional Association  
    
    -   Meet others in the area
    -   Discuss local challenges
    
    Industry user groups  
    
    -   Cisco, Microsoft, VMware, etc.
    -   Secure specific technologies

7.  Social media

    Hacking group conversations  
    
    -   Monitor the chatter
    
    Honeypot monitoring on Twitter  
    
    -   ldentify new exploit attempts
    
    Keyword monitoring  
    
    -   CVE-2020-\*, bugbounty, 0-day
    
    Analysis of vulnerabilities  
    
    -   Professionals discussing the details
    
    Command and control  
    
    -   Use social media as the transport

8.  Threat feeds

    Monitor threat announcements  
    
    -   Stay informed
    
    Many sources of information  
    
    -   U.S. Department of Homeland Security
    -   U.S. Federal Bureau of Investigation
    -   SANS Internet Storm Center
    -   VirusTotal Intelligence: Google and Facebook correlation

9.  TTP

    Tactics, techniques, and procedures A  
    
    -   What are adversaries doing and how are they doing it?
    
    Search through data and networks  
    
    -   Proactively look for threats
    -   Signatures and firewall rules can’t catch everything
    
    Different types of TTPs  
    
    -   Information on targeted victims (Finance for energy companies)
    -   Infrastructure used by attackers (DNS and IP addresses)
    -   Outbreak of a particular malware variant on a service type



## Explain the security concerns associated with various types of vulnerabilities



### Vulnerability Types

1.  Zero-day attacks

    Many applications have vulnerabilities \_  
    
    -   We&rsquo;ve just not found them yet
    
    Someone is working hard to find the next big vulnerability  
    
    -   The good guys share these with developers
    
    Attackers keep these yet-to-be-discovered holes to themselves  
    
    -   They want to use these vulnerabilities for personal gain
    
    Zero-day  
    
    -   The vulnerability has not been detected or published
    -   Zero-day exploits are increasingly common
    
    Common Vulnerabilities and Exposures (CVE)  
    
    -   <http://cve.mitre.org/>

2.  Open permissions

    Very easy to leave a door open  
    
    -   The hackers will always find it
    
    Increasingly common with cloud storage  
    
    -   Statistical chance of finding an open permission
    
    June 2017 - 14 million Verizon records exposed  
    
    -   Third-party left an Amazon S3 data repository open
    -   Researcher found the data before anyone else
    
    Many, many other examples  
    
    -   Secure your permissions!

3.  Unsecured root accounts

    The Linux root account  
    
    -   The Administrator or superuser account
    
    Can be a misconfiguration  
    
    -   Intentionally configuring an easy-to-hack password
    -   123456, ninja, football
    
    Disable direct login to the root account  
    
    -   Use the su or sudo option
    
    Protect accounts with root or administrator access  
    
    -   There should not be a lot of these

4.  Errors

    Error messages can provide useful information to an attacker  
    
    -   Service type, version information, debug data
    
    September 2015 - Patreon is compromised  
    
    -   Used a debugger to help monitor and Yroubleshoot web site issues
    -   Was left exposed to the Internet
    -   Effectively allowed for remote code executions
    -   Gigabytes of customer data was released online

5.  Weak encryption

    Encryption protocol (AES, 3DES, etc.)  
    
    -   Length of the encryption key (40 bits, 128 bits, 256 bits, etc.)
    -   Hash used for the integrity check (SHA, MD5, etc.)
    -   Wireless encryption (WEP, WPA)
    
    Some cipher suites are easier to break than others  
    
    -   Stay updated with the latest best practices
    
    TLS is one of the most common issues  
    
    -   Over 300 cipher suites
    
    Which are good and which are bad?  
    
    -   Weak or null encryption (less than 128 bit key sizes), outdated hashes (MD5)

6.  Insecure protocols

    Some protocols aren&rsquo;t encrypted  
    
    -   All traffic sent in the clear
    -   Telnet, FTP, SMTP, IMAP
    
    Verify with a packet capture  
    
    -   View everything sent over the network
    
    Use the encrypted versions  
    
    -   SSH, SFTP, IMAPS, etc.

7.  Default settings

    Every application and network  
    device has a default login  
    
    -   Not all of these are ever changed
    
    Mirai botnet  
    
    -   Takes advantage of default configurations
    -   Takes over Internet of Things (loT) devices
    -   60+ default configurations
    -   Cameras, routers, doorbells, garage door openers, etc.
    
    Mirai released as open-source software  
    
    -   There’s a lot more where that came from

8.  Open ports and services

    Services will open ports  
    
    -   It’s important to manage access
    
    Often managed with a firewall  
    
    -   Manage traffic flows
    -   Allow or deny based on port number or application
    
    Firewall rulesets can be complex  
    
    -   It’s easy to make a mistake
    
    Always test and audit  
    
    -   Double and triple check

9.  Improper patch management

    Often centrally managed  
    
    -   The update server determine when you patch
    -   Test all of your apps, then deploy
    -   Efficiently manage bandwidth
    
    Firmware  
    
    -   The BIOS of the device
    
    Operating system  
    
    -   Monthly and on-demand patches
    
    Applications  
    
    -   Provided by the manufacturer as-needed

10. Legacy platforms

    Some devices remain installed for a long time  
    
    -   Perhaps too long
    
    Legacy devices  
    
    -   Older operating systems, applications, middleware
    
    May be running end-of-life software  
    
    -   The risk needs to be compared to the return
    
    May require additional security protections  
    
    -   Additional firewall rules
    -   IPS signature rules for older operating systems 3&



### Third-party Risks

IT security doesn’t change because it’s a third-party  

-   There should be more security, not less

Always expect the worst  

-   Prepare for a breach

Human error is still the biggest issue  

-   Everyone needs to use IT security best practices

All security is important  

-   Physical security and cybersecurity work hand-in-hand

1.  System integration risk

    Professional installation and maintenance  
    
    -   Can include elevated OS access
    
    Can be on-site  
    
    -   With physical or virtual access to data and systems
    -   Keylogger installations and USB flash drive data transfers
    
    Can run software on the internal network 4  
    
    -   Less security on the inside
    -   Port scanners, traffic captures
    -   Inject malware and spyware  
        -   Sometimes inadvertently

2.  Lack of vendor support

    Security requires diligence  
    
    -   The potential for a vulnerability is always there
    
    Vendors are the only ones who can fix their products  
    
    -   Assuming they know about the problem
    -   And care about fixing it

3.  Supply chain risk

    You can’t always control security at a third-party location  
    
    -   Always maintain local security controls
    
    Hardware and software from a vendor can contain malware  
    
    -   Verify the security of new systems
    
    Counterfeit hardware is out there  
    
    -   It looks like a Cisco switch&#x2026;
    -   Is it malicious?

4.  Outsourced code development

    Accessing the code base  
    
    -   Internal access over a VPN
    -   Cloud-based access
    
    Verify security to other systems  
    
    -   The development systems should be isolated
    
    Test the code security  
    
    -   Check for backdoors
    -   Validate data protection and encryption

5.  Data storage

    Consider the type of data  
    
    -   Contact information
    -   Healthcare details, financial information
    
    Storage at a third-party may need encryption  
    
    -   Limits exposure
    -   Adds complexity
    
    Transferring data  
    
    -   The entire data flow needs to be encrypted



### Vulnerability Impacts

Malicious cyber activity cost the U.S. economy between S$S57 billion and $109 billion in 2016  

-   The Cost of Malicious Cyber Activity to the U.S. Economy, The Council of Economic Advisers, February 2018

Many other non-economic impacts  

-   Far reaching effects

These are the reasons we patch vulnerabilities  

1.  Data loss

    Vulnerability: Unsecured databases  
    
    -   No password or default password
    
    July 2020 - Internet-facing databases are being deleted  
    
    -   No warning, no explanation
    
    Thousands of databases are missing  
    
    -   hope you had a backup
    
    Overwrites data with iterations of the word “meow”  
    
    -   No messages or motivational content

2.  Identity theft

    May through July 2017 - Equifax  
    
    -   Data breach of 147.9 million Americans,
    
    15.2 inillion British citizens, 19,000 Canadian citizens  
    
    -   Names, SSNs, birthdates, addresses, some driver’s license numbers
    
    Apache Struts vulnerability from March 7, 2017  
    
    -   Breach started March 12th &rsquo; ’
    -   Wasn’t patched by Equifax until July 30th after discovering “suspicious network traffic”
    -   September 7th - Public disclosure
    
    September 15th - CIO and CSO depart Equifax  

3.  Reputation impacts

    Getting hacked isn’t a great look 8  
    
    -   Organizations are often required to disclose
    -   Stock prices drop, at least for the short term
    
    October 2016 - Uber breach  
    
    -   25.6 million Names, email addresses, mobile phone numbers
    
    Didn’t publicly announce it until November 2017  
    
    -   Allegedly paid the hackers $100,000 and had them sign an NDA
    -   2018 - Uber paid $148 million in fines
    
    Hackers pleaded guilty in October 2019  
    
    -   August 2020 - Uber’s former Chief Security Officer charged with obstruction of justice and misprision of a felony

4.  Availability loss

    Outages and downtime  
    
    -   Systems are unavailable
    
    The pervasive ransomware threat  
    
    -   Brings down the largest networks
    
    September 2020 - BancoEstado  
    
    -   One of Chile’s three biggest banks
    -   Ransomware attack over the weekend
    
    Bank closed for an extended period  
    
    -   Segmented network - Only hit internal systems
    -   Wipe and restore everything



## Summarize the techniques used in security assessments



### Threat Hunting

The constant game of cat and mouse  

-   Find the attacker before they find you

Strategies are constantly changing  

-   Firewalls get stronger, so phishing gets better

Intelligence data is reactive  

-   You can’t see the attack until it happens

Speed up the reaction time  

-   Use technology to fight

1.  Intelligence fusion

    An overwhelming amount of security data  
    
    -   Too much data to properly detect, analyze, and react
    
    Many data types  
    
    -   Dramatically different in type and scope
    
    Separate teams  
    
    -   Security operations, security intelligence, threat response
    
    Fuse the security data together with big data analytics  
    
    -   Analyze massive and diverse datasets
    -   Pick out the interesting data points and correlations -

2.  Fusing the data

    Collect the data  
    
    -   Logs and sensors, network information, Internet events, intrusion detection
    
    Add external sources  
    
    -   Threat feeds, governmental alerts, advisories and bulletins, social media
    
    Correlate with big data analytics  
    
    -   Focuses on predictive analytics and user behavior analytics
    -   Mathematical analysis of unstructured data

3.  Cybersecurity maneuvers

    In the physical world, move troops and tanks  
    
    -   Stop the enemy on a bridge or shore
    
    In the virtual world, move firewalls and operating systems  
    
    -   Set a firewall rule, block an IP address, delete malicious software
    
    Automated maneuvers  
    
    -   Moving at the speed of light
    -   The computer reacts instantly
    
    Combine with fused intelligence  
    
    -   Ongoing combat from many fronts
    
    Tomorrow it’s a different fight  



### Vulnerability Scans

Usually minimally invasive  

-   Unlike a penetration test

Port scan  

-   Poke around and see what’s open

ldentify systems  

-   And security devices

Test from the outside and inside  

-   Don’t dismiss insider threats

Gather as much information as possible  

-   We’ll separate wheat from chaff later

1.  Scan types

    Scanners are very powerful  
    
    -   Use many different techniques to identify vulnerabilities
    
    Non-intrusive scans  
    
    -   Gather information, don’t try to exploit a vulnerability
    
    Intrusive scans  
    
    -   You&rsquo;ll try out the vulnerability to see if it works
    
    Non-credentialed scans  
    
    -   The scanner can’t login to the remote device
    
    Credentialed scan  
    
    -   You’&rsquo;re a normal user, emulates an insider attack

2.  Identify vulnerabilities

    The scanner looks for everything  
    
    -   Well, not everything - The signatures are the key
    
    Application scans  
    
    -   Desktop, mobile apps
    
    Web application scans  
    
    -   Software on a web server
    
    Network scans  
    
    -   Misconfigured firewalls, open ports, vulnerable devices

3.  Vulnerability research

    The vulnerabilities can be cross-referenced online  
    
    -   Almost all scanners give you a place to go
    
    National Vulnerability Database: <http://nvd.nist.gov/>  
    Common Vulnerabilities and Exposures (CVE): <https://cve.mitre.org/cve/>  
    Microsoft Security Bulletins: <http://www.microsoft.com/technet/security/current.aspx>  
    Some vulnerabilities cannot be definitively identified  
    
    -   You’ll have to check manually to see if a system is vulnerable ‘
    -   The scanner gives you a heads-up
    
    National Vulnerability Database: <http://nvd.nist.gov/>  
    
    -   Synchronized with the CVE list
    -   Enhanced search functionality
    
    Common Vulnerability Scoring System (CVSS)  
    
    -   Quantitative scoring of a vulnerability - 0 to 10
    -   The scoring standards change over time
    -   Different scoring for CVSS 2.0 vs CVSS 3.x
    
    Industry collaboration  
    
    -   Enhanced feed sharing and automation

4.  Vulnerabilitv scan log review

    Lack of security controls  
    
    -   No firewall
    -   No anti-virus
    -   No anti-spyware
    
    Misconfigurations  
    
    -   Open shares
    -   Guest access
    
    Real vulnerabilities  
    
    -   Especially newer ones
    -   Occasionally the old ones

5.  Dealing with false positives

    False positives  
    
    -   A vulnerability is identified that doesn’t really exist
    
    This is different than a low-severity vulnerability  
    
    -   It’s real, but it may not be your highest priority
    
    False negatives  
    
    -   A vulnerability exists, but you didn’t detect it
    
    Update to the latest signatures  
    
    -   If you don’t know about it, you can’t see it
    
    Work with the vulnerability detection manufacturer  
    
    -   They may need to update their signatures for your environment

6.  Configuration review

    Validate the security of device configurations  
    
    -   It’s easy to misconfigure one thing
    -   A single unlocked window puts the entire home at risk
    
    Workstations  
    
    -   Account configurations, local device settings
    
    Servers  
    
    -   Access controls, permission settings
    
    Security devices  
    
    -   Firewall rules, authentication options



### Security Information and Event Management

1.  SIEM

    Security Information and Event Management  
    
    -   Logging of security events and information
    
    Log collection of security alerts  
    
    -   Real-time information
    
    Log aggregation and long-term storage  
    
    -   Usually includes advanced reporting features
    
    Data correlation  
    
    -   Link diverse data types
    
    Forensic analysis  
    
    -   Gather details after an event

2.  Syslog

    Standard for message logging  
    
    -   Diverse systems, consolidated log
    
    Usually a central log collector  
    
    -   Integrated into the SIEM
    
    You&rsquo;re going to need a lot of disk space  
    
    -   No, more. More than that.
    -   Data storage from many devices over an extended timeframe

3.  SIEM data

    Data inputs  
    
    -   Server authentication attempts
    -   VPN connections
    -   Firewall session logs
    -   Denied outbound traffic flows
    -   Network utilizations
    
    Packet captures  
    
    -   Network packets
    -   Often associated with a critical alert
    -   Some organizations capture everything

4.  Security monitoring

    Constant information flow  
    
    -   Important metrics in the incoming logs
    
    Track important statistics  
    
    -   Exceptions can be identified
    
    Send alerts when problems are found  
    
    -   Email, text, call, etc.
    
    Create triggers to automate responses  
    
    -   Open a ticket, reboot a server

5.  Analyzing the data

    Big data analytics  
    
    -   Analyze large data stores
    -   Identify patterns that would normally remain invisible
    
    User and entity behavior analytics (UEBA)  
    
    -   Detect insider threats
    -   Identify targeted attacks
    -   Catches what the SIEM and DLP systems might miss
    
    Sentiment analysis  
    
    -   Public discourse correlates to real-world behavior
    -   If they hate you, they hack you
    -   Social media can be a barometer

6.  SOAR

    Security orchestration, automation, and response  
    
    -   Automate routine, tedious, and time intensive activities
    
    Orchestration  
    
    -   Connect many different tools together
    -   Firewalls, account management, email filters
    
    Automation  
    
    -   Handle security tasks automatically
    
    Response  
    
    -   Make changes immediately



## Explain the techniques used in penetration testing



### Penetration testing

Pentest  

-   Simulate an attack

Similar to vulnerability scanning  

-   Except we actually try to exploit the vulnerabilities

Often a compliance mandate  

-   Regular penetration testing by a 3rd-party

National Institute of Standards and Technology Technical Guide to Information Security Testing and Assessment  

-   <https://professormesser.link/800115> (PDF download)

1.  Rules of engagement

    An important document  
    
    -   Defines purpose and scope
    -   Makes everyone aware of the test parameters
    
    Type of testing and schedule  
    
    -   On-site physical breach, internal test, external test
    -   Normal working hours, after 6 PM only, etc.
    
    The rules  
    
    -   IP address ranges
    -   Emergency contacts
    -   How to handle sensitive information
    -   In-scope and out-of-scope devices or applications

2.  Working knowledge

    How much do you know about the test?  
    
    -   Many different approaches
    
    Unknown environment  
    
    -   The pentester knows nothing about the systems under attack
    -   “Blind” test
    
    Known environment  
    
    -   Full disclosure
    
    Partially known environment  
    
    -   A mix of known and unknown
    -   Focus on certain systems or applications

3.  Exploiting vulnerabilities

    Try to break into the system  
    
    -   Be careful; this can cause a denial of service or loss of data
    -   Buffer overflows can cause instability
    -   Gain privilege escalation
    
    You may need to try many different vulnerability types  
    
    -   Password brute-force
    -   Social engineering
    -   Database injections
    -   Buffer overflows
    
    You’ll only be sure you’re vulnerable if you can bypass security  
    
    -   If you can get through, the attackers can get through

4.  The process

    Initial exploitation  
    
    -   Get into the network
    
    Lateral movement  
    
    -   Move from system to system
    -   The inside of the network is relatively unprotected
    
    Persistence  
    
    -   Once you’re there, you need to make sure there’s a way back in
    -   Set up a backdoor, build user accounts, change or verify default passwords
    
    The pivot  
    
    -   Gain access to systems that would normally not be accessible
    -   Use a vulnerable system as a proxy or relay

5.  Pentest aftermath

    Cleanup  
    
    -   Leave the network in its original state
    -   Remove any binaries or temporary files
    -   Remove any backdoors
    -   Delete user accounts created during the test
    
    Bug bounty  
    
    -   A reward for discovering vulnerabilities
    -   Earn money for hacking a system
    -   Document the vulnerability to earn cash



### Reconnaissance

Need information before the attack  

-   Can’t rush blindly into battle

Gathering a digital footprint  

-   Learn everything you can

Understand the security posture  

-   Firewalls, security configurations

Minimize the attack area  

-   Focus on key systems

Create a network map  

-   Identify routers, networks, remote sites

1.  Passive footprinting

    Learn as much as you can from open sources  
    
    -   There’s a lot of information out there
    -   Remarkably difficult to protect or identify
    
    Social media  
    Corporate web site  
    Online forums, Reddit  
    Social engineering  
    Dumpster diving  
    Business organizations  

2.  Open Source Intelligence (OSINT)

    Gathering information from many open sources  
    
    -   Find information on anyone or anything
    -   The name is not related to open-source software
    
    Data is everywhere  
    
    -   <https://osintframework.com/>
    
    Automated gathering  
    
    -   Many software tools available

3.  Wardriving or warflying

    Combine WiFi monitoring and a GPS  
    
    -   Search from your car or plane
    -   Search from a drone
    
    Huge amount of intel in a short period of time  
    
    -   And often some surprising results
    
    All of this is free  
    
    -   Kismet, inSSIDer
    -   Wireless Geographic Logging Engine <http://wigle.net>

4.  Active footprinting

    Trying the doors  
    
    -   Maybe one is unlocked
    -   Don’t open it yet
    -   Relatively easy to be seen
    
    Visible on network traffic and logs  
    Ping scans, port scans  
    DNS queries  
    OS scans, OS fingerprinting  



### Security teams

Cybersecurity involves many skills  

-   Operational security, penetration testing, exploit research, web application hardening, etc.

Become an expert in your niche  

-   Everyone has a role to play

The teams  

-   Red team
-   Blue team
-   Purple team
-   White team

1.  Red team

    Offensive security team  
    
    -   The hired attackers
    
    Ethical hacking  
    
    -   Find security holes
    
    Exploit vulnerabilities  
    
    -   Gain access
    
    Social engineering  
    
    -   Constant vigilance
    
    Web application scanning  
    
    -   Test and test again

2.  Blue teams

    Defensive security  
    
    -   Protecting the data
    
    Operational security  
    
    -   Daily security tasks
    
    Incident response  
    
    -   Damage control
    
    Threat hunting  
    
    -   Find and fix the holes
    
    Digital forensics  
    
    -   Find data everywhere

3.  Purple team

    Red and blue teams  
    
    -   Working together
    
    Competition isn’t necessarily useful  
    
    -   Internal battles can stifle organizational security
    -   Cooperate instead of compete
    
    Deploy applications and data securely  
    
    -   Everyone is on-board
    
    Create a feedback loop  
    
    -   Red informs blue, blue informs red

4.  White team

    Not on a side  
    
    -   Manages the interactions between red teams and blue teams
    
    The referees in a security exercise  
    
    -   Enforces the rules
    -   Resolves any issues
    -   Determines the score
    
    Manages the post-event assessments  
    
    -   Lessons learned
    -   Results



# Architecture and Design 21%



## Explain the importance of security concepts in an enterprise environment



### Configuration Management

The only constant is change  

-   Operating systems, patches, application updates,

network modifications, new application instances, etc.  
ldentify and document  
hardware and software settings  

-   Manage the security when changes occur

Rebuild those systems  
If a disaster occurs  

-   Documentation and processes will be critical

1.  Diagrams

    Network diagrams  
    
    -   Document the physical wire and device
    
    Physical data center layout  
    
    -   Can include physical rack locations
    
    Device diagrams  
    
    -   Individual cabling

2.  Baseline configuration

    The security of an application environment should be well defined  
    
    -   All application instances must follow this baseline
    -   Firewall settings, patch levels, OS file versions
    -   May require constant updates
    
    Integrity measurements check for the secure baseline  
    
    -   These should be performed often
    -   Check against well-documented baselines
    -   Failure requires an immediate correction

3.  Standard naming conventions

    Create a standard  
    
    -   Needs to be easily understood by everyone
    
    Devices  
    
    -   Asset tag names and numbers
    -   Computer names - location or region
    -   Serial numbers
    
    Networks  
    
    -   Port labeling
    
    Domain configurations  
    
    -   User account names
    -   Standard email addresses

4.  IP schema

    An |P address plan or model  
    
    -   Consistent addressing for network devices
    -   Helps avoid duplicate IP addressing
    
    Locations  
    
    -   Number of subnets, hosts per subnet
    
    IP ranges  
    
    -   Different sites have a different subnet
    -   10.1.x.x/24, 10.2.x.x/24, 10.3.x.x/24
    
    Reserved addresses  
    
    -   Users, printers, routers/default gateways



### Protecting data

A primary job task  

-   An organization is out of business without data

Data is everywhere  

-   On a storage drive, on the network, in a CPU

Protecting the data  

-   Encryption, security policies

Data permissions  

-   Not everyone has the same access

1.  Data sovereignty

    Data sovereignty  
    
    -   Data that resides in a country is subject to the laws of that country
    -   Legal monitoring, court orders, etc.
    
    Laws may prohibit where data is stored  
    
    -   GDPR (General Data Protection Regulation)
    -   Data tollected on EU citizens must be stored in the EU
    -   A complex mesh of technology and legalities
    
    Where is your data stored?  
    
    -   Your compliance laws may prohibit moving data out of the country

2.  Data masking

    Data obfuscation  
    
    -   Hide some of the original data
    
    Protects PII (personal identification information)  
    
    -   And other sensitive data
    
    May only be hidden from view  
    
    -   The data may still be intact in storage
    -   Control the view based on permissions
    
    Many different techniques  
    
    -   Substituting, shuffling, encrypting, masking out, etc.

3.  Data encryption

    Encode information into unreadable data 2  
    
    -   Original information is plaintext, encrypted form is ciphertext
    
    This is a two-way street  
    
    -   Convert between one and the other
    -   If you have the proper key
    
    Confusion  
    
    -   The encrypted data is drastically different than the plaintext
    
    Diffusion  
    
    -   Change one character of the input, and many characters change of the output

4.  Data at-rest

    The data is on a storage device  
    
    -   Hard drive, SSD, flash drive, etc.
    
    Encrypt the data  
    
    -   Whole disk encryption
    -   Database encryption
    -   File- or folder-level encryption
    
    Apply permissions  
    
    -   Access control lists
    -   Only authorized users can access the data

5.  Data in-transit

    Data transmitted over the network  
    
    -   Also called data in-motion
    
    Not much protection as it travels  
    
    -   Many different switches, routers, devices
    
    Network-based protection  
    
    -   Firewall, IPS
    
    Provide transport encryption  
    
    -   TLS (Transport Layer Security)
    -   IPsec (Internet Protocol Security)

6.  Data in-use

    Data is actively processing in memory  
    
    -   System RAM, CPU registers and cache
    
    The data is almost always decrypted  
    
    -   Otherwise, you couldn’t do anything with it
    
    The attackers can pick the decrypted information out of RAM  
    
    -   A very attractive option
    
    Target Corp. breach - November 2013  
    
    -   110 mil!ion credit cards
    -   Data in-transit encryption and data at-rest encryption
    -   Attackers picked the credit card numbers out of the point-of-sale RAM

7.  Tokenization

    Replace sensitive data with a non-sensitive placeholder  
    
    -   SSN 266-12-1112 is now 691-61-8539
    
    Common with credit card processing  
    
    -   Use a temporary token during payment
    -   An attacker capturing the card numbers can’t use them later
    
    This isn’t encryption or hashing  
    
    -   The original data and token aren’t mathematically related
    -   No encryption overhead
    -   how:  
        1.  User registers a credit card on their mobile phone: 411111111111 1234
        2.  Card is registered with the token service server
        3.  Token Service: Server provides a token instead: 4545 **\* \*** **\* \*** SE78
        4.  Phone is used at a store during checkout using NFC
        5.  Pay with: 4545 **\* \*** **\* \*** 5678
        6.  Card number validation: 4545 **\* \*** **\* \*** 5678
        7.  4545 **\* \*** **\* \*** 6578 is the token for 4111111111111234
        8.  Token is validated

8.  Information Rights Management (IRM)

    Control how data is used  
    
    -   Microsoft Office documents
    -   Email messages
    -   PDFs
    
    Restrict data access to unauthorized persons  
    
    -   Prevent copy and paste
    -   Control screenshots
    -   Manage printing ﬁ
    -   Restrict editing
    
    Each user has their own set of rights  
    
    -   Attackers have limited options



### Data loss prevention (DLP)

Where’s your data?  

-   Social Security numbers, credit card numbers, medical records

Stop the data before the attackers get it  

-   Data “leakage”

So many sources, so many destinations  

-   Often requires multiple solutions in different places

1.  Data Loss Prevention (DLP) systems

    On your computer  
    
    -   Data in use
    -   Endpoint DLP
    
    On your network  
    
    -   Data in motion
    
    On your server  
    
    -   Data at rest

2.  USB blocking

    DLP on a workstation  
    
    -   Allow or deny certain tasks
    
    November 2008 - U.S. Department of Defense  
    
    -   Worm virus “agent.btz” replicates using USB storage
    -   Bans removable flash media and storage devices
    
    All devices had to be updated  
    
    -   Local DLP agent handled USB blocking
    
    Ban was lifted in February 2010  
    
    -   Replaced with strict guidelines

3.  Cloud-based DLP

    Located between users and the Internet  
    
    -   Watch every byte of network traffic
    -   No hardware, no software
    
    Block custom defined data strings  
    
    -   Unique data for your organization
    
    Manage access to URLs  
    
    -   Prevent file transfers to cloud storage
    
    Block viruses and malware  
    
    -   Anything traversing the network

4.  DLP and email

    Email continues to be the most critical risk vector  
    
    -   Inbound threats, outbound data loss
    
    Check every email inbound and outbound  
    
    -   Internal system or cloud-based
    
    Inbound  
    
    -   Block keywords, identify impostors, quarantine email messages
    
    Outbound  
    
    -   Fake wire transfers, W-2 transmissions, employee information



### Managing Security

1.  Geographical considerations

    Legal implications  
    
    -   Business regulations vary between states
    -   For a recovery site outside of the country, personnel must have a passport and be able to clear immigration
    -   Refer to your legal team
    
    Offsite backup  
    
    -   Organization-owned site or 3rd-party secure facility
    
    Offsite recovery  
    
    -   Hosted in a different location, outside the scope of the disaster
    -   Travel considerations for support staff and employees

2.  Response and recovery controls

    Incident response and recovery  
    has become commonplace  
    
    -   Attacks are frequent and complex
    
    Incident response plan should be established  
    
    -   Documentation is critical
    -   ldentify the attack
    -   Contain the attack
    
    Limit the impact of an attacker  
    
    -   Limit data exfiltration
    -   Limit access to sensitive data

3.  SSL/TLS inspection

    Commonly used to examine outgoing SSL/TLS  
    
    -   Secure Sockets Layer/Transport Layer Security
    -   For example, from your computer to your bank
    
    Wait a second. Examine encrypted traffic?  
    
    -   Is that possible?
    
    SSL/TLS relies on trust  
    
    -   Without trust, none of this works
    
    Your browser contains a list of trusted CAs  
    
    -   My browser contains about 170 trusted CAs certificates
    
    Your browser doesn’t trust a web site unless a CA has signed the web server’s encryption certificate  
    
    -   The web site pays some money to the CA for this
    
    The CA has ostensibly performed some checks  
    
    -   Validated against the DNS record, phone call, etc.
    
    Your browser checks the web server’s certificate  
    
    -   If it’s sighed by a trusted CA, the encryption works seamlessly
    -   how (SSL/TLS proxy)  
        1.  create an Internal CA certificate in a proxy (firewall / SSL decryption)
        2.  add it to the user machine
        3.  the message is intercepted by the proxy, decrypted and encrypted again between the server and the user

4.  Hashing

    Represent data as a short string of text  
    
    -   A message digest
    
    One-way trip  
    
    -   Impossible to recover the original message from the digest
    -   Used to store passwords / confidentiality
    
    Verify a downloaded document is the same as the original  
    
    -   Integrity
    
    Can be a digital signature  
    
    -   Authentication, non-repudiation, and integrity
    
    Will not have a collision (hopefully)  
    
    -   Different messages will not have the same hash

5.  API considerations

    API (Application Programming Interface)  
    
    -   Control software or hardware programmatically
    
    Secure and harden the login page  
    
    -   Don’t forget about the API
    
    On-path attack  
    
    -   Intercept and modify APl messages, replay APl commands
    
    APl injection  
    
    -   Inject data into an APl message
    
    DDoS (Distributed Denial of Service)  
    
    -   One bad API call can bring down a system

6.  API security

    Authentication  
    
    -   Limit API access to legitimate users
    -   Over secure protocols
    
    Authorization  
    
    -   API should not allow extended access
    -   Each user has a limited role
    -   A read-only user should not be able to make changes
    
    WAF (Web Application Firewall)  
    
    -   Apply rules to APl communication



### Site Resiliency

Recovery site is prepped  

-   Data is synchronized

A disaster is called  

-   Business processes failover to the alternate processing site

Problem is addressed  

-   This can take hours, weeks, or longer

Revert back to the primary location  

-   The process must be documented for both directions

1.  Hot site

    An exact replica  
    
    -   Duplicate everything
    
    Stocked with hardware  
    
    -   Constantly updated
    -   You buy two of everything
    
    Applications and software are constantly updated  
    
    -   Automated replication
    
    Flip a switch and everything moves  
    
    -   This may be quite a few switches

2.  Cold site

    No hardware  
    
    -   Empty building
    
    No data  
    
    -   Bring it with you
    
    No people  
    
    -   Bus in your team

3.  Warm site

    Somewhere between cold and hot  
    
    -   Just enough to get going
    
    Big room with rack space  
    
    -   You bring the hardware
    
    Hardware is ready and waiting  
    
    -   You bring the software and data



### Honeypots and Deception

Attract the bad guys  

-   And trap them there

The “attacker” is probably a machine  

-   Makes for interesting recon

Honeypots  

-   Create a virtual world to explore

Many different options  

-   Kippo, Google Hack Honeypot, Wordpot, etc.

Constant battle to discern the real from the fake  

1.  Honeyfiles and honeynets

    Honeynets  
    
    -   More than one honeypot on a network
    -   More than one source of information
    -   Stop spammers - <https://projecthoneypot.org>
    
    Honeyfiles  
    
    -   Bait for the honeynet (passwords.txt)
    -   An alert is sent if the file is accessed
    -   A virtual bear trap

2.  Fake telemetry

    Machine learning  
    
    -   Interpret big data to identify the invisible
    
    Train the machine with actual data  
    
    -   Learn how malware looks and acts
    -   Stop malware based on actions instead of signatures
    
    Send the machine learning model fake telemetry  
    
    -   Make malicious malware look benign

3.  DNS sinkhole

    A DNS that hands out incorrect IP addresses  
    
    -   Blackhole DNS
    
    This can be bad  
    
    -   An attacker can redirect users to a malicious site
    
    This can be good  
    
    -   Redirect known malicious domains to a benign IP address
    -   Watch for any users hitting that IP address
    -   Those devices are infected
    
    Can be integrated with a firewall  
    
    -   Identify infected devices not directly connected



## Summarize virtualization and cloud computing concepts



### Cloud models

![img](res/aas.jpg "Cloud computing service models")  

1.  Infrastructure as a service (IaaS)

    Sometimes called Hardware as a Service (HaaS)  
    
    -   Outsource your equipment
    
    You’&rsquo;re still responsible for the management  
    
    -   And for the security
    
    Your data is out there, but more within your control  
    eg Web server providers  

2.  Platform as a service (PaaS)

    No servers, no software, no maintenance team, no HVAC :  
    
    -   Someone else handles the platform, you handle the development
    
    You don’t have direct control of the data, people, or infrastructure  
    
    -   Trained security professionals are watching your stuff  
        -   Choose carefully
    
    Put the building blocks together  
    
    -   Develop your app from what’s available on the platform
    -   SalesForce.com

3.  Software as a service (SaaS)

    On-demand software  
    
    -   No local installation
    -   Why manage your own email distribution? Or payroll?
    
    Central management of data and applications  
    
    -   Your data is out there
    
    A complete application offering  
    
    -   No development work required
    -   eg Google Mail

4.  Anything as a Service (XaaS)

    A broad description of all cloud models  
    
    -   Use any combination of the cloud
    
    Services delivered over the Internet  
    
    -   Not locally hosted or managed
    
    Flexible consumption model  
    
    -   No large upfront costs or ongoing licensing
    
    IT becomes more of an operating model  
    
    -   And less of a cost-center model
    -   Any IT function can be changed into a service

5.  Cloud service providers

    Provide cloud services  
    
    -   Saas, Paas, IaaS, etc.
    
    Charge a flat fee or based on use  
    
    -   More data, more cost
    
    You still manage your processes  
    
    -   Internal staff
    -   Development team
    -   Operational support

6.  Managed service providers

    Managed Service Provider (MSP)  
    
    -   Also a cloud service provider
    -   Not all cloud service providers are MSPs
    
    MSP support  
    
    -   Network connectivity management
    -   Backups and disaster recovery
    -   Growth management and planning
    
    Managed Security Service Provider (MSSP)  
    
    -   Firewall management
    -   Patch management, security audits
    -   Emergency response

7.  On-premises vs off-promises

    On-premises  
    
    -   Your applications are on local hardware
    -   Your servers are in your data center in your building
    
    Off-premises / hosted  
    
    -   Your servers are not in your building
    -   They may not even be running on your hardware
    -   Usually a specialized computing environment

8.  Cloud deployment models

    Public  
    
    -   Available to everyone over the Internet
    
    Community  
    
    -   Several organizations share the same resources
    
    Private  
    
    -   Your own virtualized local data center
    
    Hybrid  
    
    -   A mix of public and private



### Edge and Fog Computing

1.  Cloud computing

    Computing on-demand  
    
    -   Instantly available computing power
    -   Massive data storage capacity
    
    Fast implementation  
    
    -   IT teams can adjust rapidly to change
    -   Smaller startup costs and pay-as-you-go
    
    Not always the best solution  
    
    -   Latency - the cloud is far away
    -   Limited bandwidth
    -   Difficult to protect data
    -   Requires Internet/network connectivity

2.  Edge computing

    Over 30 billion IoT devices on the Internet  
    
    -   Devices with very specific functions
    -   A huge amount of data
    
    Edge computing - “Edge”  
    
    -   Process application data on an edge server
    -   Close to the user
    
    Often process data on the device itself  
    
    -   No latency, no network requirement
    -   Increased speed and performance
    -   Process where the data is, instead of processing in the cloud

3.  Fog computing

    Fog  
    
    -   A cloud that’s close to your data
    -   Cloud + Internet of Things
    
    Fog computing  
    
    -   A distributed cloud architecture
    -   Extends the cloud
    
    Distribute the data and processing  
    
    -   Immediate data stays local - No latency
    -   Local decisions made from local data - No bandwidth requirements
    -   Private data never leaves - Minimizes security concerns
    -   Long-term analysis can occur in the cloud - Internet only when required



### Designing the cloud

On-demand computing power  

-   Click a button

Elasticity  

-   Scale up or down as needed

Applications also scale  

-   Access from anywhere

How does it all happen?  

-   Planning and technology

1.  Thin client

    Basic application usage  
    
    -   Applications actually run on a remote server
    -   Virtual Desktop Infrastructure (VDI), Desktop as a Service (DaaS)
    -   Local device is a keyboard, mouse, and screen.
    
    Minimal operating system on the client  
    
    -   No huge memory or CPU needs
    
    Network connectivity  
    
    -   Big network requirement
    -   Everything happens across the wire

2.  Virtualization

    Virtualization  
    
    -   Run many different operating systems on the same hardware
    
    Each application instance has its own operating system  
    
    -   Adds overhead and complexity
    -   Virtualization is relatively expensive

3.  Application containerization

    Container  
    
    -   Contains everything you need to run an application
    -   Code and dependencies
    -   A standardized unit of software
    
    An isolated process in a sandbox  
    
    -   Self-contained
    -   Apps can’t interact with each other
    
    Container image  
    
    -   A standard for portability
    -   Lightweight, uses the host kernel
    -   Secure separation between applications

4.  Monolithic applications

    Monolithic applications  
    
    -   One big application that does everything
    
    Application contains all decision making processes  
    
    -   User interface
    -   Business logic
    -   Data input and output
    
    Code challenges  
    
    -   Large codebase
    -   Change control challenges

5.  Microservices and APIs

    APIs  
    
    -   Application Programming Interfaces
    
    APl is the “glue” for the microservices  
    
    -   Work together to act as the application
    
    Scalable  
    
    -   Scale just the microservices you need
    
    Resilient  
    
    -   Qutages are contained
    
    Security and compliance  
    
    -   Containment is built-in

6.  Serverless architectures

    Function as a Service (FaaS)  
    
    -   Applications are separated into
    
    individual, autonomous functions  
    
    -   Remove the operating system from the equation
    
    Developer still creates the server-side logic  
    
    -   Runs in a stateless compute container
    
    May be event triggered and ephemeral  
    
    -   May only run for one event
    
    Managed by a third-party  
    
    -   All OS security concerns are at the third-party

7.  Transit gateway

    Virtual Private Cloud (VPC)  
    
    -   A pool of resources created in a public cloud
    
    Common to create many VPCs  
    
    -   Many different application clouds
    
    Connect VPCs with a transit gateway  
    
    -   And users to VPCs
    -   A “cloud router”
    
    Now make it secure ‘  
    
    -   VPCs are commonly on different IP subnets
    -   Connecting to the cloud is often through a VPN

8.  Resource policies

    Assigning permissions to cloud resources RY S,  
    
    -   Not the easiest task
    -   Everything is in constant motion
    
    Specify which resources can be provisioned (Azure)  
    
    -   Create a service in a specific region, deny all others
    
    Specify the resource and what actions are permitted (Amazon)  
    
    -   Allow access to an APl gateway from an IP address range
    
    Explicitly list the users who can access the resource (Amazon)  
    
    -   Userlist is associated with the resource

9.  Service integration

    Service Integration and Management (SIAM)  
    Many different service providers  
    
    -   The natural result of multisourcing
    
    Every provider works differently  
    
    -   Different tools and processes
    
    SIAM is the integration of these diverse providers A  
    
    -   Provide a single business-facing IT organization
    
    An evolving set of processes and procedures  



### Infrastructure as Code

Describe an infrastructure  

-   Define servers, network, and applications as code

Modify the infrastructure and create versions  

-   The same way you version application code

Use the description (code) to  
build other application instances  

-   Build it the same way every time based on the code

An important concept for cloud computing  

-   Build a perfect version every time

1.  SDN (Software Defined Networking)

    Networking devices have two functional planes of operation  
    
    -   Control plane, data plane
    
    Directly programmable  
    
    -   Configuration is different than forwarding
    
    Agile  
    
    -   Changes can be made dynamically
    
    Centrally managed  
    
    -   Global view, single pane of glass
    
    Programmatically configured  
    
    -   No human intervention
    
    Open standards / vendor neutral  
    
    -   A standard interface to the network

2.  SDV (Software Defined Visibility)

    You must see the traffic to secure the data  
    
    -   React and respond
    
    Dynamic deployments include security and network visibility devices  
    
    -   Next-generation firewalls, web application firewalls, Security Information and Event Management (SIEM)
    
    Data is encapsulated and encrypted  
    
    -   VXLAN (Virtual Extensible LAN) and SSL/TLS
    
    New technologies change what you can see  
    
    -   Infrastructure as code, microservices
    
    Security devices monitor application traffic  
    
    -   SDV provides visibility to traffic flows
    
    Visibility expands as the application instances expand  
    
    -   Real-time metrics across all traffic flows
    
    Application flows can  
    be controlled via API  
    
    -   ldentify and react to threats



### Virtualization Security

1.  VM sprawl avoidance

    Click a button  
    
    -   You’ve built a server
    -   Or multiple servers, networks, and firewalls
    
    It becomes almost too easy to build instances  
    
    -   This can get out of hand very quickly
    
    The virtual machines are sprawled everywhere  
    
    -   You aren’t sure which VMs are related to which applications
    -   It becomes extremely difficult to deprovision
    
    Formal process and detailed documentation  
    
    -   You should have information on every virtual object

2.  VM escape protection

    The virtual machine is self-contained  
    
    -   There’s no way out
    -   Or is there?
    
    Virtual machine escape  
    
    -   Break out of the VM and interact with the host operating system or hardware
    
    Once you escape the VM, you have great control  
    
    -   Control the host and control other guest VMs
    
    This would be a huge exploit  
    
    -   Full control of the virtual world



## Summarize secure application development, deployment, and automation concepts



### Secure Deployments

1.  Development to production

    Your programming team has been working on a new application  
    
    -   How will you deploy it safely and reliably?
    
    Patch Tuesday  
    
    -   Test and deploy Wednesday? Thursday? Friday?
    
    Manage the process  
    
    -   Safely move from a non-production phase  to full production

2.  Sandboxing

    Isolated testing environment  
    
    -   No connection to the real world or production system
    -   A technological safe space
    
    Use during the development process  
    
    -   Try some code, break some code, nobody gets hurt
    
    Incremental development  
    
    -   Helps build the application

3.  Building the application

    Development  
    
    -   Secure environment
    -   Writing code
    -   Developers test in their sandboxes
    
    Test  
    
    -   Still in the development stage
    -   All of the pieces are put together
    -   Does it all work?
    -   Functional tests

4.  Verifying the application

    Quality Assurance (QA)  
    
    -   Verifies features are working as expected
    -   Validates new functionality
    -   Verifies old errors don’t reappear
    
    Staging  
    
    -   Almost ready to roll it out
    -   Works and feels exactly like the production environment
    -   Working with a copy of production data
    -   Run performance tests
    -   Test usability and features

5.  Using the application

    Production  
    
    -   Application is live
    -   Rolled out to the user community
    
    A challenging step  
    
    -   Impacts the users
    
    Logistical challenges  
    
    -   New servers
    -   New software
    -   Restart or interrupt of service

6.  Secure baselines

    The security of an application environment should be well defined  
    
    -   All application instances must follow this baseline
    -   Firewall settings, patch levels, OS file versions
    -   May require constant updates
    
    Integrity measurements check for the secure baseline  
    
    -   These should be performed often
    -   Check against well-documented baselines
    -   Failure requires an immediate correction



### Provisioning and Deprovisioning

1.  Provisioning

    Deploy an application  
    
    -   Web server, database server, middleware server, user workstation configurations, certificate updates, etc.
    
    Application software security  
    
    -   Operating system, application
    
    Network security,  
    
    -   Secure VLAN, internal access, external access
    
    Software deployed to workstations  
    
    -   Check executables for malicious code, verify security posture of the workstation

2.  Scalability and elasticity

    Handle application workload  
    
    -   Adapt to dynamic changes
    
    Scalability  
    
    -   The ability to increase the workload in a given infrastructure
    -   Build an application instance that can handle 100,000 transactions per second
    
    Elasticity  
    
    -   Increase or decrease available resources as the workload changes
    -   Deploy multiple application instances to handle “g’% 500,000 transactions per second S

3.  Orchestration

    Automation is the key to cloud computing  
    
    -   Services appear and disappear automatically, or at the push of a button
    
    Entire application instances can be instantly provisioned  
    
    -   All servers, networks, switches, firewalls, and policies
    
    Instances can move around the world as needed  
    
    -   Follow the sun
    
    The security policies should be part of the orchestration  
    
    -   As applications are provisioned, the proper security is automatically included

4.  Deprovisioning

    Dismantling and removing an application instance  
    
    -   All good things
    
    Security deprovisioning is important  
    
    -   Don’t leave open holes, don’t close important ones
    
    Firewall policies must be reverted  
    
    -   If the application is gone, so is the access
    
    What happens to the data?  
    
    -   Don’t leave information out there



### Secure Coding Techniques

1.  Secure coding concepts

    A balance between time and quality  
    
    -   Programming with security in mind is often secondary
    
    Testing, testing, testing  
    
    -   The Quality Assurance (QA) process
    
    Vulnerabilities will eventually be found  
    
    -   And exploited

2.  Stored procedures

    SQL databases  
    
    -   Client sends detailed requests for data
    -   &rsquo;SELECT \* FROM wp\_ options WHERE option\_id =1&rsquo;
    
    Client requests can be complex  
    
    -   And sometimes modified by the user
    -   This would not be good
    
    Stored procedures limit the client interactions  
    
    -   &rsquo;CALL get\_options&rsquo;
    -   That’s it. No modifications to the query are possible.
    
    To be really secure, use only stored procedures  
    
    -   The application doesn’t use any SQL queries

3.  Obfuscation/camouflage

    Obfuscate  
    
    -   Make something normally understandable very difficult to understand
    
    Take perfectly readable code and turn it into nonsense  
    
    -   The developer keeps the readable code and gives you the chicken scratch
    -   Both sets of code perform exactly the same way
    
    Helps prevent the search for security holes  
    
    -   Makes it more difficult to figure out what’s happening
    -   But not impossible

4.  Code reuse/dead code

    Code reuse  
    
    -   Use old code to build new applications
    -   Copy and paste
    
    If the old code has security vulnerabilities, reusing the code spreads it to other applications  
    
    -   You’re making this much more difficult for everyone Dead code
    -   Calculations are made, code is executed, results are tallied
    -   The results aren’t used anywhere else in the application
    
    All code is an opportunity for a security problem  
    
    -   Make sure your code is as alive as possible

5.  Input validation

    What is the expected input?  
    
    -   Validate actual vs. expected
    
    Document all input methods  
    
    -   Forms, fields, type
    
    Check and correct all input (normalization)  
    
    -   A zip code should be only X characters long with a letter in the X column
    -   Fix any data with improper input
    
    The fuzzers will find what you missed  
    
    -   Don’t give them an opening

6.  Validation points

    Server-side validation  
    
    -   All checks occur on the server
    -   Helps protect against malicious users
    
    Attackers may not even be using your interface  
    Client-side validation  
    
    -   The end-user’s app makes the validation decisions
    -   Can filter legitimate input from genuine users
    -   May provide additional speed to the user
    
    Use both  
    
    -   But especially server-side validation

7.  Memory management

    As a developer, you must be mindful of how memory is used  
    
    -   Many opportunities to build vulnerable code
    
    Never trust data input  
    
    -   Malicious users can attempt to circumvent your code
    
    Buffer overflows are a huge security risk  
    
    -   Make sure your data matches your buffer sizes
    
    Some built-in functions are insecure  
    
    -   Use best practices when designing your code

8.  Third-party libraries and SDKs

    Your programming language does everything  
    
    -   Almost
    
    Third-party libraries and software development kits  
    
    -   Extend the functionality of a programming language
    
    Security risk  
    
    -   Application code written by someone else
    -   Might be secure. Might not be secure.
    -   Extensive testing is required
    
    Balancing act  
    
    -   Application features vs. unknown code base

9.  Data exposure

    So much sensitive data  
    
    -   Credit card numbers, social security numbers, medical information, address details, email information
    
    How is the application handling the data?  
    
    -   No encryption when stored
    -   No encryption across the network
    -   Displaying information on the screen
    
    All input and output processes are important  
    
    -   Check them all for data exposure

10. Version control

    Create a file, make a change, make another change, and another change  
    
    -   Track those changes, revert back to a previous version
    
    Commonly used in software development  
    
    -   But also in operating systems, wiki software, and cloud-based file storage
    
    Useful for security  
    
    -   Compare versions over time
    -   Identify modifications to important files
    
    A security challenge  
    
    -   Historical information can be a security risk



### Software diversity

1.  Exploiting an application

    Attackers often exploit application vulnerabilities  
    
    -   They find the unlocked door and open it
    
    Once you exploit one binary, you can exploit them all  
    
    -   The application works the same on all systems
    -   A Windows 10 exploit affects all Windows 10 users
    
    What if all of the computers were  
    running different software?  
    
    -   Unique binaries
    -   Functionally identical

2.  Software diversity

    Alternative compiler paths would result in a different binary each time  
    
    -   Each compiled application would be a little bit different
    -   But functionally the same
    
    An attack against different binaries would only be successful on a fraction of the users  
    
    -   An attacker wouldn’t know what exploit to use
    -   Make the game much harder to win



### Automation and Scripting

Plan for change  

-   Implement automatically

Automated courses of action  

-   Many problems can be predicted
-   Have a set of automated responses

Continuous monitoring  

-   Check for a particular event, and then react

Configuration validation  

-   Cloud-based technologies allow for constant change
-   Automatically validate a configuration before going live
-   Perform ongoing automated checks

1.  Continuous integration (CI)

    Code is constantly written  
    
    -   And merged into the central repository many times a day
    
    So many chances for security problems  
    
    -   Security should be a concern from the beginning
    
    Basic set of security checks during development  
    
    -   Documented security baselines as the bare minimum
    
    Large-scale security analysis during the testing phase  
    
    -   Significant problems will have already been covered

2.  Continuous delivery/deployment (CD)

    Continuous delivery  
    
    -   Automate the testing process
    -   Automate the release process
    -   Click a button and deploy the application
    
    Continuous deployment  
    
    -   Even more automation
    -   Automatically deploy to production
    -   No human integration or manual checks



## Summarize authentication and authorization design concepts



### Authentication Methods

1.  Attestation

    Prove the hardware is really yours  
    
    -   A system you can trust
    
    Easy when it’s just your computer  
    
    -   More difficult when there are 1,000
    
    Remote attestation  
    
    -   Device provides an operational report to a verification server
    -   Encrypted and digitally sigrted with the TPM
    -   An IMEI or other unique hardware component can be included in the report

2.  Short message server (SMS)

    Text messaging  
    
    -   Includes more than text these days
    
    Login factor can be sent via SMS to a predefined phone number  
    
    -   Provide username and password
    -   Phone receives an SMS
    -   Input the SMS code into the login form
    
    Security issues exist  
    
    -   Phone number can be reassigned to a different phoné
    -   SMS messages can be intercepted

3.  Push notification

    Similar process to an SMS notification  
    
    -   Authentication factor is pushed to a specialized app
    -   Usually on a mobile device
    
    Security challenges  
    
    -   Applications can be vulnerable
    -   Some push apps send in the clear
    
    Still more secure than SMS  
    
    -   Multiple factors are better than one factor

4.  Authentication apps

    Pseudo-random token generators  
    
    -   A useful authentication factor
    
    Carry around a physical hardware token generator  
    
    -   Where are my keys again?
    
    Use software-based token generator on your phone  
    
    -   Powerful and convenient

5.  TOTP

    Time-based One-Time Password algorithm  
    
    -   Use a secret key and the time of day
    -   No incremental counter
    
    Secret key is configured ahead of time  
    
    -   Timestamps are synchronized via NTP
    
    Timestamp usually increments every 30 seconds  
    
    -   Put in your username, password, and TOTP code
    
    One of the more common OTP methods  
    
    -   Used by Google, Facebook, Microsoft, etc.

6.  HOTP

    One-time passwords  
    
    -   Use them once, and never again
    -   Once a session, once each authentication attempt
    
    HMAC-based One-Time Password algorithm  
    
    -   Keyed-hash message authentication code (HMAC)
    -   The keys are based on a secret key and a counter
    
    Token-based authentication  
    
    -   The hash is different every time
    
    Hardware and software tokens available  
    
    -   You’ll need additional technology to make this work

7.  Phone call

    A voice call provides the token  
    
    -   The computer is talking to you
    -   &ldquo;Your code is 1-6-2-5-1-7.&rdquo;
    
    Similar disadvantages to SMS  
    
    -   Phone call can be intercepted or forwarded
    -   Phone number can be added to another phone

8.  Static codes

    Authentication factors that don’t change  
    
    -   You just have to remember
    
    Personal Identification Number (PIN)  
    
    -   Your secret numbers
    
    Can also be alphanumeric  
    
    -   A password or passphrase

9.  Smart cards

    Integrated circuit card  
    
    -   Contact or contactless
    
    Common on credit cards  
    
    -   Also used for access control
    
    Must have physical card to provide digital access  
    
    -   A digital certificate
    
    Multiple factors  
    
    -   Use the card with a PIN or fingerprint



### Biometrics

Fingerprint scanner  

-   Phones, laptops, door access

Retinal scanner  

-   Unique capillary structure in the back of the eye

Iris scanner  

-   Texture, color

Voice recognition  

-   Talk for access

Facial recognition  

-   Shape of the face and features

1.  Biometric factors

    Gait analysis  
    
    -   ldentify a person based on how they walk
    -   Many unigue measurements
    
    Veins  
    
    -   Vascular scanners
    -   Match the blood vessels visible from the surface of the skin

2.  Biometric acceptance rates

    False acceptance rate (FAR)  
    
    -   Likelihood that an unauthorized user will be accepted
    -   Not sensitive enough
    
    False rejection rate (FRR)  
    
    -   Likelihood that an authorized user will be rejected
    -   Too sensitive
    
    Crossover error rate (CER)  
    
    -   Defines the overall accuracy of a biometric system
    -   The rate at which FAR and FRR are equal
    -   Adjust sensitivity to equalize both values
    
    ![img](res/biometrics_rate.png "Biometrics rate")  



### Multi-factor authentication

1.  AAA framework

    1.  Identification  
        -   This is who you claim to be
        -   Usually your username
    2.  Authentication  
        -   Prove you are who you say you are
        -   Password and other authentication factors
    3.  Authorization  
        -   Based on your identification and authentication, what access do you have?
    4.  Accounting  
        -   Resources used: Login time, data sent and received, logout time

2.  Cloud vs. on-premises authentication

    Cloud-based security  
    
    -   Third-party can manage the platform
    -   Centralized platform
    -   Automation options with APl integration
    -   May include additional options (for a cost)
    
    On-premises authentication system  
    
    -   Internal monitoring and management
    -   Need internal expertise
    -   External access must be granted and managed

3.  Multi-factor authentication

    Factors  
    
    -   Something you know
    -   Something you have
    -   Something you are
    
    Attributes  
    
    -   Somewhere you are
    -   Something you can do
    -   Something you exhibit
    -   Someone you know

4.  Something you know

    Password  
    
    -   Secret word/phrase, string of characters
    -   Very common authentication factor
    
    PIN  
    
    -   Personal identification number
    -   Not typically contained anywhere on a smart card or ATM card
    
    Pattern  
    
    -   Complete a series of patterns
    -   Only you know the right format

5.  Something you have

    Smart card  
    
    -   Integrates with devices
    -   May require a PIN
    
    USB token  
    
    -   Certificate is on the USB device
    
    Hardware or software tokens  
    
    -   Generates pseudo-random authentication codes
    
    Your phone  
    
    -   SMS a code to your phone

6.  Something you are

    Biometric authentication  
    
    -   Fingerprint, iris scan, voice print
    
    Usually stores a mathematical representation of your biometric  
    
    -   Your actual fingerprint isn’t usually saved
    
    Difficult to change  
    
    -   You can change your password
    -   You can’t change your fingerprint
    
    Used in very specific situations  
    
    -   Not foolproof

7.  Somewhere you are

    Provide a factor based on your location  
    
    -   The transaction only completes if you are in a particular geography
    
    IP address  
    
    -   Not perfect, but can help provide more info
    -   Works with IPv4, not so much with IPv6
    
    Mobile device location services  
    
    -   Geolocation to a very specific area
    -   Must be in a location that can receive GPS information or near an identified mobile or 802.11 network
    -   Still not a perfect identifier of location

8.  Something you can do

    A personal way of doing things  
    
    -   You&rsquo;re special
    
    Handwriting analysis  
    
    -   Signature comparison
    -   Writing technique
    
    Very similar to biometrics  
    
    -   Close to something you are

9.  Other attributes

    Something you exhibit  
    
    -   A unique trait, personal to you
    -   Gait analysis - the way you walk
    -   Typing analysis - the way you hit the enter key too hard
    
    Someone you know  
    
    -   A social factor
    -   It’s not what you know&#x2026;
    -   Web of trust
    -   Digital signature



## Given a scenario, implement cybersecurity resilience



### Disk redundancy

1.  Redundancy

    Duplicate parts of the system  
    
    -   If a part fails, the redundant part can be used
    
    Maintain uptime  
    
    -   The organization continues to function
    
    No hardware failure  
    
    -   Servers keep running
    
    No software failure  
    
    -   Services always available
    
    No system failure  
    
    -   Network performing optimally

2.  Geographical dispersal

    Bad things can happen in a local area  
    
    -   Hurricanes, tornadoes, flooding,
    
    Disperse technologies to different geographies  
    
    -   Use multiple data centers
    -   In different locations
    
    Data centers might be part of the normal operations  
    
    -   East coast and west coast operations centers
    
    May be part of a disaster recovery center  
    
    -   If Florida gets hit, fire up the Denver data center

3.  Disk redundancy

    Multipath I/O (Input/Output)  
    
    -   Especially useful for network-based storage subsystems
    -   Multiple Fibre Channel interfaces with multiple switches
    
    RAID  
    
    -   Redundant Array of Independent Disks
    
    Multiple drives create redundancy  
    
    -   Many different designs and implementations

4.  RAID

    <table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
    
    
    <colgroup>
    <col  class="org-right" />
    
    <col  class="org-left" />
    
    <col  class="org-left" />
    </colgroup>
    <thead>
    <tr>
    <th scope="col" class="org-right">raid level</th>
    <th scope="col" class="org-left">description</th>
    <th scope="col" class="org-left">details</th>
    </tr>
    </thead>
    
    <tbody>
    <tr>
    <td class="org-right">0</td>
    <td class="org-left">Striping without parity</td>
    <td class="org-left">High performance, no fault tolerance</td>
    </tr>
    
    
    <tr>
    <td class="org-right">1</td>
    <td class="org-left">Mirroring</td>
    <td class="org-left">Duplicates data for fault tolerance, but requires twice disk space</td>
    </tr>
    
    
    <tr>
    <td class="org-right">5</td>
    <td class="org-left">Striping with parity</td>
    <td class="org-left">Fault tolerant, only requires an additional disk for redundancy</td>
    </tr>
    
    
    <tr>
    <td class="org-right">0+1, 1+0, 5+1, etc</td>
    <td class="org-left">Multiple raid types</td>
    <td class="org-left">Combine multiple RAID methods to increase redundancy</td>
    </tr>
    </tbody>
    </table>



### Network Redundancy

1.  Load balancing

    Some servers are active  
    
    -   Others are on standby
    
    If an active server fails, the passive server takes its place  

2.  NIC teaming (network interface connection teaming)

    Load Balancing / Fail Over (LBFO)  
    
    -   Aggregate bandwidth, redundant paths
    -   Becomes more important in the virtual world
    
    Multiple network adapters  
    
    -   Looks like a single adapter
    -   Integrate with switches
    
    NICs talk to each other  
    
    -   Usually multicast instead of broadcast
    -   Fails over when a NIC doesn’t respond

3.  Port aggregation and redundancy



### Power Redundancy

1.  UPS

    Uninterruptible Power Supply  
    
    -   Short-term backup power
    -   Blackouts, brownouts, surges
    
    UPS types (from cheaper to expensive - and advances)  
    
    1.  Offline/Standby UPS
    2.  Line-interactive UPS
    3.  On-line/Double-conversion UPS
    
    Features  
    
    -   Auto shutdown battery capacity, outlets, phone line suppression

2.  Generators

    Long-term power backup  
    
    -   Fuel storage required
    
    Power an entire building  
    
    -   Some power outlets may be marked as generator-powered
    
    It may take a few minutes to get the generator up to speed  
    
    -   Use a battery UPS while the generator is starting

3.  Dual-power supplies

    Redundancy  
    
    -   Internal server power supplies
    -   External power circuits
    
    Each power supply can handle 100% of the load  
    
    -   Would normally run at 50% of the load
    
    Hot-swappable  
    
    -   Replace a faulty power supply without powering down

4.  Power distrubution units (PDUs)

    Provide multiple power outlets  
    
    -   Usually in a rack
    
    Often include monitoring and control  
    
    -   Manage power capacity
    -   Enable or disable individual outlets



### Replication

1.  SAN replication

    Share data between different devices  
    
    -   If one device fails, you can still work with the data
    -   VERY fast recovery times compared to traditional backups
    
    Storage area networks (SANSs)  
    
    -   Specialized high-performance network of storage devices
    
    SAN-to-SAN replication  
    
    -   Duplicate data from one data center to another
    
    SAN snapshot  
    
    -   Create a state of data based on a point in time
    -   Copy that state to other SANs

2.  VM replication

    Virtual machine redundancy  
    
    -   Maintain one VM, replicate to all others
    -   The virtual machine is really just one big file
    
    Consistent service offering  
    
    -   Maintain copies anywhere in the world
    
    Recover from a replicated copy  
    
    -   Provides a backup if needed
    
    Efficient copying  
    
    -   Only replicates the data that has changed

3.  On premises vs cloud redundancy

    Speed  
    
    -   Local devices are connect over very fast networks
    -   Cloud connections are almost always slower
    
    Money  
    
    -   Purchasing your own storage is an expensive capital investment
    -   Cloud costs have a low entry point and can scale
    
    Security  
    
    -   Local data is private
    -   Data stored in the cloud requires additional security controls



### Backup types

1.  File backups

    The archive attribute  
    
    -   Set when a file is modified
    
    Full  
    
    -   Everything
    -   You&rsquo;ll want this one first
    
    Incremental  
    
    -   All files changed since the last incremental backup
    
    Differential  
    
    -   All files changed since the last full backup

2.  Incremental backup

    A full backup is taken first  
    Subsequent backups contain data changed since the last full backup and last incremental backup  
    
    -   These are usually smaller than the full backup
    
    A restoration requires the full backup and all of the incremental backups  

3.  Differential backup

    A full backup is taken first  
    Subsequent backups contain data changed since the last full backup  
    
    -   These usually grow larger as data is changed
    
    A restoration requires the full backup and the last differential backup  

4.  Backup types

    <table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
    
    
    <colgroup>
    <col  class="org-left" />
    
    <col  class="org-left" />
    
    <col  class="org-left" />
    
    <col  class="org-left" />
    </colgroup>
    <thead>
    <tr>
    <th scope="col" class="org-left">type</th>
    <th scope="col" class="org-left">data selection</th>
    <th scope="col" class="org-left">backup/restore time</th>
    <th scope="col" class="org-left">archive attribute</th>
    </tr>
    </thead>
    
    <tbody>
    <tr>
    <td class="org-left">full</td>
    <td class="org-left">all selected data</td>
    <td class="org-left">high/low (one tape set)</td>
    <td class="org-left">cleared</td>
    </tr>
    
    
    <tr>
    <td class="org-left">incremental</td>
    <td class="org-left">new files and files modified since the last backup</td>
    <td class="org-left">low/high (multiple tape sets)</td>
    <td class="org-left">cleared</td>
    </tr>
    
    
    <tr>
    <td class="org-left">differential</td>
    <td class="org-left">all data modified since the last full backup</td>
    <td class="org-left">moderate/moderate (no more than 2 sets)</td>
    <td class="org-left">not cleared</td>
    </tr>
    </tbody>
    </table>

5.  Backup media

    Magnetic tape  
    
    -   Sequential storage
    -   100 GB to multiple terabytes per cartridge
    -   Easy to ship and store
    
    Disk  
    
    -   Faster than magnetic tape
    -   Deduplicate and compress
    
    Copy  
    
    -   A useful strategy
    -   May not include versioning
    -   May need to keep offsite

6.  NAS vs SAN

    Network Attached Storage (NAS)  
    
    -   Connect to a shared storage device across the network
    -   File-level access (overwrite the entire file in case of modification)
    
    Storage Area Network (SAN)  
    
    -   Looks and feels like a local storage device  
        -   Block-level access
    -   Very efficient reading and writing
    
    Requires a lot of bandwidth  
    
    -   May use an isolated network and high-speed network technologies

7.  Cloud backups

    Cloud  
    
    -   Backup to a remote device in the clouc
    -   Support many devices
    -   May be limited by bandwidth
    
    Image  
    
    -   Capture an exactly replica of everything on a storage drive
    -   Restore everything on a partition, including operating system files and user documents

8.  Backup locations

    Offline backup  
    
    -   Backup to local devices
    -   Fast and secure
    -   Must be protected and maintained
    -   Often requires offsite storage for disaster recovery
    
    Online backup  
    
    -   Remote network-connected third-party
    -   Encrypted
    -   Accessible from anywhere
    -   Speed is limited by network bandwidth



### Resiliency

1.  Non-persistence

    The cloud is always in motion  
    
    -   Application instances are constantly built and torn down
    
    Snapshots can capture the current configuration and data  
    
    -   Preserve the complete state of a device, or just the configuration
    
    Revert to known state  
    
    -   Fall back to a previous snapshot
    
    Rollback to known configuration  
    
    -   Don’t modify the data, but use a previous configuration
    
    Live boot media  
    
    -   Run the operating system from removable media - very portable!

2.  High availability

    Redundancy doesn’t always mean always available  
    
    -   May need to be powered on manually
    
    HA (high availability)  
    
    -   Always on, always available
    
    May include many different components working together  
    
    -   Active/Active can provide scalability advantages
    
    Higher availability almost always means higher costs  
    
    -   There’s always another contingency you could add
    -   Upgraded power, high-quality server components, etc.

3.  Order of restoration

    Application-specific  
    
    -   Certain components may need to be restored first
    -   Databases should be restored before the application
    
    Backup-specific  
    
    -   Incremental backups restore the full backup, then all subsequent incremental backups
    -   Differential backups restore the full backup, then the fast differential backup

4.  Diversity

    Technologies  
    
    -   A zero-day OS vulnerability can cause significant outages
    -   Multiple security devices
    
    Vendors  
    
    -   A single vendor can become a disadvantage
    -   No options during annual renewals
    -   A bad support team may not be able to resolve problems in a timely manner
    
    Cryptographic  
    
    -   All cryptography is temporary
    -   Diverse certificate authorities can provide additional protection
    
    Controls  
    
    -   Administrative controls
    -   Physical controls
    -   Technical controls
    -   Combine them together
    -   Defense in depth



## Explain the security implications of embedded and specialized systems



### Embedded systems

Hardware and software designed for a specific function  

-   Or to operate as part of a larger system

Is built with only this task in mind  

-   Can be optimized for size and/or cost

Common examples  

-   Traffic light controliers
-   Digital watches 8
-   Medical imaging systems

1.  Soc (system on a chip)

    Multiple components running on a single chip  
    
    -   Common with embedded systems
    
    Small form-factor  
    
    -   External interface support
    -   Cache memory, flash memory
    -   Usually lower power consumption g
    
    Security considerations are important  
    
    -   Difficult to upgrade hardware
    -   Limited off-the-shelf security options

2.  Field-programmable gate array (FPGA)

    An integrated circuit that can be configured after manufacturing  
    
    -   Array of logic blocks
    -   Programmed in the field
    
    A problem doesn’t require a hardware replacement  
    
    -   Reprogram the FPGA
    
    Common in infrastructure  
    
    -   Firewall logic
    -   Routers

3.  SCADA/ICS

    Supervisory Control and Data Acquisition System  
    
    -   Large-scale, multi-site Industrial Control Systems (ICS)
    
    PC manages equipment  
    
    -   Power generation, refining, manufacturing equipment
    -   Facilities, industrial, energy, logistics
    
    Distributed control systems  
    
    -   Real-time information
    -   System control
    
    Requires extensive segmentation  
    
    -   No access from the outside

4.  Smart devices / IOT (Internet of Things)

    Sensors  
    
    -   Heating and cooling, lighting
    
    Smart devices  
    
    -   Home automation, video doorbells
    
    Wearable technology  
    
    -   Watches, health monitors
    
    Facility automation  
    
    -   Temperature, air quality, lighting
    
    Weak defaults  
    
    -   IOT manufacturers are not security professionals

5.  Specialized

    Medical devices  
    
    -   Heart monitors, insulin pumps
    -   Often use older operating systems
    
    Vehicles  
    
    -   Internal network is often accessible from mobile networks
    -   Control internal electronics
    
    Aircraft  
    
    -   DoS could damage the aircraft
    -   An outage would be problematic
    
    Smart meters  
    
    -   Measure power and water usage

6.  VoIP

    Voice over Internet Protocol  
    
    -   Instead of analog phone line or the
    
    Plain Old Telephone Service (POTS)  
    A relatively complex embedded system  
    
    -   Can be relatively important
    
    Each device is a computer  
    
    -   Separate boot process
    -   Individual configurations
    -   Different capabilities and functionalities

7.  HVAC

    Heating, Ventilation, and Air Conditioning  
    
    -   Thermodynamics, fluid mechanics, and heat transfer
    
    A complex science  
    
    -   Not something you can properly design yourself
    -   Must be integrated into the fire system
    
    PC manages equipment  
    
    -   Makes cooling and heating decisions for workspaces and data centers
    
    Traditionally not built with security in mind  
    
    -   Difficult to recover from an infrastructure DoS

8.  Drones

    Flying vehicle  
    
    -   No pilot on board
    
    May be manually controlled from the ground  
    
    -   Often with some autonomy
    -   Set it and forget it
    
    Extensive commercial and non-commercial use  
    
    -   May require federal licenses
    -   Security and fail-safes are required

9.  Printers, scanners, and fax machines

    All-in-one or multifunction devices (MFD)  
    
    -   Everything you need in one single device
    
    No longer a simple printer  
    
    -   Very sophisticated firmware
    
    Some images are stored locally on the device  
    
    -   Can be retrieved externally
    
    Logs are stored on the device  
    
    -   Contain communication and fax details

10. RTOS (Real-Time Operating System)

    An operating system with a deterministic processing schedule  
    
    -   No time to wait for other processes
    -   Industrial equipment, automobiles,
    -   Military environments
    
    Extremely sensitive to security issues  
    
    -   Non-trivial systems
    -   Need to always be available
    -   Difficult to know what type of security is in place

11. Surveillance systems

    Video/audio surveillance  
    
    -   Embedded systems in the cameras and the monitoring stations
    
    Secure the security system  
    
    -   Restrict access from others
    -   Prevent a denial of service
    
    Physically difficult to replace cameras  
    
    -   Accessible independently over the network
    -   May allow for firmware upgrades



### Embedded Systems Communication

1.  5G

    Fifth generation cellular networking  
    
    -   Launched worldwide in 2020
    
    Significant performance improvements  
    
    -   At higher frequencies
    -   Eventually 10 gigabits per second
    -   Slower speeds from 100-900 Mbit/s
    
    Significant loT impact  
    
    -   Bandwidth becomes less of a constraint
    -   Larger data transfers
    -   Faster monitoring and notification
    -   Additional cloud processing

2.  Subscriber identity module (SIM)

    SIM card  
    
    -   A universal integrated circuit card
    
    Used to provide information to a cellular network provider  
    
    -   Phones, tablets, embedded systems
    
    Contains mobile details  
    
    -   IMSI (International Mobile Subscriber Identity)
    -   Authentication information, contact information
    
    Important to manage  
    
    -   Many embedded systems, many SIM cards .

3.  Narrowband

    Communicate analog signals over a narrow range of frequencies  
    
    -   Over a longer distance
    -   Conserve the frequency use
    
    Many loT devices can communicate over long distances  
    
    -   SCADA equipment
    -   Sensors in oil fields

4.  Baseband

    Generally a single cable with a digital signal  
    
    -   Can be fiber or copper
    
    The communication signal o uses all of the bandwidth v  
    
    -   Utilization is either 0% or 100%
    
    Bidirectional communication  
    
    -   But not at the same time using the same wire/fiber
    
    Ethernet standard  
    
    -   100BASE-TX, 1000BASE-T, 10GBASE-T

5.  Zigbee

    Internet of Things networking  
    
    -   Open standard - IEEE 802.15.4 PAN (personal area network)
    
    Alternative to WiFi and Bluetooth  
    
    -   Longer distances than Bluetooth
    -   Less power consumption than WiFi
    
    Mesh network of all Zigbee devices in your home  
    
    -   Light switch communicates to light bulbs
    -   Tell Amazon Echo to lock the door
    
    Uses the ISM band  
    
    -   Industrial, Scientific, and Medical
    -   900 MHz and 2.4 GHz frequencies in the US



### Embedded Systems Constraints

Not usually a fully capable computer  

-   Low cost, purpose-built

Adds additional constraints  

-   May have limited or missing features
-   Upgradability limitations
-   Limits in communication options

An ongoing trade off  

-   Low cost systems
-   Unigue management challenges

1.  Constraints

    Power  
    
    -   May not have access to a main power source
    -   Batteries may need to be replaced and maintained
    
    Compute  
    
    -   Low-power CPUs are limited in speed
    -   Cost and heat considerations
    
    Network  
    
    -   May not have the option for a wired link
    -   May be in the middle of a field
    -   Wireless is the limiting factor
    
    Crypto  
    
    -   Limited hardware options
    -   Difficult to change or modify cryptography features
    
    Inability to patch  
    
    -   Some loT devices have no field-upgradable options
    -   Upgrade options may be limited or difficult to install
    
    Authentication  
    
    -   Security features are often an afterthought
    -   Limited options, no multi-factor, limited integration with existing directory services
    
    Range  
    
    -   Purpose-built - usually does one thing very well
    -   May not provide much additional functionality
    
    Cost  
    
    -   Single-purpose functionality comes at a low cost
    -   Low cost may affect product quality
    
    Implied trust  
    
    -   Limited access to the hardware and software
    -   Difficult to verify the security posture



## Explain the importance of physical security controls



### Physical Security Controls

1.  Barricades/bollards

    Prevent access  
    
    -   There are limits to the prevention
    
    Channel people through a specific access point  
    
    -   And keep out other things
    -   Allow people, prevent cars and trucks
    
    ldentify safety concerns  
    
    -   And prevent injuries
    
    Can be used to an extreme  
    
    -   Concrete barriers / bollards
    -   Moats

2.  Access control vestibules

    Different types of vestibules  
    All doors normally unlocked  
    
    -   Opening one door causes others to lock
    
    All doors normally locked  
    
    -   Unlocking one door prevents
    
    others from being unlocked  
    One door open / other locked  
    
    -   When one is open, the other
    
    cannot be unlocked  
    One at a time, controlled groups  
    
    -   Managed control through an area

3.  Alarms

    Circuit-based  
    
    -   Circuit is opened or closed
    -   Door, window, fence
    -   Useful on the perimeter
    
    Motion detection  
    
    -   Radio reflection or passive infrared
    -   Useful in areas not often in use
    
    Duress  
    
    -   Triggered by a person
    -   The big red button

4.  Signs

    Clear and specific instructions  
    
    -   Keep people away from restricted areas
    -   Consider visitors
    
    Consider personal safety  
    
    -   Fire exits
    -   Warning signs  
        -   Chemicals
        -   Construction
    -   Medical resources
    
    Informational  
    
    -   In case of emergency, call this number

5.  Video surveillance

    CCTV (Closed circuit television)  
    
    -   Can replace physical guards
    
    Camera features are important  
    
    -   Motion recognition can alarm and alert when something moves
    -   Object detection can identify a license plate or person’s face
    
    Often many different cameras  
    
    -   Networked together and recorded over time

6.  Industrial camouflage

    Conceal an important facility in plain sight  
    
    -   Blends in to the local environment
    
    Protect a data center  
    
    -   No business signs
    -   No visual clues
    -   Surround it with a water feature
    -   Install a guard gate
    -   Planters out front are bollards

7.  Guards and access lists

    Security guard  
    
    -   Physical protection at the reception area of a facility
    -   Validates identification of existing employees
    -   Provides guest access
    
    ID badge  
    
    -   Picture, name, other details
    -   Must be worn at all times
    
    Access list  
    
    -   Physical list of names
    -   Enforced by security guard
    
    Maintains a visitor log  

8.  Guards

    Two-person integrity/control  
    
    -   Minimize exposure to an attack
    -   No single person has access to a physical asset
    
    Robot sentries  
    
    -   Monitoring
    -   Rounds / Periodic checks
    -   An emerging technology

9.  Biometrics

    Biometric authentication  
    
    -   Fingerprint, retina, voiceprint
    
    Usually stores a mathematical representation of your biometric  
    
    -   Your actual fingerprint isn’t usually saved
    
    Difficult to change  
    
    -   You can change your password
    -   You can’t change your fingerprint
    
    Used in very specific situations  
    
    -   Not foolproof

10. Door access control

    Conventional  
    
    -   Lock and key
    
    Deadbolt  
    
    -   Physical bolt
    
    Electronic  
    
    -   Keyless, PIN
    
    Token-based  
    
    -   RFID badge, magnetic swipe card, or key fob
    
    Biometric  
    
    -   Hand, fingers or retina
    
    Multi-factor  
    
    -   Smart card and PIN

11. Cable locks

    Temporary security  
    
    -   Connect your hardware to something solid
    
    Cable works almost anywhere  
    
    -   Useful when mobile
    
    Most devices have a standard connector  
    
    -   Reinforced notch
    
    Not desighed for long-term protection  
    
    -   Those cables are pretty thin

12. USB data locker

    Don’t connect to unknown USB interfaces  
    
    -   Even if you need a quick charge
    -   Prevent “juice jacking”
    
    Use a USB data blocker  
    
    -   Allow the voltage, reject the data
    
    Use your power adapter  
    
    -   Avoid the issue entirely

13. Proper lighting

    More light means more security  
    
    -   Attackers avoid the light
    -   Easier to see when lit
    -   Non IR cameras can see better
    
    Specialized design  
    
    -   Consider overall light levels
    -   Lighting angles may be important  
        -   Facial recognition
    -   Avoid shadows and glare

14. Fencing

    Build a perimeter  
    
    -   Usually very obvious
    -   May not be what you’re looking for
    
    Transparent or opaque  
    
    -   See through the fence (or not)
    
    Robust  
    
    -   Difficult to cut the fence
    
    Prevent climbing  
    
    -   Razor wire
    -   Build it high

15. Fire suppression

    Electronics require unique responses to fire  
    
    -   Water is generally a bad thing
    
    Detection  
    
    -   Smoke detector, flame detector, heat detector
    
    Suppress with water  
    
    -   Where appropriate
    
    Suppress with chemicals  
    
    -   Halon - No longer manufactured  
        -   Destroys ozone
    -   Commonly replaced with Dupont FM-200

16. Sensors

    Motion detection  
    
    -   ldentify movement in an area
    
    Noise detection  
    
    -   Recognize an increase in sound
    
    Proximity reader  
    
    -   Commonly used with electronic door locks
    -   Combined with an access card
    
    Moisture detection  
    
    -   Useful to identify water leaks
    
    Temperature  
    
    -   Monitor changes over time

17. Drones

    Quickly cover large areas  
    
    -   More than just one building
    
    More than physical security  
    
    -   Site surveys, damage assessments
    
    On-board sensors  
    
    -   Motion detection
    -   Thermal sensors
    
    Video evidence  
    
    -   High resolution video capture

18. Faraday cage

    Blocks electromagnetic fields A  
    
    -   Discovered by Michael Faraday in 1836
    
    A mesh of conductive material  
    
    -   The cage cancels the electromagnetic field’s effect on the interior
    -   The window of a microwave oven
    
    Not a comprehensive solution  
    
    -   Not all signal types are blocked
    -   Some signal types are not blocked at all
    
    Can restrict access to mobile networks  
    
    -   Some very specific contingencies would need to be in place for emergency calls

19. Screened subnet

    Formerly known as a demilitarized zone (DMZ)  
    
    -   An additional layer of security between the Internet and you
    -   Public access to public resources

20. Protected distribution

    Protected Distribution System (PDS)  
    
    -   A physically secure cabled network
    
    Protect your cables and fibers  
    
    -   All of the data flows through these conduits
    
    Prevent cable and fiber taps  
    
    -   Direct taps and inductive taps
    
    Prevent cable and fiber cuts  
    
    -   A physical denial of service (DoS)
    
    Hardened protected distribution system  
    
    -   Sealed metal conduit, periodic visual inspection



### Secure areas

Physically secure the data  

-   As important as the digital security

An important part of a security policy  

-   Not a question to leave unanswered

Secure active operations  

-   Prevent physical access to the systems

Secure offline data  

-   Backups are an important security concern

1.  Air gap

    Physical separation between networks  
    
    -   Secure network and insecure network
    -   Separate customer infrastructures
    
    Most environments are shared  
    
    -   Shared routers, switches, firewalls
    -   Some of these are virtualized
    
    Specialized networks require air gaps  
    
    -   Stock market networks
    -   Power systems/SCADA
    -   Airplanes
    -   Nuclear power plant operations

2.  Vaults and safes

    Vault  
    
    -   A secure reinforced room
    -   Store backup media
    -   Protect from disaster or theft
    -   Often onsite
    
    Safe  
    
    -   Similar to a vault, but smaller
    -   Less expensive to implement
    -   Space is limited
    -   Install at more locations

3.  Hot and cold aisles

    Data centers  
    
    -   Lots and lots of equipment
    -   This equipment generates heat
    
    Optimize cooling  
    
    -   Keep components at optimal temperatures
    
    Conserve energy  
    
    -   Data centers are usually very large rooms
    -   Focus the cooling
    -   Lower energy costs



### Secure Data Destruction

Disposal becomes a legal issue  

-   Some information must not be destroyed
-   Consider offsite storage

You don’t want critical information in the trash  

-   People really do dumpster dive
-   Recycling can be a security concern
-   Physically destroy the media

Reuse the storage media  

-   Sanitize the media for reuse
-   Ensure nothing is left behind

1.  Protect your rubbish

    Secure your garbage  
    
    -   Fence and a lock
    
    Shred your documents  
    
    -   This will only go so far
    -   Governments burn the good stuff
    
    Burn documents  
    
    -   No going back
    
    Pulp the paper  
    
    -   Large tank washing to remove ink
    -   Paper broken down into pulp
    -   Creates recycled paper

2.  Physical destruction

    Shredder / pulverizer  
    
    -   Heavy machinery
    -   Complete destruction
    
    Drill / Hammer  
    
    -   Quick and easy
    -   Platters, all the way through
    
    Electromagnetic (degaussing)  
    
    -   Remove the magnetic field
    -   Destroys the drive data and renders the drive unusable
    
    Incineration  
    
    -   Fire hot

3.  Certificate of destruction

    Destruction is often done by a 3rd party  
    
    -   How many drills and degaussers do you have?
    
    Need confirmation that your data is destroyed  
    
    -   Service should include a certificate
    
    A paper trail of broken data  
    
    -   You know exactly what happened

4.  Sanitizing media

    Purge data  
    
    -   Remove it from an existing data store
    -   Delete some of the data from a database
    
    Wipe data  
    
    -   Unrecoverable removal of data on a storage device
    -   Usually overwrites the data storage locations
    -   Useful when you need to reuse or continue using the media

5.  Data security

    July 2013 - UK National Health Service Surrey  
    
    -   Provided hard drives to a 3rd-party to be destroyed
    -   Contained 3,000 patient records
    -   Received a destruction certificate, but not actually destroyed.
    -   Sold on eBay. Buyer contacted authorities, fined £200,000
    
    File level overwriting  
    
    -   Sdelete — Windows Sysinternals
    
    Whole drive wipe secure data removal  
    
    -   DBAN - Darik’s Boot and Nuke
    
    Physical drive destruction  
    
    -   One-off or industrial removal and destroy



## Summarize the basics of cryptographic concepts



### Cryptography Concepts

Greek: “kryptos”  

-   Hidden, secret

Confidentiality  

-   It’s a secret

Authentication and access control  

-   I know it’s you. I REALLY know it’s you.

Non-repudiation  

-   You said it. You can’t deny it.

Integrity  

-   Tamper-proof

1.  Cryptography terms

    Plaintext  
    
    -   An unencrypted message (in the clear)
    
    Ciphertext  
    
    -   An encrypted message
    
    Cipher  
    
    -   The algorithm used to encrypt and/or decrypt
    
    Cryptanalysis  
    
    -   The art of cracking encryption
    -   Researchers are constantly trying to find weaknesses in ciphers  
        -   A mathematically flawed cipher is bad for everyone

2.  Cryptographic keys

    Keys  
    
    -   Add the key to the cypher to encrypt
    -   Larger keys are generally more secure
    
    Some encryption methods use one key  
    
    -   Some use more than one key
    -   Every method is a bit different

3.  Give weak keys a workout

    A weak key is a weak key  
    
    -   By itself, it’s not very secure
    
    Make a weak key stronger by performing multiple processes  
    
    -   Hash a password. Hash the hash of the password. And continue&#x2026;
    -   Key stretching, key strengthening
    
    Brute force attacks would require reversing each of those hashes  
    
    -   The attacker has to spend much more time, even though the key is small

4.  Key stretching libraries

    Already built for your application  
    
    -   No additional programming involved
    
    bcrypt  
    
    -   Generates hashes from passwords
    -   An extension to the UNIX crypt library
    -   Uses Blowfish cipher to perform multiple rounds of hashing
    
    Password-Based Key Derivation Functionkz (PBKDF2)  
    
    -   Part of RSA public key cryptography standards (PKCS #5, RFC 2898)

5.  Lightweight cryptography

    Powerful cryptography has traditionally required strength  
    
    -   A powerful CPU and lots of time
    
    Internet of Things (loT) devices have limited power  
    
    -   Both watts and CPU
    
    New standards are being created  
    
    -   National Institute of Standards and Technology (NIST) leading the effort
    -   Provide powerful encryption
    -   Include integrity features
    -   Keep costs low

6.  Homomorphic encryption (HE)

    Encrypted data is difficult to work with  
    
    -   Decrypt the data
    -   Perform a function
    -   Encrypt the answer
    
    Homomorphic encryption  
    
    -   Perform calculations of data while it’s encrypted
    -   Perform the work directly on the encrypted data
    -   The decrypted data can only be viewed with the private key
    
    Many advantages  
    
    -   Securely store data in the cloud
    -   Perform research on data without viewing the data



### Symmetric and Asymmetric Cryptography

1.  Symmetric encryption

    A single, shared key  
    
    -   Encrypt with the key
    -   Decrypt with the same key
    -   If it gets out, you’ll need another key
    
    Secret key algorithm  
    
    -   A shared secret
    
    Doesn’t scale very well  
    
    -   Can be challenging to distribute
    
    Very fast to use  
    
    -   Less overheag than asymmetric encryption
    -   Often combined with asymmetric encryption

2.  Asymmetric encryption

    Public key cryptography  
    
    -   Two (or more) mathematically related keys
    
    Private key  
    
    -   Keep this private
    
    Public key  
    
    -   Anyone can see this key
    -   Give it away
    
    The private key is the only key that can decrypt data enctypted with the public key  
    
    -   You can’t derive the private key from the public key

3.  The key pair

    Asymmetric encryption  
    
    -   Public Key Cryptography
    
    Key generation  
    
    -   Build both the public and private key at the same time
    -   Lots of randomization
    -   Large prime numbers
    -   Lots and lots of math
    
    Everyone can have the public key  
    
    -   Only Alice has the private key

4.  Symmetric key from asymmetric keys (Diffie-Hellman)

    Use public and private key cryptography to create a symmetric key  
    
    -   Math is powerful

5.  Elliptic curve cryptography (ECC)

    Asymmetric encryption  
    
    -   Need large integers composed of two or more large prime factors
    
    Instead of numbers, use curves!  
    
    -   Uses smaller keys than non-ECC asymmetric encryption
    -   Smaller storage and transmission requirements
    -   Perfect for mobile devices



### Hashing and digital signatures

1.  Hashes

    Represent data as a short string of text  
    
    -   A message digest, a fingerprint
    
    One-way trip  
    
    -   Impossible to recover the original message from the digest
    -   Used to store passwords / confidentiality
    
    Verify a downloaded document is the same as the original  
    
    -   Integrity
    
    Can be a digital signature  
    
    -   Authentication, non-repudiation, and integrity
    
    Will not have a collision (hopefully)  
    
    -   Different messages will not have the same hash

2.  Collision

    Hash functions  
    
    -   Take an input of any size
    -   Create a fixed size string
    -   Message digest, checksum
    
    The hash should be unique  
    
    -   Different inputs should never create the same hash
    -   If they do, it’s a collision
    
    MD5 has a collision problem  
    
    -   Found in 1996
    -   Don’t use MD5

3.  Practical hashing

    Verify a downloaded file  
    
    -   Hashes may be provided on the download site
    -   Compare the downloaded file hash with the posted hash value
    
    Password storage  
    
    -   Instead of storing the password, store a salted hash
    -   Compare hashes during the authentication process
    -   Nobody ever knows your actual password

4.  [Adding some salt](#org28b51ef)

5.  Salting the hash

    Each user gets a different random hash  
    
    -   The same password creates a different hash
    
    <table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
    
    
    <colgroup>
    <col  class="org-left" />
    
    <col  class="org-left" />
    </colgroup>
    <thead>
    <tr>
    <th scope="col" class="org-left">Password</th>
    <th scope="col" class="org-left">Hash</th>
    </tr>
    </thead>
    
    <tbody>
    <tr>
    <td class="org-left">dragon</td>
    <td class="org-left">a9c43be948c5cabd56ef2bacffb77cdaa5eec49dd5ebOcc4129cf3eda5fOe74c</td>
    </tr>
    
    
    <tr>
    <td class="org-left">dragon+ gsEVx</td>
    <td class="org-left">35172b0IE)7c9c3962bbf02908b3f330dde5f5eda42b6b4d5533e0759eb25686c8</td>
    </tr>
    
    
    <tr>
    <td class="org-left">dragon+ LTBkP</td>
    <td class="org-left">b9909221fbbda70bea27644b84443ddb68f78ede2253fa816409fd8b7602599a</td>
    </tr>
    
    
    <tr>
    <td class="org-left">dragon+ HTsBK</td>
    <td class="org-left">€f1c25063093411faefb09198356de6775955b5ff6e0feS9aab665a3e95d11e25</td>
    </tr>
    
    
    <tr>
    <td class="org-left">dragon+ MnNEo</td>
    <td class="org-left">99658dalaf957at6f267901891f0a1957018c0962361580c5bd5fc50d26b71579</td>
    </tr>
    </tbody>
    </table>

6.  Digital signatures

    Prove the message was not changed  
    
    -   Integrity
    
    Prove the source of the message  
    
    -   Authentication
    
    Make sure the signature isn’t fake  
    
    -   Non-repudiation
    
    Sign with the private key  
    
    -   The message doesn’t need to be encrypted
    -   Nobody else can sign this (obviously)
    
    Verify with the public key  
    
    -   Any change in the message will invalidate the signature
    
    ![img](res/digital_sign.png "Digital signatures - creation")  
    
    ![img](res/digital_sign2.png "Digital signatures - verification")  



### Cryptographyc Keys

There’s very little that isn’t known about the cryptographic process  

-   The algorithm is usually a known entity
-   The only thing you don’t know is the key

The key determines the output  

-   Encrypted data
-   Hash value
-   Digital signature

Keep your key private!  

-   It’s the only thing protecting your data

1.  Key strength

    Larger keys tend to be more secure  
    
    -   Prevent brute-force attacks
    -   Attackers can try every possible key combination
    
    Symmetric encryption  
    
    -   128-bit or larger symmetric keys are common
    -   These numbers get larger as time goes on
    
    Asymmetric encryption  
    
    -   Complex calculations of prime numbers
    -   Larger keys than symmetric encryption
    -   Common to see key lengths of 3,072 bits or larger

2.  Key exchange

    A logistical challenge  
    
    -   How do you transfer an encryption key across an insecure medium without having an encryption key?
    
    Out-of-band key exchange  
    
    -   Don’t send the symmetric key over the ‘net
    -   Telephone, courier, in-person, etc.
    
    In-band key exchange  
    
    -   It’s on the network
    -   Protect the key with additional encryption
    -   Use asymmetric encryption to deliver a symmetric key

3.  Real-time encryption/decryption

    There’s a need for fast security  
    
    -   Without compromising the security part
    
    Share a symmetric session key using asymmetric encryption  
    
    -   Client encrypts a random (symmetric) key with a server’s public key
    -   The server decrypts this shared key and uses it to encrypt data
    -   This is the session key
    
    Implement session keys carefully  
    
    -   Need to be changed often (ephemeral keys)
    -   Need to be unpredictable

4.  Traditional web server encryption

    SSL/TLS uses encryption keys to protect web server communication  
    
    -   Traditionally, this has been based on the web server’s RSA key pair
    -   One key that encrypts all symmetric keys
    
    This server’s private key can rebuild everything  
    
    -   If you capture all of the traffic, you can decrypt all of the data
    
    One point of failure for all of your web site encryption  

5.  Perfect Forward Secrecy (PFS)

    Change the method of key exchange  
    
    -   Don’t use the server’s private RSA key
    
    Elliptic curve or Diffie-Hellman ephemeral  
    
    -   The session keys aren’t kept around
    
    Can’t decrypt with the private server key  
    
    -   Every session uses a different private key for the exchange
    
    PFS requires more computing power  
    
    -   Not all servers choose to use PFS
    
    The browser must support PFS  
    
    -   Check your SSL/TLS information for details



### Steganography

1.  Obfuscation

    The process of making something unclear  
    
    -   It’s now much more difficult to understand
    
    But it’s not impossible to understand  
    
    -   If you know how to read it
    
    Make source code difficult to read  
    
    -   But it doesn’t change the functionality of the code
    
    Hide information inside of an image  
    
    -   Steganography

2.  Steganography

    Greek for “concealed writing”  
    
    -   Security through obscurity
    
    Message is invisible  
    
    -   But it’s really there
    
    The covertext  
    
    -   The container document or file

3.  Common steganography techniques

    Network based  
    
    -   Embed messages in TCP packets
    
    Use an image  
    
    -   Embed the message in
    
    the image itself  
    Invisible watermarks  
    
    -   Yellow dots on printers

4.  Other steganography types

    Audio steganography  
    
    -   Modify the digital audio file
    -   Interlace a secret message within the audio
    -   Similar technique to image steganography
    
    Video steganography  
    
    -   A sequence of images
    -   Use image steganography on a larger scale
    -   Manage the signal to noise ratio
    -   Potentially transfer much more information



### Quantum Computing

Computers based on quantum physics  

-   This is not an upgrade to your existing computer
-   This is a new computing technology

Classical mechanics  

-   Smallest form of information is a bit
-   Bits are zeros and ones N

Quantum mechanics  

-   Smallest form of information is a qubit
-   Bits are zeros, ones, and any combination in-between, at the same time  
    -   This is called quantum superposition

1.  Quantum computing

    Search quickly through large databases  
    
    -   Index everything at the same time
    
    Simulate the quantum world  
    
    -   Medical advances
    -   Weather prediction
    -   Astrophysics
    -   And much more

2.  Post-quantum cryptography

    Breaks our existing encryption mechanisms  
    
    -   Quickly factor large prime numbers
    
    This would cause significant issues  
    
    -   None of the existing cryptography could be trusted
    -   No financial transactions wbuld be safe
    -   No data would be private
    
    Peter Shor invented Shor’s algorithm in 1994  
    
    -   Given an integer N, find its prime factors
    -   Traditional computers would take longer than the lifetime of the universe
    -   Shor’s algorithm would theoretically be much, much faster
    
    Time for updated cryptography  
    
    -   Not vulnerable to quantum computer based attacks
    
    NTRU  
    
    -   A cryptosystem using lattice theory
    -   Relies on the “closest-vector” problem
    -   Instead of finding the prime factorizations of large numbers
    
    We will need to consider our options for future cryptography  
    
    -   This is a problem that can be easily seen and addressed

3.  Quantum communication

    Protect against eavesdropping using quantum cryptography  
    
    -   Quantum Key Distribution (QKD)
    
    Create unbreakable encryption  
    
    -   Send a random stream of qubits (the key) across a quantum network channel
    
    Both sides can verify the key  
    
    -   If it’s identical, the key was not viewed during transmission
    
    An attacker eavesdropping on the communication would modify the data stream  
    
    -   The attacker would have to violate quantum physics



### Stream and block ciphers

1.  Stream ciphers

    Encryption is done one bit or byte at a time  
    
    -   High speed, low hardware complexity
    
    Used with symmetric encryption  
    
    -   Not commonly used with asymmetric encryption
    
    The starting state should never be the same twice  
    
    -   Key is often combined with an initialization vector (IV)

2.  Block ciphers

    Encrypt fixed-length groups  
    
    -   Often 64-bit or 128-bit blocks
    -   Pad added to short blocks
    -   Each block is encrypted or decrypted independently
    
    Symmetric encryption  
    
    -   Similar to stream ciphers
    
    Block cipher modes of operation  
    
    -   Avoid patterns in the encryption
    -   Many different modes to choose from

3.  Block cipher mode of operation

    Encrypt one fixed-length group of bits at a time  
    
    -   A block
    
    Mode of operation  
    
    -   Defines the method of encryption
    -   May provide a method of authentication
    
    The block size is a fixed size  
    
    -   Not all data matches the block size perfectly
    -   Split your plaintext into smaller blocks
    -   Some modes require padding before encrypting
    
    1.  ECB (electronic codebook)
    
        The simplest encryption mode  
        
        -   Too simple for most use cases
        
        Each block is encrypted with the same key  
        
        -   ldentical plaintext blocks create identical ciphertext blocks
    
    2.  CBC (Cipher Block Chaining)
    
        A popular mode of operation  
        
        -   Relatively easy to implement
        
        Each plaintext block is XORed with the previous ciphertext block  
        
        -   Adds additional randomization
        -   Use an initialization vector for the first block
    
    3.  CTR (counter)
    
        Block cipher mode / acts like a stream cipher  
        
        -   Encrypts successive values of a “counter”
        
        Plaintext can be any size, since it’s part of the XOR  
        
        -   i.e., 8 bits at a time (streaming) instead of a 128-bit block
    
    4.  GCM (Galois/Counter Mode)
    
        Encryption with authentication  
        
        -   Authentication is part of the block mode
        -   Combines Counter Mode with
        
        Galois authentication  
        Minimum latency, minimum operation overhead  
        
        -   Very efficient encryption and authentication
        
        Commonly used in packetized data  
        
        -   Network traffic security (wireless, |Psec)
        -   SSH, TLS



### Blockchain Technology

A distributed ledger  

-   Keep track of transactions

Everyone on the blockchain network maintains the ledger  

-   Records and replicates to anyone and everyone

Many practical applications  

-   Payment processing
-   Digital identification
-   Supply chain monitoring
-   Digital voting

1.  The blockchain process

    1.  A transaction is requested.  
        The transaction could be any digital transaction from transferring Bitcoins, medical records, data backups, or transferring house title information.
    2.  The transaction is sent to every computer (or node) in a decentralized network to be verified.
    3.  The verified transaction is added to a new block of data containing other recently verified transactions.
    4.  A secure code (a hash) is calculated from the previous blocks of transaction data in the Blockchain.  
        The hash is added to the new block of verified transactions.
    5.  The block is added to the end of the Blockchain, which is then updated to all nodes in the network for security.  
        The transaction is complete.
    6.  If any blocks are altered, its hash and all following hashes in the chain are automatically recalculated.  
        The altered chain will not longer match the chains stored by the rest of the network, and will be rejected.



### Cryptography Use Cases

1.  Finding the balance

    Low power devices  
    
    -   Mobile devices, portable systems
    -   Smaller symmetric key sizes
    -   Use elliptic curve cryptography (ECC) for asymmetric encryption
    
    Low latency  
    
    -   Fast computation time
    -   Symmetric encryption, smaller key sizes
    
    High resiliency  
    
    -   Larger key sizes
    -   Encryption algorithm quality
    -   Hashing provides data integrity

2.  Use cases

    Confidentiality  
    
    -   Secrecy and privacy
    -   Encryption (file-level, drive-level, email)
    
    Integrity  
    
    -   Prevent modification of data
    -   Validate the contents with hashes
    -   File downloads, password storage
    
    Obfuscation  
    
    -   Modern malware
    -   Encrypted data hides the active malware code
    -   Decryption occurs during execution
    
    Authentication  
    
    -   Password hashing
    -   Protect the original password
    -   Add salt to randomize the stored password hash
    
    Non-Repudiation  
    
    -   Confirm the authenticity of data
    -   Digital signature provides both integrity and non-repudiation



### Cryptography limitations

1.  Finding balance

    Cryptography isn&rsquo;t a perfect solution  
    
    -   It can have significant limitations
    
    Not all implementations are the same  
    
    -   Different platforms, different cryptographic options
    
    Cryptography can’t fix bad technique  
    
    -   Hashing easily guessed passwords without a salt
    
    Every situation is different  
    
    -   Do your homework

2.  Limitations

    Speed  
    
    -   Cryptography adds overhead
    -   A system needs CPU, CPU needs power
    -   More involved encryption increases the load
    
    Size  
    
    -   Typical block ciphers don’t increase the size of encrypted data
    -   AES block size is 128 bits/16 bytes
    -   Encrypting 8 bytes would potentially double the storage size
    
    Weak keys  
    
    -   Larger keys are generally
    
    more difficult to brute force  
    
    -   The weak IV in RC4 resulted
    
    in the WEP security issues  
    Time  
    
    -   Encryption and hashing takes time
    -   Larger files take longer
    -   Asymmetric is slower than symmetric
    
    Longevity  
    
    -   A specific cryptographic technology can becomes less secure over time
    -   Smaller keys are easier to brute force, larger keys take longer to process
    -   Key retirement is a good best practice
    
    Predictability and entropy  
    
    -   Random numbers are critical for secure cryptography
    -   Hardware random number generators can be predictable
    -   A passphrase needs to be appropriately random
    
    Key reuse  
    
    -   Reusing the same key reduces complexity  
        -   Less cost and effort to recertify keys
        -   Less administrative overhead
    -   If the key is compromised, everything using that key is at risk
    -   IoT devices often have keys embedded in the firmware
    
    Resource vs. security constraints  
    
    -   IoT devices have limited CPU, memory, and power
    -   Real-time applications can’t delay
    -   Difficult to maintain and update security components



# Implementation 25%



## Given a scenario, implement secure protocols



### Secure protocols

1.  Voice and Video

    SRTP  
    
    -   Secure Real-Time Transport Protocol / Secure RTP
    
    Adds security features to RTP  
    
    -   Keep conversations private
    
    Encryption  
    
    -   Uses AES to encrypt the voice/video flow
    
    Authentication, integrity, and replay protection  
    
    -   HMAC-SHA1 - Hash-based message authentication code using SHA1

2.  Time synchronization

    Classic NTP has no security features  
    
    -   Exploited as amplifiers in DDoS attacks
    -   NTP has been around prior to 1985
    
    NTPsec  
    
    -   Secure network time protocol
    -   Began development in June of 2015
    
    Cleaned up the code base  
    
    -   Fixed a number of vulnerabilities

3.  Email

    S/MIME  
    
    -   Secure/Multipurpose Internet Mail Extensions
    -   Public key encryption and digital signing of mail content
    -   Requires a PKI (public key infrastructure) or similar organization of keys
    
    Secure POP and Secure IMAP  
    
    -   Use a STARTTLS extension to encrypt POP3 with SSL or use IMAP with SSL
    
    SSL/TLS  
    
    -   If the mail is browser based, always encrypt with SSL

4.  Web

    SSL/TLS  
    
    -   Secure Sockets Layer/Transport Layer Security
    
    HTTPS  
    
    -   HTTP over TLS / HTTP over SSL / HTTP Secure
    
    Uses public key encryption  
    
    -   Private key on the server
    -   Symmetric session key is transferred using asymmetric encryption
    -   Security and speed

5.  IPsec (internet protocol security)

    Security for OSI Layer 3  
    
    -   Authentication and encryption for every packet
    
    Confidentiality and integrity/anti-replay  
    
    -   Encryption and packet signing
    
    Very standardized  
    
    -   Common to use multi-vendor implementations
    
    Two core IPsec protocols  
    
    -   Authentication Header (AH)
    -   Encapsulation Security Payload (ESP)

6.  File transfer

    FTPS  
    
    -   FTP over SSL (FTP-SSL)
    -   File Transfer Protocol Secure
    -   This is not SFTP
    
    SFTP  
    
    -   SSH File Transfer Protocol
    -   Provides file system functiogality
    -   Resuming interrupted transfers, directory listings, remote file removal

7.  LDAP (Lightweight Directory Access Protocol)

    Protocol for reading and writing directories over an IP network  
    
    -   An organized set of records, like a phone directory
    
    X.500 specification was written by the International Telecommunications Union (ITU)  
    
    -   They know directories!
    
    DAP ran on the OSI protocol stack  
    
    -   LDAP is lightweight, and uses TCP/IP
    
    LDAP is the protocol used to query and update an X.500 directory  
    
    -   Used in Windows Active Directory, Apple OpenDirectory, OpenLDAP, etc.

8.  Directory services

    LDAP (Lightweight Directory Access Protocol)  
    LDAPS (LDAP Secure)  
    
    -   A non-standard implementation of LDAP over SSL.
    
    SASL (Simple Authentication and Security Layer)  
    
    -   Provides authentication using many different methods, i.e., Kerberos or client certificate

9.  Remote access

    SSH (Secure Shell)  
    
    -   Encrypted terminal commumcatlon
    -   Replaces Telnet (and FTP)
    -   Provides secure terminal communication and file transfer features

10. Domain name resolution

    DNS had no security in the original design  
    
    -   Relatively easy to poison a DNS
    
    DNSSEC  
    
    -   Domain Name System Security Extensions
    
    Validate DNS responses  
    
    -   Origin authentication
    -   Data integrity
    
    Public key cryptography  
    
    -   DNS records are signed with a trusted third party
    -   Signed DNS records are published in DNS

11. Routing and switching

    SSH - Secure Shell  
    
    -   Encrypted terminal communication
    
    SNMPv3 - Simple Network Management Protocol version 3  
    
    -   Confidentiality - Encrypted data
    -   Integrity - No tampering of data
    -   Authentication - Verifies the source
    
    HTTPS  
    
    -   Browser-based management
    -   Encrypted communication

12. Network address allocation

    Securing DHCP  
    
    -   DHCP does not include any built-in security
    -   There is no “secure” version of the DHCP protocol
    
    Rogue DHCP servers  
    
    -   In Active Directory, DHCP servers must be authorized
    -   Some switches can be configured with “trusted” interfaces
    -   DHCP distribution is only allowed from trusted interfaces
    -   Cisco calls this DHCP Snooping

13. Network address allocation

    DHCP client DoS - Starvation attack  
    
    -   Use spoofed MAC addresses to exhaust the DHCP pool
    
    Switches can be configured to limit the number of MAC addresses per interface  
    
    -   Disable an interface when multiple MAC addresses are seen

14. Subscription services

    Automated subscriptions  
    
    -   Anti-virus / Anti-malware signature updates
    -   IPS updates
    -   Malicious IP address databases / Firewall updates
    
    Constant updates  
    
    -   Each subscription uses a different update method
    
    Check for encryption and integrity checks  
    
    -   May require an additional public key configuration
    -   Set up a trust relationship  
        -   Certificates, IP addresses



## Given a scenario, implement host or application security solutions



### Endpoint protection

1.  The endpoint

    The user’s access  
    
    -   Applications and data
    
    Stop the attackers  
    
    -   Inbound attacks
    -   Qutbound attacks
    
    Many different platforms  
    
    -   Mobile, desktop
    
    Protection is multi-faceted  
    
    -   Defense in depth

2.  Anti-virus and anti-malware

    Anti-virus is the popular term  
    
    -   Refers specifically to a type of malware
    -   Trojans, worms, macro viruses
    
    Malware refers to the broad malicious software category  
    
    -   Anti-malware stops spyware, ransomware, fileless malware
    
    The terms are effectively the same these days  
    
    -   The names are more of a marketing tool
    -   Anti-virus software is also
    
    anti-malware software now  
    
    -   Make sure your system is using a comprehensive solution

3.  Endpoint detection and response (EDR)

    A different method of threat protection  
    
    -   Scale to meet the increasing number of threats
    
    Detect a threat  
    
    -   Signatures aren’t the only detection tool
    -   Behavioral analysis, machine learning, process monitoring
    -   Lightweight agent on the endpoint
    
    Investigate the threat  
    
    -   Root cause analysis
    
    Respond to the threat  
    
    -   Isolate the system, quarantine the threat, rollback to a previous config
    -   API driven, no user or technician intervention required

4.  Data Loss Prevention (DLP)

    Where’s your data?  
    
    -   Social Security numbers, credit card numbers, medical records
    
    Stop the data before the attacker gets it  
    
    -   Data “leakage”
    
    So many sources, so many destinations  
    
    -   Often requires multiple solutions
    -   Endpoint clients ‘
    -   Cloud-based systems i  
        -   Email, cloud storage, collaboration tools

5.  Next-generation firewall (NGFW)

    The OSI Application Layer  
    
    -   All data in every packet
    
    Can be called different names  
    
    -   Application layer gateway
    -   Stateful multilayer inspection
    -   Deep packet inspection
    
    Broad security controls  
    
    -   Allow or disallow application features
    -   Identify attacks and malware
    -   Examine encrypted data
    -   Prevent access to URLs or URL categories

6.  Host based firewall

    Software-based firewall  
    
    -   Personal firewall, runs on every endpoint
    
    Allow or disallow incoming or outgoing application traffic  
    
    -   Control by application process
    -   View all data
    
    ldentify and block unknown processes  
    
    -   Stop malware before it can start
    
    Manage centrally  

7.  Finding intrusions

    Host-based Intrusion Detection System (HIDS)  
    
    -   Uses log files to identify intrusions
    -   Can reconfigure firewalls to block
    
    Host-based Intrusion Prevention System (HIPS)  
    
    -   Recognize and block known attacks
    -   Secure OS and application configs, validate incoming service requests
    -   Often built into endpoint protection software
    
    HIPS identification  
    
    -   Signatures, heuristics, behavioral
    -   Buffer overflows, registry updates, writing files to the Windows folder
    -   Access to non-encrypted data



### Boot integrity

The attack on our systems is constant  

-   Techniques are constantly changing

Attackers compromise a device  

-   And want it to stay compromised

The boot process is a perfect infection point  

-   Rootkits run in kernel mode
-   Have the same rights as the operating system

Protecting the boot process is important  

-   Secure boot, trusted boot, and measured boot
-   A chain of trust

1.  Hardware root of trust

    Security is based on trust  
    
    -   Is your data safely encrypted?
    -   Is this web site legitimate?
    -   Has the operating system been infected?
    
    The trust has to start somewhere  
    
    -   Trusted Platform Module (TPM), Hardware Security Module (HSM)
    -   Designed to be the hardware root of the trust
    
    Difficult to change or avoid  
    
    -   It’s hardware
    -   Won’t work without the hardware

2.  Trusted Platform Module (TPM)

    A specification for cryptographic functions  
    
    -   Hardware to help with encryption functions
    
    Cryptographic processor  
    
    -   Random number generator, key generators
    
    Persistent memory  
    
    -   Comes with unique keys burned in during production
    
    Versatile memory  
    
    -   Storage keys, hardware configuration information
    
    Password protected  
    
    -   No dictionary attacks

3.  UEFI BIOS Secure Boot

    Secure Boot  
    
    -   Part of the UEFI specification
    
    UEFI BIOS protections  
    
    -   BIOS includes the manufacturer’s public key
    -   Digital signhature is checked during a BIOS update
    -   BIOS prevents unauthorized writes to the flash
    
    Secure Boot verifies the bootloader  
    
    -   Checks the bootloader’s digital signature
    -   Bootloader must be sighed with a trusted certificate
    -   Or a manually approved the digital sighature

4.  Trusted Boot

    Bootloader verifies digital signature of the OS kernel  
    
    -   A corrupted kernel will halt the boot process
    
    The kernel verifies all of the other startup components  
    
    -   Boot drivers, startup files
    
    Just before loading the drivers, ELAM (Early Launch Anti-Malware) starts  
    
    -   Checks ever§l driver to see if it’s trusted
    -   Windows won’t load an untrusted driver

5.  Measured boot

    Nothing on this computer has changed  
    
    -   There have been no malware infections
    -   How do you know?
    
    Easy when it’s just your computer  
    
    -   More difficult when there are 1,000
    
    UEFI stores a hash of the firmware, boot drivers, and everything else loaded during the Secure Boot and Trusted Boot process  
    
    -   Stored in the TPM
    
    Remote attestation  
    
    -   Device provides an operational report to a verification server
    -   Encrypted and digitally sighed with the TPM
    
    Attestation server receives the boot report  
    
    -   Changes are identified and managed



### Database security

Protecting stored data  

-   And the transmission of that data

Intellectual property storage  

-   Data is valuable

Compliance issues  

-   PCI DSS, HIPAA, GDPR, etc.

Keep the business running  

-   Security provides continuity

Breaches are expensive  

-   Keep costs low

1.  [Tokenization](#orgea4daa8)

2.  [Hashing password](#org83ad77a)

3.  [Adding some salt](#org28b51ef)

4.  [Salting the hash](#org364cefc)



### Application security

1.  [Secure coding concepts](#org652051a)

2.  [Input validation](#org5838aa6)

3.  Dynamic analysis (fuzzing)

    Send random input to an application  
    
    -   Fault-injecting, robustness testing, syntax testing, negative testing
    
    Looking for something out of the ordinary  
    
    -   Application crash, server error, exception
    
    1988 class project at the University of Wisconsin  
    
    -   &ldquo;Operating System Utility Program Reliability”
    -   Professor Barton Miller
    -   The Fuzz Generator

4.  Fuzzing engines and networks

    Many different fuzzing options  
    
    -   Platform specific, language specific, etc.
    
    Very time and processor resource heavy  
    
    -   Many, many different iterations to try
    -   Many fuzzing engines use high-probability tests
    
    Carnegie Mellon Computer Emergency Response Team (CERT)  
    
    -   CERT Basic Fuzzing Framework (BFF)
    -   <https://professormesser.link/bff>

5.  Secure cookies

    Cookies  
    
    -   Information stored on your computer by the browser
    
    Used for tracking, personalization, session management  
    
    -   Not executable, not generally a security risk  
        -   Unless someone gets access to them
    
    Secure cookies have a Secure attribute set  
    
    -   Browser will only send it over HTTPS
    
    Sensitive information should not be saved in a cookie  
    
    -   This isn’t designed to be secure storage

6.  HTTP Secure Headers

    An additional layer of security  
    
    -   Add these to the web server configuration
    -   You can’t fix every bad application
    
    Enforce HTTPS communication  
    
    -   Ensure encrypted communication
    
    Only allow scripts, stylesheets, or images from the local skite  
    
    -   Prevent XSS attacks
    
    Prevent data from loading into an inline frame (iframe)  
    
    -   Also helps to prevent XSS attacks

7.  Code signing

    An application is deployed  
    
    -   Users run application executable or scripts
    
    SO many security questions  
    
    -   Has the application been modified in any way?
    -   Can you confirm that the application was written by a specific developer?
    
    The application code can be digitally signed by the developer  
    
    -   Asymmetric encryption
    -   A trusted CA signs the developer’s public key
    -   Developer signs the code with their private key
    -   For internal apps, use your own CA

8.  Allow list / deny list

    Any application can be dangerous  
    
    -   Vulnerabilities, trojan horses, malware
    
    Security policy can control app execution  
    
    -   Allow list, deny/block list
    
    Allow list  
    
    -   Nothing runs unless it’s approved
    -   Very restrictive
    
    Deny list  
    
    -   Nothing on the “bad list” can be executed
    -   Anti-virus, anti-malware
    
    Quarantine  
    
    -   Anything suspicious can be moved to a safe area

9.  Examples of allow and deny list

    Decisions are made in the operating system  
    
    -   Often built-in to the operating system management
    
    Application hash  
    
    -   Only allows applications with this unique identifier
    
    Certificate  
    
    -   Allow digitally signed apps from certain publishers
    
    Path  
    
    -   Only run applications in these folders
    
    Network zone  
    
    -   The apps can only run from this network zone

10. Static code analyzers

    Static Application Security Testing (SAST)  
    
    -   Help to identify security flaws
    
    Many security vulnerabilities found easily  
    
    -   Buffer overflows, database injections, etc.
    
    Not everything can be identified through analysis  
    
    -   Authentication security, insecure cryptography, etc.
    -   Don’t rely on automation for everything
    
    Still have to verify each finding  
    
    -   False positives are an issue



### Application hardening

Minimize the attack surface  

-   Remove all possible entry points

Remove the potential for all known vulnerabilities  

-   As well as the unknown

Some hardening may have compliance mandates  

-   HIPAA servers, PCI DSS, etc.

There are many different resources  

-   Center for Internet Security (CIS)
-   Network and Security Institute (SANS)
-   National Institute of Standards and Technology (NIST)

1.  Open ports and services

    Every open port is a possible entry point  
    
    -   Close everything except required ports
    
    Control access with a firewall  
    
    -   NGFW would be ideal
    
    Unused or unknown services  
    
    -   Installed with the OS or from other applications
    
    Applications with broad port ranges  
    
    -   Open port 0 through 65,535
    
    Use Nmap or similar port scanner to verify  
    
    -   Ongoing monitoring Is important

2.  Registry

    The primary configuration database for Windows  
    
    -   Almost everything can be configured from the registry
    
    Useful to know what an application modifies  
    
    -   Many third-party tools can show registry changes
    
    Some registry changes are important security settings  
    
    -   Configure registry permissions
    -   Disable SMBv1

3.  Disk encryption

    Prevent access to application data files  
    
    -   File system encryption
    
    Full disk encryption (FDE)  
    
    -   Encrypt everything on the drive
    -   BitLocker, FileVault, etc.
    
    Self-encrypting drive (SED)  
    
    -   Hardware-based full disk encryption
    -   No operating system software needed
    
    Opal storage specification  
    
    -   The standard for of SED storage

4.  Operating system hardening

    Many and varied  
    
    -   Windows, Linux, iOS, Android, et al.
    
    Updates  
    
    -   Operating system updates/service packs, security patches
    
    User accounts  
    
    -   Minimum password lengths and complexity
    -   Account limitations
    
    Network access and security  
    
    -   Limit network access
    
    Monitor and secure  
    
    -   Anti-virus, anti-malware

5.  Patch management

    Incredibly important  
    
    -   System stability, security fixes
    
    Monthly updates  
    
    -   Incremental (and important)
    
    Third-party updates  
    
    -   Application developers, device drivers
    
    Auto-update  
    
    -   Not always the best option
    
    Emergency out-of-band updates  
    
    -   Zero-dav and important security discoveries

6.  Sandboxing

    Applications cannot access unrelated resources  
    
    -   They play in their own sandbox
    
    Commonly used during development  
    
    -   Can be a useful production technique
    
    Used in many different deployments  
    
    -   Virtual machines
    -   Mobile devices
    -   Browser iframes (Inline Frames)
    -   Windows User Account Control (UAC)



## Given a scenario, implement secure network designs



### Load balancing

Distribute the load  

-   Multiple servers
-   Invisible to the end-user

Large-scale implementations  

-   Web server farms, database farms

Fault tolerance  

-   Server outages have no effect
-   Very fast convergence

Configurable load  

-   Manage dCross servers

TCP offload  

-   Protocol overhead

SSL offload  

-   Encryption/Decryption

Caching  

-   Fast response

Prioritization  

-   QO0S

Content switching  

-   Application-centric balancing

1.  Scheduling

    Round-robin  
    
    -   Each server is selected in turn
    
    Weighted round-robin  
    
    -   Prioritize the server use
    
    Dynamic round-robin  
    
    -   Monitor the server load and distribute to the server with the lowest use
    
    Active/active load balancing  

2.  Affinity

    Affinity  
    
    -   A kinship, a likeness
    
    Many applications require communication to the same instance  
    
    -   Each user is “stuck” to the same server
    -   Tracked through IP address or session IDs
    -   Source affinity / sticky session / session persistence

3.  Active/passive load balancing

    Some servers are active  
    
    -   Others are on standby
    
    If an active server fails, the passive server takes its place  



### Network segmentation

Physical, logical, or virtual segmentation  

-   Devices, VLANS, virtual networks

Performance  

-   High-bandwidth applications

Security  

-   Users should not talk directly to database servers
-   The only applications in the core are SQL and SSH

Compliance  

-   Mandated segmentation (PCI compliance)
-   Makes change control much easier

1.  Physical segmentation

    Devices are physically separate  
    
    -   Air gap between Switch A and Switch B
    
    Must be connected to provide communication  
    
    -   Direct connect, or another switch or router
    
    Web servers in one rack  
    
    -   Database servers on another
    
    Customer A on one switch, customer B on another  
    
    -   No opportunity for mixing data
    
    Separate devices  
    
    -   Multiple units, separate infrastructure

2.  Logical segmentation with VLANs

    Virtual Local Area Networks (VLANS)  
    
    -   Separated logically instead of physically
    -   Cannot communicate between VLANs without a Layer 3 device / router

3.  [Screened subnet](#org22af51f)

4.  Extranet

    A private network for partners  
    
    -   Vendors, suppliers
    
    Usually requires additional authentication  
    
    -   Only allow access to authorized users

5.  Intranet

    Private network  
    
    -   Only available internally
    
    Company announcements, important documents, other company business  
    
    -   Employees only
    
    No external access  
    
    -   Internal or VPN access only

6.  East-west traffic

    Traffic flows within a data center  
    
    -   Important to know where traffic starts and ends
    
    East-west  
    
    -   Traffic between devices in the same data center
    -   Relatively fast response times
    
    North-south traffic  
    
    -   Ingress/egress to an outside device
    -   A different security posture than east-west traffic

7.  Zero trust

    Many networks are relatively open on the inside  
    
    -   Once you&rsquo;re through the firewall, there are few security controls
    
    Zero trust is a holistic approach to network security  
    
    -   Covers every device, every process, every person
    
    Everything must be verified  
    
    -   Nothing is trusted
    -   Multifactor authentication, encryption, system permissions, additional firewalls, monitoring and analytics, etc.



### Virtual Private Networks (VPNs)

Virtual Private Networks  

-   Encrypted (private) data traversing a public network

Concentrator  

-   Encryption/decryption access device
-   Often integrated into a firewall

Many deployment options  

-   Specialized cryptographic hardware
-   Software-based options available

Used with client software  

-   Sometimes built into the OS

On-demand access from a remote device  

-   Software connects to a VPN concentrator

Some software can be configured as always-on  

1.  SSL VPN (Secure Sockets Layer VPN)

    Uses common SSL/TLS protocol (tcp/443)  
    
    -   (Almost) No firewall issues!
    
    No big VPN clients  
    
    -   Usually remote access communication
    
    Authenticate users  
    
    -   No requirement for digital certificates or shared passwords (like IP Sec)
    
    Can be run from a browser or from a (usually light) VPN client  
    
    -   Across many operating systems

2.  HTMLS5 VPNs

    Hypertext Markup Language version 5  
    
    -   The language commonly used in web browsers
    
    Includes comprehensive APl support  
    
    -   Application Programming Interface
    -   Web cryptography API
    
    Create a VPN tunnel without a separate VPN application  
    
    -   Nothing to install
    
    Use an HTML5 compliant browser  
    
    -   Communicate directly to the VPN concentrator

3.  Tunnel type

    Full tunnel  
    
    -   All of the data is going to the encrypted tunnel, doesn&rsquo;t matter the destination
    
    Split tunnel  
    
    -   Only configured destinations are encrypted and pass through the VPN concentrator
    -   Configurable

4.  Site-to-site VPN

    Always-on  
    
    -   Or almost always
    
    Firewalls often act as VPN concentrators  
    
    -   Probably already have firewalls in place

5.  L2TP

    Layer 2 Tunneling Protocol  
    
    -   Connecting sites over a layer 3 network as if they were connected at layer 2
    
    Commonly implemented with IPsec  
    
    -   L2TP for the tunnel, IPsec for the encryption
    -   L2TP over IPsec (L2TP/IPsec)

6.  [IPSec (Internet Protocol Security)](#org28b7280)

    1.  Transport mode and tunnel mode
    
        Tunnel mode protect not only the data, but also the IP data  
        ![img](res/ipsec.png)  

7.  Authentication Header (AH)

    Hash of the packet and a shared key  
    
    -   SHA-2 Is common
    -   Adds the AH to the packet header
    
    This doesn’t provide encryption  
    
    -   Provides data integrity (hash)
    -   Guarantees the data origin (authentication)
    -   Prevents replay attacks (sequence numbers)

8.  Encapsulation Security Payload (ESP)

    Encrypts and authenticates the tunneled data  
    
    -   Commonly uses SHA-2 for hash, AES for encryption
    -   Adds a header, a trailer, and an Integrity Check Value
    
    Combine with Authentication Header (AH) for integrity and authentication of the outer header  

9.  IPsec Transport mode and Tunnel mode

    Tunnel mode is the most common  
    
    -   Transport mode may not even be an option



### Port security

There’s a lot of security that happens at the physical switch interface  

-   Often the first and last point of transmission

Control and protect  

-   Limit overall traffic
-   Control specific traffic types
-   Watch for unusual or unwanted traffic

Different options are available  

-   Manage different security issues

1.  Broadcasts

    Send information to everyone at once  
    
    -   One frame or packet, received by everyone
    -   Every device must examine the broadcast
    
    Limited scope  
    
    -   The broadcast domain
    
    Routing updates, ARP requests  
    
    -   Can add up quickly
    
    Malicious software or a bad NIC  
    
    -   Not always normal traffic
    
    Not used in IPv6  
    
    -   Focus on multicast

2.  Broadcast storm control

    The switch can control broadcasts  
    
    -   Limit the number of broadcasts per second
    
    Can often be used to control multicast and unknown unicast traffic  
    
    -   Tight security posture
    
    Manage by specific values or by percentage  
    
    -   Or the change over normal traffic patterns

3.  Loop protection

    Connect two switches to each other  
    
    -   They’ll send traffic back and forth forever
    -   There’s no “counting” mechanism at the MAC layer
    
    This is an easy way to bring down a network  
    
    -   And somewhat difficult to troubleshoot
    -   Relatively easy to resolve
    
    IEEE standard 802.1D to prevent loops in bridged (switched) networks (1990)  
    
    -   Created by Radia Perlman
    -   Used practically everywhere
    -   spanning tree protocol:  
        -   administrator disable some ports to avoid loops (*blocked ports*)
        -   constant monitoring itself (check for available interfaces) to block/unblock ports in case of unexpected failure

4.  BPDU guard

    Spanning tree takes time to determine if a switch port should forward frames  
    
    -   Bypass the listening and learning states
    -   Cisco calls this PortFast
    
    BPDU (Bridge Protocol Data Unit)  
    
    -   The spanning tree control protocol
    
    If a BPDU frame is seen on a PortFast configured interface (i.e., a workstation), shut down the interface  
    
    -   This shouldn’t happen
    -   Workstations don’t send BPDUs

5.  DHCP snooping

    IP tracking on a layer 2 device (switch)  
    
    -   The switch is a DHCP firewall
    -   Trusted: Routers, switches, DHCP seryers
    -   Untrusted: Other computers, unofficial DHCP servers
    
    Switch watches for DHCP conversations  
    
    -   Adds a list of untrusted devices to a table
    
    Filters invalid IP and DHCP information  
    
    -   Static IP addresses
    -   Devices acting as DHCP servers
    -   Other invalid traffic patterns

6.  MAC filtering

    Media Access Control  
    
    -   The “hardware” address
    
    Limit access through the physical hardware address  
    
    -   Keeps the neighbors out
    -   Additional administration with visitors
    
    Easy to find working MAC addresses through wireless LAN analysis  
    
    -   MAC addresses can be spoofed
    -   Free open-source software
    -   Security through obscurity
    
    <table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
    
    
    <colgroup>
    <col  class="org-right" />
    
    <col  class="org-left" />
    
    <col  class="org-left" />
    
    <col  class="org-right" />
    
    <col  class="org-left" />
    
    <col  class="org-left" />
    </colgroup>
    <thead>
    <tr>
    <th scope="col" class="org-right">rule number</th>
    <th scope="col" class="org-left">remote IP</th>
    <th scope="col" class="org-left">remote port</th>
    <th scope="col" class="org-right">local port</th>
    <th scope="col" class="org-left">protocol</th>
    <th scope="col" class="org-left">action</th>
    </tr>
    </thead>
    
    <tbody>
    <tr>
    <td class="org-right">1</td>
    <td class="org-left">all</td>
    <td class="org-left">any</td>
    <td class="org-right">22</td>
    <td class="org-left">TCP</td>
    <td class="org-left">allow</td>
    </tr>
    
    
    <tr>
    <td class="org-right">2</td>
    <td class="org-left">all</td>
    <td class="org-left">any</td>
    <td class="org-right">80</td>
    <td class="org-left">TCP</td>
    <td class="org-left">allow</td>
    </tr>
    
    
    <tr>
    <td class="org-right">3</td>
    <td class="org-left">all</td>
    <td class="org-left">any</td>
    <td class="org-right">443</td>
    <td class="org-left">TCP</td>
    <td class="org-left">allow</td>
    </tr>
    
    
    <tr>
    <td class="org-right">4</td>
    <td class="org-left">all</td>
    <td class="org-left">any</td>
    <td class="org-right">3389</td>
    <td class="org-left">TCP</td>
    <td class="org-left">allow</td>
    </tr>
    
    
    <tr>
    <td class="org-right">5</td>
    <td class="org-left">all</td>
    <td class="org-left">53</td>
    <td class="org-right">any</td>
    <td class="org-left">UDP</td>
    <td class="org-left">allow</td>
    </tr>
    
    
    <tr>
    <td class="org-right">6</td>
    <td class="org-left">all</td>
    <td class="org-left">123</td>
    <td class="org-right">any</td>
    <td class="org-left">UDP</td>
    <td class="org-left">allow</td>
    </tr>
    
    
    <tr>
    <td class="org-right">7</td>
    <td class="org-left">all</td>
    <td class="org-left">&#xa0;</td>
    <td class="org-right">&#xa0;</td>
    <td class="org-left">ICMP</td>
    <td class="org-left">deny</td>
    </tr>
    </tbody>
    </table>

7.  Firewall characterics

    Open-source vs. proprietary  
    
    -   Open-source provides traditional firewall functionality
    -   Proprietary features include application control and high-speed hardware
    
    Hardware vs. software  
    
    -   Purpose-built hardware provides efficient and flexible connectivity optlons
    -   Software-based firewalls can be installed almost anywhere
    
    Appliance vs. host-based vs. virtual  
    
    -   Appliances provide the fastest throughput
    -   Host-based firewalls are application-aware and can view non-encrypted data
    -   Virtual firewalls provide valuable East/West network security



### Network access control

1.  Edge vs access control

    Control at the edge  
    
    -   Your Internet link
    -   Managed primarily through firewall rules
    -   Firewall rules rarely change
    
    Access control  
    
    -   Control from wherever you are  
        -   Inside or outside
    -   Access can be based on many rules  
        -   By user, group, location, application, etc.
    -   Access can be easily revoked or changed  
        -   Change your security posture at any time

2.  Posture assessment

    You can’t trust everyone’s computer  
    
    -   BYOD (Bring Your Own Device)
    -   Malware infections / missing anti-malware
    -   Unauthorized applications
    
    Before connecting to the network, perform a health check  
    
    -   Is it a trusted device?
    -   Is it running anti-virus? Which one? Is it updated?
    -   Are the corporate applications installed?
    -   Is it a mobile device? Is the disk encrypted?
    -   The type of device doesn’t matter - Windows, Mac, Linux, iOS, Android

3.  Health checks / posture assessment

    Persistent agents  
    
    -   Permanently installed onto a system
    -   Periodic updates may be required
    
    Dissolvable agents  
    
    -   No installation is required
    -   Runs during the posture assessment
    -   Terminates when no longer required
    
    Agentless NAC  
    
    -   Integrated with Active Directory (in Windows)
    -   Checks are made during login and logoff
    -   Can&rsquo;t be scheduled

4.  Failing your assessment

    What happens when a posture assessment fails?  
    
    -   Too dangerous to allow access
    
    Quarantine network, notify administrators  
    
    -   Just enough network access to fix the issue
    
    Once resolved, try again  
    
    -   May require additional fixes



### Proxy servers

Sits between the users and the external network  
Receives the user requests and sends the request on their behalf (the proxy)  
Useful for caching information, access control, URL filtering, content scanning  
Applications may need to know how to use the proxy (explicit)  
Some proxies are invisible (transparent)  

1.  Application proxies

    One of the simplest “proxies” is NAT  
    
    -   A network-level proxy
    
    Most proxies In use are application proxies  
    
    -   The proxy understands the way the application works
    
    A proxy may only know one application  
    
    -   HTTP
    
    Many proxies are multipurpose proxies  
    
    -   HTTP, HTTPS, FTP, etc.

2.  Forward proxy

    An “internal proxy”  
    
    -   Commonly used to protect and control user access to the Internet

3.  Reverse proxy

    Inbound traffic from the Internet to your internal service  

4.  Open proxy

    A third-party, uncontrolled proxy  
    
    -   Can be a significant security concern
    -   Often used to circumvent existing security controls



### Intrusion prevention

1.  NIDS and NIPS

    Intrusion Detection System / Intrusion Prevention System  
    
    -   Watch network traffic
    
    Intrusions  
    
    -   Exploits against operating systems, applications, etc.
    -   Buffer overflows, cross-site scripting, other vulnerabilities
    
    Detection vs. Prevention  
    
    -   Detection - Alarm or alert
    -   Prevention - Stop it before it gets into the network

2.  Passive monitoring

    Examine a copy of the traffic  
    
    -   Port mirror (SPAN), network tap
    
    No way to block (prevent) traffic  

3.  Out-of-band response

    When malicious traffic is identified, IPS sends TCP RST (reset) frames  
    
    -   After-the-fact
    -   Limited UDP response available

4.  Inline monitoring

    IDS/IPS sits physically inline  
    
    -   All traffic passes through the IDS/IPS

5.  In-band response

    Malicious traffic is immediately identified  
    
    -   Dropped at the IPS
    -   Does not proceed through the network

6.  Identification technologies

    Signature-based  
    
    -   Look for a perfect match
    
    Anomaly-based  
    
    -   Build a baseline of what’s “normal”
    
    Behavior-based  
    
    -   Observe and report
    
    Heuristics  
    
    -   Use artificial intelligence to identify



### Other network appliances

1.  Jump server

    Access secure network zones  
    
    -   Provides an access mechanism to a protected network
    
    Highly-secured device  
    
    -   Hardened and monitored
    
    SSH / Tunnel / VPN to the jump server  
    
    -   RDP, SSH, or jump from there
    
    A significant security concern  
    
    -   Compromise to the jump server is a significant breach

2.  Hardware Security Module (HSM)

    Used in large environments  
    
    -   Clusters, redundant power
    
    High-end cryptographic hardware  
    
    -   Plug-in card or separate hardware device
    
    Key backup  
    
    -   Secured storage
    
    Cryptographic accelerators  
    
    -   Offload that CPU overhead from other devices

3.  Sensors and collectors

    Aggregate information from network devices  
    
    -   Built-in sensors, separate devices
    -   Integrated into switches, routers, servers, firewalls, etc.
    
    Sensors  
    
    -   Intrusion prevention systems, firewall logs, authentication logs,
    
    web server access logs, database transaction logs, email logs  
    Collectors  
    
    -   Proprietary consoles (IPS, firewall), SIEM consoles, syslog servers
    -   Many SIEMs include a correlation engine to compare diverse sensor data



## Given a scenario, install and configure wireless security settings

> **This section is lost/messed up due to poor vi-regex emulation inside emacs&#x2026;**  

Supplicant - the client  
Authenticator - The device that provides access  
Authentication server - Validates the client credentials  

1.  EAP-FAST

    EAP Flexible Authentication via Secure Tunneling  
    
    -   Authentication server (AS) and supplicant share a protected access credential (PAC) (shared secret)
    
    Supplicant receives the PAC  
    Supplicant and AS mutually authenticate and negotiate a Transport Layer Security (TLS) tunnel  
    User authentication occurs over the TLS tunnel  
    Need a RADIUS server  
    Provides the authentication database and EAP-FAST services  

2.  PEAP

    Protected Extensible Authentication Protocol  
    
    -   Protected EAP
    -   Created by Cisco, Microsoft, and RSA Security
    
    Also encapsulates EAP in a TLS tunnel  
    
    -   AS uses a digital certificate instead of a PAC
    -   Client doesn’t use a certificate
    
    User authenticates with MSCHAPv2  
    
    -   Authenticates to Microsoft’s MS-CHAPv2 databases
    
    User can also authenticate with a GTC  
    
    -   Generic Token Card
    -   Hardware token generator

3.  EAP-TLS

    EAP Transport Layer Security  
    
    -   Strong security, wide adoption
    -   Support from most of the industry
    
    Requires digital certificates on the AS and all other devices  
    
    -   AS and supplicant exchange certificates for mutual authentication
    -   TLS tunnel is then built for the user authentication process
    
    Relatively complex implementation  
    
    -   Need a public key infrastructure (PKI)
    -   Must deploy and manage certificates to all wireless clients
    -   Not all devices can support the use of digital certificates

4.  EAP-TTLS

    EAP Tunneled Transport Layer Security  
    
    -   Support other authentication protocols in a TLS tunnel
    
    Requires a digital certificate on the AS  
    
    -   Does not require digital certificates on every device
    -   Builds a TLS tunnel using this digital certificate
    
    Use any authentication method inside the TLS tunnel  
    
    -   Other EAPs
    -   MSCHAPvVZ
    -   Anything else

5.  RADIUS Federation

    Use RADIUS with federation  
    
    -   Members of one organization can authenticate to the network of another organization
    -   Use their normal credentials
    
    Use 802.1X as the authentication method  
    
    -   And RADIUS on the backend
    -   EAP to authenticate
    
    Driven by eduroam (education roaming)  
    
    -   Educators can use theit normal authentication when visiting a different campus
    -   <https://www.eduroam.org/>



### Installing wireless networks

1.  Site surveys

    Determine existing wireless landscape  
    
    -   Sample the existing wireless spectrum
    
    ldentify existing access points  
    
    -   You may not control all of them
    
    Work around existing frequencies  
    
    -   Layout and plan for interference
    
    Plan for ongoing site surveys  
    
    -   Things will certainly change
    
    Heat maps  
    
    -   ldentify wireless signal strengths

2.  Wireless surveys tools

    Signal coverage  
    Potential interference  
    Built-in tools  
    3rd-party tools  
    Spectrum analyzer  

3.  Wireless packet analyzer

    Wireless networks are incredibly easy to monitor  
    
    -   Everyone “hears” everything
    
    You have to be quiet  
    
    -   You can’t hear the network if you’re busy transmitting
    
    Some network drivers won’t  
    capture wireless information  
    
    -   You’ll need specialized adapters/chipsets and drivers
    
    View wireless-specific information  
    
    -   Signal-to-noise ratio, channel information, etc.
    
    Try it yourself!  
    
    -   <http://www.wireshark.org>

4.  Channel selection and overlaps

    Overlapping channels  
    
    -   Frequency conflicts - use non-overlapping channels
    -   Automatic or manual configurations

5.  Access point placement

    Minimal overlap  
    
    -   Maximize coverage, minimize the number of access points
    
    Avoid interference  
    
    -   Electronic devices (microwaves)
    -   Building materials
    -   Third-party wireless networks
    
    Signal control  
    
    -   Place APs where the users are
    -   Avoid excessive signal distance

6.  Wireless infrastructure security

    Wireless controllers  
    
    -   Centralized management of wireless access points
    -   Manage system configuration and performance
    
    Securing wireless controllers  
    
    -   Control access to management console
    -   Use strong encryption with HTTPS
    -   Automatic logout after no activity
    
    Securing access points  
    
    -   Use strong passwords
    -   Update to the latest firmware



## Given a scenario, implement secure mobile solutions



### Mobile Networks

1.  Point-to-point

    One-to-one connection  
    
    -   Conversation between two devices
    
    Connections between buildings  
    
    -   Point-to-point network links
    
    Wi-Fi repeaters  
    
    -   Extend the length of an existing network

2.  Point-to-multipoint

    One of the most popular communication methods today  
    
    -   802.11 wireless
    
    Does not imply full connectivity between nodes  

3.  Cellular networks

    Mobile devices  
    
    -   “Cell” phones
    
    Separate land into “cells”  
    
    -   Antenna coverages a cell with certain frequencies
    
    Security concerns  
    
    -   Traffic monitoring
    -   Location tracking
    -   Worldwide access to a mobile device

4.  Wi-Fi

    Local network access  
    
    -   Local security problems
    
    Same security concerns as other Wi-Fi devices  
    Data capture  
    
    -   Encrypt your data!
    
    On-path attack  
    
    -   Modify and/or monitor data
    
    Denial of service  
    
    -   Frequency interference

5.  Bluetooth

    High speed communication over short distances  
    
    -   PAN (Personal Area Network)
    
    Connects our mobile devices  
    
    -   Smartphones
    -   Tethering
    -   Headsets and headphones
    -   Health monitors
    -   Automobile and phone integration
    -   Smartwatches
    -   External speakers

6.  [RFID (Radio-frequency identification)](#orgaea4b97)

7.  [Near field communication (NFC)](#orgfc9cbb5)

    1.  [NCF secutiry concerns](#orgba1d006)

8.  IR (infrared)

    Included on many smartphones, tablets, and smartwatches  
    
    -   Not really used much for printing
    
    Control your entertainment center  
    
    -   Almost exclusively IR
    
    File transfers are possible  
    Other phones can be used to control yout IR devices  

9.  USB (universal serial bus)

    Physical connectivity to your mobile device  
    
    -   USB to your computer
    -   USB, Lightning, or proprietary on your phone
    
    Physical access is always a concern  
    
    -   May be easier to gain access than over a remote connection
    
    A locked device is relatively secure  
    
    -   Always auto-lock
    
    Mobile phones can also exfiltrate  
    
    -   Phone can appear to be a USB storage device

10. Global Positioning System (GPS)

    Created by the U.S. Department of Defense  
    
    -   Over 30 satellites currently in orbit
    
    Precise navigation  
    
    -   Need to see at least 4 satellites
    
    Determines location based on timing dlfferences  
    
    -   Longitude, latitude, altitude
    
    Mobile device location services and geotracking  
    
    -   Maps, directions
    -   Determine physical location based on GPS, WiFi, and cellular towers



### Mobile device management (MDM)

Manage company-                                                                   owned and user-owned mobile devices  

-   BYOD - Bring Your Own Device

Centralized management of the mobile devices  

-   Specialized functionality

Set policies on apps, data, camera, etc.  

-   Control the remote device
-   The entire device or a “partition”

Manage access control  

-   Force screen locks and PINs on these single user devices

1.  Application management

    Managing mobile apps are a challenge  
    
    -   Mobile devices install apps constantly
    
    Not all applications are secure  
    
    -   And some are malicious
    -   Android malware is a rapidly growing security concern
    
    Manage application use through allow lists  
    
    -   Only approved applications can be installed
    -   Managed through the MDM
    
    A management challenge  
    
    -   New applications must be checked and added

2.  Content management

    Mobile Content Management (MCM)  
    
    -   Secure access to data
    -   Protect data from outsiders
    
    File sharing and viewing  
    
    -   On-site content (Microsoft Sharepoint, file servers)
    -   Cloud-based storage (Box, Office 365)
    
    Data sent from the mobile device  
    
    -   DLP (Data Loss Prevention) prevents copy/paste of sensitive data
    -   Ensure data is encrypted on the mobile device
    
    Managed from the mobile device manager (MDM)  

3.  Remote wipe

    Remove all data from your mobile device  
    
    -   Even if you have no idea where it is
    -   Often managed from the MDM
    
    Connect and wipe from the web  
    
    -   Nuke it from anywhere
    
    Need to plan for this  
    
    -   Configure your mobile device now
    
    Always have a backup  
    
    -   Your data can be removed at any time
    -   As you are walking out the door

4.  Geolocation

    Precise tracking details  
    
    -   Tracks within feet
    
    Can be used for good (or bad)  
    
    -   Find your phone
    -   Find you
    
    Most phones provide an option to disable  
    
    -   Limits functionality of the phones
    
    May be managed by the MDM  

5.  Geofencing

    Some MDMs allow for geofencing  
    
    -   Restrict or allow features when the device is in a particular area
    
    Cameras  
    
    -   The camera might only work when outside the office
    
    Authentication  
    
    -   Only allow logins when the device is located in a particular area

6.  Screen lock

    All mobile devices can be locked  
    
    -   Keep people out of your data
    
    Simple passcode or strong passcode  
    
    -   Numbers vs. Alphanumeric
    
    Fail too many times?  
    
    -   Erase the phone
    
    Define a lockout policy  
    
    -   Create aggressive lockout timers
    -   Completely lock the phone

7.  Push notification services

    Information appears on the mobile device screen  
    
    -   The notification is “pushed” to your device
    
    No user intervention  
    
    -   Receive notifications from one app when using a completely different app
    
    Control of displayed notifications can be managed from the MDM  
    
    -   Or notifications can be pushed from the MDM

8.  Passwords and PINs

    The universal help desk call  
    
    -   I need to reset my password
    
    Mobile devices use multiple authentication methods  
    
    -   Password/passphrase, PINs, patterns
    
    Recovery process can be initiated from the MDM  
    
    -   Password reset option is provided on the mobile device
    -   “What is the name of your favorite car maiden cat’s color?”
    
    MDM also has full control  
    
    -   Completely remove all security controls
    -   Not the default or best practice

9.  Biometrics

    You are the authentication factor  
    
    -   Fingerprint, face
    
    May not be the most secure authentication factor  
    
    -   Useful in some environments
    -   Completely forbidden in others
    
    Availability is managed through the MDM  
    
    -   Organization determines the security of the device
    
    Can be managed per-                                                                   app  
    
    -   Some apps require additional biometric authentication

10. Context-                                                                   aware authentication

    Who needs 2FA?  
    
    -   The attackers can get around anything
    
    Authentication can be contextual  
    
    -   If it walks like a duck&#x2026;
    
    Combine multiple contexts  
    
    -   Where you normally login (IP address)
    -   Where you normally frequent (GPS information)
    -   Other devices that may be paired (Bluetooth, etc.)
    -   And others
    
    An emerging technology  
    
    -   Another way to keep data safe

11. Containerization

    Difficult to separate personal from business  
    
    -   Especially when the device is BYOD
    -   Owned by the employee
    
    Separate enterprise mobile apps and data  
    
    -   Create a virtual “container” for company data
    -   A contained area - limit data sharing
    -   Storage segmentation keeps data separate
    
    Easy to manage offboarding  
    
    -   Only the company information is deleted
    -   Personal data is retained
    -   Keep your pictures, video, music, email, etc.

12. Full device encryption

    Scramble all of the data on the mobile device  
    
    -   Even if you lose it, the contents are safe
    
    Devices handle this in different ways  
    
    -   Strongest/stronger/strong ?
    
    Encryption isn’t trivial  
    
    -   Uses a lot of CPU cycles
    -   Complex integration between hardware and software
    
    Don’t lose or forget your password!  
    
    -   There’s no recovery
    -   Often backed un on the MDM



### Mobile device security

1.  MicroSD HSM

    Shrink the PCl Express Hardware Security Module  
    
    -   Now in a microSD card form
    
    Provides security services  
    
    -   Encryption
    -   Key generation
    -   Digital signatures
    -   Authentication
    
    Secure storage  
    
    -   Protect private keys
    -   Cryptocurrency storage

2.  Unified Endpoint Management (UEM)

    Manage mobile and non-                         mobile devices  
    
    -   An evolution of the Mobile Device Manager (MDM)
    
    End users use different types of devices  
    
    -   Their use has blended together
    
    Applications can be used across different platforms  
    
    -   Work on a laptop and a smartphone
    
    All of these devices can be used from anywhere  
    
    -   User’s don’t stay in one place

3.  Mobile Application Management (MAM)

    Provision, update, and remove apps  
    
    -   Keep everyone running at the correct version
    
    Create an enterprise app catalog  
    
    -   Users can choose and install the apps they need
    
    Monitor application use  
    
    -   Apps used on a device
    -   Devices with unauthorized apps
    
    Remotely wipe application data  
    
    -   Securely manage remote data

4.  SEAndroid

    Security Enhancements for Android  
    
    -   SELinux (Security-Enhanced Linux) in the Android OS
    -   Supports access control security policies
    
    A project from the US National Security Agency (NSA)  
    
    -   Based on the NSA’s SELinux
    
    Addresses a broad scope of system security  
    
    -   Kernel, userspace, and policy configuration
    
    Enabled by default with Android version 4.3  
    
    -   July 2013
    
    Protect privileged Android system daemons  
    
    -   Prevent malicious activity
    
    Change from Discretionary Access Control (DAC) to Mandatory Access Control (MAC)  
    
    -   Move from user-assigned control to object labels and minimum user access
    -   Isolates and sandboxes Android apps
    
    Centralized policy configuration  
    
    -   Manage Android deployments



### Mobile device enforcement

1.  Third-    party app stores

    Centralized app clearinghouses  
    
    -   Apple App Store
    -   Google Play
    
    Not all applications are secure  
    
    -   Vulnerabilities, data leakage
    
    Not all applications are appropriate for business use  
    
    -   Games, instant messaging, etc.
    
    MDM can allow or deny app store use  

2.  Rooting/jailbreaking

    Mobile devices are purpose-      built systems  
    
    -   You don’t need access to the operating system
    
    Gaining access  
    
    -   Android - Rooting
    -   Apple i0S - Jailbreaking
    
    Install custom firmware  
    
    -   Replaces the existing operating system
    
    Uncontrolled access  
    
    -   Circumvent security features, sideload apps without using an app store
    -   The MDM becomes relatively useless

3.  Carrier unlocking

    Most phones are locked to a carrier  
    
    -   You can’t use an AT&T phone on Verizon
    -   Your contract with a carrier subsidizes the cost of the phone
    
    You can unlock the phone  
    
    -   If your carrier allows it
    -   A carrier lock may be illegal in your country
    
    Security revolves around connectivity  
    
    -   Moving to another carrier can circumvent the MDM
    -   Preventing a SIM unlock may not be possible on a personal device

4.  Firmware OTA updates

    The operating system of a mobile device is constantly changing  
    
    -   Similar to a desktop computer
    
    Updates are provided over the air (OTA)  
    
    -   No cable required
    
    Security patches or entire operating system updates  
    
    -   Significant changes without connecting the device
    
    This may not be a good thing  
    
    -   The MDM can manage what OTA updates are allowed

5.  Camera use

    Cameras are controversial  
    
    -   They’re not always a good thing
    -   Corporate espionage, inappropriate use
    
    Almost impossible to control on the device  
    
    -   No good way to ensure the camera won’t be used
    
    Camera use can be controlled by the MDM  
    
    -   Always disabled
    -   Enabled except for certain locations (geo-fencing)

6.  SMS/MMS

    Short Message Service / Multimedia Messaging Service  
    
    -   Text messages, video, audio
    
    Control of data can be a concern  
    
    -   OQutbound data leaks, financial disclosures
    -   Inbound notifications, phishing attempts
    
    MDM can enable or disable SMS/MMS  
    
    -   Or only allow during certain timeframes or locations

7.  External media

    Store data onto external or removable drives  
    
    -   SD flash memory or USB/lightning drives
    
    Transfer data from flash  
    
    -   Connect to a computer to retrieve
    
    This is very easy to do  
    
    -   Limit data written to removable drives
    -   Or prevent the use of them from the MDM

8.  USB OTG

    USB On-The-Go  
    
    -   Connect mobile devices directly together
    -   No computer required, only a cable
    
    The mobile device can be both a host and a device  
    
    -   Read from an external device, then act as a storage device itself
    -   No need for a third-party storage device
    
    A USB 2.0 standard  
    
    -   Commonly seen on Android devices
    
    Extremely convenient  
    
    -   From a security perspective, it&rsquo;s too convenient

9.  Recording microphone

    Audio recordings  
    
    -   There are microphones on every mobile device
    
    Useful for meetings and note taking  
    
    -   A standard for college classes
    
    A legal liability  
    
    -   Every state has different laws
    -   Every situation is different
    
    Disable or geo-fence  
    
    -   Manage from the MDM

10. Geotagging / GPS tagging

    Your phone knows where you are  
    
    -   Location Services, GPS
    
    Adds your location to document metadata  
    
    -   Longitude, latitude
    -   Photos, videos, etc.
    
    Every document may contain geotagged information  
    
    -   You can track a user quite easily
    
    This may cause security concerns  
    
    -   Take picture, upload to social media

11. Wifi Direct / ad hoc

    We&rsquo;re so used to access points  
    
    -   SSID configurations
    
    The wireless standard includes an ad hoc mode  
    
    -   Connect wireless devices directly
    -   Without an access point
    
    WiFi Direct simplifies the process  
    
    -   Easily connect many devices together
    -   Common to see in home devices
    
    Simplicity can aid vulnerabilities  
    
    -   Invisible access to important devices

12. Hotspot / tethering

    Turn your phone into a WiFi hotspot  
    
    -   Your own personal wireless router
    -   Extend the cellular data network to all of your devices
    
    Dependent on phone type and provider  
    
    -   May require additional
    
    charges and data costs  
    May provide inadvertent access to an internal network  
    
    -   Ensure proper security / passcode

13. Payment methods

    Send small amounts of data wirelessly over a limited area (NFC)  
    
    -   Built into your phone
    -   Payment systems, transportation, in-person information exchange
    
    A few different standards  
    
    -   Apple Pay, Android Pay, Samsung Pay
    
    Bypassing primary authentication would allow payment  
    
    -   Use proper security
    -   Or disable completely



### Mobile Deployment Models

1.  BYOD

    Bring Your Own Device  
    Bring Your Own Technology  
    Employee owns the device  
    
    -   Need to meet the company’s requirements
    
    Difficult to secure  
    
    -   It&rsquo;s both a home device and a work device
    -   How is data protected?
    -   What happens to the data when a device is sold or traded in?

2.  COPE

    Corporate owned, personally enabled  
    
    -   Company buys the device
    -   Used as both a corporate device and a personal device
    
    Organization keeps full control of the device  
    
    -   Similar to company-owned laptops and desktops
    
    Information is protected using corporate policies  
    
    -   Information can be deleted at any time
    
    CYOD - Choose Your Own Device  
    
    -   Similar to COPE, but with the user’s choice of device

3.  Corporate owned

    The company owns the device  
    
    -   And controls the content on the device
    
    The device is not for personal use  
    
    -   You’ll need to buy your own device for home
    
    Very specific security requirements  
    
    -   Not able to mix business with home use

4.  VDI/VMI

    Virtual Desktop Infrastructure / Virtual Mobile Infrastructure  
    
    -   The apps are separated from the mobile device
    -   The data is separated from the mobile device
    
    Data is stored securely, centralized  
    Physical device loss - Risk is minimized  
    Centralized app development  
    
    -   Write for a single VMI platform
    
    Applications are managed centrally  
    
    -   No need to update all mobile devices



## Given a scenario, apply cybersecurity solutions to the cloud



### Cloud Security Controls

1.  HA across zones

    Availability zones (AZ)  
    
    -   Isolated locations within a cloud region (geographical location)
    -   AZ commonly spans across multiple regions
    -   Each AZ has independent power, HVAC, and networking
    
    Build applications to be highly available (HA)  
    
    -   Run as active/standby or active/active
    -   Application recognizes an outage and moves to the other AZ
    
    Use load balancers to provide seamless HA  
    
    -   Users don’t experience any application issues

2.  Resource policies

    ldentity and access management (IAM)  
    
    -   Who gets access
    -   What they get access to
    
    Map job functions to roles  
    
    -   Combine users into groups
    
    Provide access to cloud resources  
    
    -   Set granular policies
    -   Group, |IP address, date and time
    
    Centralize user accounts  
    
    -   Synchronize across all platforms

3.  Secrets management

    Cloud computing includes many secrets  
    
    -   APl keys, passwords, certificates
    
    This can quickly become overwhelming  
    
    -   Difficult to manage and protect
    
    Authorize access to the secrets  
    
    -   Limit access to the secret service A Reest
    
    Manage an access control policy  
    
    -   Limit users to only necessary secrets
    
    Provide an audit trail  
    
    -   Know exactly who accesses secrets and when

4.  Integration and auditing

    Integrate security across multiple platforms  
    
    -   Different operating systems and applications
    
    Consolidate log storage and reporting  
    
    -   Cloud-based Security Information and Event Management (SIEM)
    
    Auditing  
    
    -   Validate the security controls
    -   Verify compliance with financial and user data



### Securing cloud storage

Data is on a public cloud  

-   But may not be public data

Access can be limited  

-   And protected

Data may be required in  
different geographical locations  

-   A backup is always required

Availability is always important  

-   Data is available as the cloud changes

1.  Permissions

    A significant cloud storage concern  
    
    -   One permission mistake can cause a data breach
    -   Accenture, Uber, US Department of Defense
    
    Public access  
    
    -   Should not usually be the default
    
    Many different options  
    
    -   ldentity and Access Management (IAM)
    -   Bucket policies
    -   Globally blocking public access
    -   Don’t put data in the cloud unless it really needs to be there

2.  Encryption

    Cloud data is more accessible than non-cloud data  
    
    -   More access by more people
    
    Server-side encryption  
    
    -   Encrypt the data in the cloud
    -   Data is encrypted when stored on disk
    
    Client-side encryption  
    
    -   Data is already encrypted when it’s sent to the cloud
    -   Performed by the application
    
    Key management is critical  

3.  Replication

    Copy data from one place to another  
    
    -   Real-time data duplication in multiple locations
    
    Disaster recovery, high availability  
    
    -   Plan for problems
    -   Maintain uptime if an outage occurs
    -   Hot site for disaster recovery
    
    Data analysis  
    
    -   Analytics, big data analysis
    
    Backups  
    
    -   Constant duplication of data



### Securing cloud networks

Connect cloud components  

-   Connectivity within the cloud
-   Connectivity from outside the cloud

Users communicate to the cloud  

-   From the public Internet
-   Over a VPN tunnel

Cloud devices communicate between each other  

-   Cloud-based network
-   East/west and north/south communication
-   No external traffic flows

1.  Virtual networks

    A cloud contains virtual devices  
    
    -   Servers, databases, storage devices
    
    Virtual switches, virtual routers  
    
    -   Build the network from the cloud console
    -   The same configurations as a physical device
    
    The network changes with the rest of the infrastructure  
    
    -   On-demand
    -   Rapid elasticity

2.  Public and private subnets

    Private cloud  
    
    -   All internal IP addresses
    -   Connect to the private cloud over a VPN
    -   No access from the Internet
    
    Public cloud  
    
    -   External IP addresses
    -   Connect to the cloud from anywhere
    
    Hybrid cloud  
    
    -   Combine internal cloud resources with external
    -   May combine both public and private subnets

3.  Segmentation

    The cloud contains separate VPCs, containers, and microservices  
    
    -   Application segmentation is almost guaranteed
    
    Separation Is a security opportunity  
    
    -   Data is separate from the application
    -   Add security systems between application components
    
    Virtualized security technologies  
    
    -   Web Application Firewall (WAF)
    -   Next-Generation Firewall (NGFW)  
        -   Intrusion Prevention System (IPS)

4.  API inspection and integration

    Microservice architecture is the underlying application engine  
    
    -   A significant security concern
    
    API calls can include risk  
    
    -   Attempts to access critical data
    -   Geographic origin
    -   Unusual API calls
    
    APl monitoring  
    
    -   View specific APl queries
    -   Monitor incoming and outgoing data



### Securing compute clouds

1.  Compute cloud instances

    The IaaS component for the cloud computing environment  
    
    -   Amazon Elastic Compute Cloud (EC2)
    -   Google Compute Engine (GCE)
    -   Microsoft Azure Virtual Machines
    
    Manage computing resources  
    
    -   Launch a VM or container
    -   Allocate additional resources
    -   Disable/remove a VM or container

2.  Security groups

    A firewall for compute instances  
    
    -   Control inbound and outbound traffic flows
    
    Layer 4 port number  
    
    -   TCP or UDP port
    
    Layer 3 address  
    
    -   Individual addresses
    -   CIDR block notation
    -   IPv4 or IPv6

3.  Dynamic resource allocation

    Provision resources when they are needed  
    
    -   Based on demand
    -   Provisioned automatically
    
    Scale up and down  
    
    -   Allocate compute resources where and when they are needed
    -   Rapid elasticity
    -   Pay for only what’s used
    
    Ongoing monitoring  
    
    -   If CPU utilization hits a particular threshold, provision a new application instance

4.  Instance awareness

    Granular security controls  
    
    -   Identify and manage very specific data flows
    -   Each instance of a data flow is different
    
    Define and set policies  
    
    -   Allow uploads to the corporate box.com file share  
        -   Corporate file shares can contain PII
        -   Any department can upload to the corporate file share
    -   Deny certain uploads to a personal box.com file share  
        -   Allow graphics files
        -   Deny any spreadsheet
        -   Deny files containing credit card numbers
        -   Quarantine the file and send an alert

5.  Virtual private cloud endpoints

    VPC gateway endpoints  
    
    -   Allow private cloud subnets to communicate to otherkcloud services
    
    Keep private resources private  
    
    -   Internet connectivity not required
    
    Add an endpoint to connect  
    VPC resources  

6.  Container security

    Containers have similar security concerns as any other application deployment method  
    
    -   Bugs, insufficient security controls, misconfigurations
    
    Use container-specific operating systems  
    
    -   A minimalist OS designed for containers
    
    Group container types on the same host  
    
    -   The same purpose, sensitivity, and threat posture
    -   Limit the scope of any intrusion



### Cloud security solutions

1.  Cloud access security broker (CASB)

    Clients are at work, data is in the cloud  
    
    -   How do you keep everything secure?
    -   The organization already has well-defined security policies
    
    How do you make your security policies work in the cloud?  
    
    -   Integrate a CASB
    -   Implemented as client software, local security appliances, or cloud-based security solutions
    
    Components:  
    
    1.  Visibility  
        -   Determine what apps are in use
        -   Are they authorized to use the apps?
    2.  Compliance  
        -   Are users complying with HIPAA? PCI?
    3.  Threat prevention  
        -   Allow access by authorized users, prevent attacks
    4.  Data security  
        -   Ensure that all data transfers are encrypted
        -   Protect the transfer of PIl with DLP

2.  Application security

    Secure cloud-based applications  
    
    -   Complexity increases in the cloud
    
    Application misconfigurations  
    
    -   One of the most common security issues
    -   Especially cloud storage
    
    Authorization and access s,  
    
    -   Controls should be strong enough for access from anywhere .
    
    APl security  
    
    -   Attackers will try to exploit interfaces and APIs

3.  Next-Gen Secure Web Gateway (SWG)

    Protect users and devices  
    
    -   Regardless of location and activity
    
    Go beyond URLs and GET requests  
    
    -   Examine the application API
    -   Dropbox for personal use or corporate use?
    
    Examine JSON strings and API requests  
    
    -   Allow or disallow certain activities
    
    Instance-aware security  
    
    -   A development instance is different than a production instance

4.  Firewalls in the cloud

    Control traffic flows in the cloud  
    
    -   Inside the cloud and external flows
    
    Cost  
    
    -   Relatively inexpensive compared to appliances
    -   Virtual firewalls
    -   Host-based firewalls
    
    Segmentation  
    
    -   Between microservices, VMSs, or VPCs
    
    OSl layers  
    
    -   Layer 4 (TCP/UDP), Layer 7 (Application)

5.  Security controls

    Cloud-native security controls  
    
    -   Integrated and supported by the cloud provider
    -   Many configuration options
    -   Security is part of the infrastructure
    -   No additional costs
    
    Third-party solutions  
    
    -   Support across multiple cloud providers
    -   Single pane of glass
    -   Extend policies outside the scope of the cloud provider
    -   More extensive reporting



## Given a scenario, implement identity and account management controls



### Identity controls

1.  Identity provider (IdP)

    Who are you?  
    
    -   A service needs to vouch for you
    -   Authentication as a Service
    
    A list of entities  
    
    -   Users and devices
    
    Commonly used by SSO applications or an authentication process  
    
    -   Cloud-based services need to know who you are
    
    Uses standard authentication methods  
    
    -   SAML, OAuth, OpenlID Connect, etc.

2.  Attributes

    An identifier or property of an entity  
    
    -   Provides identification
    
    Personal attributes  
    
    -   Name, email address, phone number, Employee ID
    
    Other attributes  
    
    -   Department name, job title, mail stop
    
    One or more attributes can be used for identification  
    
    -   Combine them for more detail

3.  Certificates

    Digital certificate  
    
    -   Assignhed to a person or device
    
    Binds the identity of the certificate owner to a public and private key  
    
    -   Encrypt data
    -   Create digital signatures
    
    Requires an existing public-key infrastructure (PKl)  
    
    -   The Certificate Authority (CA) is the trusted entity
    -   The CA digitally signs the certificates

4.  Token and cards

    Smart card  
    
    -   Integrates with devices
    -   May require a PIN
    
    USB token  
    
    -   Certificate is on the USB device

5.  SSH keys

    Secure Shell (SSH)  
    
    -   Secure terminal communication
    
    Use a key instead of username and password  
    
    -   Public/private keys
    -   Critical for automation
    
    Key management is critical  
    
    -   Centralize, control, and audit key use
    
    SSH key managers  
    
    -   Open source
    -   Commercial

6.  SSH key-based authentication

    Create a public/private key pair  
    
    -   ssh-keygen
    
    Copy the public key to the SSH server  
    
    -   ssh-copy-id -user@host
    
    Try it out  
    
    -   ssh user@host
    -   No password prompt!



### Account types

1.  User accounts

    An account on a computer associated with a specific person  
    
    -   The computer associates the user with a specific identification number
    
    Storage and files can be private to that user  
    
    -   Even if another person is using the same computer
    
    No privileged access to the operating system  
    
    -   Specifically not allowed on a user account
    
    This is the account type most people will use  
    
    -   Your user community

2.  Shared and generic accounts

    Shared account  
    
    -   Used by more than one person
    -   Guest login, anonymous login
    
    Very difficult to create an audit trail  
    
    -   No way to know exactly who was working
    -   Difficult to determine the proper privileges
    
    Password management becomes difficult  
    
    -   Password changes require notifying everyone
    -   Difficult to remember so many password changes
    -   Just write it down on this yellow sticky paper
    
    Best practice: Don’t use these accounts  

3.  Guest accounts

    Access to a computer for guests  
    
    -   No access to change settings, modify applications, view other user’s files, and more
    -   Usually no password
    
    This brings significant security challenges  
    
    -   Access to the userspace is one step closer to an exploit
    
    Must be controlled  
    
    -   Not the default
    -   Removed from Windows 10 build 10159

4.  Service accounts

    Used exclusively by services running on a computer  
    
    -   No interactive/user access (ideally)
    -   Web server, database server, etc.
    
    Access can be defined for a specific service  
    
    -   Web server rights and permissions will be different than a database server
    
    Commonly use usernames and passwords  
    
    -   You’ll need to determine the best policy for password updates

5.  Privileged accounts

    Elevated access to one or more systems  
    
    -   Administrator, Root
    
    Complete access to the system  
    
    -   Often used to manage hardware, drivers, and software installation
    
    This account should not be used for normal administration  
    
    -   User accounts should be used
    
    Needs to be highly secured  
    
    -   Strong passwords, 2FA
    -   Scheduled password changes



### Account policies

Control access to an account  

-   It’&rsquo;s more than just username and password
-   Determine what policies are best for an organization

The authentication process  

-   Password policies
-   Authentication factor policies
-   Other considerations

Permissions after login  

-   Another line of defense

1.  Perform routine audits

    Is everything following the policy?  
    
    -   You have to police yourself
    
    It’s amazing how quickly things can change  
    
    -   Make sure the routine is scheduled
    
    Certain actions can be automatically identified  
    
    -   Consider a tool for log analysis

2.  Auditing

    Permission auditing  
    
    -   Does everyone have the correct permissions?
    -   Some Administrators don’t need to be there
    -   Scheduled recertification
    
    Usage auditing  
    
    -   How are your resources used? A
    -   Are your systems and applications secure?

3.  Password complexity and length

    Make your password strong  
    
    -   Resist guessing or brute-force attack
    
    Increase password entropy  
    
    -   No single words, no obvious passwords  
        -   What’s the name of your dog?
    -   Mix upper and lower case and use special characters  
        -   Don’t replace a o with a O, t with a 7
    
    Stronger passwords are at least 8 characters  
    
    -   Consider a phrase or set of words
    
    Prevent password reuse  
    
    -   System remembers password history, requires unique passwords

4.  Account lockout and disablement

    Too many incorrect passwords will cause a lockout  
    
    -   Prevents online brute force attacks
    -   This should be normal for most user accounts
    -   This can cause big issues for service accounts  
        -   You might want this
    
    Disabling accounts  
    
    -   Part of the normal change process
    -   You don’t want to delete accounts  
        -   At least not initially
        -   May contain important decryption keys

5.  Location-based policies

    Network location  
    
    -   Identify based on IP subnet
    -   Can be difficult with mobile devices
    
    Geolocation - determine a user’s location  
    
    -   GPS - mobile devices, very accurate
    -   802.11 wireless, less accurate
    -   IP address, not very accurate
    
    Geofencing  
    
    -   Automatically allow or restrict access when the user is in a particular location
    -   Don’t allow this app to run unless you’re near the office
    
    Geotagging  
    
    -   Add location metadata to a document or file
    -   Latitude and longitude, distance, time stamps
    
    Location-based access rules  
    
    -   Your IP address is associated with an IP block in Russia
    -   We don’t have an office in Russia
    -   You were in Colorado Springs an hour ago
    -   Permission not granted
    
    Time-based access rules  
    
    -   Nobody needs to access the lab at 3 AM



## Given a scenario, implement authentication and authorization solutions



### Authentication management

1.  Password keys

    Hardware-based authentication  
    
    -   Something you have
    
    Helps prevent unauthorized logins and account takeovers  
    
    -   The key must be present to login
    
    Doesn’t replace other factors  
    
    -   Passwords are still important

2.  Password vaults

    Password managers  
    
    -   All passwords in one location
    -   A database of credentials
    
    Secure storage  
    
    -   All credentials are encrypted
    -   Cloud-based synchronization options
    
    Create unique passwords  
    
    -   Passwords are not the same across sites
    
    Personal and enterprise options  
    
    -   Corporate access

3.  [Trusted Platform Module (TPM)](#org9e5494e)

4.  [Hardware Security Module (HSM)](#org0f03c9d)

5.  Knowledge-based authentication (KBA)

    Use personal knowledge as an authentication factor  
    
    -   Something you know
    
    Static KBA  
    
    -   Pre-configured shared secrets
    -   Often used with account recovery
    -   What was the make and model of your first car?
    
    Dynamic KBA  
    
    -   Questions are based on an identity verification service
    -   What was your street number when you lived in Pembroke Pines, Florida?



### PAP and CHAP

1.  PAP (Password Authentication Protocol)

    A basic authentication method  
    
    -   Used in legacy operating systems
    -   Rare to see singularly used
    
    PAP is in the clear v  
    
    -   Weak authentication scheme
    -   Non-encrypted password exchange
    -   We didn’t require encryption on analog dialup lines
    -   The application would need to provide any encryption

2.  CHAP

    Challenge-Handshake Authentication Protocol  
    
    -   Encrypted challenge sent over the network
    
    Three-way handshake  
    
    -   After link is established, server sends a challenge message
    -   Client responds with a password hash calculated from the challenge and the password
    -   Server compares received hash with stored hash
    
    Challenge-Response continues  
    
    -   Occurs periodically during the connection
    -   User never knows it happens

3.  MS-CHAP

    Microsoft’s implementation of CHAP  
    
    -   Used commonly on Microsoft’s Point-to-Point Tunneling Protocol (PPTP) MS-CHAP v2 is the more recent version
    
    Security issues related to the use of DES  
    
    -   Relatively easy to brute force the 256 possible keys to decrypt the NTLM hash
    -   Don’t use MS-CHAP!
    -   Consider L2TP, IPsec, 802.1X or some other secure authentication method



### Identity and access services

1.  RADIUS (Remote Authentication Dial-in User Service)

    One of the more common AAA protocols  
    
    -   Supported on a wide variety of platforms and devices
    -   Not just for dial-in
    
    Centralize authentication for users  
    
    -   Routers, switches, firewalls
    -   Server authentication
    -   Remote VPN access
    -   802.1X network access
    
    RADIUS services available on almost any server operating system  

2.  TACACS

    Terminal Access Controller Access-Control System  
    
    -   Remote authentication protocol
    -   Created to control access to dial-up lines to ARPANET
    
    XTACACS (Extended TACACS)  
    
    -   A Cisco-created (proprietary) version of TACACS
    -   Additional support for accounting and auditing
    
    TACACS+  
    
    -   The Iatesf version of TACACS, not backwards compatible
    -   More authentication requests and response codes
    -   Released as an open standard in 1993

3.  Kerberos

    Network authentication protocol  
    
    -   Authenticate once, trusted by the system
    -   No need to re-authenticate to everything
    -   Mutual authentication - the client and the server  
        -   Protect against on-path or replay attacks
    
    Standard since the 1980s  
    
    -   Developed by the Massachusetts Institute of Technology (MIT)
    
    Microsoft starting using Kerberos in Windows 2000  
    
    -   Based on Kerberos 5.0 open standard
    -   Compatible with other operating systems and devices

4.  SSO with Kerberos

    Authenticate one time  
    
    -   Lots of backend ticketing
    -   Cryptographic tickets
    
    No constant username and password input!  
    
    -   Save time
    
    Only works with Kerberos  
    
    -   Not everything is Kerberos-friendly
    
    There are many other SSO methods  
    
    -   Smart-cards, SAML, etc

5.  RADIUS, TACACS+, or Kerberos?

    Three different ways to communicate to an authentication server  
    
    -   More than a simple login process
    
    Often determined by what is at hand  
    
    -   VPN concentrator can talk to a RADIUS server
    -   We have a RADIUS server
    
    TACACS+  
    
    -   Probably a Cisco device
    
    Kerberos  
    
    -   Probably a Microsoft network

6.  IEEE 802.1X

    IEEE 802.1X  
    
    -   Port-based Network Access Control (NAC)
    -   You don’t get access to the network until you authenticate
    
    EAP integrates with 802.1X  
    
    -   Extensible Authentication Protocol ,
    -   802.1X prevents access to the network [until the authentication succeeds
    
    Used in conjunction with an access database  
    
    -   RADIUS, LDAP, TACACS+



### Federated identities

1.  Federation

    Provide network access to others  
    
    -   Not just employees Partners, suppliers, customers, etc.
    
    Third-parties can establish a federated network  
    
    -   Authenticate and authorize between the two organizations
    -   Login with your Facebook credentials
    
    The third-parties must establish a trust relationship  
    
    -   And the degree of the trust

2.  Security Assertion Markup Language (SAML)

    Open standard for authentication and authorization  
    
    -   You can authenticate through a third-party to gain access
    -   One standard does it all, sort of
    
    Not originally designed for mobile apps  
    
    -   This has been SAML’s largest roadblock

3.  OAuth

    Authorization framework  
    
    -   Determines what resources a user will be able to access
    
    Created by Twitter, Google, and many others  
    
    -   Significant industry support
    
    Not an authentication protocol  
    
    -   OpenlD Connect handles the single sign-on authentication
    -   OAuth provides authorization between applications
    
    Relatively popular  
    
    -   Used by Twitter, Google, Facebook, LinkedIn, and more



### Access Control

Authorization  

-   The process of ensuring only authorized rights are exercised  
    -   Policy enforcement
-   The process of determining rights  
    -   Policy definition

Users receive rights based on Access Control models  

-   Different business needs or mission requirements

1.  Mandatory Access Control (MAC)

    The operating system limits the operation on an object  
    
    -   Based on security clearance levels
    
    Every object gets a label  
    
    -   Confidential, secret, top secret, etc.
    
    Labeling of objects uses predefined rules  
    
    -   The administrator decides who gets access te what security level
    -   Users cannot change these settings

2.  Discretionary Access Control (DAC)

    Used in most operating systems  
    
    -   A familiar access control model
    
    You create a spreadsheet  
    
    -   As the owner, you control who has access
    -   You can modify access at any time
    
    Very flexible access control  
    
    -   And very weak security

3.  Role-based access control (RBAC)

    You have a role in your organization  
    
    -   Manager, director, team lead, project manager
    
    Administrators provide access based on the role of the user  
    
    -   Rights are gained implicitly instead of explicitly
    
    In Windows, use Groups to provide role-based access control  
    
    -   You are in shipping and receiving, so you can use the shipping software
    -   You are the manager, so you can review shipping logs

4.  Attribute-based access control (ABAC)

    Users can have complex relationships to applications and data  
    
    -   Access may be based on many different criteria
    
    ABAC can consider many parameters  
    
    -   A “next generation” authorization model
    -   Aware of context
    
    Combine and evaluate multiple parameters  
    
    -   Resource informatlon, IP address, time of day, desired action, relationship to the data, etc.

5.  Rule-based access control

    Generic term for following rules  
    
    -   Conditions other than who you are
    
    Access is determined through system-enforced rules  
    
    -   System administrators. not users
    
    The rule is associated with the object  
    
    -   System checks the ACLs for that object
    
    Rule examples  
    
    -   Lab network access is only available between 9 AM and 5 PM
    -   Only Chrome browsers may complete this web form

6.  File system security

    Store files and access them  
    
    -   Hard drive, SSDs, flash drives, DVDs
    -   Part of most operating systems
    
    Accessing information  
    
    -   Access control list
    -   Group/user rights and permissions
    -   Can be centrally administered and/or users can manage files they own
    
    Encryption can be built-in  
    
    -   The file system handles encryption and decryption

7.  Conditional access

    Difficult to apply old methods of authentication to new methods of working  
    
    -   Mobile workforce, many different devices, constantly changing cloud
    
    Conditions  
    
    -   Employee or partner, location, type of application accessed, device
    
    Controls  
    
    -   Allow or block, require MFA, provide limited access, require password reset
    
    Administrators can build complex access rules  
    
    -   Complete control over data access

8.  Privileged access management (PAM)

    Managing superuser access  
    
    -   Administrator and Root
    -   You don’t want this in the wrong hands
    
    Store privileged accounts in a digital vault  
    
    -   Access is only granted from the vault by request
    -   These privileges are temporary
    
    PAM advantages  
    
    -   Centralized password management
    -   Enables automation
    -   Manage access for each user
    -   Extensive tracking and auditing



## Given a scenario, implement public key infrastructure



### Public Key Infrastructure (PKI)

Policies, procedures, hardware, software, people  

-   Digital certificates: create, distribute, manage, store, revoke

This is a big, big, endeavor  

-   Lots of planning

Also refers to the binding of public keys to people or devices  

-   The certificate authority
-   It’s all about trust

1.  The key management lifecycle

    Key generation  
    
    -   Create a key with the requested strength using the proper cipher
    
    Certificate generation  
    
    -   Allocate a key to a user
    
    Distribution  
    
    -   Make the key available to the user
    
    Storage  
    
    -   Securely store and protect against unauthorized use
    
    Revocation  
    
    -   Manage keys that have been compromised
    
    Expiration  
    
    -   A certificate may only have a certain “shelf life”

2.  Digital certificates

    A public key certificate  
    
    -   Binds a public key with a digital signature
    -   And other details about the key holder
    
    A digital signature adds trust  
    
    -   PKI uses Certificate Authority for additional trust
    -   Web of Trust adds other users for additional trust
    
    Certificate creation can be built into the OS  
    
    -   Part of Windows Domain services
    -   3rd-party Linux options

3.  Commercial certificate authorities

    Built-in to your browser  
    
    -   Any browser
    
    Purchase your web site certificate  
    
    -   It will be trusted by everyone’s browser
    
    Create a key pair, send the public key to the CA to be signed  
    
    -   A certificate signing request (CSR)
    
    May provide different levels of trust and additional features  
    
    -   Add a new “tag” to your web site

4.  Private certificate authorities

    You are your own CA  
    
    -   Build it in-house
    -   Your devices must trust the internal CA
    
    Needed for medium-to-large organizations  
    
    -   Many web servers and privacy requirements
    
    Implement as part of your overall computing strategy  
    
    -   Windows Certificate Services, OpenCA

5.  PKI trust relationships

    Single CA  
    
    -   Everyone receives their certificates from one authority
    
    Hierarchical  
    
    -   Single CA issues certs to intermediate CAs
    -   Distributes the certificate management load
    -   Easier to deal with the revocation of an intermediate CA than the root CA

6.  Registration authority (RA)

    The entity requesting the certificate needs to be verified  
    
    -   The RA identifies and authenticates the requester
    
    Approval or rejection  
    
    -   The foundation of trust in this model
    
    Also responsible for revocations  
    
    -   Administratively revoked or by request
    
    Manages renewals and re-key requests  
    
    -   Maintains certificates for current cert holders

7.  Important certificate attributes

    Common Name (CN)  
    
    -   The FQDN (Fully Qualified Domain Name) for the certificate
    
    Subject alternative name  
    
    -   Additional host names for the cert
    -   Common on web servers
    -   professormesser.com and
    
    www.professormesser.com  
    Expiration  
    
    -   Limit exposure to compromise
    -   398 day browser limit (13 months)

8.  Key revocation

    Certificate Revocation List (CRL)  
    
    -   Maintained by the Certificate Authority (CA)
    -   Can contain many revocations in a large file
    
    Many different reasons  
    
    -   Changes all the time
    
    April 2014 - CVE-2014-0160  
    
    -   Heartbleed
    -   OpenSSL flaw put the private key of affected web servers at risk
    -   OpenSSL was patched, every web server certificate was replaced
    -   Older certificates were moved to the CRL

9.  Getting revocation details to the browser

    OCSP (Online Certificate Status Protocol)  
    
    -   The browser can check certificate revocation
    
    Messages usually sent to an OCSP responder via HTTP  
    
    -   Easy to support over Internet links
    -   More efficient than downloading a CRL
    
    Not all browsers/apps support OCSP  
    
    -   Early Internet Explorer versions did not support OCSP
    -   Some support OCSP, but don’t bother checking



### Certificates

1.  Web server SSL certificates

    Domain validation certificate (DV)  
    
    -   Owner of the certificate has some control over a DNS domain
    
    Extended validation certificate (EV)  
    
    -   Additional checks have verified the certificate owner’s identity
    -   Browsers used to show a green name on the address bar
    -   Promoting the use of SSL is now outdated
    
    Subject Alternative Name (SAN)  
    
    -   Extension to an X.509 certificate
    -   Lists additional identification information
    -   Allows a certificate to support many different domains
    
    Wildcard domain  
    
    -   Certificates are based on the name of the server
    -   A wildcard domain will apply to all server names in a domain
    -   \* professormesser.com

2.  Code signing certificate

    Developers can provide a level of trust  
    
    -   Applications can be signed by the developer
    
    The user’s operating system will examine the signature  
    
    -   Checks the developer signature
    -   Validates that the software has not been modified
    
    Is it from a trusted entity?  
    
    -   The user will have the opportunity to stop the application execution

3.  Root certificate

    The public key certificate that identifies the root CA (Certificate Authority)  
    
    -   Everything starts with this certificate
    
    The root certificate issues other certificates  
    
    -   Intermediate CA certificates
    -   Any other certificates
    
    This is a very important certificate  
    
    -   Take all security precautions
    -   Access to the root certificate allows for the creation of any trusted certificate

4.  Self-signed certificates

    Internal certificates don’t need to be signed by a public CA  
    
    -   Your company is the only one going to use it
    -   No need to purchase trust for devices that already trust you
    
    Build your own CA  
    
    -   Issue your own certificates signed by your own CA
    
    Install the CA certificate/trusted chain on all devices  
    
    -   They’ll now trust any certificates sighed by your internal CA
    -   Works exactly like a certificate you purchased

5.  Machine and computer certificates

    You have to manage many devices  
    
    -   Often devices that you’ll never physically see
    
    How can you truly authenticate a device?  
    
    -   Put a certificate on the device that you signed
    
    Other business processes rely on the certificate  
    
    -   Access to the remote access VPN from authorized devices
    -   Management software can validate the end device

6.  Email certificates

    Use cryptography in an email platform  
    
    -   You’ll need public key cryptography
    
    Encrypting emails  
    
    -   Use a recipient’s public key to encrypt
    
    Receiving encrypted emails  
    
    -   Use your private key to decrypt
    
    Digital signatures  
    
    -   Use your private key to digitally sign an email
    -   Non-repudiation, integrity

7.  User certificates

    Associate a certificate with a user  
    
    -   A powerful electronic “id card”
    
    Use as an additional authentication factor  
    
    -   Limit access without the certificate
    
    Integrate onto smart cards  
    
    -   Use as both a physical and digital access card



### Certificate formats

1.  Certificate file formats

    X.509 digital certificates  
    
    -   The structure of the certification is standardized
    -   The format of the actual certificate file can take many alirerent rorms
    
    There are many certificate file formats  
    
    -   You can convert between many of the formats
    -   Use openssl or a similar application to view the certificate contents

2.  DER (Distinguished Encoding Rules)

    Format designed to transfer syntax for data structures  
    
    -   A very specific encoding format
    -   Perfect for an X.509 certificate
    
    Binary format  
    
    -   Not human-readable
    
    A common format  
    
    -   Used across many platforms
    -   Often used with Java certificates

3.  PEM (Privacy-Enhanced Mail)

    A very common format  
    
    -   BASE64 encoded DER certificate
    -   Generally the format provided by CAs
    -   Supported on many different platforms
    
    ASCII format  
    
    -   Letters and numbers
    -   Easy to email
    -   Readable

4.  PKCS #12

    Public Key Cryptography Standards #12  
    Personal Information Exchange Syntax Standard  
    
    -   Developed by RSA Security, now an RFC standard
    
    Container format for many certificates  
    
    -   Store many X.509 certificates in a single .pl12 or .pfx file
    -   Often used to transfer a private and public key pair
    -   The container can be password protected
    
    Extended from Microsoft’s . pfx format  
    
    -   Personal Information Exchange (PFX)
    -   The two standards are very similar
    -   Often referenced interchangeably

5.  CER (Certificate)

    Primarily a Windows X.509 file extension  
    
    -   Can be encoded as binary DER format or as the ASCII PEM format
    
    Usually contains a public key  
    
    -   Private keys would be transferred in the . pfx file format
    
    Common format for Windows certificates  
    
    -   Look for the .cer extension

6.  PKCS #7

    Public Key Cryptography Standards #7  
    Cryptographic Message Syntax Standard  
    
    -   Associated with the . p7b file
    
    Stored in ASCII format  
    
    -   Human-readable
    
    Contains certificates and chain certificates  
    
    -   Private keys are not included ina .p7b file
    
    Wide platform support  
    
    -   Microsoft Windows, Java Tomcat



### Certificate concepts

1.  Online and offline CAs

    A compromised certificate authority  
    
    -   A very, very bad thing
    -   No certificates issued by that CA can be trusted
    
    Distribute the load  
    
    -   Then take the root CA offline and protect it

2.  OCSP stapling

    Online Certificate Status Protocol  
    
    -   Provides scalability for OCSP checks
    
    The CA is responsible for responding to all client OCSP requests  
    
    -   This may not scale well
    
    Instead, have the certificate holder verify their own status  
    
    -   Status information is stored on the certificate holder’s server
    
    OCSP status is “stapled” into the SSL/TLS handshake  
    
    -   Digitally signed by the CA

3.  Pinning

    You&rsquo;re communicating over TLS/SSL to a server  
    
    -   How do you really know it’s a legitimate server?
    
    “Pin” the expected certificate or public key to an application  
    
    -   Compiled in the app or added at first run
    
    If the expected certificate or public key doesn’t match, the application can  
    decide what to do  
    
    -   Shut down, show a message

4.  PKI trust relationship

    Single CA  
    
    -   Everyone receives their certificates from one authority
    
    Hierarchical  
    
    -   Single CA issues certs to intermediate CAs
    
    Mesh  
    
    -   Cross-certifying CAs
    -   Doesn’t scale well
    
    Web-of-trust  
    
    -   Alternative to traditional PKI
    
    Mutual Authentication  
    
    -   Server authenticates to the client and the client authenticates to the server

5.  Key escrow

    Someone else holds your decryption keys  
    
    -   Your private keys are in the hands of a 3rd-party
    
    This can be a legitimate business arrangement  
    
    -   A business might need access to employee information
    -   Government agencies may need to decrypt partner data

6.  It&rsquo;s all about the process

    Need clear process and procedures  
    
    -   Keys are incredibly important pieces of information
    
    You must be able to trust your 3rd-party  
    
    -   Access to the keys is at the control of the 3rd-party
    
    Carefully controlled conditions 4  
    
    -   Legal proceedings and court orders

7.  Certificate chaining

    Chain of trust  
    
    -   List all of the certs between the server and the root CA
    
    The chain starts with the SSL certificate  
    
    -   And ends with the Root CA certificate
    
    Any certificate between the SSL certificate and the root certificate is a chain certificate  
    
    -   Or intermediate certificate
    
    The web server needs to be configured with the proper chain  
    
    -   Or the end user may receive an error



# Operations and Incident Response 16%



## Given a scenario, use the appropriate tool to assess organizational security



### Reconnaissance Tools

1.  `traceroute`

    Determine the route a packet takes to a destination  
    
    -   Map the entire path
    -   tracert (Windows) or traceroute (Unix/Linux/macOS)
    
    Takes advantage of ICMP Time to Live Exceeded error message  
    
    -   The time in TTL refers to hops, not seconds or minutes
    -   TTL=1 is the first router, TTL=2 is the second router, etc.
    
    Not all devices will reply with ICMP Time Exceeded messages  
    
    -   Some firewalls filter ICMP
    -   ICMP is low-priority for many devices
    
    1.  Flavors of traceroute
    
        Not all traceroutes are the same  
        
        -   Minor differences in the transmitted payload
        
        Windows commonly sends ICMP echo requests  
        
        -   Receives ICMP time exceeded messages
        -   And an ICMP echo reply from the final/destination device
        -   Unfortunately, outgoing ICMP is commonly filtered
        
        Some operating systems allow you to specify the protocol used  
        
        -   Linux, Unix, Mac OS, etc.
        
        IOS devices send UDP datagrams over port 33434 g  
        
        -   The port number can be changed with extended options

2.  `nslookup` and `dig`

    Lookup information from DNS servers  
    
    -   Canonical names, IP addresses, cache timers, etc.
    
    `nslookup`  
    
    -   Both Windows and POSIX-based
    -   Lookup names and IP addresses
    -   Deprecated (use dig instead)
    
    `dig` (Domain Information Groper)  
    
    -   More advanced domain information
    -   Probably your first choice
    -   Install in Windows: <https://professormesser.link/digwin>

3.  `ipconfig` and `ifconfig`

    Most of your troubleshooting starts with your IP address  
    
    -   Ping your local router/gateway
    
    Determine TCP/IP and network adapter information  
    
    -   And some additional IP details
    
    ipconfig— Windows TCP/IP configuratior  
    ifconfig - Linux interface configuration  

4.  `ping`

    Test reachability  
    
    -   Determine round-trip time
    -   Uses Internet Control Message Protocol (ICMP)
    
    One of your primary troubleshooting tools  
    
    -   Can you ping the host?
    
    Written by Mike Muuss in 1983  
    
    -   The sound made by sonar
    -   Not an acronym for Packet INternet Groper  
        -   A backronym

5.  `pathping`

    Combine ping and traceroute  
    
    -   Included with Windows NT and later
    
    First phase runs a traceroute  
    
    -   Build a map
    
    Second phase  
    
    -   Measure round trip time and packet loss at each hdp

6.  `netstat`

    Network statistics  
    
    -   Many different operating systems
    
    netstat -a  
    
    -   Show all active connections
    
    netstat -b  
    
    -   Show binaries (Windows)
    
    netstat -n  
    
    -   Do not resolve names

7.  Address resolution protocol - `arp`

    Determine a MAC address based on an IP address  
    
    -   You need the hardware address to communicate
    
    arp -a  
    
    -   View local ARP table

8.  `route`

    View the device’s routing table  
    
    -   Find out which way the packets will go
    
    Windows: route print  
    Linux and macOS: netstat -r  

9.  `curl`

    Client URL  
    
    -   Retrieve data using a URL
    -   Uniform Resource Locator
    -   Web pages, FTP, emails, databases, etc.
    
    Grab the raw data  
    
    -   Search
    -   Parse
    -   Automate

10. IP scanners

    Search a network for IP addresses  
    
    -   Locate active devices
    -   Avoid doing work on an IP address that isn’t there
    
    Many different techniques  
    
    -   ARP (if on the local subnet)
    -   ICMP requests (ping)
    -   TCP ACK
    -   ICMP timestamp requests
    
    A response means more recon can be done  
    
    -   Keep gathering information
    -   Nmap, hping, etc.
    
    1.  `hping`
    
        TCP/IP packet assembler/analyzer  
        
        -   A ping that can send almost anything
        
        Ping a device  
        
        -   ICMP, TCP, UDP  
            
                hping3 --destport 80 10.1.10.1
                hping3 --scan 80-443 -S 10.1.10.1 -V
        
        Send crafted frames  
        
        -   Modify all IP, TCP, UDP, and ICMP values
        
        A powerful tool  
        
        -   It’s easy to accidentally flood and DoS
        -   Be careful!
    
    2.  `nmap`
    
        Network mapper  
        
        -   Find and learn more about network devices
        
        Port scan  
        
        -   Find devices and identify open ports
        
        Operating system scan  
        
        -   Discover the OS without logging in to a device
        
        Service scan  
        
        -   What service is available on a device? Name, version, details
        
        Additional scripts  
        
        -   Nmap Scripting Engine (NSE) - extend capabilities, vulnerability scans
        
            sudo nmap 10.1.10.1 -vv

11. `theHarvester`

    Gather OSINT  
    
    -   Open-Source Intelligence
    
    Scrape information from Google or Bing  
    
    -   Find associated IP addresses
    
    List of people from LinkedIn  
    
    -   Names and titles
    
    DNS brute force  
    
    -   Find those unknown hosts; vpn, chat, mail, partner, etc.
    
        theHarvester -d example.com -1 100 -b bing

12. `sn1per`

    Combine many recon tools into a single framework  
    
    -   dnsenum, metasploit, nmap, theHarvester, and much more
    
    Both non-intrusive and very intrusive scanning options  
    
    -   You choose the volume
    
    Another tool that can cause problems  
    
    -   Brute force, server scanning, etc
    -   Make sure you know what you’re doing
    
        sniper -t example.com -m web

13. `scanless`

    Run port scans from a different host  
    
    -   Port scan proxy
    
    Many different services  
    
    -   Choose the option for scan origination
    -   Your IP is hidden as the scan source
    
        scanless -t scanme.nmap.org -s spideripjj

14. `dnsenum`

    Enumerate DNS information  
    
    -   Find host names
    
    View host information from DNS servers  
    
    -   Many services and hosts are listed in DNS
    
    Find host names in Google  
    
    -   More hosts can probably be found in the index
    
        dnsenum -v example.com

15. Nessus

    Industry leader in vulnerability scanning  
    
    -   Extensive support
    -   Free and commercial options
    
    Identify known vulnerabilities  
    
    -   Find systems before they can be exploited
    
    Extensive reporting  
    
    -   A checklist of issues
    -   Filter out the false positives

16. Cuckoo

    A sandbox for malware  
    
    -   Test a file in a safe environment
    
    A virtualized environment  
    
    -   Windows, Linux, macOS, Android
    
    Track and trace  
    
    -   API calls, network traffic, memory analysis
    -   Traffic captures
    -   Screenshots



### File manipulation tools

1.  `cat`

    Concatenate  
    
    -   Link together in a series
    
    Copy a file/files to the screen  
    
    -   cat filel.txt file2.txt
    
    Copy a file/files to another file  
    
    -   cat filel.txt file2.txt > both.txt

2.  `head`

    View the first part of a file  
    
    -   The head, or beginning, of the file
    -   head [OPTION] .. [FILE] ..
    
    Use -n to specify the number of lines  
    
    -   head -n 5 syslog

3.  `tail`

    View the last part of a file  
    
    -   The tail, or end, or the file
    
    tail [OPTION] .. [FILE] ..  
    Use -n to specify the number of lines  
    
    -   tail -n 5 syslog

4.  `grep`

    Find text in a file  
    
    -   Search through many files at a time
    
    grep PATTERN [FILE]  
    
    -   grep failed auth.log

5.  `chmod`

    Change mode of a file system object  
    
    -   r=read, w=write, x=execute
    -   Can also use octal notation
    -   Set for the file owner (u), the group(g), others(o), or all(a)
    
    chmod mode FILE  
    
    -   chmod 744 script.sh
    
    ![img](res/permission2.png)  
    ![img](res/permission.png)  
    chmod 744 first.txt  
    
    -   User; read, write execute
    -   Group; read only
    -   Other; read only
    
    chmod a-w first.txt  
    
    -   All users, no writing to first.txt
    
    chmod u+x script.sp  
    
    -   The owner of script.sh can execute the file

6.  `logger`

    Add entries to the system log  
    
    -   syslog
    
    Adding to the local syslog file  
    
    -   logger “This information is added to syslog”
    
    Useful for including information in a local or remote syslog file  
    
    -   Include as part of an automation script
    -   Log an important event



### Shell and script environments

1.  `ssh`

    Encrypted console communication - tcp/22  
    Looks and acts the same as Telnet  

2.  Windows PowerShell

    Command line for system administrators  
    
    -   .ps1 file extension
    -   Included with Windows 8/8.1 and 10
    
    Extend command-line functions  
    
    -   Uses cmmdlets (command-lets)
    -   PowerShell scripts and functions
    -   Standalone executables
    
    Automate and integrate  
    
    -   System administration
    -   Active Domain administration

3.  Python

    General-purpose scripting language  
    
    -   .py file extension
    
    Popular in many technologies  
    
    -   Broad appeal and support

4.  OpenSSL

    A toolkit and crypto library for SSL/TLS  
    
    -   Build certificates, manage SSL/TLS communication
    
    Create X.509 certificates  
    
    -   Manage certificate signing requests (CSRs) and certificate revocation lists (CRLs)
    
    Message digests  
    
    -   Support for many hashing protocols
    
    Encryption and Decryption  
    
    -   SSL/TLS for services



### Packet tools

1.  Wireshark

    Graphical packet analyzer  
    
    -   Get into the details
    
    Gathers frames on the network  
    
    -   Or in the air
    -   Sometimes built into the device
    
    View traffic patterns  
    
    -   ldentify unknown traffic
    -   Verify packet filtering and security controls
    
    Extensive decodes  
    
    -   View the application traffic

2.  `tcpdump`

    Capture packets from the command line  
    
    -   Display packets on the screen
    -   Werite packets to a file

3.  Tcpreplay

    A suite of packet replay utilities  
    
    -   Replay and edit packet captures
    -   Open source
    
    Test security devices  
    
    -   Check IPS signatures and firewall rules
    
    Test and tune IP Flow/NetFlow devices  
    
    -   Send hundreds of thousands of traffic flows per second
    
    Evaluate the performance of security devices  
    
    -   Test throughput and flows per second



### Forensic tools

1.  `dd`

    A reference to the DD command in IBM mainframe JCL (Job Control Language)  
    
    -   Data Definition (ASCIl to EBCDIC converter)
    
    Create a bit-by-bit copy of a drive  
    
    -   Used by many forensics tools
    
    Create a disk image  
    
    -   dd if=/dev/sda of=/tmp/sda-image.img
    
    Restore from an image  
    
    -   dd if=/tmp/sda-image.img of=/dev/sda

2.  `memdump`

    Copy information in system memory to the standard output stream  
    
    -   Everything that happens is in memory
    -   Many third-party tools can read a memory dumg
    
    Copy to another host across the network  
    
    -   Use netcat, stunnel, openssl, etc.

3.  WinHex

    A universal hexadecimal editor  
    
    -   Windows OS
    
    Edit disks, files, RAM  
    
    -   Includes data recovery features
    
    Disk cloning  
    
    -   Drive replication
    
    Secure wipe  
    
    -   Hard drive cleaning
    
    Much more  
    
    -   A full-featured forensics tool

4.  FTK imager

    AccessData forensic drive imaging tool  
    
    -   Includes file utilities and read-only image mounting
    -   Windows executable
    
    Widely supported in many forensics tools  
    
    -   Third-party analysis
    
    Support for many different file systems and  
    full disk encryption methods  
    
    -   Investigator still needs the password
    
    Can also import other image formats  
    
    -   dd, Ghost, Expert Witness, etc.

5.  Autopsy

    Perform digital forensics of hard drives, smartphones  
    
    -   View and recover data from storage devices
    
    Extract many different data types  
    
    -   Downloaded files
    -   Browser history and cache
    -   Email messages
    -   Databases
    -   Much more

6.  Exploitation frameworks

    A pre-built toolkit for exploitations  
    
    -   Build custom attacks
    -   Add more tools as vulnerabilities are found
    -   Increasingly powerful utilities
    
    Metasploit  
    
    -   Attack known vulnerabilities
    
    The Social-Engineer Toolkit (SET)  
    
    -   Spear phishing, Infectious media generator

7.  Password crackers

    The keys to the kingdom  
    
    -   Find the passwords
    
    Online cracking  
    
    -   Try username/password combinations
    
    Offline cracking  
    
    -   Brute force a hash file
    
    Limitations  
    
    -   Password complexity / strength (entropy)
    -   Hashing method and CPU power
    -   Graphics processors are useful hardware tools

8.  Data sanitization

    Completely remove data  
    
    -   No usable information remains
    
    Many different use cases  
    
    -   Clean a hard drive for future use
    
    Permanently delete a single file  
    A one-way trip  
    
    -   Once it’s gone, it’s really gone
    -   No recovery with forensics tools



## Summarize the importance of policies, processes, and procedures for incident response



### Incident Response Process

1.  Security incidents

    User clicks an email attachment and executes malware  
    
    -   Malware then communicates with external servers
    
    DDoS  
    
    -   Botnet attack
    
    Confidential information is stolen  
    
    -   Thief wants money or it goes public
    
    User installs peer-to-peer software and allows external access to internal servers  

2.  Roles and responsibilities

    Incident response team  
    
    -   Specialized group, trained and tested
    
    IT security management  
    
    -   Corporate support
    
    Compliance officers  
    
    -   Intricate knowledge of compliance rules
    
    Technical staff  
    
    -   Your team In the trenches
    
    User community  
    
    -   They see everything

3.  NIST SP800-61

    National Institute of Standards and Technology  
    
    -   NIST Special Publication 800-61 Revision 2
    -   Computer Security Incident Handling Guide
    
    The incident response lifecycle:  
    
    -   Preparation
    -   Detection and Analysis
    -   Containment, Eradication, and Recovery
    -   Post-incident Activity

4.  Preparing for an incident

    Communication methods  
    
    -   Phones and contact information
    
    Incident handling hardware and software  
    
    -   Laptops, removable media, forensic software, digital cameras, etc.
    
    Incident analysis resources  
    
    -   Documentation, network diagrams, baselines, critical file hash values  
        Incident mitigation software
    -   Clean OS and application images
    
    Policies needed for incident handling  
    
    -   Everyone knows what to do

5.  The challenge of detection

    Many different detection sources  
    
    -   Different levels of detail, different levels of perception
    
    A large amount of “volume”  
    
    -   Attacks are incoming all the time
    -   How do you identify the legitimate threats?  
        Incidents are almost always complex
    -   Extensive knowledge needed

6.  Incident precursors

    An incident might occur in the future  
    
    -   This is your heads-up
    
    Web server log  
    
    -   Vulnerability scanner in use
    
    Exploit announcement  
    
    -   Monthly Microsoft patch release, Adobe Flash update
    
    Direct threats  
    
    -   A hacking group doesn’t like you

7.  Incident indicators

    An attack is underway  
    
    -   Or an exploit is successful
    
    Buffer overflow attempt  
    
    -   Identified by an intrusion detection/prevention system
    
    Anti-virus software identifies malware  
    
    -   Deletes from OS and notifies administrator
    
    Host-based monitor detects a configuration change  
    
    -   Constantly monitors system files
    
    Network traffic flows deviate from the norm  
    
    -   Requires constant monitoring

8.  Isolation and containment

    Generally a bad idea to let things run their course  
    
    -   An incident can spread quickly
    -   It’s your fault at that point
    
    Sandboxes  
    
    -   An isolated operating system
    -   Run malware and analyze the results
    -   Clean out the sandbox when done
    
    Isolation can be sometimes be problematic  
    
    -   Malware or infections can monitor connectivity
    -   When connectivity is lost, everything could be deleted/encrypted/damaged

9.  Recovery after an incident

    Get things back to normal  
    
    -   Remove the bad, keep the good
    
    Eradicate the bug  
    
    -   Remove malware
    -   Disable breached user accounts
    -   Fix vulnerabilities
    
    Recover the system  
    
    -   Restore from backups
    -   Rebuild from scratch
    -   Replace compromised files
    -   Tighten down the perimeter

10. Reconstitution

    A phased approach  
    
    -   It’s difficult to fix everything at once
    
    Recovery may take months  
    
    -   Large-scale incidents require a large amount of work
    
    The plan should be efficient  
    
    -   Start with quick, high-value security changes  
        -   Patches, firewall policy changes
    -   Later phases involve much “heavier Ilf&rsquo;tmg  
        -   Infrastructure changes, large-scale security rollouts

11. Lessons learned

    Learn and improve  
    
    -   No system is perfect
    
    Post-incident meeting  
    
    -   Invite everyone affected by the incident
    
    Don’t wait too long  
    
    -   Memories fade over time
    -   Some recommendations can be applied to the next event

12. Answer the tough questions

    What happened, exactly?  
    
    -   Timestamp of the events
    
    How did your incident plans work?  
    
    -   Did the process operate successfully?
    
    What would you do differently next time?  
    
    -   Retrospective views provide context
    
    Which indicators would you watch next time?  
    
    -   Different precursors may give you better alerts



### Incident response planning

1.  Exercise

    Test yourselves before an actual event  
    
    -   Scheduled update sessions (annual, semi-annual, etc.)
    
    Use well-defined rules of engagement  
    
    -   Do not touch the production systems
    
    Very specific scenario  
    
    -   Limited time to run the event
    
    Evaluate response  
    
    -   Document and discuss

2.  Tabletop exercises

    Performing a full-scale disaster drill can be costly  
    
    -   And time consuming
    
    Many of the logistics can be determined through analysis  
    
    -   You don’t physically have to go through a disaster or drill
    
    Get key players together for a tabletop exercise  
    
    -   Talk through a simulated disaster

3.  Walkthrough

    Include responders  
    
    -   A step beyond a tabletop exercise
    -   Many moving parts
    
    Test processes and procedures before an event  
    
    -   Walk through each step
    -   Involve all groups
    -   Reference actual response materials
    
    Identifies actual faults or missing steps  
    
    -   The walkthrough applies the concepts from the tabletop exercise

4.  Simulation

    Test with a simulated event  
    
    -   Phishing attack, password requests, data breaches
    
    Going phishing  
    
    -   Create a phishing email attack
    -   Send to your actual user community
    -   See who bites
    
    Test internal security  
    
    -   Did the phishing get past the filter?
    
    Test the users  
    
    -   Who clicked?
    -   Additional training may be required

5.  Stakeholder management

    Keeping an good ongoing relationship with customers of IT  
    
    -   These can be internal or external customers
    -   An incident response will require teamwork
    -   Without the stakeholder, IT would not exist
    
    Most of this happens prior to an incident  
    
    -   Ongoing communication and meetings
    -   Exercises should include the customers
    
    Continues after the incident  
    
    -   Prepare for the next event

6.  Communication plan

    Get your contact list together  
    
    -   There are a lot of people in the loop
    
    Corporate / Organization  
    
    -   CIO / Head of Information Security / Internal Response Teams
    
    Internal non-IT  
    
    -   Human resources
    -   Public affairs
    -   Legal department
    
    External contacts  
    
    -   System owner, law enforcement
    -   US-CERT (for U.S. Government agencies)

7.  Disaster recovery plan

    If a disaster happens, IT should be ready  
    
    -   Part of business continuity planning
    -   Keep the organization up and running
    
    Disasters are many and varied  
    
    -   Natural disasters
    -   Technology or system failures
    -   Human-created disasters
    
    A comprehensive plan  
    
    -   Recovery location
    -   Data recovery method
    -   Application restoration
    -   IT team and employee availability

8.  Continuity of operations planning (COOP)

    Not everything goes according to plan  
    
    -   Disasters can cause a disruption to the norm
    
    We rely on our computer systems  
    
    -   Technology is pervasive
    
    There needs to be an alternative  
    
    -   Manual transactions
    -   Paper receipts
    -   Phone calls for transaction approvals
    
    These must be documented and tested before a problem occurs  

9.  Incident response team

    Receives, reviews, and responds  
    
    -   A predefined group of professionals
    
    Determine what type of events require a response  
    
    -   A virus infection? Ransomware? DDoS?
    
    May or may not be part of the organizational structure  
    
    -   Pulled together on an as-needed basis
    
    Focuses on incident handling  
    
    -   Incident response
    -   Incident analysis
    -   Incident reporting

10. Retention policies

    Backup your data  
    
    -   How much and where?
    -   Copies, versions of copies, lifecycle of data, purging old data
    
    Regulatory compliance  
    
    -   A certain amount of data backup may be required
    
    Operational needs  
    
    -   Accidental deletion
    -   Disaster recovery
    
    Differentiate by type and application  
    
    -   Recover the data you need when you need it



### Attack frameworks

1.  Attacks and responses

    A constantly moving chessboard  
    
    -   The rules are also constantly changing
    
    Response and intelligence teams need assistance  
    
    -   Gather and maintain ongoing reconnaissance
    
    Understand attacks  
    
    -   Many different vectors
    
    Assess the risk in an organization  
    
    -   Determine if a risk exists
    -   Use appropriate mitigation

2.  MITRE ATT&CK framework

    The MITRE corporation  
    
    -   US not-for-profit based in Massachusetts and Virginia
    -   Supports several U.S. government agencies
    
    The MITRE ATT&CK framework  
    
    -   <https://attack.mitre.org/>
    
    Determine the actions of an attacker  
    
    -   Identify point of intrusion
    -   Understand methods used to move around
    -   ldentify potential security techniques to block future attacks

3.  Diamond Model of Intrusion Analysis

    Designed by the intelligence community  
    
    -   <https://apps.dtic.mil/docs/citations/ADA586960>
    -   Guide analysts to help understand intrusions
    -   Integrates well with other frameworks
    
    Apply scientific principles to intrusion analysis  
    
    -   Measurement, testability, and repeatability
    -   Appears simple, but is remarkably complex
    
    An adversary deploys a capability over some infrastructure against a victim  
    
    -   Use the model to analyze and fill in the details
    
    ![img](res/diamond_model.png)  

4.  Cyber Kill Chain

    Seven phases of a cyber attack  
    
    -   A military concept
    
    <table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
    
    
    <colgroup>
    <col  class="org-left" />
    
    <col  class="org-left" />
    </colgroup>
    <thead>
    <tr>
    <th scope="col" class="org-left">Phase</th>
    <th scope="col" class="org-left">Description</th>
    </tr>
    </thead>
    
    <tbody>
    <tr>
    <td class="org-left">Reconnaissance</td>
    <td class="org-left">Gather intel, harvest emails from Google and LinkedIn</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Weaponization</td>
    <td class="org-left">Build a deliverable payload that includes an exploit and backdoor</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Delivery</td>
    <td class="org-left">Send the weapon - Deliver an executable over email</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Exploit</td>
    <td class="org-left">Execute code on the victim’s device</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Installation</td>
    <td class="org-left">Malware is installed into the operating system</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Command &amp; Control</td>
    <td class="org-left">A C2 channel is created for remote access</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Actions on objectives</td>
    <td class="org-left">Attacker can remotely carry out objectives</td>
    </tr>
    </tbody>
    </table>



## Given an incident, utilize appropriate data sources to support an investigation



### Vulnerability Scan Output

1.  Identify vulnerability

    The scanner looks for everything  
    
    -   Well, not <span class="underline">everything</span>
    -   The signatures are the key
    
    The vulnerabilities can be cross-referenced online  
    
    -   Almost all scanners give you a place to go
    -   National Vulnerability Database: <http://nvd.nist.gov/>
    -   Microsoft Security Bulletins: <https://docs.microsoft.cczm/en-us/security-updates/>
    
    Some vulnerabilities cannot be definitively identified  
    
    -   You’ll have to check manually to see if a system is vulnerable
    -   But the scanner gives you a heads-up

2.  Vulnerability scan results

    Lack of security controls  
    
    -   No firewall
    -   No anti-virus
    -   No anti-spyware
    
    Misconfigurations  
    
    -   Open shares
    -   Guest access
    
    Real vulnerabilities  
    
    -   Especially newer ones
    -   Occasionally the old ones

3.  Dealing with false positives

    False positives  
    
    -   A vulnerability is identified that doesn’t really exist
    
    This is different than a low-severity vulnerability  
    
    -   It’s real, but it may not be your highest priority
    
    False negatives  
    
    -   A vulnerability exists, but you didn’t detect it
    
    Update to the latest signatures  
    
    -   If you don’t know about it, you can’t see it
    
    Work with the vulnerability detection manufacturer  
    
    -   They may need to update their signatures for your environment



### SIEM dashboard

1.  [SIEM](#org8359816)

2.  Getting the data

    Sensors and logs  
    
    -   Operating systems
    -   Infrastructure devices
    -   NetFlow sensors
    
    Sensitivity settings  
    
    -   Easy to be overwhelmed with data
    -   Some information is unnecessary
    -   Informational, Warning, Urgent

3.  Viewing the data

    Trends  
    
    -   ldentify changes over time
    -   Easily view constant attack metrics
    
    Alerts  
    
    -   Identify a security event
    -   View raw data
    -   Visualize the log information
    
    Correlation  
    
    -   Combine and compare
    -   View data in different ways



### Log files

1.  Network log files

    Switches, routers, access points, VPN concentrators  
    
    -   And other infrastructure devices
    
    Network changes  
    
    -   Routing updates
    -   Authentication issues
    -   Network security issues

2.  System log files

    Operating system information  
    
    -   Extensive logs
    -   File system information
    -   Authentication details
    
    Can also include security events  
    
    -   Monitoring apps
    -   Brute force, file changes
    
    May require filtering  
    
    -   Don’t forward everything

3.  Application log files

    Specific to the application  
    
    -   Information varies widely
    
    Windows  
    
    -   Event Viewer / Application Log
    
    Linux / macOS  
    
    -   /var/log
    
    Parse the log details on the SIEM  
    
    -   Filter out unneeded info

4.  Security log files

    Detailed security-related information  
    
    -   Blocked and allowed traffic flows
    -   Exploit attempts
    -   Blocked URL categories
    -   DNS sinkhole traffic
    
    Security devices  
    
    -   IPS, firewall, proxy
    
    Critical security information  
    
    -   Documentation of every traffic flow
    -   Summary of attack info
    -   Correlate with other logs

5.  Web log files

    Web server access  
    
    -   |P address, web page URL
    
    AcCcess errors  
    
    -   Unauthorized or
    
    non-existent folders/files  
    Exploit attempts  
    
    -   Attempt to access files
    
    containing known vulnerabilities  
    Server activity  
    
    -   Startup and shutdown notices
    -   Restart messages

6.  DNS log files

    View lookup requests  
    
    -   And other DNS queries
    
    IP address of the request  
    
    -   The request FQDN or IP
    
    ldentify queries to known bad URLs  
    
    -   Malware sites, known command and control domains
    
    Block or modify known bad requests at the DNS server  
    
    -   Log the results
    -   Report on malware activity

7.  Authentication log files

    Know who logged in (or didn’t)  
    
    -   Account names
    -   Source IP address
    -   Authentication method
    -   Success and failure reports
    
    ldentify multiple failures  
    
    -   Potential brute force attacks
    
    Correlate with other events  
    
    -   File transfers
    -   Authentications to other devices
    -   Application installation

8.  Dump files

    Store all contents of memory into a diagnostic file  
    
    -   Developers can use this info
    
    Easy to create from the Windows Task Manager  
    
    -   Right-click, Create dump file
    
    Some applications have their own dump file process  
    
    -   Contact the appropriate support team for additional details

9.  VoIP and call manager logs

    View inbound and outbound call info  
    
    -   Endpoint details
    -   Gateway communication
    
    Security information  
    
    -   Authentications
    -   Audit trail
    
    SIP traffic logs  
    
    -   Session Initiation Protocol
    -   Call setup, management, and teardown
    -   Inbound and outbound calls
    -   Alert on unusual numbers or country codes



### Log management

1.  Syslog

    Standard for message logging  
    
    -   Diverse systems create a consolidated log
    
    Usually a central logging receiver  
    
    -   Integrated into the SIEM (Security Information and Event Manager)
    
    Each log entry is labeled  
    
    -   Facility code (program that created the log) and severity level
    
    Syslog daemon options  
    
    -   Rsyslog -“Rocket-fast System for log processing”
    -   syslog-ng - A popular syslog daemon with additional filtering and storage options
    -   NXLog - Collection from many diverse log types

2.  Journalctl

    Linux has a lot of logs  
    
    -   The OS, daemons, applications, etc.
    
    System logs are stored in a binary format  
    
    -   Optimized for storage and queries
    -   Can’t read them with a text editor
    
    Journalctl provides a method for querying the system journal  
    
    -   Search and filter
    -   View as plain text

3.  Bandwidth monitors

    The fundamental network statistic  
    
    -   Percentage of network use over time
    
    Many different ways to gather this metric  
    The fundamental network statistic  
    
    -   Percentage of network use over time
    
    Many different ways to gather this metric  

4.  Metadata

    Metadata  
    
    -   Data that describes other data sources
    
    Email  
    
    -   Header details, sending servers, destination address
    
    Mobile  
    
    -   Type of phone, GPS location
    
    Web  
    
    -   Operating system, browser type, IP address
    
    Files  
    
    -   Name, address, phone number, title

5.  Netflow

    Gather traffic statistics from all traffic flows  
    
    -   Shared communication between devices
    
    NetFlow  
    
    -   Standard collection method
    -   Many products and options
    
    Probe and collector  
    
    -   Probe watches network communication
    -   Summary records are sent to the collector
    
    Usually a separate reporting app  
    
    -   Closely tied to the collector

6.  IPFIX

    IP Flow Information Export  
    
    -   A newer, NetFlow-based standard
    -   Evolved from NetFlow
    
    Flexible data support  
    
    -   Templates are used to describe the data

7.  sFlow

    sFlow (Sampled Flow)  
    
    -   Only a portion of the actual network traffic
    -   So, technically not a flow
    
    Usually embedded in the infrastructure  
    
    -   Switches, routers
    -   Sampling usually occurs in hardware/ASICs
    
    Relatively accurate statistics  
    
    -   Useful information regarding video streaming and high-traffic applications

8.  Protocol analyzer output

    Solve complex application issues  
    
    -   Get into the details
    
    Gathers packets on the network  
    
    -   Or in the air
    -   Sometimes built into the device
    
    View detailed traffic information  
    
    -   Identify unknown traffic
    -   Verify packet filtering and security controls
    -   View a plain-language description of the application data



## Given an incident, apply mitigation techniques or controls to secure an environment



### Endpoint Security Configuration

1.  The endpoint

    The end user device  
    
    -   Desktop PC, laptop, tablet, phone, etc.
    
    Many ways to exploit a system  
    
    -   OS vulnerability, malware, user intervention
    
    Security team has to cover all of the bases  
    
    -   Recognize and react to any malicious activity

2.  [Allow list / deny list](#orgee4d18b)

3.  [Examples of allow and deny list](#orgdef6a9f)



### Security configurations

1.  Configuration changes

    Firewall rules  
    
    -   Manage application flows
    -   Block dangerous applications
    
    Mobile Device Manager (MDM)  
    
    -   Enable or disable phone and tablet functionality
    -   Regardless of physical location
    
    Data Loss Prevention (DLP)  
    
    -   Block transfer of personally identifiable information (Pll) or sensitive data
    -   Credit card numbers, social security numbers, etc.
    
    Content filter/URL filter  
    
    -   Limit access to untrusted websites
    -   Block known malicious sites
    -   Large blocklists are used to share suspicious site URLs
    
    Updating or revoking certificates  
    
    -   Manage device certificates to verify trust
    -   Revoking a certificate effectively removes access

2.  Isolation

    Administratively isolate a compromised device from everything else  
    
    -   Prevent the spread of malicious software
    -   Prevent remote access or C2 (Command and Control)
    
    Network isolation  
    
    -   Isolate to a remediation VLAN
    -   No communication to other devices
    
    Process isolation  
    
    -   Limit application execution
    -   Prevent malicious activity but allow device management

3.  Containment

    Application containment  
    
    -   Run each application in its own sandbox
    -   Limit interaction with the host operating system and other applications
    -   Ransomware would have no method of infection
    
    Contain the spread of a multi-device security event, i.e., ransomware  
    
    -   Disable administrative shares
    -   Disable remote management
    -   Disable local account access and change local administrator password

4.  Segmentation

    Separate the network  
    
    -   Prevent unauthorized movement
    -   Limit the scope of a breach

5.  [SOAR](#orga9b3ed1)

    Runbooks  
    
    -   Linear checklist of steps to perform
    -   Step-by-step approach to automation
    -   Reset a password, create a website certificate, back up application data
    
    Playbooks  
    
    -   Conditional steps to follow; a broad process
    -   Investigate a data breach, recover from ransomware



## Explain the key aspects of digital forensics



### Digital forensics

Collect and protect information relating to an intrusion  

-   Many different data sources and protection mechanisms

RFC 3227 - Guidelines for Evidence Collection and Archiving  

-   A good set of best practices

Standard digital forensic process  

-   Acquisition, analysis, and reporting

Must be detail oriented  

-   Take extensive notes

1.  Legal hold

    A legal technique to preserve relevant information  
    
    -   Prepare for impending litigation
    -   Initiated by legal counsel
    
    Hold notification  
    
    -   Custodians are instructed to preserve data
    
    Separate repository for electronically stored information (ESI)  
    
    -   Many different data sources and types
    -   Unique workflow and retention requirements
    
    Ongoing preservation  
    
    -   Once notified, there’s an ongoing obligation to preserve data

2.  Capture video

    A moving record of the event  
    
    -   Gathers information external to the computer and network
    
    Captures the status of the screen and other volatile information  
    
    -   Today’s mobile video devices are remarkable
    
    Don’t forget security cameras and your phone  
    The video content must also be archived  
    
    -   May have some of the most important record of information

3.  Admissibility

    Not all data can be used in a court of law  
    
    -   Different rules in different jurisdictions
    
    Legal authorization  
    
    -   Search and seizure of information
    
    Procedures and tools  
    
    -   The correct tools used the correct way
    
    Laboratories  
    
    -   Proper scientific principles used to analyze the evidence
    
    Technical and academic qualifications  
    
    -   Competence and qualifications of experts

4.  Chain of custody

    Control evidence  
    
    -   Maintain integrity
    
    Everyone who contacts the evidence  
    
    -   Use hashes
    -   Avoid tampering
    
    Label and catalog everything  
    
    -   Digitally tag all items for ongoing documentation
    -   Seal and store

5.  Recording time offsets

    The time zone determines how the time is displayed  
    
    -   Document the local device settings
    
    Different file systems store timestamps differently  
    
    -   FAT: Time is stored in local time
    -   NTFS: Time is stored in GMT
    
    Record the time offset from the operating system  
    
    -   The Windows Registry
    -   Many different values (daylight saving time, time change information, etc.)

6.  Event logs

    System logs  
    
    -   Documents important operating system and application events
    
    Export and store for future reference  
    
    -   Filter and parse
    
    Log store  
    
    -   Linux: /var/log
    -   Windows: Event Viewer

7.  Interviews

    Who might have seen this?  
    
    -   You won’t know until you ask
    
    Interview and document  
    
    -   These folks might not be around later
    
    Not all withess statements are 100% accurate  
    
    -   Humans are fallible

8.  Reports

    Document the findings  
    
    -   For Internal use, legal proceedings, etc.
    
    Summary information  
    
    -   Overview of the security event
    
    Detailed explanation of data acquisition  
    
    -   Step-by-step method of the process
    
    The findings  
    
    -   An analysis of the data
    
    Conclusion  
    
    -   Professional results, given the analysis



### Forensic data acquisition

1.  Order of volatility

    How long does data stick around?  
    
    -   Some media is much more volatile than others
    -   Gather data in order from the most volatile to less volatile
    
    From most to least volatile medium:  
    
    <table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">
    
    
    <colgroup>
    <col  class="org-left" />
    </colgroup>
    <tbody>
    <tr>
    <td class="org-left">CPU registers, CPU cache</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Router table, ARP cache, process table, kernel statistics, memory</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Temporary file systems</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Disk</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Remote logging and monitoring data</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Physical configuration, network topology</td>
    </tr>
    
    
    <tr>
    <td class="org-left">Archival media</td>
    </tr>
    </tbody>
    </table>

2.  Disk

    Copy everything on a storage drive  
    
    -   Hard drive, SSD, flash drive
    
    Drive image preparation  
    
    -   Power down to prevent changes
    -   Remove storage drive
    
    Connect to imaging device  
    
    -   With write-protection
    
    Forensic clone  
    
    -   Bit-for-bit copy
    -   Preserve all data (even the “deleted” data)

3.  Random-access memory (RAM)

    A difficult target to capture  
    
    -   Changes constantly
    -   Capturing data changes the data
    
    Memory dump  
    
    -   Grab everything in active RAM
    -   Many third-party tools
    
    Important data  
    
    -   Browsing history
    -   Clipboard information
    -   Encryption keys
    -   Command history

4.  Swap/pagefile

    Used by different operating systems  
    
    -   Slightly different usage in each
    
    A place to store RAM when memory is depleted  
    
    -   There’s a lot more space on the storage drive
    -   Transfer pages of RAM to a storage drive
    
    Can also contain portions of an application  
    
    -   Page out portions that aren’t in use
    
    Contains data similar to a RAM dump  
    
    -   Anything active on the system

5.  Operating system

    OS files and data  
    
    -   May have been modified
    
    Core operating system  
    
    -   Executable files and libraries
    -   Can be compared later to known-good files
    -   Usually captured with a drive image
    
    Other OS data  
    
    -   Logged in users
    -   Open ports
    -   Processes currently running
    -   Attached device list

6.  Device

    Mobile devices and tablets  
    
    -   A more challenging forensics task
    
    Capture data  
    
    -   Use an existing backup file
    -   Transfer image over USB
    
    Data  
    
    -   Phone calls
    -   Contact information
    -   Text messages
    -   Email data
    -   Images and movies

7.  Firmware

    Extract the device firmware  
    
    -   Rootkits and exploited hardware device
    -   A reprogrammed firmware or ROM
    
    Specific to the platform  
    
    -   Firmware implementations vary widely
    
    Attacker gains access to the device  
    
    -   Maintains access through OS updates
    
    Data discovery  
    
    -   Exploit data
    -   Firmware functionality
    -   Real-time data

8.  Snapshot

    Generally associated with virtual machines (VMs)  
    
    -   A point-in-time system image
    
    Incremental between snapshots  
    
    -   Original image is the full backup
    -   Each snapshot is incremented from the last
    -   Restoring requires the original and all snapshots
    
    Contains all files and information about a VM  
    
    -   Similar to a system image
    -   Operating system, applications, user data, etc.

9.  Cache

    Store data for use later  
    
    -   Often used to increase performance
    -   Many different caches (CPU, disk, Internet, etc.)
    
    Can contain specialized data  
    
    -   CPU cache is very short-term instruction storage
    
    Some data may never be used  
    
    -   Erased after a specified timeframe or when the cache is full
    -   Browser caches are often long-lived
    
    Data  
    
    -   URL locations
    -   Browser page components (text, images)

10. Network

    Gather information about and from the network  
    
    -   Network connections, packet captures
    
    Inbound and outbound sessions  
    
    -   OS and application traffic
    
    Packet data  
    
    -   Capture raw network data
    -   May include long-term packet captures
    
    Third-party packet captures  
    
    -   Firewalls, IPS, etc.

11. Artifacts

    Digital items left behind  
    
    -   Every contact leaves a trace
    -   May not be obvious to access
    
    Artifact locations  
    
    -   Log information
    -   Flash memory
    -   Prefetch cache files
    -   Recycle Bin
    -   Browser bookmarks and logins



### On-premises vs Cloud forensics

1.  Forensics in the cloud

    Adding complexity to the digital forensics process  
    
    -   Cloud technologies
    
    Technical challenges  
    
    -   Devices are not totally in your control
    -   There may be limited access
    -   Associate data with a specific user
    
    Legal issues  
    
    -   Laws are different around the world
    -   The rules may not be immediately obvious

2.  Right-to-audit clauses

    Common to work with business partners  
    
    -   Data sharing
    -   Outsourcing
    
    Cloud computing providers  
    
    -   Can hold all of the data
    -   Manage Internet access
    -   Are they secure?
    
    Right-to-audit should be in the contract  
    
    -   A legal agreement to have the option to perform a security audit at any time
    -   Everyone agrees to the terms and conditions
    -   Ability to verify security before a breach occurs

3.  Regulation/jurisdiction

    Cloud computing technology appeared relatively quickly  
    
    -   The legal world is scrambling to catch up
    
    Forensics professionals must know their legal rights  
    
    -   Data in a different jurisdiction may be bound by very different regulations
    
    Data stored in cloud may not be located in the same country  
    
    -   Location of the data center may determine how data can be treated
    
    Location of the data is critical  
    
    -   Legal frameworks vary widely between countries
    -   Some countries don’t allow electronic searches outside of their borders

4.  Data breach notification laws

    Notification laws  
    
    -   If consumer data is breached, the consumer must be informed
    
    Many data breach notification laws  
    
    -   Vary widely across countries and localities
    -   If you’re in the cloud, you’re a global entity
    
    Notification requirements also vary  
    
    -   Type of data breached
    -   Who gets notified
    -   How quickly



### Managing evidence

1.  Integrity

    Hashing  
    
    -   Cryptographic integrity verification
    -   A digital “fingerprint”
    
    Checksums  
    
    -   Protects against accidental changes during transmission
    -   A relatively simple integrity check
    -   Not designed to replace a hash
    
    Provenance  
    
    -   Documentation of authenticity
    -   [A chain of custody](#org4cd497a) for data handling
    -   Blockchain technology

2.  Preservation

    Handling evidence  
    
    -   Isolate and protect the data
    -   Analyze the data later without any alterations
    
    Manage the collection process  
    
    -   Work from copies
    -   Manage the data collection from mobile devices
    
    Live collection has become an important skill  
    
    -   Data may be encrypted or difficult to collect after powering down
    
    Follow best practices to ensure admissibility of data in court  
    
    -   What happens now affects the future

3.  E-discovery

    Electronic discovery  
    
    -   Collect, prepare, review, interpret, and produce electronic documents
    
    E-discovery gathers data required by the legal process  
    
    -   Does not generally involve analysis
    -   There’s no consideration of intent
    
    Works together with digital forensics  
    
    -   The e-discovery process obtains a storage drive
    -   Data on the drive is smaller than expected
    -   Forensics experts determine that data was deleted and attempt to recover the data

4.  Data recovery

    Extract missing data without affecting the integrity of the data  
    
    -   Requires training and expertise
    
    The recovery process can vary  
    
    -   Deleted files
    -   Hidden data
    -   Hardware or software corruption
    -   Storage device is physically damaged

5.  Non-repudiation

    Proof of data integrity and the origin of the data  
    
    -   The data is unchanged and really did come from the sender
    -   Hashing the data
    
    Authentication that is genuine with high confidence  
    
    -   The only person who could have sent the data is the sender
    
    Message Authentication Code (MAC)  
    
    -   The two parties can verify non-repudiation
    
    Digital Signature  
    
    -   The non-repudiation can be publicly verified

6.  Strategic intelligence/counterintelligence

    Strategic intelligence  
    
    -   A focus on key threat activity for a domain
    -   Business sectors, geographical regions, countries
    -   Gather information from internal threat reports, third-party data sources, and other data inputs
    -   Determine the threat landscape based on the trends
    
    Strategic counterintelligence (Cl)  
    
    -   Prevent hostile intelligence operations
    -   Discover and disrupt foreign intelligence threats
    -   Gather threat information on foreign intelligence operations



# Governance, Risk, and Compliance 14%



## Compare and contrast various types of controls



### Security Controls

Security risks are out there  

-   Many different types to consider

Assets are also varied  

-   Data, physical property, computer systems

Prevent security events, minimize the impact, and limit the damage  

-   Security controls

1.  Control categories

    1.  Managerial controls  
        -   Controls that address security design and implementation
        -   Security policies, standard operating procedures
    2.  Operational controls  
        -   Controls that are implemented by people
        -   Security guards, awareness programs
    3.  Technical controls  
        -   Controls implemented using systems
        -   Operating system controls
        -   Firewalls, anti-virus

2.  Control types

    Preventive  
    
    -   Physically control access
    -   Door lock
    -   Security guard
    -   Firewall
    
    Detective  
    
    -   May not prevent access
    -   Identifies and records any intrusion attempt
    -   Motion detector, IDS
    
    Corrective  
    
    -   Desighed to mitigate damage
    -   IPS can block an attacker
    -   Backups can mitigate a ransomware infection
    -   A backup site can provide options when a storm hits
    
    Deterrent  
    
    -   May not directly prevent access
    -   Discourages an intrusion attempt
    -   Warning signs, login banner, lights
    
    Compensating  
    
    -   Doesn’t prevent an attack
    -   Restores using other means
    -   Re-image or restore from backup
    -   Hot site
    -   Backup power system
    
    Physical  
    
    -   Fences, locks, mantraps
    -   Real-world security



## Explain the importance of applicable regulations, standards, or frameworks that impact organizational security posture



### Security Regulations and Standards

1.  Compliance

    Compliance  
    
    -   Meeting the standards of laws, policies, and regulations
    
    A healthy catalog of regulations and laws  
    
    -   Across many aspects of business and life
    -   Many are industry-specific or situational
    
    Penalties  
    
    -   Fines, incarceration, loss of employment
    
    Scope  
    
    -   Covers national, territory, or state laws
    -   Domestic and international requirements

2.  GDPR - General Data Protection Regulation

    European Union regulation  
    
    -   Data protection and privacy for individuals in the EU
    -   Name, address, photo, email address, bank details, posts on social networking websites, medical information, a computer&rsquo;s IP address, etc.
    
    Controls export of personal data  
    
    -   Users can decide where their data goes
    
    Gives individuals control of their personal data  
    
    -   A right to be forgotten
    
    Site privacy policy  
    
    -   Details all of the privacy rights for a user

3.  PCI DSS

    Payment Card Industry Data Security Standard (PCI DSS)  
    
    -   A standard for protecting credit cards
    
    Six control objectives  
    
    -   Build and maintain a secure network and systems
    -   Protect cardholder data
    -   Maintain a vulnerability management program
    -   Implement strong access control measures
    -   Regularly monitor and test networks
    -   Maintain an information security policy



### Security frameworks

Secure your data.  

-   Where do you start? What are the best practices?
-   If only there was a book.

Often a complex problem  

-   Unique organizational requirements
-   Compliance and regulatory requirements
-   Many different processes and tools are available

Use a security framework  

-   Documented processes
-   A guide for creating a security program
-   Define tasks and prioritize projects

1.  Center for Internet Security (CIS)

    Center for Internet Security Critical Security Controls for Effective Cyber Defense  
    
    -   CIS CSC
    
    Improve cyber defenses  
    
    -   Twenty key actions (the critical security controls)
    -   Categorized for different organization sizes
    
    Designed for implementation  
    
    -   Weritten for IT professionals
    -   Includes practical and actionable tasks

2.  NIST RMF

    National Institute of Standards and Technology Risk Management Framework (RMF)  
    
    -   Mandatory for US federal agencies and organizations that handle federal data
    
    Six step process  
    
    1.  Categorize - Define the environment
    2.  Select - Pick appropriate controls
    3.  Implement - Define proper implementation
    4.  Assess - Determine if controls are working
    5.  Authorize - Make a decision to authorize a system
    6.  Monitor - Check for ongoing compliance

3.  NIST CSF

    National Institute of Standards and Technology Cybersecurity Framework (CSF)  
    
    -   A voluntary commercial framework
    
    Framework Core  
    
    -   Identify, Protect, Detect, Respond, and Recover
    
    Framework Implementation Tiers  
    
    -   An organization’s view of cybersecurity risk and processes to manage the risk
    
    Framework Profile  
    
    -   The alignment of standards, guidelines, and practices to the Framework Core

4.  ISO/IEC frameworks

    International Organization for Standardization  
    International Electrotechnical Commission  
    ISO/IEC 27001  
    
    -   Standard for an Information Security Management System (ISMS)
    
    ISO/IEC 27002  
    
    -   Code of practice for information security controls
    
    ISO/IEC 27701  
    
    -   Privacy Information Management Systems (PIMS)
    
    ISO 31000  
    
    -   International standards for risk management practices

5.  SSAE SOC 2 Type I/II

    The American Institute of Certified Public Accountants (AICPA) auditing standard Statement on Standards for Attestation Engagements number 18 (SSAE 18)  
    SOC 2 (System and Organization control) - Trust Services Criteria (security controls)  
    
    -   Firewalls, intrusion detection, and multi-factor authentication
    
    Type I audit  
    
    -   Tests controls in place at a particular point in time
    
    Type II  
    
    -   Tests controls over a period of at least six consecutive months

6.  Cloud Security Alliance (CSA)

    Security in cloud computing  
    
    -   Not-for-profit organization
    
    Cloud Controls Matrix (CCM)  
    
    -   Cloud-specific security controls
    -   Controls are mapped to standards, best practices, and regulations
    
    Enterprise Architecture  
    
    -   Methodology and tools
    -   Assess internal IT groups and cloud providers
    -   Determine security capabilities
    -   Build a roadmap



### Secure configurations

No system is secure with the default configurations  

-   You need some guidelines to keep everything safe

Hardening guides are specific to the software or platform  

-   Get feedback from the manufacturer or Internet interest group
-   They’ll have the best details

Other general-purpose guides are available online  

1.  Web server hardening

    Access a server with your browser  
    
    -   The fundamental server on the Internet
    -   Microsoft Internet Information Server, Apache HTTP Server, et al.
    
    Huge potential for access issues  
    
    -   Data leaks, server access
    
    Secure configuration  
    
    -   Information leakage: Banner information, directory browsing
    -   Permissions: Run from a non-privileged account, configure file permissions
    -   Configure SSL: Manage and install certificates
    -   Log files: Monitor access and error logs

2.  Operating system hardening

    Many and varied  
    
    -   Windows, Linux, iOS, Android, et al.
    
    Updates  
    
    -   Operating system updates/service packs, security patches
    
    User accounts  
    
    -   Minimum password lengths and complexity
    -   Account limitations
    
    Network access and security  
    
    -   Limit network access
    
    Monitor and secure  
    
    -   Anti-virus, anti-malware

3.  Application server

    Programming languages, runtime libraries, etc.  
    
    -   Usually between the web server and the database
    -   Middleware
    
    Very specific functionality  
    
    -   Disable all unnecessary services  
        Operating system updates
    -   Security patches
    
    File permissions and access controls  
    
    -   Limit rights to what’s required
    -   Limit access from other devices

4.  Network infrastructure devices

    Switches, routers, firewalls, IPS, etc.  
    
    -   You never see them, but they’re always there
    
    Purpose-built devices  
    
    -   Embedded OS, limited OS access
    
    Configure authentication  
    
    -   Don’t use the defaults
    
    Check with the manufacturer  
    
    -   Security updates
    -   Not usually updated frequently
    -   Updates are usually important



## Explain the importance of policies to organizational security



### Personnel security

1.  Acceptable use policies (AUP)

    What is acceptable use of company assets?  
    
    -   Detailed documentation
    -   May be documented in the Rules of Behavior
    
    Covers many topics  
    
    -   Internet use, telephones, computers, mobile devices, etc.
    
    Used by an organization to limit legal liability  
    
    -   If someone is dismissed, these are the well-documented reasons why

2.  Business policies

    Job rotation  
    
    -   Keep people moving between responsibilities
    -   No one person maintains control for long periods of time
    
    Mandatory vacations  
    
    -   Rotate others through the job
    -   The longer the vacation, the better chance to identify fraud
    -   Especially important in high-security environments
    
    Separation of duties  
    
    -   Split knowledge  
        -   No one person has all of the details
        -   Half of a safe combination
    -   Dual control  
        -   Two people must be present to perform the business function
        -   Two keys open a safe (or launch a missile)
    
    Clean desk policy  
    
    -   When you leave, nothing is on your desk
    -   Limit the exposure of sensitive data to third-parties

3.  Least privilege

    Rights and permissions should be set to the bare minimum  
    
    -   You only get exactly what’s needed to complete your objective
    
    All user accounts must be limited  
    
    -   Applications should run with minimal privileges
    
    Don’t allow users to run with administrative privileges  
    
    -   Limits the scope of malicious behavior

4.  Background checks

    Background checks  
    
    -   Pre-employment screening
    -   Verify the applicant’s claims
    -   Discover criminal history, workers compensation claims, etc.
    -   Legalities vary by country
    
    Adverse actions  
    
    -   An action that denies employment based on the background check
    -   May require extensive documentation
    -   Can also include existing employees

5.  Personnel security procedures

    NDA (Non-disclosure agreement)  
    
    -   Confidentiality agreement / Legal contract
    -   Prevents the use and dissemination of confidential information
    
    Social media analysis  
    
    -   Gather data from social media
    -   Facebook, Twitter, LinkedIn, Instagram
    -   Build a personal profile
    -   Another data point when making a hiring decision

6.  On-boarding

    Bring a new person into the organization  
    
    -   New hires or transfers
    
    IT agreements need to be sighed  
    
    -   May be part of the employee handbook or a separate AUP
    
    Create accounts  
    
    -   Associate the user with the proper groups and departments
    
    Provide required IT hardware  
    
    -   Laptops, tablets, etc.
    -   Preconfigured and ready to go

7.  Off-boarding

    All good things&#x2026;  
    
    -   But you knew this day would come
    
    This process should be pre-planned  
    
    -   You don’t want to decide how to do things at this point
    
    What happens to the hardware?  
    What happens to the data?  
    Account information is usually deactivated  
    
    -   But not always deleted

8.  User training

    Gamification  
    
    -   Score points
    -   Compete with others
    -   Collect badges
    
    Capture the flag (CTF)  
    
    -   Security competition
    -   Hack into a server to steal data (the flag)
    -   Can involve highly technical simulations
    -   A practical learning environment
    
    Phishing simulation  
    
    -   Send simulated phishing emails
    -   Make vishing calls
    -   See which users are susceptible to phishing attacks without being a victim of phishing  
        Computer-based training (CBT)
    -   Automated pre-built training
    -   May include video, audio, and Q&A
    -   Users all receive the same training experience

9.  Role-based security awareness training

    Before providing access, train your users  
    
    -   Detailed security requirements
    
    Specialized training  
    
    -   Each user role has
    
    unique security responsibilities  
    Also applies to third-parties  
    
    -   Contractors, partners, suppliers
    
    Detailed documentation and records  
    
    -   Problems later can be severe for everyone



### Third-party risk management

1.  Vendors

    Every organization works with vendors  
    
    -   Payroll, customer relationship management, email marketing, travel, raw materials
    
    Important company data is often shared  
    
    -   May be required for cloud-based services
    
    Perform a risk assessment  
    
    -   Categorize risk by vendor and manage the risk
    
    Use contracts for clear understanding  
    
    -   Make sure everyone understands the expectations
    -   Use the contract to enforce a secure environment

2.  Supply chain

    The system involved when creating a product  
    
    -   Involves organizations, people, activities, and resources
    
    Supply chain assessment  
    
    -   Get a product or service from supplier to customer
    -   Evaluate coordination between groups
    -   Identify areas of improvement
    -   Assess the IT systems supporting the operation
    -   Document the business process changes

3.  Business partners

    Much closer to your data than a vendor  
    
    -   May require direct access
    -   May be a larger security concern than an outside hacker
    
    Often involves communication over a trusted connection  
    
    -   More difficult to identify malicious activity
    
    Partner risk management should be included  
    
    -   Requirements for best practices, data handling, intellectual property
    
    Include additional security between partners  
    
    -   Firewalls and traffic filters

4.  Common agreements

    Service Level Agreement (SLA)  
    
    -   Minimum terms for services provided
    -   Uptime, response time agreement, etc.
    -   Commonly used between customers and service providers
    
    Memorandum of Understanding (MOU)  
    
    -   Both sides agree on the contents of the memorandum
    -   Usually includes statements of confidentiality
    -   Informal letter of intent; not a signed contract
    
    Measurement system analysis (MSA)  
    
    -   Don’t make decisions based on incorrect data!
    -   Used with quality management systems, i.e., Six Sigma
    -   Assess the measurement process
    -   Calculate measurement uncertainty
    
    Business Partnership Agreement (BPA)  
    
    -   Going into business together
    -   Owner stake
    -   Financial contract
    -   Decision-making agreements
    -   Prepare for contingencies

5.  Non-disclosure agreement (NDA)

    Confidentiality agreement between parties  
    
    -   Information in the agreement should not be disclosed
    
    Protects confidential information  
    
    -   Trade secrets
    -   Business activities
    -   Anything else listed in the NDA
    
    Unilateral or bilateral (or multilateral)  
    
    -   One-way NDA or mutual NDA
    
    Formal contract  
    
    -   Signatures are usually required

6.  Product support lifetime

    End of life (EOL)  
    
    -   Manufacturer stops selling a product
    -   May continue supporting the product
    -   Important for security patches and updates
    
    End of service life (EOSL)  
    
    -   Manufacturer stops selling a product
    -   Support is no longer available for the product
    -   No ongoing security patches or updates
    -   May have a premium-cost support option
    
    Technology EOSL is a significant concern  
    
    -   Security patches are part of normal operation



### Managing data

1.  Data governance

    Rules, processes, and accountability associated with an organization’s data  
    
    -   Data is used in the right ways
    
    Data steward  
    
    -   Manages the governance processes
    -   Responsible for data accuracy, privacy, and security
    -   Associates sensitivity labels to the data
    -   Ensures compliance with any applicable laws and standards
    
    Formal rules for data  
    
    -   Everyone must know and follow the processes

2.  Data classification

    Identify data types  
    
    -   Personal, public, restricted, etc.
    -   Use and protect data efficiently
    
    Associate governance controls to the classification levels  
    
    -   How the data class should be managed
    
    Data compliance  
    
    -   Laws and regulations regarding certain types of data
    -   GDPR - General Data Protection Regulation

3.  Data retention

    Keep files that change frequently for version control  
    
    -   Files change often
    -   Keep at least a week, perhaps more
    
    Recover from virus infection  
    
    -   Infection may not be identified immediately
    -   May need to retain 30 days of backups
    
    Often legal requirements for data retention  
    
    -   Email storage may be required over years
    -   Some industries must legally store certain data types
    -   Different data types have different storage requirements  
        -   Corporate tax information, customer Pll, tape backups, etc.



### Credential policies

1.  Credential management

    All that stands between the outside world and all of the data  
    
    -   The data is everything
    
    Passwords must not be embedded in the application  
    
    -   Everything needs to reside on the server, not the client
    
    Communication across the network should be encrypted  
    
    -   Authentication traffic should be impossible to see

2.  Personnel accounts

    An account on a computer associated with a specific person  
    
    -   The computer associates the user with a specific identification number
    
    Storage and files can be private to that user  
    
    -   Even if another person is using the same computer
    
    No privileged access to the operating system  
    
    -   Specifically not allowed on a user account
    
    This is the account type most people will use  
    
    -   Your user community

3.  Third-party accounts

    Access to external third-party systems  
    
    -   Cloud platforms for payroll, enterprise resource planning, etc
    
    Third-party access to corporate systems  
    
    -   Access can come from anywhere
    
    Add additional layers of security  
    
    -   2FA (two factor authentication)
    -   Audit the security posture of third-parties
    
    Don’t allow account sharing  
    
    -   All users should have their own account

4.  Device accounts

    Access to devices  
    
    -   Mobile devices
    
    Local security  
    
    -   Device certificate
    -   Require screen locks and unlocking standards
    -   Manage through a Mobile Device Manager (MDM)
    
    Add additional security  
    
    -   Geography-based
    -   Include additional authentication factors
    -   Associate a device with a user

5.  Service accounts

    Used exclusively by services running on a computer  
    
    -   No interactive/user access (ideally)
    -   Web server, database server, etc.
    
    Access can be defined for a specific service  
    
    -   Web server rights and permissions will be different than a database server
    
    Commonly use usernames and passwords  
    
    -   You’ll need to determine the best policy for password updates

6.  Administrator/root accounts

    Elevated access to one or more systems  
    
    -   Super user access
    
    Complete access to the system  
    
    -   Often used to manage hardware,
    
    drivers, and software installation  
    This account should not be used for normal administration  
    
    -   User accounts should be used
    
    Needs to be highly secured  
    
    -   Strong passwords, 2FA
    -   Scheduled password changes



### Organizational policies

1.  Change management

    How to make a change  
    
    -   Upgrade software, change firewall configuration, modify switch ports
    
    One of the most common risks in the enterprise  
    
    -   Occurs very frequently
    
    Often overlooked or ignored  
    
    -   Did you feel that bite?
    
    Have clear policies  
    
    -   Frequency, duration, installation process, fallback procedures
    
    Sometimes extremely difficult to implement  
    
    -   It’s hard to change corporate culture

2.  Change control

    A formal process for managing change  
    
    -   Avoid downtime, confusion, and mistakes
    
    Nothing changes without the process  
    
    -   Determine the scope of the change
    -   Analyze the risk associated with the change
    -   Create a plan
    -   Get end-user approval
    -   Present the proposal to the change control board
    -   Have a backout plan if the change doesn’t work
    -   Document the changes

3.  Asset management

    ldentify and track computing assets  
    
    -   Usually an automated process
    
    Respond faster to security problem  
    
    -   You know who, what, and where
    
    Keep an eye on the most valuable assets  
    
    -   Both hardware and data
    
    Track licenses  
    
    -   You know exactly how many you’ll need
    
    Verify that all devices are up to date  
    
    -   Security patches, anti-malware signature updates, etc.



## Summarize risk management processes and concepts



### Risk Management Types

1.  Risk assessment

    ldentify assets that could be affected by an attack  
    
    -   Define the risk associated with each asset
    -   Hardware, customer data, intellectual property
    
    Identify threats  
    
    -   Loss of data, disruption of services, etc.
    
    Determine the risk  
    
    -   High, medium, or low risk
    
    Assess the total risk to the organization  
    
    -   Make future security plans
    
    External threats  
    
    -   Outside the organization
    -   Hacker groups, former employees
    
    Internal threats  
    
    -   Employees and partners
    -   Disgruntled employees
    
    Legacy systems  
    
    -   Outdated, older technologies
    -   May not be supported by the manufacturer
    -   May not have security updates
    -   Depending on the age, may not be easily accessible

2.  Multi-party risk

    Breaches involving multiple parties  
    
    -   Often trusted business relationships
    -   Events often involve many different parties
    
    Intellectual Property (IP) theft  
    
    -   Theft of ideas, inventions, and creative expressions
    -   Human error, hacking, employees with access, etc.
    -   ldentify and protect IP
    -   Educate employees and increase security
    
    Software compliance/licensing  
    
    -   Operational risk with too few licenses
    -   Financial risk with budgeting and over-allocated licenses
    -   Legal risk if proper licensing is not followed

3.  Risk management strategies

    Acceptance  
    
    -   A business decision; we’ll take the risk!
    
    Risk-avoidance  
    
    -   Stop participating in a high-risk activity
    
    Transference  
    
    -   Buy some cybersecurity insurance
    
    Mitigation  
    
    -   Decrease the risk level
    -   Invest In security systems



### Risk analysis

1.  Evaluating risk

    Risk register  
    
    -   Every project has a plan, but also has risk
    -   ldentify and document the risk associated with each step
    -   Apply possible solutions to the identified risks
    -   Monitor the results
    
    Risk matrix / risk heat map  
    
    -   View the results of the risk assessment
    -   Visually identify risk based on color
    -   Combines the likelihood of an event with the potential impact
    -   Assists with making strategic decisions
    
    ![img](res/risk_heat_map.png)  

2.  Audit risk model

    Inherent risk  
    
    -   Impact + Likelihood
    
    Risk that exists in the absence of controls  
    
    -   Some models include the existing set of controls
    
    Residual risk  
    
    -   Inherent risk + control effectiveness
    -   Risk that exists after controls are considered
    -   Some models base it on including additional controls
    
    Risk appetite  
    
    -   The amount of risk an organization is willing to take

3.  Risk control assessment

    Risk has been determined  
    
    -   Heat maps have been created
    
    Time to build cybersecurity requirements  
    
    -   Based on the identified risks
    
    Find the gap  
    
    -   Often requires a formal audit
    -   Self-assessments may be an option
    
    Build and maintain security systems based on the requirements  
    
    -   The organizational risk determines the proper controls
    
    Determine if existing controls are compliant or non-compliant  
    
    -   Make plans to bring everything into compliance

4.  Risk awareness

    A constantly changing battlefield  
    
    -   New risks, emerging risks
    -   A nearly overwhelming amount of information
    -   Difficult to manage a defense
    
    Knowledge is key  
    
    -   Part of every employee’s daily job role
    -   Part of the onboarding process for employees and partners
    
    Maintaining awareness  
    
    -   Ongoing group discussions
    -   Presentations from law enforcement
    -   Attend security conferences and programs

5.  Regulations that affect risk posture

    Many of them  
    
    -   Regulations tend to regulate
    
    Regulations directly associated to cybersecurity  
    
    -   Protection of personal information, disclosure of information breaches
    -   Requires a minimum level of information security
    
    HIPAA - Health Insurance Portability and Accountability Act  
    
    -   Privacy of patient records
    -   New storage requirements, network security, protect against threats
    
    GDPR - General Data Protection Regulation  
    
    -   European Union data protection and privacy
    -   Personal data must be protected and managed for privacy

6.  Qualitative risk assessment

    Identify significant risk factors  
    
    -   Ask opinions about the significance
    -   Display visually with traffic light grid or similar method
    
    ![img](res/risk_example.png)  

7.  Quantitative risk assessment

    Likelihood  
    
    -   Annualized Rate of Occurrence (ARO)
    -   How likely is it that a hurricane will hit? In Montana? In Florida?
    
    SLE (Single Loss Expectancy)  
    
    -   What is the monetary loss if a single event occurs?
    -   Laptop stolen (asset value or AV) = $1,000
    
    ALE (Annualized Loss Expectancy)  
    
    -   ARO x SLE
    -   Seven laptops stolen a year (ARO) x $1,000 (SLE) = $7,000
    
    The business impact can be more than monetary  
    
    -   Quantitative vs. qualitative

8.  Disaster types

    Environmental threats  
    
    -   Tornado, hurricane, earthquake, severe weather
    
    Person-made threats  
    
    -   Human intent, negligence, or error
    -   Arson, crime, civil disorder, fires, riots, etc.
    
    Internal and external  
    
    -   Internal threats are from employees
    -   External threats are from outside the organization



### Business impact analysis

1.  Recovery

    Recovery time objective (RTO)  
    
    -   Get up and running quickly
    -   Get back to a particular service level
    
    Recovery point objective (RPO)  
    
    -   How much data loss is acceptable?
    -   Bring the system back online; how far back does data go?
    
    Mean time to repair (MTTR)  
    
    -   Time required to fix the issue
    
    Mean time between failures (MTBF)  
    
    -   Predict the time between outages

2.  Functional recovery plans

    Recover from an outage  
    
    -   Step-by-step guide
    
    Contact information  
    
    -   Someone is on-call
    -   Keep everyone up to date
    
    Technical process  
    
    -   Reference the knowledge base
    -   Follow the internal processes
    
    Recover and test  
    
    -   Confirm normal operation

3.  Removing single point of failure

    A single event can ruin your day  
    
    -   Unless you make some plans
    
    Network configuration  
    
    -   Multiple devices
    
    Facility / Utilities  
    
    -   Backup power, multiple cooling devices
    
    People / Location  
    
    -   A good hurricane can disrupt personnel travel
    
    There’s no practical way to remove all points of failure  
    
    -   Money drives redundancy

4.  Disaster recovery plan (DRP)

    Detailed plan for resuming operations after a disaster  
    
    -   Application, data center, building, campus, region, etc.
    
    Extensive planning prior to the disaster  
    
    -   Backups
    -   Off-site data replication
    -   Cloud alternatives
    -   Remote site
    
    Many third-party options  
    
    -   Physical locations
    -   Recovery services

5.  Impact

    Life  
    
    -   The most important consideration
    
    Property  
    
    -   The risk to buildings and assets
    
    Safety  
    
    -   Some environments are too dangerous to work
    
    Finance  
    
    -   The resulting financial cost
    
    Reputation  
    
    -   An event can cause status or character problems

6.  Mission-essential functions

    If a hurricane blew through, what functions would be essential to the organization?  
    
    -   That’s where you start your analysis
    -   These are broad business requirements
    
    What computing systems are required for these mission-essential business functions?  
    
    -   Identify the critical systems

7.  Site risk assessment

    All locations are a bit different  
    
    -   Even those designed to be similar
    
    Recovery plans should consider unique environments  
    
    -   Applications
    -   Personnel
    -   Equipment
    -   Work environment



## Explain privacy and sensitive data concepts in relation to security



### Privacy and Data Breaches

1.  Information life cycle

    Creation and receipt  
    
    -   Create data internally or receive data from a third-party
    
    Distribution  
    
    -   Records are sorted and stored
    
    Use  
    
    -   Make business decisions, create products and services
    
    Maintenance  
    
    -   Ongoing data retrieval and data transfers
    
    Disposition  
    
    -   Archiving or disposal of data

2.  Consequences

    Reputation damage  
    
    -   Opinion of the organization becomes negative
    -   Can have an impact on products or services
    -   Can impact stock price
    
    Identity theft  
    
    -   Company and/or customers information becomes public
    -   May require public disclosure
    -   Credit monitoring costs
    
    Fines  
    Intellectual Property (IP) theft  
    
    -   Stealing company secrets
    -   Can put an organization out of business

3.  Notification

    Internal escalation process  
    
    -   Breaches are often found by technicians
    -   Provide a process for making those findings known
    
    External escalation process  
    
    -   Know when to ask for assistance from external resources
    -   Security experts can find and stop an active breach
    
    Public notifications and disclosures  
    
    -   Refer to security breach notification laws
    -   All 50 US states, EU, Australia, etc.
    -   Delays might be allowed for criminal investigations

4.  Privacy impact assessment (PIA)

    Almost everything can affect privacy  
    
    -   New business relationships, product updates, website features, service offering
    
    Privacy risk needs to be identified in each initiative  
    
    -   How could the process compromise customer privacy?
    
    Advantages  
    
    -   Fix privacy issues before they become a problem
    -   Provides evidence of a focus on privacy
    -   Avoid data breach
    -   Shows the importance of privacy to everyone

5.  Notices

    Terms of service  
    
    -   Terms of use, terms and congitions (T&C)
    -   Legal agreement between service provider and user
    -   User must agree to the terms to use the service
    
    Privacy notice, privacy policy  
    
    -   May be required by law
    -   Documents the handling of personal data
    -   May provide additional data options and contact information



### Data classifications

1.  Labeling sensitive data

    Not all data has the same level of sensitivity  
    
    -   License tag numbers vs. health records
    
    Different levels require different security and handling  
    
    -   Additional permissions
    -   A different process to view
    -   Restricted network access

2.  Data classifications

    Proprietary  
    
    -   Data that is the property of an organization
    -   May also include trade secrets
    -   Often data unique to an organization
    
    PII - Personally Identifiable Information  
    
    -   Data that can be used to identify an individual
    -   Name, date of birth, mother’s maiden name, biometric information
    
    PHI - Protected Health Information  
    
    -   Health information associated with an individual
    -   Health status, health care records, payments for health care, and much more
    
    Public / Unclassified  
    
    -   No restrictions on viewing the data
    
    Private / Classified / Restricted / Internal use only  
    
    -   Restricted access, may require a non-disclosure agreement (NDA)
    
    Sensitive  
    
    -   Intellectual property, PII, PHI
    
    Confidential  
    
    -   Very sensitive, must be approved to view
    
    Critical  
    
    -   Data should always be available
    
    Financial information  
    
    -   Internal company financial information
    -   Customer financial details
    
    Government data  
    
    -   Open data
    -   Transfer between government entities
    -   May be protected by law
    
    Customer data  
    
    -   Data associated with customers
    -   May include user-specific details
    -   Legal handling requirements



### Enhancing privacy

1.  [Tokenization](#orgea4daa8)

2.  Data minimization

    Minimal data collection  
    
    -   Only collect and retain necessary data
    
    Included in many regulations  
    
    -   HIPAA has a “Minimum Necessary” rule
    -   GDPR - “Personal data shall be adequate, relevant and not excessive in relation to the purpose or purposes for which they are processed.”
    
    Some information may not be required  
    
    -   Do you need a telephone number or address?
    
    Internal data use should be limited  
    
    -   Only access data required for the task

3.  [Data masking](#org63acc83)

4.  Anonymization

    Make it impossible to identify individual data from a dataset  
    
    -   Allows for data use without privacy concerns
    
    Many different anonymization techniques  
    
    -   Hashing, masking, etc.
    
    Convert from detailed customer purchase data  
    
    -   Remove name, address, change phone number to ### ### ####
    -   Keep product name, quantity, total, and sale date
    
    Anonymization cannot be reversed  
    
    -   No way to associate the data to a user

5.  Pseudo-anonymization

    Pseudonymization  
    
    -   Replace personal information with pseudonyms
    -   Often used to maintain statistical relationships
    
    May be reversible  
    
    -   Hide the personal data for daily use or in case of breach
    -   Convert it back for other processes
    
    Random replacement  
    
    -   James Messer -> Jack O’Neill -> Sam Carter -> Daniel Jackson
    
    Consistent replacements  
    
    -   James Messer is always converted to George Hammond



### Data roles and responsibilities

High-level data relationships  

-   Organizational responsibilities, not always technical

Data owner  

-   Accouhtable for specific data, often a senior officer
-   VP of Sales owns the customer relationship data
-   Treasurer owns the financial information

1.  Data roles

    Data controller  
    
    -   Manages the purposes and means by which personal data is processed
    
    Data processor  
    
    -   Processes data on behalf of the data controller
    -   Often a third-party or different group
    
    eg: Payroll controller and processor  
    
    -   Payroll department (data controller) defines payroll amounts and timeframes
    -   Payroll company (data processor) processes payroll and stores employee information

2.  Additional data roles

    Data custodian/steward  
    
    -   Responsible for data accuracy, privacy, and security
    -   Associates sensitivity labels to the data
    -   Ensures compliance with any applicable laws and standards
    -   Manages the access rights to the data
    -   Implements security controls
    
    Data protection officer (DPO)  
    
    -   Responsible for the organization’s data privacy
    -   Sets policies, implements processes and procedures

