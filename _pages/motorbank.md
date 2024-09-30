---
title: "Bairclaw Robotic Hand Expansion"
permalink: /motorbank/
classes: wide
author_profile: false
sidebar:
  - title: "UCLA Biomechatronics Lab"
    image: /assets/images/MotorBankIcon.png
    text: "Undergraduate Researcher"
gallery:
  - url: /assets/images/MotorBank6b685ed4-4db9-4b18-a07e-475b54298c8c.jfif
    image_path: /assets/images/MotorBank6b685ed4-4db9-4b18-a07e-475b54298c8c.jfif
    alt: "placeholder image 1"
    title: "Assembly without strain gauges"
  - url: /assets/images/MotorBank583f2bf9-bc72-4ee4-aa26-ead637149433.jfif
    image_path: /assets/images/MotorBank583f2bf9-bc72-4ee4-aa26-ead637149433.jfif
    alt: "placeholder image 1"
    title: "No electronics"
  - url: /assets/images/MotorBankdcb2c517-995a-4c45-9bfd-dcc8397066ac.jfif
    image_path: /assets/images/MotorBankdcb2c517-995a-4c45-9bfd-dcc8397066ac.jfif
    alt: "placeholder image 1"
    title: "Where the tendon tubes go"
  - url: /assets/images/MotorBanke5f980fa-11fe-4af3-af23-c6591c790258.jfif
    image_path: /assets/images/MotorBanke5f980fa-11fe-4af3-af23-c6591c790258.jfif
    alt: "placeholder image 1"
    title: "The original bairclaw finger"
gallery2:
  - url: /assets/images/MotorBank6c8f6ce7-0673-4801-b6db-4e548f4ae156.png
    image_path: /assets/images/MotorBank6c8f6ce7-0673-4801-b6db-4e548f4ae156.png
    alt: "placeholder image 1"
    title: "Springs on the balconies"
  - url: /assets/images/MotorBankdc74d0f9-b2fd-401b-a764-362d9d60bb73.jfif
    image_path: /assets/images/MotorBankdc74d0f9-b2fd-401b-a764-362d9d60bb73.jfif
    alt: "placeholder image 1"
    title: "Baseplate"
  - url: /assets/images/MotorBank7552e5da-8258-4185-96da-bc2a82794934.jfif
    image_path: /assets/images/MotorBank7552e5da-8258-4185-96da-bc2a82794934.jfif
    alt: "placeholder image 1"
    title: "Balconies for redirecting"
  - url: /assets/images/MotorBanka21285c1-ab56-4356-9a8b-f10821957bf0.jfif
    image_path: /assets/images/MotorBanka21285c1-ab56-4356-9a8b-f10821957bf0.jfif
    alt: "placeholder image 1"
    title: "Strain gauge installation"
gallery3:
  - url: /assets/images/MotorBankad7141a9-68be-4123-9a5e-bde3ae161f6d.jfif
    image_path: /assets/images/MotorBankad7141a9-68be-4123-9a5e-bde3ae161f6d.jfif
    alt: "placeholder image 1"
    title: "Springs on the balconies"
  - url: /assets/images/MotorBankd7e2f4a6-17b2-49cc-8244-baccc65d2b0f.jfif
    image_path: /assets/images/MotorBankd7e2f4a6-17b2-49cc-8244-baccc65d2b0f.jfif
    alt: "placeholder image 1"
    title: "Baseplate"
  - url: /assets/images/MotorBank9dadd73f-ab2e-4a36-9e2e-2d4f6fb666aa.jfif
    image_path: /assets/images/MotorBank9dadd73f-ab2e-4a36-9e2e-2d4f6fb666aa.jfif
    alt: "placeholder image 1"
    title: "Balconies for redirecting"
gallery4:
  - url: /assets/images/MotorBank795613b6-6588-4f4f-b61b-aee9c1d0445a.jfif
    image_path: /assets/images/MotorBank795613b6-6588-4f4f-b61b-aee9c1d0445a.jfif
    alt: "placeholder image 1"
    title: "Redirect pulleys"
  - url: /assets/images/MotorBank7cf1ce4c-e680-40c8-9bcd-9005276dec33.jfif
    image_path: /assets/images/MotorBank7cf1ce4c-e680-40c8-9bcd-9005276dec33.jfif
    alt: "placeholder image 1"
    title: "FEA"
---

In the UCLA Biomechatronics Lab are Barrett Technology’s WAM robotic arm and  tendon-driven fingers made by the lab for a prospective robotic hand, nicknamed the “Bairclaw.” My duty was to merge these two systems together with an adapter and expand the testbed from one to three fingers by building a motor bank.

# Motor Bank

## Expanding the Bairclaw System

With three modular motor units, the motor bank was designed to accommodate 18 tendons for three fingers, which each had four degrees of freedom. Stepper motors in the bank controlled tendons. Pulleys redirected the tendons towards yellow vacuum tubes that housed six separate Teflon tubes through which the tendons individually traveled. Each pulley mount was only 1/16 inches wide, 3/8 inches long, and as small as 0.09 inches tall--a fairly tough machining challenge!

{% include gallery caption="Some assembly photos." %}

## Springs and Cantilever Beams with Strain Gauges

Springs allowed the user to pre-load the tendons to prevent their detachment from the pulleys during operation. The tabs on which half of the pulleys resided acted as cantilever beams. Their deflection during operation could be measured by strain gauges and used to determine tendon tension.

{% include gallery id="gallery2" caption="Redirecting the tendons." %}

## Modular Orientation via T-Slot Frames

The motor bank could switch between two orientations: the one on the previous page and the one here. This second orientation kept all the vacuum tubes close together, while the first shrank the motor bank footprint.

{% include gallery id="gallery3" caption="Different arrangements of the motor bank assembly." %}

# WAM Adapter

## Pulleys Redirecting Tendons

The tendons were guided from the edge to the finger holders, through the pocket of the finger holders, and then up into the fingers. It was expected that tension from the motor bank would keep the tendons on their respective pulleys.

{% include gallery id="gallery4" caption="Redirect pulleys holders." %}

## Modular Finger Holder Design

The tendons were guided into the edge pulley holders (circled green) that could translate along the edge of the baseplate to a desired position. The finger holders were screwed into the baseplate (circled blue) at any desired position. Once everything was fastened down, the threaded circular part that linked the baseplate to the WAM was screwed in (circled red).

## Merging the Bairclaw Fingers to the WAM

The Bairclaw fingers were fastened onto the finger holders via the screws at the top of the part. These finger holders could be fixed over any pair of holes on the baseplate. To attach the adapter to the WAM, a ring clamped onto the WAM wrist as it screwed onto the threads of the WAM adapter at the base (as seen in "Assembly 2" photo).