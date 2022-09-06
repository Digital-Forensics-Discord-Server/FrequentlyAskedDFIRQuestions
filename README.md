# Digital Forensics Discord Server FAQs

A repository to store curated answers for some of the most commonly asked questions within the [Digital Forensics Discord Server](https://discord.com/servers/digital-forensics-427876741990711298).

## Questions

### I'm looking to build a new forensic computer. What considerations should I be aware of when speccing out a build?

#### Working Ideal Answer (delete this header and adjust all the below subheaders when finalized)

##### CPU

If you want to futureproof a prospective build, then strongly consider 8 cores/16 threads as the bare minimum and ideally consider 16 cores/32 threads as a best case scenario in most instances. A stretch goal would be AMD's [Threadripper](https://en.wikipedia.org/wiki/List_of_AMD_Ryzen_processors) line, which can provide options including 12 cores/24 threads, 16 cores/32 threads, 24 cores/48 threads, 32 cores/64 threads, and even 64 cores/128 threads. 24 or 32 cores is excessive while still being within the realm of reason, but 64 cores is arguably unreasonably excessive for almost any possible scenario in DFIR. The law of [diminishing returns](https://en.wikipedia.org/wiki/Diminishing_returns) will come into play.

##### GPU

If you're into password cracking, you'll want the best GPU available, and likely multiple of them. Otherwise, if you're not into password cracking, get a GPU that has enough monitor ports to satisfy the needs of your examiner(s). 

##### RAM

Some commercial forensic suites are RAM hogs, and some are not. As with everything, know your tool and cater your build towards the tools you'll be using on the forensic machine(s). In general, the more the merrier, but nowadays anything less than 32GB of RAM is not advised. 

One other thing to consider is if you have 128GB or more RAM in a computer, you can allocate some of that RAM to a RAM Disk for much faster read speeds of data you're parsing with a forensic tool. 

For example, see the image below ([Source](https://www.geckoandfly.com/21507/ramdisk-virtual-disk-memory/)):

![test](https://th.bing.com/th/id/R.34637985be3be016f7e3d389a3fff608?rik=Yrmd%2bSaad7ML3A&riu=http%3a%2f%2fcdn3.geckoandfly.com%2fwp-content%2fuploads%2f2016%2f06%2fram-disk-comparison-830x272.jpg&ehk=xexSnn5iW0JRfONzt3Hx34BZzCWDLDpYsNSyeXhq%2fWQ%3d&risl=&pid=ImgRaw&r=0)

##### Storage

Going off the above graphic, you can see why you should move on from HDD storage unless you need to take advantage of the larger capacities they offer. HDDs are fine for NAS devices, but for your forensic machine, they should only be used for storage of evidence that's not actively being processed, if at all. SSDs should be the bare minimum and ideally at least one or multiple M.2 storage devices would be considered for an everyday forensic machine. As of September 2022, M.2 devices max out at 4TB in storage capacity. While that will rise over time, they are definitely more expensive than SSDs and HDDs per terabyte. 

##### Other Things to Consider

###### Bottlenecks

You can have the fastest CPU, GPU, and RAM available, but if you're using 5400 RPM Hard Disk Drives (HDDs), your computer is going to move very slow as it can only go as fast as the slowest component, which is what we call a performance bottleneck.

##### Forensic Software

Not all forensic software is created equal. However, generally speaking, fast storage and CPU with lots of RAM will serve most commercial forensic suites well. Most forensic suites break down processing of artifacts/files by thread so that's where a high core/thread count will come into play to make processing artifacts/files completed in a quicker manner.

##### Other Resources

[Ryan Collins](https://github.com/ryancollins-dev), a member of the Digital Forensics Discord Server, put together [this page](https://ryd3v.rocks/posts/wrkstnbuild) in response to this commonly asked question. This answer can also be found [here](https://github.com/Digital-Forensics-Discord-Server/FrequentlyAskedDFIRQuestions/blob/main/wrkstnbuild.md) on GitHub.

TODO

include screenshots from common forensic suites showing thread processing examples

#### Answer A (to be cleaned up)

You'll probably want it to be able to comfortably run some VMs, both for analysis (i.e. SIFT Workstation, FlareVM, etc), and for sandboxing (combustion chamber for malware analysis, etc).  More processor cores and memory tends to help the most with those use-cases.

If you'll be handling lots of device/disk images on it, more disk space is useful for that case.

If you'll regularly be performing any kind of brute forcing or credential auditing (i.e. hashing/cracking) on it, then faster processor/gpu can be helpful (depending on what you're running to perform the audit)

#### Ideal answer template

An ideal answer should have good guidelines by component or even by forensic suite?

* [x] CPU - Cores/threads
* [ ] GPU - password cracking
* [x] RAM - RAM disks, multitasking, etc
* [x] Storage - m.2 vs SSD vs HDD (include graph with speed comparisons)
* [ ] Writeblockers - link to various options

AXIOM/X-Ways/Cellebrite/Thor - lots of cores/threads, fast storage to minimize bottlenecks, RAM to handle processing

### How do I get started in DFIR?

Here are some videos to get you started:

* [Getting started in DFIR: Testing 1,2,3 | Phill Moore](https://youtu.be/-IUJnDs6rbE)
* [Securing Your Future in DFIR](https://www.youtube.com/watch?v=H-735uP9nFg)

Also, check out the [The Ultimate Guide to Getting Started in Digital Forensics & Incident Response (DFIR)](https://www.sans.org/white-papers/ultimate-guide-getting-started-digital-forensics-incident-response/) by [SANS](https://www.sans.org/). 

Doing research and posting about it is free. It only costs you your time! [Starting a blog](https://thisweekin4n6.com/starting-a-blog/) has a very low barrier for entry. Anyone can do it if they actually follow through!

### More to come.....

Please PR new questions here and answers will be populated in due time!
