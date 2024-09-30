---
title: "Sensitive Instrumented Objects"
permalink: /senseobject/
classes: wide
author_profile: false
sidebar:
  - title: "UCLA Biomechatronics Lab"
    image: /assets/images/SenseObjectIcon.png
    text: "Undergraduate Researcher"
gallery:
  - url: /assets/images/SenseObjectPicture6.jpg
    image_path: /assets/images/SenseObjectPicture6.jpg
    alt: "placeholder image 1"
    title: "Cylinder"
  - url: /assets/images/SenseObjectPicture7.jpg
    image_path: /assets/images/SenseObjectPicture7.jpg
    alt: "placeholder image 1"
    title: "Disk"
  - url: /assets/images/SenseObjectPicture8.jpg
    image_path: /assets/images/SenseObjectPicture8.jpg
    alt: "placeholder image 1"
    title: "Sphere"
  - url: /assets/images/SenseObjectPicture9.jpg
    image_path: /assets/images/SenseObjectPicture9.jpg
    alt: "placeholder image 1"
    title: "Rectangle"
gallery2:
  - url: /assets/images/SenseObjectPicture2.jpg
    image_path: /assets/images/SenseObjectPicture2.jpg
    alt: "placeholder image 1"
    title: "Cylinder guts"
  - url: /assets/images/SenseObjectPicture3.jpg
    image_path: /assets/images/SenseObjectPicture3.jpg
    alt: "placeholder image 1"
    title: "Disk guts"
  - url: /assets/images/SenseObjectPicture4_OG.jpg
    image_path: /assets/images/SenseObjectPicture4_OG.jpg
    alt: "placeholder image 1"
    title: "Sphere guts"
  - url: /assets/images/SenseObjectPicture5.jpg
    image_path: /assets/images/SenseObjectPicture5.jpg
    alt: "placeholder image 1"
    title: "Rectangle guts"
gallery3:
  - url: /assets/images/SenseObjectPicture 16.jpg
    image_path: /assets/images/SenseObjectPicture 16.jpg
    alt: "placeholder image 1"
    title: "Disassembled object"
  - url: /assets/images/SenseObjectPicture1.jpg
    image_path: /assets/images/SenseObjectPicture1.jpg
    alt: "placeholder image 1"
    title: "The hand"
  - url: /assets/images/SenseObjectPicture10.jpg
    image_path: /assets/images/SenseObjectPicture10.jpg
    alt: "placeholder image 1"
    title: "The glue"
  - url: /assets/images/SenseObjectPicture11.jpg
    image_path: /assets/images/SenseObjectPicture11.jpg
    alt: "placeholder image 1"
    title: "Inserting the sensor"
  - url: /assets/images/SenseObjectPicture12.jpg
    image_path: /assets/images/SenseObjectPicture12.jpg
    alt: "placeholder image 1"
    title: "Ribbon cables"
  - url: /assets/images/SenseObjectPicture13.jpg
    image_path: /assets/images/SenseObjectPicture13.jpg
    alt: "placeholder image 1"
    title: "The sand bin"
  - url: /assets/images/SenseObjectPicture14.jpg
    image_path: /assets/images/SenseObjectPicture14.jpg
    alt: "placeholder image 1"
    title: "Sphere surface"
  - url: /assets/images/SenseObjectPicture15.jpg
    image_path: /assets/images/SenseObjectPicture15.jpg
    alt: "placeholder image 1"
    title: "Sphere disassembled"
---

As the go-to designer and manufacturer in the UCLA Biomechatronics Lab, I assisted in the development of pressure-sensitive instrumented objects to be used for an Office of Naval Research (ONR) project. Specifically, these objects would be implemented in various experiments to study the haptic search and retrieval of mock ordnances buried within granular media. My task was to design and manufacture a sphere, box, and disk.

{% include gallery caption="The objects assembled." %}

## Sensor Implementation

Each object (including the sphere) comprised of six "tiles," or faces, that contained a well with walls angled at 45 degrees. Pressure sensors were embedded into each of these tiles, with four sensors on the walls and one or two on the flat bottom of the wells. Silicone rubber was then cast in these wells, and a vacuum chamber was used to draw the rubber mixture into the sensors. Before the elastomer completely set, a "shell" was pressed into the rubber. With each of the six shells in place, the object would take its desired three-dimensional shape. The sensors could then record a pressure distribution when a robotic gripper contacted the shell surface, albeit without high resolution. Data was sent via bluetooth signals.

{% include gallery id="gallery2" caption="The insides of the sensitive objects." %}

## Unique Geometries and Design Constraints

Each object had to fit within the 6-inch grip of the robotic gripper fastened to a Barrett Technology backdrivable manipulator. Additionally, the objects would be placed into sand, so the design had to be sealed to protect the internal electronics from granular media. Furthermore, the completed objects were covered with a modified stocking mesh. Another major factor I had to consider was electronics packaging. The physical size of the electronic components demanded more internal volume, but the external shells of the objects were constrained by the 6-inch grasp of the gripper. Especially with the shells that were curved, I designed the tiles such that they would take up as much of the space between the shell and the tile as possible without compromising structural integrity.

{% include gallery id="gallery3" caption="Assembly and use case of the sensitive objects." %}