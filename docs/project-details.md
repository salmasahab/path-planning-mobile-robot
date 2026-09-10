# Project Details

## Problem Statement

Mobile robots face challenges when navigating unknown and changing environments where obstacles may appear unexpectedly. This project focuses on developing a hybrid path planning system that enables safe and efficient navigation using real-time sensor data.

## Objectives

- Develop a differential-drive mobile robot using RPLIDAR A1 and MPU6050.
- Perform real-time environment mapping using SLAM.
- Enable autonomous navigation using the Nav2 stack.
- Implement real-time obstacle detection using LiDAR.
- Use A* for global path planning and DWA for local obstacle avoidance.
- Evaluate mapping accuracy, path planning, and obstacle avoidance performance.

## Hardware

- Raspberry Pi 3 (1 GB)
- Arduino Uno
- RPLIDAR A1
- MPU6050 IMU
- TB6612FNG motor driver
- 2WD chassis
- DC geared motors with incremental encoders

## Software

- Ubuntu 22.04
- ROS 2 Humble
- Gazebo
- RViz2
- SLAM Toolbox
- Nav2
- Python

## Methodology

The robot uses LiDAR and IMU sensing for perception and localization. SLAM Toolbox generates an occupancy-grid map of the environment. A* is used to generate the global path, while DWA continuously adjusts the local path for obstacle avoidance. The resulting velocity commands are sent to the robot for navigation.

## Results

The system was validated in an indoor laboratory environment. LiDAR and SLAM Toolbox were used to generate a real-time occupancy-grid map, while the integrated navigation framework supported autonomous path planning and obstacle avoidance.

## Limitations

- Testing was limited to an indoor laboratory environment.
- Raspberry Pi 3 has limited RAM for computationally intensive processes.
- Moving obstacles were not tracked or predicted.
- Camera data was not used for navigation decisions.
- Motor response varies slightly with battery level.

## Future Work

- Improve dynamic obstacle detection using AI/deep learning.
- Improve sensor fusion and real-time decision making.
- Test the system in larger and outdoor environments.
- Extend the system toward multi-robot coordination.



### System Architecture
![System Architecture](./images/system-architecture.png)

### Robot and Development Setup
![Robot and Laptop](./images/robot-and-laptop.jpg)
