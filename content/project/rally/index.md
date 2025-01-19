---
title: Bluetooth Rally Remote Controller
subtitle: RallyOTA
summary: An Arduino-based Bluetooth controller for motorcycle rally navigation with over-the-air updates.
tags: ["arduino", "3d-model"]
date: 2024-03-04
github: "https://github.com/l-gonz/RallyOTA"
links:
  - icon: github
    icon_pack: fab
    name: Repository
    url: https://github.com/l-gonz/RallyOTA
---

## About This Project
RallyOTA is a custom-built Bluetooth remote controller designed for motorcycle rally enthusiasts (me 😊). Built around the ESP32 microcontroller, this compact and versatile remote makes it easy to switch between rally roadbook navigation and mapping apps while riding. The controller also supports over-the-air (OTA) updates, so you can improve its functionality without unscrewing a single bolt.

The board and other physical components are enclosed on holder designed in Fusion 360 and 3D printed using PETG filament.

This project combines hardware tinkering with Arduino programming and 3D modelling, creating a robust solution that has been tested in real-world motorcycle navigation challenges.

---

## Key Features
- **Bluetooth Low Energy (BLE) Support**: Seamlessly connects to Android devices to control rally apps and navigation tools.
- **Over-the-Air Updates**: Update the firmware without needing to re-solder or disassemble the device.
- **Dual Mode**: Quickly switch between controlling rally roadbooks and OsmAnd maps.
- **Durable Hardware**: Designed to withstand the rigors of outdoor motorcycle use, powered via USB from the bike's supply.

---

## Tech Stack
- **Languages**: C++ (Arduino)
- **Hardware**:
  - ESP32-C3 SuperMini
  - PBS-33B buttons (3)
  - MTS-123 rocker switch
- **Libraries**:
  - PlatformIO
  - ESP32 BLE Keyboard
  - ESP2SOTA
  - OneButton

---

## How I Built It
### Design and Assembly
- **Hardware**: The controller uses an ESP32-C3 microcontroller, three push buttons, and a rocker switch to provide intuitive navigation control. It connects to the motorcycle’s onboard power supply via USB for consistent power.
- **Software**: The code includes two main modes:
  - **Rally Mode**: Navigate a roadbook by advancing and retracting pages or adjusting the trip meter.
  - **Navigation Mode**: Control zoom and centering in OsmAnd maps using button inputs.
- **OTA Updates**: With ESP2SOTA, the remote can receive firmware updates over Wi-Fi, making it easy to add new features.

### Key Challenges
- Ensuring Bluetooth stability for a reliable connection during rides.
- Integrating OTA updates into the ESP32 firmware while maintaining security and usability.

---

## See It in Action

![RallyOTA in action in a breadboard](images/rally/demo-v1.gif "First tests")

![RallyOTA in action with soldered circuits](images/rally/demo-v2.gif "With completed build")

- [GitHub Repository](https://github.com/l-gonz/RallyOTA)

---

## 3D model

[3D model in Fusion 360](images/rally/model.jpg "Holder designed in Fusion 360 for the custom hardware.")

---

## What’s Next?
- **Hardware Refinements**: Improving the weatherproofing for bad outdoor conditions.
- **Advanced Controls**: Add new mapping possibilities to control other Android applications.

---

This project reflects my passion for DIY electronics and practical engineering solutions. RallyOTA not only solves a real-world problem but also demonstrates the versatility of embedded systems and Arduino programming.
