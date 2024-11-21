# Autonomous-Car-Object-Detection

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

