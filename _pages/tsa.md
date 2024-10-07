---
title: "Twisted-Winching Hybrid String Actuator"
permalink: /tsa/
classes: wide
author_profile: false
sidebar:
  - title: "MIT Bioinstrumentation Lab"
    image: /assets/images/TwistWinchIcon.png
    text: "PhD Candidate Student"
gallery:
  - url: /assets/images/TwistWinch1.png
    image_path: /assets/images/TwistWinch1.png
    alt: "Render of actuator"
    title: "Swappable tabletops"
  - url: /assets/images/TwistWinchActuatorLabeled-1.png
    image_path: /assets/images/TwistWinchActuatorLabeled-1.png
    alt: "placeholder image 1"
    title: "Labeled actuator"
gallery2:
  - url: /assets/images/TwistWinchCrossSection-1.png
    image_path: /assets/images/TwistWinchCrossSection-1.png
    alt: "Render of actuator"
    title: "labeled cross section of setup"
  - url: /assets/images/TwistWinchExperimentalSetupStepperCompressed.jpg
    image_path: /assets/images/TwistWinchExperimentalSetupStepperCompressed.jpg
    alt: "placeholder image 1"
    title: "Experimental setup with steppers for displacement/velocity"
  - url: /assets/images/TwistWinchExperimentalSetupBrushed.jpg
    image_path: /assets/images/TwistWinchExperimentalSetupBrushed.jpg
    alt: "placeholder image 1"
    title: "Experimental setup with brushed motors for force measurements"
gallery3:
  - url: /assets/images/TwistWinchDisplacementMultiple2.png
    image_path: /assets/images/TwistWinchDisplacementMultiple2.png
    alt: "Render of actuator"
    title: "Multiple winch-twist cycles"
  - url: /assets/images/TwistWinchDisplacementZoomedIn.png
    image_path: /assets/images/TwistWinchDisplacementZoomedIn.png
    alt: "placeholder image 1"
    title: "Single winch twist cycle"
  - url: /assets/images/TwistWinchVelocityTwist.png
    image_path: /assets/images/TwistWinchVelocityTwist.png
    alt: "Render of actuator"
    title: "Velocity from pure twisting"
  - url: /assets/images/TwistWinchWinchVel.png
    image_path: /assets/images/TwistWinchWinchVel.png
    alt: "placeholder image 1"
    title: "Single winch twist cycle"
gallery4:
  - url: /assets/images/TwistWinchForceTwist.png
    image_path: /assets/images/TwistWinchForceTwist.png
    alt: "Render of actuator"
    title: "Force output of twist"
  - url: /assets/images/TwistWinchForceWinchSmooth.png
    image_path: /assets/images/TwistWinchForceWinchSmooth.png
    alt: "placeholder image 1"
    title: "Force output of winch"
---
This project stemmed out of a problem I encountered during the development of my climbing robot. Essentially, I had a hook latch mechanism where I needed an actuator with a long initial linear stroke followed by a high force action. One of my labmates (thanks Vineet!) suggested a twisted string actuator, which seemed perfect. When I was testing my robot, I would tie together the arms with some cord, stick a screw into the cord, and then twist to tighten the arms closer. However, the issue with twisted string actuators is that they tend to have low stroke despite the high force output. Hence came the "brilliant" idea: combining a winch with a twisted string actuator.

We scraped the internet to see if anyone had published or made something like this before. The patent lawyers couldn't find anything similar during their prior art search. So, we jumped at the opportunity. At the core of our idea is any mechanism that allows a winch to rotate about both its cylindrical and radial axes. Fortunately, I had the mechanism already in use on my climbing robot.

Our first paper submitted to ICRA:

[Download PDF]({{ site.baseurl }}/assets/pdf/A_Novel_Twisted_Winching_String_Actuator_for_Robotic_Applications__Design_and_Validation.pdf)

Patent pending: U.S. Patent Application No. 63/694,401

## Design Description

{% include gallery caption="The actuator twisting and winching actions." %}

## Experimental Setups

{% include gallery id="gallery2" caption="Experimental setup for testing actuator." %}

## Displacement and Velocity

{% include gallery id="gallery3" caption="Displacement and velocity experimental results." %}

## Force Output

{% include gallery id="gallery4" caption="Force output experimental results." %}