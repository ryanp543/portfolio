---
title: "CLIMR: Cabled Limb Interlocking Modular Robot"
permalink: /climber/
author_profile: false
sidebar:
  - title: "MIT Bioinstrumentation Lab"
    image: /assets/images/ClimberIcon.png
    text: "PhD Candidate Student"
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
gallery:
  - url: /assets/images/ClimberIMG_1175.JPG
    image_path: /assets/images/ClimberIMG_1175.JPG
    alt: "placeholder image 1"
    title: "The tree climber"
gallery2:
  - url: /assets/images/ClimberFuncReq.png
    image_path: /assets/images/ClimberFuncReq.png
    alt: "placeholder image 1"
    title: "CLIMR Functional Requirements"
gallery3:
  - url: /assets/images/ClimberDriveCrossSection-1.png
    image_path: /assets/images/ClimberDriveCrossSection-1.png
    alt: "placeholder image 1"
    title: "CLIMR drive system cross section"
  - url: /assets/images/Climber451573681_1137907953933609_3463007586565563867_n.jpg
    image_path: /assets/images/Climber451573681_1137907953933609_3463007586565563867_n.jpg
    alt: "placeholder image 1"
    title: "CLIMR wheel top down view"
---
This robot is designed to climb poles and trunks (I use "columns" as a more general term). Essentially, this robot has two grasping arms that can autonomously wrap about a column. An automated latch at the end of one arm hooks onto the end of the other arm. Each arm is made up of modular links and is driven by a single tendon string that runs through them all. The number of links per arm can be adjusted to adapt for different column diameters. To achieve self-locking on the column (meaning the robot stays on the column when all electronics are off), the center of mass is designed to be off to the side of the column via a cantilever tail, generating a moment that creates a frictional force from the wheel pressing against the climbing surface. The drive wheel is mounted on a turret that rotates to achieve both vertical climbing and rotation about the column. 

{% include gallery caption="CLIMR: Cabled Limb Interlocking Modular Robot." %}

On the electronics side of things, I have a Raspberry Pi 4B running Ubuntu and ROS 2. This talks with a Teensy 4.1 mounted on a custom PCB with motor drivers and buck converters to control the various motors and servos on the robot. Lots of modeling was done for this robot, but the development revolved around extreme rapid prototyping because many features were difficult to model for. There were some semesters and summers where I was building a brand new robot every two weeks for testing!

This work has been submitted to **IEEE Robotics and Automation Letters (RA-L)** in March 2025.

# Video Breakdown

This 4-minute video gives a breakdown of the robot's features and functionality. 

{% include video id="1WSQJP4kC-aXU1f2CUtThtIFyaepYN8Zy" provider="google-drive" %}

# Design Constraints and Functional Requirements

The general design constraints were formed from the commonly desired features found across past climbing robot research works and are tabulated below.

| Constraint | Reasons | 
|-----------|-----------|
| Low Mass | Reduce drive power consumption and overall cost | 
| Simple Build | Lower complexity generally means low risk of breakage| 
| Non-Destructive Climbing | Climbing surface typically hard to puncture, surface damage undesirable | 
| Self-Locking | Safety, can commit all power to payload |
| Automated Grasping | Removes need for human assembly before climbing |
| Adaptive to Column Diameter | Broadens variety of tasks, allows frequent climbing, limits max column diameter |

From here, a list of guiding functional requirements could be devised. While these weren't set in stone, they gave some metrics when it came to selecting things like motors, materials, and part dimensions.

{% include gallery id="gallery2" caption="CLIMR Functional Requirements." %}

Spreadsheet of functional requirements can be found here: [Download Excel Document]({{ site.baseurl }}/assets/excel/Functional Requirements and Design Constraints.xlsx)

# Self Locking Body

## Design and Materials

The main body houses the drive and turret motors. The drive motor (1) rotates a through-hole drive shaft (2), which moves the wheel (4) on the turret through a bevel gear transmission system (3). The turret itself is twisted by a brushless worm gear motor. The body is made of 3D printed PLA plastic and waterjetted 6061 aluminum components, primarily for their structural strength and relatively light weight. However, weight on the main body was not minimized, mainly because it assists in offsetting the center of mass for self-locking. Nevertheless, it was ensured that the main body was not too heavy for the drive motor. 

{% include gallery id="gallery3" caption="CLIMR Drive System Cross Section." %}

The main body is attached to a cantilever tail to offset the center of mass away from the column axis. This offset creates a moment arm, which generates a normal force on the drive wheel and a frictional force that supports the mass of the robot when all the motors are off. The drive motor has a worm gearbox, which prevents backdrivability. The end of the cantilever tail has the Raspberry Pi computer, the tendon-driving motors, the Kobalt tool battery, and mounting holes for modular weight additions if needed. 



## Kinematics and Statics Modeling

# Underactuated Tendon Driven Arms

## Design and Materials

## End Link Clutch Rollers

## The Latch

## Kinematics and Statics Modeling

# Drive Motor and Turret Motor Selection

## Drive System Breakdown

## Modeling

# Main Body Microcontroller PCB

## Design and Breakout Boards

## Feedback Controllers

# Tail Electronics

## Raspberry Pi

Ubuntu linux ROS2 nodes and code

## CANBus Commands and Packages

## Remote and Manual E-Stops


{% include video id="1v9oS6sE4rDcAeWOoxOasQBHs3BesEweo" provider="google-drive" %}
{% include video id="1HtABnQpHiPgBNZxBrSGnRcrOLGhLZYDp" provider="google-drive" %}
{% include video id="1hgglDvoinb6c50ODsUlSWKkqUdGROMxw" provider="google-drive" %}
{% include video id="1YVuWXlhMFWJfs8xfQFiyXE3O3xXGz4Ht" provider="google-drive" %}