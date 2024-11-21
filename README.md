# Autonomous-Car-Object-Detection

# Intelligent Pedestrian and Traffic Interaction in CARLA

## Project Title
"**Autonomous Driving in Dynamic Environments: Real-Time Pedestrian Detection and Response in CARLA**"

## Description

This project showcases the development of a **real-time autonomous driving system** using the CARLA simulator and advanced object detection with YOLOv8. The system equips a self-driving vehicle with the ability to **detect pedestrians and other objects** and dynamically adapt its behavior to ensure safety and compliance with road environments.

Key features include:
- **Pedestrian response system**: Reduces speed upon detecting a pedestrian.
- **Dynamic visualization**: Real-time display of detected objects with bounding boxes.
- **Smooth integration with CARLA Traffic Manager** for seamless autonomous navigation.

This project highlights how **AI and simulation** can converge to create safer autonomous systems.

---

## Features

- **Advanced Object Detection**:
  - Detects pedestrians, traffic lights, and other objects with high accuracy using YOLOv8.
  - Confidence threshold filtering (≥ 60%) to minimize false positives.

- **Dynamic Autonomous Behavior**:
  - Slows down the vehicle by 50% for five seconds upon detecting a pedestrian, enhancing safety.
  - Resumes normal speed automatically.

- **Interactive Visual Feedback**:
  - Displays detected objects directly in the simulation feed.

- **Scalable Architecture**:
  - Extensible for detecting additional objects or implementing other behaviors.

---

## Setup Instructions

### Prerequisites

1. Install [CARLA Simulator](https://carla.org/) on your local machine.
2. Ensure you have **Python 3.8 or above** installed.
3. Install required libraries:
   ```bash
   pip install carla opencv-python ultralytics numpy math
