# Digital Forensics Discord Server FAQs

A repository to store curated answers for some of the most commonly asked questions within the [Digital Forensics Discord Server](https://discord.com/servers/digital-forensics-427876741990711298).

## Questions

### I'm looking to build a new forensic computer. What considerations should I be aware of when speccing out a build?

#### Working Ideal Answer

##### CPU

If you want to futureproof a prospective build, then strongly consider 8 cores/16 threads as the bare minimum and ideally consider 16 cores/32 threads as a best case scenario in most instances. A stretch goal would be AMD's Threadripper line, which can provide options including 12 cores/24 threads, 16 cores/32 threads, 24 cores/48 threads, 32 cores/64 threads, and even 64 cores/128 threads. 24 or 32 cores is excessive while still being within the realm of reason, but 64 cores is arguably unreasonably excessive for almost any possible scenario in DFIR. The law of [diminishing returns](https://en.wikipedia.org/wiki/Diminishing_returns) will come into play.

##### GPU

If you're into password cracking, you'll want the best GPU available and likely multiple of them. Otherwise, if you're not into password cracking, get a GPU that has enough monitor ports to satisfy the needs of your examiner(s). 

#### Answer A (to be cleaned up)

You'll probably want it to be able to comfortably run some VMs, both for analysis (i.e. SIFT Workstation, FlareVM, etc), and for sandboxing (combustion chamber for malware analysis, etc).  More processor cores and memory tends to help the most with those use-cases.

If you'll be handling lots of device/disk images on it, more disk space is useful for that case.

If you'll regularly be performing any kind of brute forcing or credential auditing (i.e. hashing/cracking) on it, then faster processor/gpu can be helpful (depending on what you're running to perform the audit)

#### Answer B (to be cleaned up)

Definitely focus on cores/threads for processing power. If you're cracking passwords, you want GPU power. If you're doing anything else, CPU power should reign supreme. Threadripper would be pretty awesome but it's expensive. I wouldn't go any less than 8 cores nowadays and for futureproofing your build. Ideally, get an Intel or AMD CPU that has double digit cores, i.e., 16 Cores/32 Threads. That should last you quite a bit yet still not be as expensive as a 32 core/64 thread Threadripper.

#### Ideal answer template

An ideal answer should have good guidelines by component or even by forensic suite?

CPU - Cores/threads
GPU - password cracking
RAM - RAM disks, multitasking, etc
Storage - m.2 vs SSD vs HDD (include graph with speed comparisons)
Writeblockers - link to various options

AXIOM/X-Ways/Cellebrite/Thor - lots of cores/threads, fast storage to minimize bottlenecks, RAM to handle processing

### How do I get started in DFIR?

Here are some videos to get you started:

* [Getting started in DFIR: Testing 1,2,3 | Phill Moore](https://youtu.be/-IUJnDs6rbE)
* [Securing Your Future in DFIR](https://www.youtube.com/watch?v=H-735uP9nFg)

Also, check out the [The Ultimate Guide to Getting Started in Digital Forensics & Incident Response (DFIR)](https://www.sans.org/white-papers/ultimate-guide-getting-started-digital-forensics-incident-response/) by [SANS](https://www.sans.org/). 

Doing research and posting about it is free. It only costs you your time! [Starting a blog](https://thisweekin4n6.com/starting-a-blog/) has a very low barrier for entry. Anyone can do it if they actually follow through!

### More to come.....

Please PR new questions here and answers will be populated in due time!
