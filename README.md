# Autonomous Vehicle Object Detection Using YOLOv8 and CARLA Simulator

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
# Components
1.CARLA Simulator:

Simulates a city environment (Town02) with pedestrians, vehicles, and traffic lights.
Provides sensor data (camera feed) for processing.
YOLOv8 Integration:

Processes images from the RGB camera.
Identifies objects such as pedestrians and traffic lights with confidence thresholds.
Autonomous Vehicle Behavior:

The vehicle operates on autopilot.
When a pedestrian is detected, the Traffic Manager adjusts the speed.
Workflow
The CARLA simulator initializes the urban environment and spawns vehicles and pedestrians.
The onboard RGB camera captures live video.
Images are processed with YOLOv8 to detect objects.
If a pedestrian is detected:
The Traffic Manager reduces the vehicle's speed by 50% for 5 seconds.
The system logs detection details and overlays bounding boxes on detected objects.














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

