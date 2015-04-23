---
layout: post
title:  "Modeling a Water Bottle Rocket"
date:   2015-04-23 00:00:00
categories: 
---

![alt text](/rocket.jpg)
For my senior lab class I was tasked with modeling the behavior of a water-bottle rocket.  I did this by creating a mathematical model of the rocket and then solving it using a MATLAB ODE (ordinary differential eqution) solver.  Most of the equations used in the model are based on Newton's second law or the unsteady Bernoulli equation.  In the end it turned out to be between a 4 and 5 degree of freedom model.  The basic set of equations that I derived is shown below.
![alt text](/equations.PNG)

Many more equations were used, but this set describes the motion of the rocket in its most basic form.  Below is example of how several of the model's parameters change during a simulation.
![alt text](/4040.jpg)

To make the model predict how my particular rocket will behave, I characterized it by taking measurements (for the simple parameters) and conducting experiments (for the more complicated parameters).  For example, to determine the rocket's moment of inertia about its long axis, I devised an experiment where it was hung from a support structre and swung like a pendulum.  By measuring the frequency of oscillation and knowing the inertia of the support structure I was able to calculate the rocket's moment of inertia with the parallel axis theorem.
![alt text](/inertia.jpg) 

If you are wondering what the variables in the equations are or want to know how the equations were derived, check out the [full report](clharman_Sect3_Lab4.pdf).  If you want to simulate a rocket for yourself in MATLAB, download the programs from the [github repository](https://github.com/clharman/rocket-ode).