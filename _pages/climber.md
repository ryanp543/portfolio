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
---
This robot is designed to climb poles and trunks (I use "columns" as a more general term). Essentially, this robot has two grasping arms that can autonomously wrap about a column. An automated latch at the end of one arm hooks onto the end of the other arm. Each arm is made up of modular links and is driven by a single tendon string that runs through them all. The number of links per arm can be adjusted to adapt for different column diameters. To achieve self-locking on the column (meaning the robot stays on the column when all electronics are off), the center of mass is designed to be off to the side of the column via a cantilever tail, generating a moment that creates a frictional force from the wheel pressing against the climbing surface. The drive wheel is mounted on a turret that rotates to achieve both vertical climbing and rotation about the column. 

{% include gallery caption="CLIMR: Cabled Limb Interlocking Modular Robot" %}

On the electronics side of things, I have a Raspberry Pi 4B running Ubuntu and ROS 2. This talks with a Teensy 4.1 mounted on a custom PCB with motor drivers and buck converters to control the various motors and servos on the robot. Lots of modeling was done for this robot, but the development revolved around extreme rapid prototyping because many features were difficult to model for. There were some semesters and summers where I was building a brand new robot every two weeks for testing!

This work has been submitted to IEEE Robotics and Automation Letters (RA-L) in March 2025. 

# Proof of Life

This 4-minute video gives a breakdown of the robot's features and functionality. 

{% include video id="1WSQJP4kC-aXU1f2CUtThtIFyaepYN8Zy" provider="google-drive" %}

# Design Constraints and Functional Requirements

# Self Locking Body

## Design and Materials

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