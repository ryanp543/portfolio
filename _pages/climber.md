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
  - url: /assets/images/ClimberSelfLockingPics-1.png
    image_path: /assets/images/ClimberSelfLockingPics-1.png
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
gallery4:
  - url: /assets/images/ClimberSelfLockingCOMDiagram.png
    image_path: /assets/images/ClimberSelfLockingCOMDiagram.png
    alt: "placeholder image 1"
    title: "Line diagram"
gallery5:
  - url: /assets/images/ClimberLinkAssembly-1.png
    image_path: /assets/images/ClimberLinkAssembly-1.png
    alt: "placeholder image 1"
    title: "Modular link assembly"
  - url: /assets/images/Climber473333034_28132523703061865_1868369504961547215_n (1).jpg
    image_path: /assets/images/Climber473333034_28132523703061865_1868369504961547215_n (1).jpg
    alt: "placeholder image 1"
    title: "Modular link"  
gallery6:
  - url: /assets/images/Climber482479309_1566441444020475_908920091449129282_n.jpg
    image_path: /assets/images/Climber482479309_1566441444020475_908920091449129282_n.jpg
    alt: "placeholder image 1"
    title: "End link roller"
  - url: /assets/images/Climber456274052_8890150284335385_1481794253590260374_n.jpg
    image_path: /assets/images/Climber456274052_8890150284335385_1481794253590260374_n.jpg
    alt: "placeholder image 1"
    title: "End link servo"  
  - url: /assets/images/Climber481593232_1303847770902018_6268652223769221977_n.jpg
    image_path: /assets/images/Climber481593232_1303847770902018_6268652223769221977_n.jpg
    alt: "placeholder image 1"
    title: "End link roller latch side"
  - url: /assets/images/Climber481927257_991245856279180_745589058561134465_n.jpg
    image_path: /assets/images/Climber481927257_991245856279180_745589058561134465_n.jpg
    alt: "placeholder image 1"
    title: "End link servo latch side"  
gallery7:
  - url: /assets/images/Climberrollercross.png
    image_path: /assets/images/Climberrollercross.png
    alt: "placeholder image 1"
    title: "End link roller cross section"
gallery8:
  - url: /assets/images/Climber482340634_1190037402690547_4233205666734714003_n.jpg
    image_path: /assets/images/Climber482340634_1190037402690547_4233205666734714003_n.jpg
    alt: "placeholder image 1"
    title: "The latch and compound pulley system"
  - url: /assets/images/Climber462536978_1282907199544871_7110130987847451592_n.jpg
    image_path: /assets/images/Climber462536978_1282907199544871_7110130987847451592_n.jpg
    alt: "placeholder image 1"
    title: "Pulley close up"  
  - url: /assets/images/Climber459996903_467435282985741_4716885768589179217_n.jpg
    image_path: /assets/images/Climber459996903_467435282985741_4716885768589179217_n.jpg
    alt: "placeholder image 1"
    title: "Latch actuation"    
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

{% include gallery id="gallery2" caption="CLIMR functional requirements." %}

Spreadsheet of functional requirements can be found here: [Download Excel Document]({{ site.baseurl }}/assets/excel/Functional Requirements and Design Constraints.xlsx)

# Self Locking Body

## Design and Materials

The main body houses the drive and turret motors. The drive motor (1) rotates a through-hole drive shaft (2), which moves the wheel (4) on the turret through a bevel gear transmission system (3). The turret itself is twisted by a brushless worm gear motor. The body is made of 3D printed PLA plastic and waterjetted 6061 aluminum components, primarily for their structural strength and relatively light weight. However, weight on the main body was not minimized, mainly because it assists in offsetting the center of mass for self-locking. Nevertheless, it was ensured that the main body was not too heavy for the drive motor. 

{% include gallery id="gallery3" caption="CLIMR drive system cross section." %}

The main body is attached to a cantilever tail to offset the center of mass away from the column axis. This offset creates a moment arm, which generates a normal force on the drive wheel and a frictional force that supports the mass of the robot when all the motors are off. The drive motor has a worm gearbox, which prevents backdrivability. The end of the cantilever tail has the Raspberry Pi computer, the tendon-driving motors, the Kobalt tool battery, and mounting holes for modular weight additions if needed. 

## Kinematics and Statics Modeling

Finding the condition for self-locking depended on the force balance equation in the vertical direction and the moment balance equation about the wheel's column contact point. This condition tells us the necessary distance between the center of mass and the column axis. On the actual robot, the center of mass can be shifted on the body using the modular tail weights and the arm link modules. It should be noted that solving for this condition is significantly easier if it is assumed that the ball transfer bearings do not have any friction (which isn't true in reality). Because the distribution of force along the arms is nonuniform, the force and moment balance equations become incredibly complicated if ball transfer bearing friction is considered to be nontrivial. 

{% include gallery id="gallery4" caption="Line diagram used to find the self-locking condition." %}

# Underactuated Tendon Driven Arms

## Design and Materials

The grasping arms were made of modular links with a single ultra high molecular weight polyethylene (UHMWPE) tendon going through all of them. This was done to minimize the mass of the modular units, as the maximum climbable column diameter was dependent on the number of links that could be added and the maximum torque of the drive motor. Furthermore, the tendon-driving worm gear motors could be placed on the tail to facilitate self-locking. To add links, first the rotation pin and retaining screws are inserted (1-3), followed by the electrical connection (4) and the antagonist spring (5). 

{% include gallery id="gallery5" caption="Modular link assembly." %}

Each link is connected by a rotating pin joint. To enhance stability and improve contact with the column, each link is equipped with two steel ball transfer bearings. These bearings reduce sliding friction that could impede climbing forces, with at least two ball transfers per link necessary to ensure that the link maintains its proper orientation when the tendon tightens during grasping. The tendon is routed through each link using small idler pulleys, which help minimize friction along the tendon path. The arrangement of the pulleys facilitates sequential bending, ensuring that each link only bends once the preceding one has fully bent. The end links are secured with serrated flanged screws to anchor the tendons in place.

## End Link Clutch Rollers

The end links were designed differently than the standard modular linkages. Because the normal force experienced by these links would be the greatest due to the moment created by the cantilever tail, links with standard ball transfer bearing contacts would experience excessive amounts of friction that would inhibit climbing. As a result, these end links has unidirectional clutch roller bearings mounted on rotational stages actuated by high power 12V brushless servos. 

{% include gallery id="gallery6" caption="End link clutch roller bearings and servos." %}

These clutch roller bearings assisted with self-locking due to their unidirectional nature while still producing low rolling friction despite the high normal forces. Mounting them was non-trivial, however, to ensure that there was minimal friction. In general, roller bearings do not support any loads in the axial direction, but they had to be constrained in the axial direction for this robot. To do so, the clutch bearings were mounted on a custom set screw shaft collar and D-shaft with a spacer and flange bearing at each end to both constrain the clutch bearing axially while also minimizing friction in case it slid to far to either side. 

{% include gallery id="gallery7" caption="End link clutch roller bearing mount cross section." %}

## The Latch

The tendons that pass through the arm do not generate enough torque at the joints to provide secure grasping around a column. Hence, an automated latch is attached to one end link. It is designed to hook onto a pin on the opposite end link, pulling the arms together for a more secure grasp before climbing. This latch consists of both a rotary joint and a prismatic joint. Once the arm links are fully in contact with the column, continued tension on the tendon causes the latch to rotate around its rotary joint until it aligns with the pin on the opposite end link. A 15 mm micro worm gear motor then pulls the latch along the linear shafts using a compound pulley system until the latch hooks onto the pin. A constant force spring provides the restoring force.



## Kinematics and Statics Modeling

# Drive Motor and Turret Motor Selection

## Modeling

Mention balance between climbing and self locking

# Main Body Microcontroller PCB

## Design and Breakout Boards

## Feedback Controllers

# Tail Electronics

## Raspberry Pi

Ubuntu linux ROS2 nodes and code

## CANBus Commands and Packages

## Remote and Manual E-Stops
