# Autonomous Vehicle Object Detection Using YOLOv8 and CARLA 

## Overview
This project demonstrates the integration of real-time object detection in an autonomous vehicle using the CARLA simulator and the YOLOv8 model. The system identifies pedestrians and traffic lights in a dynamic urban environment and modifies vehicle behavior accordingly.



---

## Features
- **CARLA Integration**: Simulates urban driving scenarios.
- **YOLOv8 Object Detection**: Detects pedestrians and traffic lights with high accuracy.
- **Real-Time Action**: Slows down the vehicle by 50% for 5 seconds when a pedestrian is detected, similar to how real-world vehicles respond to nearby pedestrians.
- **RGB Camera Processing**: Captures and processes live feed from an onboard camera.

---

## Project Architecture
    Components
   1.CARLA Simulator:

Simulates a city environment (Town02) with pedestrians, vehicles, and traffic lights.
Provides sensor data (camera feed) for processing.
YOLOv8 Integration:

Processes images from the RGB camera.
Identifies objects such as pedestrians and traffic lights with confidence thresholds.
Autonomous Vehicle Behavior:

The vehicle operates on autopilot.
When a pedestrian is detected, the Traffic Manager adjusts the speed.

## Workflow
The CARLA simulator initializes the urban environment and spawns vehicles and pedestrians.
The onboard RGB camera captures live video.
Images are processed with YOLOv8 to detect objects.
If a pedestrian is detected:
The Traffic Manager reduces the vehicle's speed by 50% for 5 seconds.
The system logs detection details and overlays bounding boxes on detected objects.

# Video Demonstration

[![Watch the game in action]

## Screenshots
   # Detection Visualization
![image](https://github.com/user-attachments/assets/647e6ea6-7509-4219-9ee3-42c379981ae5)

![image](https://github.com/user-attachments/assets/c8567970-202d-49fd-a1dc-1b62f05c7922)

---

## Features
- **CARLA Integration**: Simulates urban driving scenarios with realistic environments.
- **YOLOv8 Object Detection**: Detects pedestrians, traffic lights, and other objects. To improve detection accuracy, only objects with a confidence level above 0.6 (on a scale of 0 to 1) are processed. This filtering ensures that the system reacts only to reliable detections.
- **Real-Time Action**: Slows down the vehicle by 50% for 5 seconds when a pedestrian is detected, similar to how real-world vehicles respond to nearby pedestrians.
- **RGB Camera Processing**: Captures and processes live feed from an onboard camera for continuous object detection.
