---
title: Computer Vision for UAVs
summary: A project developed for my Final Year report for Aeroespace Engineer Bachelor Degree.
subtitle: Exploration of Vision-Based Control Solutions for PX4-Driven UAVs
description: "Using computer vision to teach drones how to follow people and respond to gestures."
tags: ['py', 'cv']
date: 2022-12-01
github: "https://github.com/l-gonz/tfg-giaa-dronecontrol"
links:
  - icon: github
    icon_pack: fab
    external_link: https://github.com/l-gonz/tfg-giaa-dronecontrol
---


## The DroneVisionControl application

Have you ever wanted a drone that could follow you around or respond to your hand gestures? That’s exactly what I set out to do with this project! Using the PX4 autopilot platform and some popular computer vision tools, I created a system that lets a drone track a person or respond to gestures in real time.

The project combined software development, hardware tinkering, and simulation to explore how vision-based control can make drones smarter and more interactive.

This application was developed as the Final Year project for my bachelor in Aerospace Engineering. The project report is hosted in the [university's archive](https://burjcdigital.urjc.es/handle/10115/25414).

---

## Key Features
- **Follow Mode**: The drone uses a camera to track a person and follow their movements automatically.
- **Gesture Control Mode**: Simple hand gestures can control the drone’s movement, like telling it to move forward or turn.
- **Simulation and Flight Tests**: Developed a platform to test control algorithms in a virtual environment (built on Unreal Engine) before trying it out on a real drone.
- **Low-Cost Hardware**: Built using affordable components like a Raspberry Pi and a basic webcam.

---

## Tech Stack
- **Languages**: Python  
- **Tools**: PX4 (autopilot), Google's MediaPipe (for gesture detection), OpenCV (for image processing)  
- **Simulation**: AirSim + Unreal Engine  
- **Hardware**: Pixhawk 4, Raspberry Pi 4, Logitech C920  

---

## Software architecture
![Hand gesture control](images/giaa/software-arch.jpg)

---

## Showcase

### Hand gesture control

Available gestures
![Possible gestures](images/giaa/hand-gestures.jpg)

Interface
![Hand gesture control](images/giaa/hand-interface.png)

### Person follow control

Inputs for drone control
![Follow vectors](images/giaa/follow-vectors.jpg)

Interface
![Follow control](images/giaa/follow-interface.png)

---

## Development Journey
### Phase 1: Prototyping  
I started with a simple idea: controlling the drone with hand gestures. Using MediaPipe for gesture detection and the PX4 platform for flight control, I created a prototype and tested it in a simulator called AirSim, built on top of Unreal Engine.

### Phase 2: Human Tracking  
Next, I upgraded the system so the drone could follow a person. The camera detects the person’s position, and the drone adjusts its flight to keep them centered in its view.  

### Phase 3: Real-World Testing  
Once everything worked in the simulator, I built a custom quadcopter and tested it outdoors. After a lot of tweaking, the drone successfully followed people and responded to gestures in real flight!  

---

## See It in Action
![Demo GIF](images/giaa/9h762f.gif)

Want to explore more?  
- [Check out the code on GitHub](https://github.com/l-gonz/tfg-giaa-dronecontrol)  
- [Watch the full demo](https://www.youtube.com/watch?v=-CW-B27O4Y0)  

---

## What’s Next?
I’d love to expand on this project with:  
- **Better Tracking**: Improving detection in challenging conditions like low light.  
- **Obstacle Avoidance**: So the drone can safely navigate around objects.  
- **Multi-Drone Support**: Imagine a team of drones working together!

---

This project was such a fun way to explore what’s possible with drones and computer vision. It’s a mix of tech, creativity, and problem-solving.