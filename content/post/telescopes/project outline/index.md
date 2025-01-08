+++
title = 'Telescope Project Outline'
date = 2024-10-15T11:30:37-07:00
draft = true
categories = [
    "engineering",
    "3D printing",
    "projects",
    "telescopes"
]
tags = [
    "telescope",
    "electronics",
    "WIP"
]
+++

## The Long Shot

&emsp;(Written november 2024)

&emsp;I've had this idea for a while, but it ultimately got started with [this](https://astrodennis.com/Guide.pdf) document: NASA's "A Practical Guide to Exoplanet Observing," made for hobbyists who want to spot exoplanets. I hadn't thought it was possible, but once I knew it was, I had to do it. It's *exoplanets*. This wasn't anywhere close to possible twenty years ago.

&emsp;So, my "long shot" is to spot an exoplanet. Problem is, I am going into this knowing nothing about how astronomy works. I can't jump straight to spotting the exoplanet, that's just a recipe for burnout and wasted money. I have to build my way up, so I'm documenting my project outline here as I work on it.

## Step 1: Hadley

&emsp;I need to walk before I run. I also have a very low budget, so I need something to get into the hobby first. The [Hadley telescope](https://www.printables.com/model/224383-astronomical-telescope-hadley-an-easy-assembly-hig) seems to be a good bet. It's relatively cheap, 3D printable, and looks like there's good community support. It should be a good way of learning the ropes before I aim higher.

### Update 1: Hadley 11-15-24

&emsp;I've ordered all the optics parts online, got gcodes for all the parts I need, and am just waiting for a few more amazon orders. I've started 
modeling a simple mount as well, something that will work for hadley and be near the scale I'll need for any larger telescopes. I'm modeling on the 
assumption that I'll be able to laser cut all the parts from 8mm acrylic. I'm also modeling it so that there are gears I'll be able to use to accurately 
position the telescope. I'm not motorizing the gears, but that's the long-term plan for the big scope.

&emsp;I'm laser cutting the parts because large acrylic sheets are cheap and laser cutting is far more accurate than 3D printing. For a system so 
sensitive to small changes, that accuracy is going to be important. I'm using acrylic over wood because it's more stable to temperature and humidity. 

### Update 2: Hadley 12-3-24

&emsp;I got the optics parts pretty easy, no real problems. I chose to make the mount out of plywood, as it's much cheaper and should be rigid enough. 
The larger telescope's mount should be made of carbon fiber or acrylic though, this wooden mount is barely suitable.

&emsp;I printed all the parts I needed, and basic assembly is done. The first day using the telescope wasn't very productive - I destroyed the small 
altitude gear. The telescope was too top-heavy and was trying to lean forward, applying torque on a tiny plywood gear. It got destroyed in short notice. 
For a counterweight, I just zip-tied a water bottle onto the end of the telescope. It *works*, though I'll need to find some metal scrap and print a 
proper replacement.

&emsp;Collimation and focusing has had a learning curve. The documentation isn't bad, but it's hard to get things *just right*. I think I'll print 
a bahtinov mask to help with focusing. I was able to lock onto Jupiter last night, but the view was very blurry, and I think focusing is the #1 culprit.

&emsp;Next plans are probably to use the telescope and learn it intuitively. I also want to figure out some of the astrophotography basics, so I'll just 
use my phone to take some photos. Some new optics might also be in order, like a zoom eyepiece. 

### Update 2: Hadley 12-6-24

&emsp;I've been messing around with the telescope for a bit, learning a lot about the issues with my mount design.

1. There isn't enough clearance for me to point the telescope straight up.
2. There was little thought put into ergonomics, adjusting the scope while observing can be annoying.
3. There was no thought put into counterbalancing, and all my solutions have been lacking.

&emsp;However, I've also been making incremental improvements. I changed the driving gears so I have much finer control over the direction of the telescope. I've designed phone mounts that should allow me to use the website [astrohopper](https://artyom-beilis.github.io/astrohopper.html) to properly aim the telescope, though I haven't had the time to print them properly. I've had decent observations of jupiter, and a tantalizing observation of the Horsehead nebula, but I wasn't able to properly aim and focus the telescope while the nebula was in my FOV, so all I saw was a vaguely horse-shaped blob. 
&emsp;I've been learning a lot about the basic operation of a telescope, however. I think I'll try my hand at a motorized mount soon, maybe after winter break. I've ordered a zoom lens that should be much more convenient. 

### Lessons for the future telescope

&emsp;Accuracy is going to be *hard*. The NASA guide says that reliability up to a few arcseconds is heavily preferred. Rigidity is also king - I'll need 
to take long exposures, and if there's any bump, it'll ruin the exposure. 