---
title: Project overview
weight: 20  # section position on page

design:
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns: '1'
---

## Overview
This project explored the integration of computer vision techniques into unmanned aerial vehicle (UAV) control systems, leveraging the PX4 open-source autopilot platform. The primary goal was to create a system capable of autonomous tracking and following a human target, using affordable hardware and real-time image analysis.

Two control solutions were developed: a **hand-gesture-based control mechanism** (proof-of-concept) and a more advanced **human-following control system**, showcasing the adaptability of vision-based controls in UAVs. Simulations and flight tests validated the effectiveness of these solutions, paving the way for future improvements in UAV autonomy.

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

## Showcase
![Human-Following Demonstration](images/human-following-demo.jpg)

Experience the project:
- [GitHub Repository](https://github.com/yourusername/project-repo)
- [Live Demo](https://your-live-demo-link.com)

---

## Future Improvements
- Enhance detection algorithms for better performance in low-light conditions.
- Integrate obstacle avoidance for safer autonomous navigation.
- Expand to multi-drone systems for collaborative tasks.

---

This project demonstrates how cutting-edge computer vision can transform UAV autonomy, showcasing the versatility and power of open-source tools like PX4. It’s a testament to the potential of accessible, innovative solutions in advancing aerospace technology.
