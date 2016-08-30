---
layout: post
title:  "Audio Output Selector"
date:   2009-10-11 12:00:00
categories: ['blog']
bigimg: '/img/audio_output_selector.jpg'
---
Using my headphones with my computer is frustrating.  Whenever I want to use my headphones, I have to move my computer so I can access the back panel, unplug my computer speakers, and plug-in my headphones.  Okay, maybe it isn’t that difficult, but it should be easier.  How about a device that allows you to select between headphones or computer speakers?

## Solution

After some careful thought, I realized such a device could be implemented using three 3.5mm jacks and one dual-pole dual-throw (DPDT) switch (see the schematic below).

![audio output selector schematic](/img/audio_output_selector_schematic.png)

As you can see, the DPDT switch simply selects whether the input is connected to the headphones or the computer speakers.

## Other Possibilities

A similar device can be implemented using two dual-pole single-throw (DPST) switches.  This would allow the user to select headphones, computer speakers, or both.  A much more sophisticated implementation might include operational amplifiers allowing the user to adjust the gain on each output.
