---
layout: post
title:  "Quadcopter time?"
date:   2014-08-01 00:00:00
categories: project update quad
---

I have decided to build a quadcopter.


Why?  I want to practice my controls theory and filtering as well as create a platform for autonomous flight.  I'm buying a kit for the hardware -- frame, motors, battery, motor controllers -- but will be using my own selection of parts for the control system.  The setup:

* [Quadcopter Combo Kit ARF](http://www.hobbyking.com/hobbyking/store/__52863__HobbyKing_Spec_FPV250_V2_Quad_Copter_ARF_Combo_Kit_Mini_Sized_FPV_Multi_Rotor_ARF_.html): very basic but well priced
* [Beaglebone Black](http://www.newark.com/beagle-bone-accessories): powerful, linux-running processor small enough to fit on the quadcopter and flexible enough to accomodate countless other projects
* [BBB Prototyping Cape](http://www.adafruit.com/products/572): this board securely plugs into the Beaglebone's output pins and allows soldered connections, a must for a soon-to-be flying object
* [Battery Monitor](http://www.hobbyking.com/hobbyking/store/__7223__Hobby_King_Battery_Monitor_3S.html): tiny, crappy, cheap bit of circuitry that beeps when the battery gets low (Lithium Polymer batteries can be damaged if their voltage drops too low)
* [UBEC](http://www.hobbyking.com/hobbyking/store/__4319__TURNIGY_3A_UBEC_w_Noise_Reduction.html): Transforms the Li-Po battery's 11.1V output to 5V to power the Beaglebone
* [AltIMU-10](http://www.pololu.com/product/2469): This IMU from Pololu contains 3-axis accelerometers, 3-axis angular rate sensors, 3-axis magnetometer (compass), and a barometer.  Communicates using I2C.  This will provide the inputs to the control algorithm


This should be pretty much everything I need, wires and fastening excluded.  I'll take care of those with "stuff laying around."