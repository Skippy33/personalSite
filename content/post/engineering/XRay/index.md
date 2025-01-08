+++
title = 'Kiln Project'
date = 2025-01-05T1:30:37-07:00
draft = true
categories = [
    "engineering",
    "3D printing",
    "projects",
    "metallurgy"
]
tags = [
    "X rays",
    "electronics",
    "high voltage",
    "DANGER ZONE",
    "WIP"
]
+++


## Safety Briefing

### Lead

&emsp; Lead a long-term neurotoxin and lead metal will shed lead oxide. There is no way to remove lead from your body, and it must be treated very carefully. ALWAYS handle with gloves, ALWAYS handle outside, NEVER touch your face when handling lead, and safely double-bad anything with lead to safely handle it. If you solder lead, do it OUTSIDE and use something to push lead fumes away from you. Lead has a high vapor pressure, it will evaporate easily when in liquid form. 

### High Voltage

&emsp; High voltage will kill you dead before you can react. Do Not Fuck With High Voltage, It Will Fuck With You. Refer to safety handbooks, but most importantly, just don't get near it. DC is generally safer than AC, but neither should be messed with. Only make your own power supply if you're good with electronics and know *exactly* how this works. I am not an electronics person, so I bought my power supply.

### X-Rays

&emsp; X Rays will give you cancer. Treat them with respect. Do not mess with them without adequate shielding, a radiation sensor, remote access to the power supply, and a good idea of how much radiation you'll be making. Voltage does not correspond linearly to x-ray output - 50kV will output a thousand times more x-rays than 25kV.

## The Project(s)

### X-Ray Photography

&emsp;X ray photography is undeniably cool. It's also surprisingly simple - shoot x-ray beam through object at a detector, view output. Unfortunately, it's a bit more complicated. 

&emsp;Proper x-ray photography the old-fashioned way requires a lot of gear. You need cartridges, film, and developer, none of which is easy to get or cheap. Film and developer are particularly expensive, since nobody makes it anymore. Film also has the problem that it's not very sensitive - from some internet sources, exposure times might be fifteen or more minutes. I'm not too comfortable with the x-ray beam being left on for that long, so I'd rather not.

&emsp;So instead, I'm going to try a workaround. X-ray film doesn't actually detect x-rays - it detects light emitted by an amplifier screen, which emits green or blue light in response to x-rays. Instead of using film as an intermediary for photo production, why can't I just take a photo of the amplifier? With a long exposure time, I should be able to see the patterns just fine. the photos won't be the best, and the setup might be awkward, but it should be *possible.* The point isn't to make a medical x-ray scanner, it's to show that I *can* make an x-ray photograph.

### X-Ray Crystallography

&emsp;This was what originally inspired me to work with x-rays. I realized that x-ray crystallography is a pretty old technology, so it should be possible for me to recreate. The method is relatively simple - point an x-ray beam at a crystal and look at the pattern on the other side. X-rays diffract through the crystal and make patterns that can be used to determine the crystal structure of said crystal. This is most famous as the method by which DNA's structure was found, but it's been the standard for over a hundred years. 

&emsp;I just want to show that I *can* do it. My setup won't be useful for research, but I want to show that it's possible. 

&emsp;Ultimately, this is a very similar setup to photography, but I need to use a mask to only allow x-rays that have diffracted through the crystal to hit the amplifier screen.

## The Actual Build

### The **BOX**

&emsp;When working with the x-ray tube, I wanted to make sure it's not spraying x-rays everywhere. The tube emits in a weird hollow cone pattern, but that's not terribly useful for me, and if it's pointed to me, could be dangerous. I also needed a way to angle the cone so it hits the photograph's subject head-on, rather than at an angle. So, I put the tube in a box. It's on an angled segment cut out of the box and allowed to hang, being held at a certain angle inside the box by tape. This is easily adjustable, and while crude, it provides a platform to line the box with lead. Handling lead isn't ideal - bismuth would have been less toxic, but is much more expensive. Sheet metal works for low-power x-rays, but I'd rather be future-proof in case I want or need to handle higher power x-rays. I've left a hole in the top of the box for photography, but that hole should only ever be pointed up while the x-ray is on.

### The Wiring

&emsp;I bought a CO2 laser supply for my high-voltage source. It should provide 23kV at a few mA, and that's what I'm comfortable with. I don't have the skills where I'd trust myself to make my own source, and the laser source wasn't too expensive. Oil lighting transformers might also work, but the laser supply was simple, self-contained, and cheap.

&emsp; WIP, haven't started construction