---
layout: post
title:  "First quadcopter challenges"
date:   2014-09-04 00:00:01
categories: project update quad
---

Somehow everything soldered together correctly on the first try.  Here's the flowchart I used to keep it all straight:

![alt text](/flowchart.png)

It only took me an hour or so to figure out how to control the motors using PWM.  After that I attempted some balancing exercises (balancing on two points located at opposite propellers, like a see-saw).  Using a very simple low-pass filter and proportional control the quadcopter became unstable nearly immediately.  Oscillations grew exponentially and within a second it had flipped off the table, broken a propeller, and flung nuts and washers across the room.