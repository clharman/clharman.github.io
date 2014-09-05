---
layout: post
title:  "Programming an IMU"
date:   2014-08-15 00:00:00
categories: project update quad
---

I got the first two parts for the quadcopter: the Beaglebone Black and the AltIMU-10, or, one could say, the brain and the ears.  Why ears?  Inner ears, actually.  Obviously the Beaglebone Black (BBB) is intended as the controller, processor, brain, whatever -- what is the IMU and what does it do?

![alt text](/IMU-BBB.jpg)

IMU stands for Inertial Measurement Unit, which means that it is a collection of sensors that senses changes in its state of motion.  This IMU contains a total of 10 individual sensors: three axes of accelerometers, three axes of angular rate sensors (gyros), 3 axes of magnetometers (think 3-D compass), and a barometer (for rough altitude estimations).

Because quadcopters are inherently unstable, they must use input from an IMU to calculate the perfect motor outputs to maintain stability.  Those calculations are not trivial but before I can start writing controls algorithms I need to be able to talk to my IMU.  Because I plan on conducting the entire project in Python and then repeating it in C++, I am currently writing sensor libraries in Python.  They can be viewed in the [github repository](https://github.com/clharman/IMU-datalogger) for this project.