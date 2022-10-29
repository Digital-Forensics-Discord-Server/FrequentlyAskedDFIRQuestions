Intel Launches 13th Gen Intel Core Processor Family Sept. 27, 2022 and with that I decided to update my workstation built to reflect the new processors. The new 13th Gen Intel Core family includes six new unlocked desktop processors with up to 24 cores and 32 threads and clock speeds up to 5.8 GHz. For this build since we used a ThreadRipper from AMD the last time, I think this time we will use the best Intel CPU. Since I have previously covered the design methodology, in this post we will focus just on the parts and specs.

## Schema

> 1. Motherboard
> 2. CPU
> 3. CPU Cooler
> 4. Memory
> 5. Storage
> 6. Video Card(s) [Skipped availability?]
> 7. Case
> 8. Power Supply
> 9. Case Fan(s) [Skipped]

## Motherboard

I tend to stick with a few brands, that over the years have served me and my clients very well. Usually I go with [Asus](https://www.asus.com/ca-en/Motherboards-Components/Motherboards/All-series/), or [Gigabyte](https://www.gigabyte.com/Motherboard). MSI boards are also decent, just in my experience I've had more issues with them in the past, I would't hesitate to use a quality MSI board though.

Since this is a forensics machine designed for a lab environment and not for gaming, I would go with a **workstation** specific board, however availability of workstation specific boards are limited, I'll go with something slightly cheaper that fits my criteria, DDR5 with Gen 13 support. Feel free to swap this motherboard for any other board that works best for you.

For this build [GIGABYTE Z790 AERO G LGA 1700 Intel Z790 ATX Motherboard with DDR5 ](https://www.gigabyte.com/Motherboard/Z790-AERO-G-rev-10#kf)

What makes this motherboard stand out?

- LGA1700 socket: Support for the 13th and 12th Generation Intel, Intel Z790 Express Chipset
- 4 x DDR5 DIMM sockets supporting up to 128 GB
- 1 x USB Type-C port, supporting USB 3.2 Gen 2 and DisplayPort video
- Intel 2.5GbE LAN chip, Intel Wi-Fi 6E
- PCIe 5.0 M.2 Storage x5
- 4 x SATA 6Gb/s connectors
- 1 x Trusted Platform Module header
- Support for ECC Un-buffered DIMM
- Support for Windows 11 64-bit
- Support for Q-Flash Plus

This motherboard is available on Newegg.

Buy [GIGABYTE Z790 AERO G](https://www.newegg.ca/p/N82E16813145416?Item=N82E16813145416)

`$409.99 CAD`

## CPU

13th Gen Raptor Lake, Intel Core i9-13900K. The new King of Intel chips. [Intel Core™ i9-13900K Processor](https://www.intel.ca/content/www/ca/en/products/sku/230496/intel-core-i913900k-processor-36m-cache-up-to-5-80-ghz/specifications.html)

- CPU Cores 24, 32 Threads
- TDP 280W
- Base Clock: 2.20GHz, up to 5.8GHz
- PCIe 5.0 and 4.0
- DDR5 up to 5600MHz

Availible on Newegg at the time of writing [Intel Core i9-13900K](https://www.newegg.ca/intel-core-i9-13900k-core-i9-13th-gen/p/N82E16819118412)

`$809.99 CAD`

## Water cooling

I have always built my PC's with water-cooling, more specifically an AIO, "AiO" stands for "All in One", which means that you'll get a complete package, consisting of radiator, fan, pump, tubes and cooling unit, which reliably cools your CPU, and keeps your workspace quiet. Unless the client want's a custom loop, usually though for simplicity, I go with an AIO.

For our build since the CPU is absolutely "insane", I chose the [CORSAIR iCUE H150i RGB ELITE Liquid CPU Cooler](https://www.corsair.com/us/en/Categories/Products/Liquid-Cooling/iCUE-RGB-ELITE-Liquid-CPU-Cooler/p/CW-9060060-WW).

- Zero RPM and Variable Pump Speed
- Low Noise
- optimized copper cold plate and pre-applied thermal compound
- Noise Level 10 - 31.5 dBa
- 360mm Rad size
- 5-Year Warranty

Newegg [CORSAIR CW-9060060-WW](https://www.newegg.ca/corsair-liquid-cooling-system/p/N82E16835181319?Item=N82E16835181319)
`$89.99 CAD`

## Memory

This motherboard supports DDR5 memory, and although it does support [ECC memory](https://en.wikipedia.org/wiki/ECC_memory), I will be using standard DDR5. For our build, I'll stay with in the spec speed, but feel free to grab ram at a higher clock if overclocking is your thing, and your budget allows. For our build I decided on [DOMINATOR® PLATINUM RGB 128GB (4 x 32GB) DDR4 DRAM 3200MHz C16 Memory Kit](https://www.corsair.com/ca/en/Categories/Products/Memory/DOMINATOR-PLATINUM-RGB/p/CMT128GX4M4E3200C16).

Newegg [CORSAIR Dominator Platinum RGB 128GB](https://www.newegg.ca/corsair-128gb-288-pin-ddr4-sdram/p/N82E16820236661)

`$727.99 CAD`

## Storage

For my host OS I always go with a fast booting, high I/O NVME SSD, and since we saved a bit on the motherboard, I'm going to splurge a bit on a good fast boot drive. The [WD_BLACK SN850X NVMe™ SSD](https://www.westerndigital.com/en-ca/products/internal-drives/wd-black-sn850x-nvme-ssd#WDS100T2XHE) is my choice this time around. Sequential Read Performance 7300MB/s, what else is there to say lol. It's fast.

Newegg [WD_BLACK SN850X NVMe M.2 2280 1TB](https://www.newegg.ca/western-digital-1tb-black-sn850x-nvme/p/N82E16820250245)

`$204.99 CAD`

Additional drives, I usually advise on an additional SSD for Virtual machines or games, software etc. So for a secondary drive I usually name _Data_, I'll select [SAMSUNG 870 EVO Series 2.5" 2TB](https://www.newegg.ca/samsung-2tb-870-evo-series/p/N82E16820147794?Item=N82E16820147794), good amount of space for virtual machines, V-NAND with 560MB/s Seq. Write. Excellent.

`$239.99`

For the final drive, I like to have a good solid backup drive, and while this is optional you want backups. I like backups, the more the merrier. Last time we chose a 4TB drive, but for this build For my backup drive, I went with [WD Red Plus 8TB CMR NAS Hard Drive](https://www.newegg.ca/red-plus-wd80efzz-8tb/p/N82E16822234504)

`$209.99`

## Video Card

For some builds a video card may not be required, however a forensic examiner will likely need to crack some hashes, at the time of writing a 40 series Nvidia card availability is low, so for the sake of brevity choose the best card you can get that fits within your budget.

## Case

For our last build the case we choose really fit the build, but since this time a more workstation, industrial build is what I'm going for, and since our CPU/mobo combo won't be upgraded for a few years, and also there is a good chance you will eventually put a 40 series card, I decided to go with the [CORSAIR 7000D AIRFLOW Full-Tower ATX](https://www.newegg.ca/p/N82E16811139169). It is a little more expensive than our last build, and notability larger, but I think the added airflow will help in this build. This is a beautiful case coming in at 23" tall and 21" long, almost 10" thick. Chonk.

`$339.99`

## Power supply

Another item that I normally do not cheap out on is the power supply. Next to the Motherboard your system can't run without it, and for efficiency the higher grade you go, the better. For this reason and future proofing, I selected the [EVGA SuperNOVA 1000 T2](https://www.newegg.ca/evga-220-t2-1000-x1-1000w/p/N82E16817438065?Item=N82E16817438065)

`$449.99 CAD`

## Summary

`$3,482.91`

This build is awesome. Future proof, great chip. I wanted to mention, in all my builds you can freely choose another part or brand depending on your preference. See a better motherboard? No problem, drop me a line on Twitter, let me know if you like this build. Twitter, [@ryd3v](https://twitter.com/ryd3v)
