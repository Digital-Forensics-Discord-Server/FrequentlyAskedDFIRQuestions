## Design Methodology

I've been designing and building computers, workstations and enterprise servers now for over 25 years. I started my first builds when [Windows 95](https://en.wikipedia.org/wiki/Windows_95) was released, and have enjoyed building systems ever since. A lot has changed since then, and technology within the past few years has skyrocket upwards.

I personally use a Apple Mac Mini with the M1 chip, and it's been fantastic. Not one complaint, except a bit a of a learning curve coming from x86 architecture to Arm64, and some software compatibility.

This post however isn't about Apple or Mac, it's about my design process for x86 based workhorses. I will briefly explain my design methodology, why I go about a particular design method, and some general tips on how I settle on a design pattern for myself, and my clientele. Let's jump right into it.

<br>

### Method preview

For my custom builds, for all my customers I use the latest and greatest tested components, sourced and purchased from reputable suppliers, I don't cut corners to save a buck. I do however put a lot of research into product cost factors, based on market fluctuations, and usually mention in my quotes that market fluctuations happen, sometimes hardware can go up and down in price rather quickly, I always leave about a 20% buffer into my quotes for this variation.

### System design

When I design a system step one is to ask myself or the customer, what is your goal for this system? Based on the response, the next question is probably the most important factor, what is your budget? From here we can proceed to the design phase, where I spend a good amount of time comparing prices, specs and product availability. For the purposes of this post, we will hypothetically lay out the schema for a forensics workstation.

### System Schema

When building a system I start my build design in somewhat of an unorthodox approach, and while some builders do the same, in the professional workspace it can sometimes go against the grain. Change can be hard sometimes but stick with me.

My build schema always starts with the motherboard. Why? Think of the motherboard as the central nervous system. I always start with the newest and most feature rich motherboard currently available within my budget parameters. In this scenario, Chip manufacturer selection isn't a priority, Intel or AMD based doesn't matter, and for the sake of brevity, when I design a system, I offer both options with comparable specs and leave it up to the customer to decide, which CPU brand they would like t go with.

#### Schema

> 1. Motherboard
> 2. CPU
> 3. CPU Cooler
> 4. Memory
> 5. Storage
> 6. Video Card(s)
> 7. Case
> 8. Power Supply
> 9. Case Fan(s)

Reasons for motherboard first? I've always had the philosophy that you can easily upgrade a CPU, however motherboard upgrades, are much much harder, especially when it comes to your host software installation, OS corruption etc. It's a lot easier to swap a CPU, than to swap a motherboard, and you can save a little money in the beginning by using less or cheaper ram, and then upgrading that as needed also, it's not hard to pop a new stick in, or swap a CPU on thermal paste days right. Also maxing out on the motherboard guarantees a better overall system stability.

Ok, now that's out of the way, how do I make a mock-up for clientele? Honestly speaking, usually pen and paper, haha kidding. I use [PCPARTPICKER](https://pcpartpicker.com/), you can easily compare pricing, and share with your customers within seconds. Keep in mind builds are public, so if you're making a super secret build, use the old fashioned mock-up quote from Excel :)

Alright let's go through a sample build for a forensics workstation, with a fairly aggressive budget, and some future proofing options, I'll do my best to stay a bit conservative, so your manager doesn't have a heart attack.

## Motherboard

I tend to stick with a few brands, that over the years have served me and my clients well. Usually I go with [Asus](https://www.asus.com/ca-en/Motherboards-Components/Motherboards/All-series/), or [Gigabyte](https://www.gigabyte.com/Motherboard).

Since this is a forensics machine designed for a lab environment and not for gaming, I would go with a workstation specific board.

For this build [AMD WRX80 Ryzen™ Threadripper™ PRO extended-ATX workstation motherboard ](https://www.asus.com/ca-en/Motherboards-Components/Motherboards/Workstation/Pro-WS-WRX80E-SAGE-SE-WIFI/)

What makes this motherboard stand out?

> Dual Intel 10G Ethernet
>
> 1x USB 3.2 Gen 2 Type-C port
>
> 1x USB 3.2 Gen 2x2 Type-C port 20Gbps
>
> 7xFull x16 PCI Express 4.0 safe slots
>
> 16 Power stages
>
> 8x SATA 6Gbps ports
>
> 3x M.2 PCIe 4.0 slots
>
> ECC memory support, up to 2048 GB
>
> Intel WiFi 6 on board.
>
> Integrated BMC (Baseboard Management Controller)
>
> 2x PCIe 6-pin power connectors
>
> BIOS Flashback

This motherboard isn't available on PCPARTPICKER at the moment, so we will just add the other components to our final build list, that are compatible with the CPU selected.

Buy [ASUS Pro WS WRX80E-SAGE SE WIFI](https://www.newegg.ca/asus-pro-ws-wrx80e-sage-se-wifi/p/N82E16813119391?sid=6316910932c8cb440d745303&nm_mc=otc-hatch&cm_mmc=otc-hatchca-_-motherboards+amd-_-asus-_-13119391)

> $1,289.00 CAD

## CPU

CPU compatibility is small for this particular board, however since we are desiging a AMD system today we will continue. CPU compatibility can be found at the [CPU Support](https://www.asus.com/ca-en/Motherboards-Components/Motherboards/Workstation/Pro-WS-WRX80E-SAGE-SE-WIFI/HelpDesk_CPU/) page.

The cheapest option currently availible is the [AMD Ryzen Threadripper PRO 3955WX](https://www.newegg.ca/amd-ryzen-threadripper-pro-3955wx/p/N82E16819113673)

[AMD Ryzen™ Threadripper™ PRO 3955WX Desktop Processors](https://www.amd.com/en/products/cpu/amd-ryzen-threadripper-pro-3955wx) specs.

> CPU Cores 16, 32 Threads
>
> TDP 280W
>
> Base Clock: 3.9GHz, up to 4.2GHz
>
> PCIe 4.0
>
> DDR 4 up to 3200MHz

Beast

> $2,189.99 CAD

Ok so we have our main components, and eventhough they aren't cheap, keep in mind this is for a commercial workstation, that is designed to run 24/7 - 365

## Water cooling

I have always built my PC's with water-cooling, more specifically an AIO, "AiO" stands for "All in One", which means that you'll get a complete package, consisting of radiator, fan, pump, tubes and cooling unit, which reliably cools your CPU. Unless the client want's a custom loop, usually though for simplicity, I go with an AIO. Just like the other components, from my testing I stick with a particular brand that I've put through the paces, and have always been happy with. _EVGA_

For our build since the CPU is an absolute "Unit", shout out to my British folk, I chose the [EVGA CLC 360mm All-In-One](https://www.evga.com/products/product.aspx?pn=400-HY-CL36-V1). EVGA has a awesome warranty process, and I've had great success with their products, adn returns/replacements, to be fair, I've only had one product returned, and it was actually purchased through Amazon, so I don't know if it was just the handling of the product(video card), nevertheless they exchanged my product hassle free, and the build was a great success. They stand by their product and are quality made. Whew, that was a mouth-full.

Notable mentions, 100% copper pad, max 20dB(A) pump noise, Aluminum radiator, 3x 120x120x25mm fans, quiet out of the box. 5-Year Warranty.

> $89.99 CAD

## Memory

This motherboard supports DDR4 memory, and although it does support [ECC memory](https://en.wikipedia.org/wiki/ECC_memory), I will be using standard DDR 4 at the speed specified by Asus. I've had great success with G.Skill branded memory in the past, and for this build I'll use [Ripjaws V DDR4-3200 CL16-18-18-38 1.35V 256GB 8x32GB](https://www.gskill.com/product/165/184/1571734171/F4-3200C16Q2-256GVK), they are supported and tested by Asus for this motherboard [Memory](https://www.asus.com/ca-en/Motherboards-Components/Motherboards/Workstation/Pro-WS-WRX80E-SAGE-SE-WIFI/HelpDesk_QVL_Memory/). Price point is actually good, considering the ammount of ram you're getting, **256GB (8x32GB)**, and **Limited Lifetime Warranty**. Epic

> $716.56 CAD

## Storage

For my host OS I always go with a fast booting, high I/O NVME SSD, and for this build I will go with the [980 PRO PCIe® 4.0 NVMe™ SSD 1TB](https://www.samsung.com/us/computing/memory-storage/solid-state-drives/980-pro-pcie-4-0-nvme-ssd-1tb-mz-v8p1t0b-am/). I've had excellent performance and durability under extreme conditions with Samsung drives and in my opinion are the best. Samsung says "Genuine PCIe 4.0 NVMe® speed (up to 7,000/5,000MB/s for read/write speed)" and that's great. I will add this on the list, and select a few additional drives.

> $129.99 CAD

Additional drives, I usually advise on an additional SSD for Virtual machines or games, software etc. So for a secondary drive I usually name _Data_, I'll select [870 EVO SATA 2.5" SSD 2TB](https://www.samsung.com/us/computing/memory-storage/solid-state-drives/870-evo-sata-2-5-ssd-2tb-mz-77e2t0b-am/), good amount of space for virtual machines, V-NAND with 530MB/s Seq. Write. Excellent. I'll add this to the list and and an additional drive that's not required, but recommended.

> $179.99

For the final drive, I like to have a good solid backup drive, and while this is optional, believe me you want backups. I know I like backups, the more the merrier. For my backup drive, I have had great success with [WD Red Pro NAS Hard Drive](https://www.westerndigital.com/en-ca/products/internal-drives/wd-red-pro-sata-hdd#WD6003FFBX), excellent transfer speeds, at time comparable to a cheaper SSD. Four our build I've opted for a 6TB model.

> $179.99

## Video Card

For some builds a video card may not be required, but since our chosen CPU _does not_ have a built in graphics chip, we will need one. Also a forensic examiner will likely need to crack some hashes, so let's pick one from my favorite brand again [EVGA](https://www.evga.com/)

Since we are legends and we have come this far, let's treat ourselves to a card that is not quite as good as a Titan, but good enough to get the job done with pretty much anything we can throw at it. [EVGA GeForce RTX 3090 Ti FTW3](https://www.evga.com/products/product.aspx?pn=24G-P5-4985-KR), yes it has RGB but that's ok, who says we can't look cool while cracking some hashes? What it also has is 25GB GDDR6X memory, and 10752 CUDA Cores, with a 1920 MHz Boost Clock and 1,008 GB/s Memory Bandwidth, so yeah just think about that. Great price and available today.

> $1149.99

## Case

Now cases are really a personal preference, and everyone has their favorite. For our build though, we want motherboard and water-cooling compatibility, for this reason going with another one of my all time favorite brands, [Phanteks ENTHOO 719](http://phanteks.com/Enthoo-719.html). This case is beautifully built and really completes this system.
At 9.45 in x 22.6 in x 23.6 inches this Full tower Chassis is a beast. This case even supports two completely independent builds, with two motherboards and two power supplies, wow.

> $219.99

## Power supply

Another item that I normally do not cheap out on is the power supply. Next to the Motherboard you're system can't run without it, and for efficiency the higher grade you go, the better. For this reason and future proofing, I selected the [EVGA SuperNOVA 1600 T2, 80+ TITANIUM 1600W](https://www.evga.com/products/product.aspx?pn=220-T2-1600-X1). Key features,

> 10 Year Warranty
>
> ECO mode, under low load the fans shut off
>
> 94% Efficiency
>
> Fully modular
>
> 100% Japanese Capacitors
>
> Standard ATX form factor size
>
> 1600W @ +50C
>
> High quality braided cables

I've been using these for years and they are super awesome. Never had one fail. I recommend buying directly from EVGA, unless locally available. This is basically the best power supply you can get, current pricing is a steal. Our estimated wattage not including the CPU or any additional drives or video cards is 689W, so you see a power supply of this size, can definitely get used up pretty quick.

> $349.99 CAD

## Case fans

In some cases you may need better fans, to be completely honest with you, the fans included in this build would more than suffice. I Will add my recommended fans, but not include them in the price as it's completely un-necessary, if you do decide to grab some fans, checkout [ML120 PRO 120mm PWM Premium Magnetic Levitation Fan](https://www.corsair.com/us/en/Categories/Products/Fans/Magnetic-Levitation-Fans/ml-pro-config/p/CO-9050040-WW).

## Summary

This is an amazing build, probably overkill for the everyday user, however for a professional developer, content creator or forensics analyst, this machine would be a good starting point. I would consider this a base model for a professional workstation in a high output lab, especially if it would be running 24/7, say processing, copying drive images, or a data recovery rig, hash cracking machine etc.

A summary on [4n6 Build](https://pcpartpicker.com/user/ryd3v/saved/YvZ3wP) does not include the CPU and motherboard, so we will add that amount manually now.

Our build cost before taxes and shipping is **$6545.48 CAD**, and that is not to bad considering the gear we have here. If you are interested in a build like this for your lab, drop me a line [Ryd3v](https://ryd3v.rocks/), I ship internationally, and provide 1 year of technical support for each system I build.

Stay tuned for a Intel variant build, for those who like to live dangerously ;)

Did you like this article? Drop me a line on Twitter, [@ryd3v](https://twitter.com/ryd3v)
