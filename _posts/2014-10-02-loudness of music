---
layout: post
title:  "Are drops loud?"
date:   2014-10-02 00:00:00
categories: project update dropfinder
---

In the newest episode of my never-ending quest to write a simple program to find the drop in an EDM song, I use an API, and then graph two things!


I stumbled across the [echonest remix API](http://echonest.github.io/remix/) while looking for, what else, some easy way to analyze sounds.  It's really brilliant; it is able to analyze an mp3 file and then spit out a bunch of technical information about it.  Many cool uses, like automatically remixing songs by 'beats', are linked on the API page and I suggest checking them out (although some of them don't seem to work).  Anyway, it seemed like the perfect tool to help me attain my holy grail of a trivial pursuit.  One of the examples of its use was an analysis of song build-ups, accomplished by simply graphing "loudness" as the song progressed.  The song was broken into "sections", short bits of sound in which the sound is similar, and then the maximum loudness of each section was graphed.  I decided to do nearly the same thing.  Using Python and the echonest API I wrote a short program to graph the maximum loudness of each section and starting loudness of each section against time.  The result is shown below for [Drop It Like It's Hot - Tim Gunter Remix](https://soundcloud.com/timgunter/drop-it-like-its-hot-tim-gunter-remix).
![alt text](/dropit.png)
A very blunt drop exists at 0:58, but this is nearly imperceptible on the graph and without it being pointed out it would be impossible to guess.  If you haven't guessed, the maximum loudness plot is the top one.

I did another song with a different sort of drop - [Skinny Love - Vanic Remix](https://soundcloud.com/djvanic/skinny-love-vanic) - which features a nice drop at 1:22 (0:88):
![alt text](/birdy.png)
Neither is the drop visible here.

This test being unsuccessful, I have a couple options with which to proceed:
* Consider these results inconclusive and do some filtering
* Try echonest remix tools other than sections and loudness

They are both easy, but then this whole project should be easy.  I'll try the first one and write another update with more pretty graphs.
