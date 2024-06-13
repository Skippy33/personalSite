+++
title = 'The Ender 3 Saga'
date = 2024-06-06T12:42:43-07:00
draft = false
categories = [
    "engineering",
    "3D printing",
]
tags = [
    "upgrades",
    "nerd shit",
]
+++

## So, the Ender 3

&emsp;If you're as much of a 3D printing nerd as me, you'll know the name. The Ender 3. Some say it with fear or disgust, some with respect. I'm somewhere in the middle. Should *you* get an ender 3? Hell no. I'd recommend almost anything else - an SVO6 or SVO7 is far better for not much more money.

&emsp;But there's a reason this printer is so infamous. It's the most popular 3D printer by far, and its successors continue to be quite popular. It has a dedicated modding community, and a heavily modded ender 3 [currently holds the world record for fastest speedbenchy](https://www.youtube.com/watch?v=Y199h1UaJ7U). 

&emsp;The unfortunate reason this printer is so heavily modded is that it's shit. Creality is not known for their quality control, and that started with the ender 3. Out of the box, mine came with a bent lead screw and bed more warped than a taco. It uses manual leveling with screws and knobs. The tiny 4010 fan is practically an afterthought. **BUT**, the printer was able to provide a few servicable prints before falling apart. It hooked people by showing them the possibilities of printing before showing them the dark sides of maintenance and calibration. This page is meant to serve as a cautionary tale against the ender 3, but also show what the printer was good at - teaching you, in exquisite and painful detail, *exactly* how a 3D printer works.

## The Early Years

&emsp;I don't remember much of this time or how I modded the printer since it was few years ago. All I remember was picking up the printer, naming it Monica, and setting it up one excited evening. The next day was spent leveling, trying out filament, and getting my first real print - a bracket to hold the printer's tools. I still remember the feeling, looking at a part that the printer had created seemingly from thin air. Then, an obligatory benchy for testing, and I was off to the races.

&emsp;My first large print showed me the flaws of the printer. I had first bought the printer to make anthropological models, as I am a huge fan of human evolution and wanted models of the hominins. I was never able to get really *good* large prints from the ender 3, and that was apparent pretty early on. I don't remember many details, I just remember things not going great, and a few times I considered quitting printing all together.

&emsp;I also ended up installing Octoprint at this time, which I'd highly recommend if klipper isn't your jam. It's stupid simple and only takes a Raspberry Pi. It probably saved a few SD cards and got me used to SSH and Putty, which besides just being a useful skill, is necessary for a klipper install.

## The Road to Klipper

&emsp;First, my mainboard broke. It was probably my fault, but I can't really remember. I ended up using the BTT SKR mini v3 as my replacement, and since I'd heard of klipper as the "better firmware," I thought I'd try it out. The ender 3 was the first place I really tried out klipper, and while I'm not sure it was an actual benefit over the Octoprint I'd been using, it *was* a nice testbed where I could learn about KIAUH and all the other intricacies and eccentricities of klipper. I never got input shaping on the printer, but I also never really wanted it - it's not as if I'm moving fast enough that I need it. This also got me used to the workflows and software I'd need for klipperizing future printers, as I've done for the FLSUN SR. If you like speed and modability, klipper is for you.

## Volcano Nozzle

&emsp;This, in hindsight, was a terrible idea. I'd seen in a CNC Kitchen video that you could use a volcano nozzle right in a standard V6. This is possible, and it works just as he describes in the video - the problem is, it messes up cooling and z offsets. Also, volcano nozzles only improve volumetric flow, an issue I was not having. I (mistakenly) installed a volcano nozzle on a printer that could not benefit from a volcano and only recently learned my lesson. Don't do this unless your cooling and homing setups are ready for it.

## CR-Touch

&emsp;This was a flat waste of money. The probe broke after about a month. It was a pain to calibrate. That's all I'll really say on the subject. Refer to some lower sections for what you should get instead.

## Klackender

&emsp;The [klackender](https://kevinakasam.com/klackender/) is a mostly-free automatic bed probe for the ender 3 that uses common microswitches and magnets to give your printer capabilities similar to the klicky probe found on many Vorons, Ratrigs, and other DIY printers. It's accurate and cheap, but entirely DIY. Luckily, the macros required were provided by KevinAkaSam, so you don't need to worry about the headache that can be klipper macros.

&emsp;BUT, and this is a huge BUT, it's an entirely DIY mod. There are easier ways to do this that aren't too expensive. An inductive probe like a PINDA is $5-15 on aliexpress and a pretty easy mod. Honestly, I'd probably recommend the inductive probe over the klackender for most use cases.

## Hero Me

&emsp;This is probably the first upgrade I'll completely remove from my printer. I found that the Hero Me system was bulky and didn't work all that well together. While configurable, it was configurable at the expense of anything else. The system is near-impossible to actually perform maintenance on. I also found that the direct drive mod for the Hero Me didn't work well. Soooo... yeah. Might work for others, but I had a universally bad experience with it.