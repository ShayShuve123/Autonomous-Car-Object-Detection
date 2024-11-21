# Autonomous Vehicle Object Detection Using YOLOv8 and CARLA 

## Overview
This project demonstrates the integration of real-time object detection in an autonomous vehicle using the CARLA simulator and the YOLOv8 model. The system identifies pedestrians and traffic lights in a dynamic urban environment and modifies vehicle behavior accordingly.

---

## Features
- **CARLA Integration**: Simulates urban driving scenarios.
- **YOLOv8 Object Detection**: Detects pedestrians and traffic lights with high accuracy.
- **Real-Time Action**: Reduces vehicle speed by 50% for 5 seconds when a pedestrian is detected.
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

### Video Demonstration

[![Watch the game in action]([https://drive.google.com/thumbnail?id=1hDyzmLHcLvUdbY_WbIBFBXrmECBR7FX7](https://drive.google.com/file/d/1YoiyYKKcEb6YuYje_Ls3Pfg4JML29rqE/view?usp=drive_link))](https://drive.google.com/file/d/1hDyzmLHcLvUdbY_WbIBFBXrmECBR7FX7/view?usp=sharing)



Screenshots
Detection Visualization

Urban Driving Scene











--------------------------------------------------------------------------------------------
## Getting Started

### Prerequisites
Before running this project, ensure the following libraries and tools are installed:
- [CARLA Simulator](https://carla.org)
- [Ultralytics YOLOv8](https://docs.ultralytics.com/)
- Python libraries: `opencv-python`, `numpy`, `math`, `time`

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/AutonomousCarDetection.git
   cd AutonomousCarDetection










## Overview
This project demonstrates the integration of real-time object detection in an autonomous vehicle using the CARLA simulator and the YOLOv8 model. The system identifies pedestrians and traffic lights in a dynamic urban environment and modifies vehicle behavior to emulate real-world scenarios. For example, when pedestrians are detected, the vehicle slows down, mimicking the behavior of human drivers in real life.

---

## Features
- **CARLA Integration**: Simulates urban driving scenarios with realistic environments.
- **YOLOv8 Object Detection**: Detects pedestrians, traffic lights, and other objects. To improve detection accuracy, only objects with a confidence level above 0.6 (on a scale of 0 to 1) are processed. This filtering ensures that the system reacts only to reliable detections.
- **Real-Time Action**: Slows down the vehicle by 50% for 5 seconds when a pedestrian is detected, similar to how real-world vehicles respond to nearby pedestrians.
- **RGB Camera Processing**: Captures and processes live feed from an onboard camera for continuous object detection.
