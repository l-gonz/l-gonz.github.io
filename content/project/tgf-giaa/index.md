---
title: Computer Vision for UAVs
summary: A project developed for my Final Year dissertation for Aeroespace Engineer Bachelor Degree.
subtitle: Exploration of Vision-Based Control Solutions for PX4-Driven UAVs
tags: ['py', 'cv']
date: 2022-12-01
github: "https://github.com/l-gonz/tfg-giaa-dronecontrol"
links:
  - icon: github
    icon_pack: fab
    external_link: https://github.com/l-gonz/tfg-giaa-dronecontrol
---


## Overview

This project was developed as the end-of-degree project for my bachelor in Aerospace Engineering. You can find the project report in the [university's archive](https://burjcdigital.urjc.es/handle/10115/25414).

This project explored the integration of computer vision techniques into unmanned aerial vehicle (UAV) control systems, leveraging the PX4 open-source autopilot platform. The primary goal was to create a system capable of autonomous tracking and following a human target, using affordable hardware and real-time image analysis.

Two control solutions were developed: a **hand-gesture-based control mechanism** (proof-of-concept) and a more advanced **human-following control system**, showcasing the adaptability of vision-based controls in UAVs. Simulations and flight tests validated the effectiveness of these solutions, paving the way for future improvements in UAV autonomy.



---

## Software architecture
![Hand gesture control](images/giaa/software-arch.jpg)

---

## Key Features
- **Vision-Based Human Following**: Utilized onboard cameras and real-time image processing to track and follow a human subject.
- **Hand-Gesture Control**: Interpreted gestures to generate flight commands.
- **Simulation-Driven Development**: Developed and tested solutions in AirSim, a high-fidelity UAV simulator.
- **Accessible Hardware**: Employed cost-effective components, including a Raspberry Pi and Logitech C920 camera.

---

## Tech Stack
- **Languages**: Python
- **Frameworks & Libraries**: PX4, MediaPipe, OpenCV, MAVSDK
- **Simulation Tools**: Unreal Engine with AirSim
- **Hardware**: Pixhawk 4, Raspberry Pi 4, Logitech C920

---

## Showcase

### Hand gesture control

Available gestures
![Possible gestures](images/giaa/hand-gestures.jpg)

Interface
![Hand gesture control](images/giaa/hand-interface.png)

### Human follow control

Axes for drone control
![Follow vectors](images/giaa/follow-vectors.jpg)

Interface
![Follow control](images/giaa/follow-interface.png)

---

## Development Journey
### Phase 1: Proof-of-Concept
- Developed a hand-gesture-based control mechanism to test basic integration between the PX4 platform and MediaPipe.
- Used AirSim for initial validation and refinement.

### Phase 2: Human-Following Control
- Designed an onboard system to detect and track a person using the drone’s camera.
- Tuned PID controllers for precise tracking and movement.
- Conducted comprehensive testing in both simulated and real-world environments.

### Phase 3: Real-World Validation
- Built and calibrated a custom quadcopter.
- Integrated hardware and tested control solutions in outdoor flights.
- Identified and resolved challenges in vision-based control under varying conditions.

---

## Future Improvements
- Enhance detection algorithms for better performance in low-light conditions.
- Integrate obstacle avoidance for safer autonomous navigation.
- Expand to multi-drone systems for collaborative tasks.
