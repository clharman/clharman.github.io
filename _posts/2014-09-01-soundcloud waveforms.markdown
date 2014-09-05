---
layout: post
title:  "Soundcloud Waveforms"
date:   2014-09-01 00:00:00
categories: project update music
---

I was hoping to be able to analyze the waveform of a Soundcloud track, collected using the Soundcloud API, for visual patterns corresponding to sonic phenomena, primarily: the presence of drops in a given song.

"Cooler Than Latch" Waveform
![Alt text](/cooler-than-latch.png "'Cooler Than Latch' Waveform")

After inspecting the waveforms I concluded that there is not nearly enough information contained in the 1800 x 280 .png to make any definite statements about the nature of the song.  Here's the fiddle I used to quickly grab the waveform pic: [http://jsfiddle.net/ej2pyzce/](http://jsfiddle.net/ej2pyzce/)

No separation can be seen between curves even at full zoom.

On to the next method.  My ideas:

* Analyzing the streaming sound directly
* Accessing the locally cached sound file and performing some analysis on that
* ...