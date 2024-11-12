---
title: "Modular Climbing Robot"
permalink: /climber/
classes: wide
author_profile: false
sidebar:
  - title: "MIT Bioinstrumentation Lab"
    image: /assets/images/ClimberIcon.png
    text: "PhD Candidate Student"
---
# Coming soon!

In the process of finishing the build. Still working on publishing a paper on it, hence the lack of content on this page. Happy to talk more about the robot in person, though! I have some cool videos of it working. 

This robot is designed to climb poles and trunks (I use "columns" as a more general term). Essentially, this robot has two grasping arms that can autonomously wrap about a column. An automated latch at the end of one arm hooks onto the end of the other arm. Each arm is made up of modular links and is driven by a single tendon string that runs through them all. The number of links per arm can be adjusted to adapt for different column diameters. To achieve self-locking on the column (meaning the robot stays on the column when all electronics are off), the center of mass is designed to be off to the side of the column via a cantilever tail, generating a moment that creates a frictional force from the wheel pressing against the climbing surface. The drive wheel is mounted on a turret that rotates to achieve both vertical climbing and rotation about the column. On the electronics side of things, I have a Raspberry Pi 4B running Ubuntu and ROS 2. This talks with a Teensy 4.1 mounted on a custom PCB with motor drivers and buck converters to control the various motors and servos on the robot. Lots of modeling was done for this robot, but the development revolved around extreme rapid prototyping because many features were difficult to model for. There were some semesters and summers where I was building a brand new robot every two weeks for testing!