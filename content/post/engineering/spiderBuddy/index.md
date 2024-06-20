+++
title = 'SpiderBuddy'
date = 2024-06-18T18:30:37-07:00
draft = false
categories = [
    "engineering",
    "3D printing",
    "projects",
    "WIP"
]
tags = [
    "nerd shit",
    "science fiction",
    "wearable"
]
+++

## The Inspiration

&emsp;In one name, Jorvon Moss. His wearable projects are incredible and really got my mind working on what cool things I could make for myself. In particular, his Parado-Asi and Asi bots got me thinking on what cool projects I could build that are wearable.

&emsp;I'm going to be making periodic updates to explain my design process. Hopefully this is a better system of documenting my projects.

## Pre-Design

### Eariler Projects

&emsp;I haven't made a post on it, but I have previously made a similar (though smaller) project. I made it right before school ended, and it was meant as a super simple weekend project. It was relatively simple, though I learned a lot of lessons from it.

1. Don't use levers. Just connect the legs directly to the servos.
2. Keep things mechanically simple when things are so small.
3. Just because your CAD program can make things really small doesn't mean your printer can. Avoid sub-2mm details.
4. Battery placement/wiring is deceptively difficult. PLAN AHEAD FOR IT.
5. Use Dupont connectors. Soldering everything, while effective and strong, is a pain and hard to reconfigure.
6. Leave plenty of space for wiring. Wires can take up way more space than you expect and get snagged on things. Don't fall for it.

### Requirements

&emsp;Lessons from earlier - always have clearly defined baseline and stretch goals.

Baseline goals -

- can move 4 legs
- can swivel head
- battery powered
- looks cool

Stretch goals -

- pixel array "face"
- jointed, more "articulated" arms that act more naturally
- programmed movement sequences
- maybe remote control of those sequences?

### Basic Design Decisions

1. Control each leg individually with a servo. It keeps things simple and allows more complex arm programming
2. 4 legs. It's simpler. Might aim for more in the future?
3. Replaceable battery cartridge. This is something I want to reuse on other projects, and I don't want to have to think too hard about this in the future.
4. Bilateral symmetry. It's easier to design, and I've already got other things that I can use as a model.
5. Use a AA or AAA battery pack. I'd prefer to use a USB battery pack, but can't find one that's small enough for my purposes. I don't want to use LIPOs because they're flamey, I'ma be wearing this device, and I don't know how to deal with them safely. AAs and AAAs are cheap, available, and easy to use.
6. Use a raspberry pi pico as the microcontroller because it's small and I know how to use it.

## 6/17/24

&emsp;Project start. I'm writing this the day after, as I didn't think to start writing docs when I'd just started.

&emsp;I made a circular body with mounting places for 4 9g servos, the super tiny and simple ones. I also made space for 4 legs. I'm using 4 legs and servos because I don't want to have to try and fit 6 in the body. In hindsight, I may have been able to fit them with a radially symmetrical design, but I've already got a bilateral design and don't want to redesign so radically. The body is 100mm diameter, which is a *bit* big, but I want to leave myself plenty of space for the future.

&emsp;I've split the current model into a top shell and bottom body, though I still need to design a way to fasten them together. I printed a basic model of the body, and it seems to be around the right size. I imported 3D models of the servos into the CAD file for fit testing, and it all seemed to work out.

## 6/18/24

&emsp;First big change, I made the body hexagonal. I thought it looked cooler, and it shouldn't lead to any big issues. I also added a place for another servo in the noddle so the head can swivel.

&emsp;I also started working on the head. I designed it as a relatively tall hexagon, as I need to fit the batteries and the pixel array in there. The pixel array was pretty hard to design around, as it's *barely* smaller than one face of the head. Mounting it is going to be a pain, but should be *possible*. I may need to mount it with glue (*shock horror!*), but I'll try anything I can to avoid that. 

&emsp;I designed the battery box. It's pretty simple, it just has three AA batteries in series. That provides almost exactly 5v, which is perfect for the raspberry pi pico. The box needs assembly with nickel strips and wiring, but that shouldn't be too bad, and by the end of this, I'm going to have a box design that I can use elsewhere. The thing is just going to be held in the head with two screws - simple, yet effective. I copied many aspects of the design from an old RC car.

&emsp;I also found the servo mounts in the base were too weak, so I made them much thicker and gave the servos some extra clearance.

## 6/19/24

&emsp;I got the main printer running again, so that means it's PROTOTYPE TIME!

&emsp;But first, I designed some small holes at the corners where I can use screws to fasten the top and bottom halves together. I printed this for a sanity check, and many of the aspects I wanted to check worked - it's always nice to do a sanity check. I had some issues with the corner bits, so I redesigned them to fit heat-set inserts. I spent most of the day hiking, and I'm waiting on parts, so I wasn't able to work too much on this.
