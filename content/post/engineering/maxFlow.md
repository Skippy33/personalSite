+++
title = 'Max Flow'
date = 2024-06-04T11:10:57-07:00
draft = false
categories = [
    "engineering",
    "3D printing",
]
tags = [
    "old project"
]
+++

## Max Volumetric Flow

&emsp;For me, this is one of the most important variables on the printer to maximize, as my motion system can support far faster movement than my nozzle. Unfortunately, I'm bad at maximizing this. I'll try to cover all the possible issues I've ran into with flow rate to maybe help future printer people.

### Temperature

&emsp;This is one of the easiest and fastest ways to increase speed - just bump up your temps. However, this isn't a great long-term strategy. I'm skeptical of increasing temps for PLA past ~240 degrees, as that seems to be where thermal degradataion starts to become an issue and cooling is strained. It's not *pointless*, but in my experience, you start running into dimishing returns.

### Filament Friction

&emsp;This wasn't something I realized early on, but it's obvious in hindsight - if filament is hard for your extruder to pull off the spool, your extruder won't be able to push it to the nozzle very well. This is not great for me, as I use giant 3kg spools that have a lot of intertia. Having a bowden tube for the whole filament path seems to help a ton.

### Extruder Pressure

&emsp;Again, seems obvious in hindsight - if your extruder can exert more pressure, it can push more plastic out of the hotend. For me, this means just cranking down on the tensioner spring. There are practical limits from filament grinding, but this is a surprisingly good way to fix low flow.