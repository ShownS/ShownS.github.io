---
layout: single
author_profile: true
title: "Mechatronics and Integrated Prototyping"
permalink: /projects/mechatronics/
---

This section highlights projects that bring together mechanical design, sensing, electronics, controls, and software into working mechatronic systems. Across these projects, I worked on prototypes that required more than individual subsystems working on their own. The mechanical layout, wiring, code, user interface, and testing procedures all had to integrate with each other. These experiences reflect my interest in multidisciplinary engineering work, system integration, and learning how design choices affect the behavior of a full system.

## Mobility Scooter Automation

This project began as a class project and later transferred into research work through Oregon State University’s Robotics Lab. A student had approached the lab asking for help automating his mobility scooter so it could move between the docking point on his vehicle and the driver’s seat. The goal was to help him continue his hobby of drag racing with less reliance on another person to move the scooter into and out of position.

<img src="{{ '/assets/images/Scooter.jpg' | relative_url }}" alt="Mobility scooter automation prototype in the robotics lab" class="project-image">
*Mobility scooter prototype during integration and testing.*

The project was handed off to a group of five robotics students, including myself, to build a remote-controlled prototype that the lab could later refine with additional autonomous features. My main responsibility was the distance-sensing subsystem, along with assisting in integration and control-code debugging. I started by sourcing ultrasonic distance sensors and designing 3D printed mounting bracketry. I then built wiring for the system, wrote Python code for use on a Raspberry Pi, and ran tests to revise the subsystem during integration.

The final prototype combined sensors, actuators, and control code so the scooter could be controlled remotely while giving the user information about the scooter’s surroundings. This project strengthened my interest in mechatronics because it required mechanical design, electronics, software, testing, and communication to work together in a physical system. It also gave me experience with early-stage product development, where the goal is not only to make a prototype function, but to understand how each subsystem affects the usability of the full design.


## Sumobot Design and Programming

For my undergraduate capstone at Oregon State University, I worked with a team of two other students to develop a Sumobot for a Winter Showcase competition. My interest in this project stemmed from my growing interest in controls, integration, and mechanical design. The Sumobot competition required us to design, iterate, and complete a functional remote-controlled robot for a tournament. The process began with concept generation, subsystem mock-ups, and market research before moving into design, testing, and refinement.

My main role was leading the controls, electronics, and overall integration of the robot system. I also assisted with smaller tasks such as parts selection and subsystem design. I initially used readily available electronics to make a prototype drivetrain before moving into final component selection and assembly. The main components were four DC motors, a servo, and an ESP32. Additional smaller electronics, such as buck converters, were also used. I wrote the control code in Arduino IDE using Bluetooth communication and a common controller interface, so the system was easy to operate remotely during competition. I also used aspects of my materials science background to select chassis materials and strengthen 3D printed ABS parts with acetone vapor smoothing.

<img src="{{ '/assets/images/Sumobot.jpg' | relative_url }}" alt="Sumobot prototype and controller" class="project-image">
*Remote-controlled Sumobot prototype developed for OSU’s Winter Showcase.*

The final robot earned second place in the tournament based on both match wins and points. The project served as a useful transition to my graduate work because it strengthened my skills in mechanical design, mechatronics, and system integration while giving me hands-on experience with the challenges of building and refining a robotic system.

## PiCar / Robot Arm Projects

These projects were completed alongside each other as a way to get more experience with system control, mechatronic assembly, and common robotics platforms. Both systems came from kits, but still required changes to the existing code and setup to complete more advanced tasks. For the PiCar, I modified the control code so the car could be driven remotely, stream video to a laptop, follow lines with grayscale sensors, use camera-based navigation, and respond to obstacles. I also added Ackermann-style steering behavior in software, which improved drivability even though traction was still a limitation on some surfaces.

<img src="{{ '/assets/images/PiCar.jpg' | relative_url }}" alt="PiCar robotics kit used for control and navigation testing" class="project-image">
*PiCar platform used for control, navigation, and remote streaming experiments.*

The robot arm project focused more on object detection and motion routines. The arm used a camera to detect a colored block, load it into a basket, grab the basket, throw the block, and place the basket back on its rest. The most useful part of this project was learning how much the physical setup can affect whether the code works well. The arm and camera struggled to detect and grab objects consistently, especially with only a single 2D camera. Adding the basket and rest made the task more repeatable and simplified the throwing routine in a way that code changes alone could not.

<img src="{{ '/assets/images/RobotArm.png' | relative_url }}" alt="Robot arm setup with basket and block handling fixture" class="project-image">
*Robot arm setup with the basket and rest used to improve block handling during the throwing routine.*
