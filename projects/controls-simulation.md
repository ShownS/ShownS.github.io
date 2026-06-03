---
layout: single
author_profile: true
title: "Robotics and Control Simulation"
permalink: /projects/controls-simulation/
---

This section focuses on simulation-based robotics and control work. These projects show how modeling and simulation can be used to study system behavior, test controller decisions, and understand robotic motion before or alongside physical prototyping.

## Salp-Inspired Robot RL Controller Simulation

<p class="skills-line"><strong>Relevant skills:</strong> Reinforcement learning · PPO · MuJoCo · Parameter tuning · Simulation-based research · Technical communication</p>

This project focused on using reinforcement learning to control a simulated salp-inspired robot. Salps are underwater organisms that move using jet propulsion. This propulsion system leads to their robotic equivalent being underactuated, meaning that they cannot directly control all directions of motion. The group explored whether a learning-based controller could train a simulated salp robot to reach target points without requiring separate motion planners.

<img src="{{ '/assets/images/Salp.png' | relative_url }}" alt="Salp-inspired robot simulation or model" class="project-image">
*Salp-inspired robot simulation used to study learning-based locomotion and target reaching.*

My role on the group research project was mainly helping connect the simulation and controls aspects of the work. Because of this, I worked across both parts of the project to help make sure integration went smoothly. This included contributing to the framing of the problem, tuning parameters for the reinforcement learning controller, adjusting parts of the learning approach, and communicating the project cohesively in the final report.

The final work used Proximal Policy Optimization in a MuJoCo simulation environment to train the salp robot to move toward randomized target points. The project gave me experience with learning-based control methods, simulation-based research, and the importance of clear communication when working with team members focused on different parts of a technical problem. It also served as my first experience using AI methods in controls.

## Quadcopter Controller Simulation

<p class="skills-line"><strong>Relevant skills:</strong> LQR control · MATLAB simulation · Dynamic modeling · Disturbance testing · Motor-loss modeling · Control analysis</p>

The goal of this project was to model a simplified quadcopter system and test how a Linear Quadratic Regulator (LQR) controller responded to realistic scenarios. These included wind forces, added payloads, and motor loss. The scenarios were used to test the controller under conditions closer to real-world operation instead of only using an ideal simulation environment.

<img src="{{ '/assets/images/Quadcopter.png' | relative_url }}" alt="Quadcopter simulation trajectory and controller response" class="project-image">
*Quadcopter simulation used to evaluate controller response under wind, payload, and motor-loss scenarios.*

I primarily worked to develop the simulation and visualize the quadcopter’s response. I also worked with the group on modeling the disturbance scenarios, specifically focusing on the motor-loss conditions. This was done by abruptly setting one motor’s speed to approximately zero and evaluating the stability of the system. This case helped show the limitations of the LQR approach more clearly than the moderate wind or payload tests.

Final results showed that the LQR controller performed well for moderate wind and payload changes, but motor loss exposed the limits of the simplified controller. The project strengthened my understanding of classical control methods, as well as how to simulate them in non-ideal environments. An additional key takeaway was that controller performance depends heavily on the assumptions used to simplify a system, especially when the simulation moves away from ideal conditions.

