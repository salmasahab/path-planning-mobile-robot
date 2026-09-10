
# Path Planning Algorithm for Mobile Robots in Unknown Environments

## Project Overview

This project focuses on developing a hybrid path planning and autonomous navigation system for a differential-drive mobile robot operating in unknown environments.

The system uses real-time LiDAR and IMU sensor data with ROS 2, SLAM, and Nav2 to support mapping, path planning, obstacle detection, and autonomous navigation.

## Hardware

- Raspberry Pi 3 (1 GB)
- Arduino Uno
- RPLIDAR A1
- MPU6050 IMU
- TB6612FNG Motor Driver
- DC Geared Motors with Incremental Encoders
- DIY 2WD Mobile Robot Chassis

## Software & Tools

- Ubuntu 22.04
- ROS 2 Humble
- Gazebo
- RViz2
- SLAM Toolbox
- Nav2
- Python
- Arduino IDE

## Navigation Approach

- Real-time environment mapping using LiDAR and SLAM
- A* for global path planning
- DWA for local obstacle avoidance
- Nav2 for autonomous navigation
- IMU and encoder feedback for robot motion estimation and correction

## System Architecture

The system follows a three-tier architecture consisting of:

1. High-level ROS 2 navigation and planning
2. Raspberry Pi-based processing and sensor integration
3. Arduino-based low-level motor control

## Results

The developed system was tested in an indoor laboratory environment. The robot was able to generate an occupancy-grid map using LiDAR and SLAM and perform navigation using the integrated path planning and obstacle avoidance framework.

## Limitations

- Testing was limited to indoor environments.
- Raspberry Pi 3 has limited RAM for computationally intensive processes.
- Moving obstacles were not tracked or predicted.
- Camera data was not used for navigation decisions.
- Motor performance can vary with battery level.

## Future Work

- Improve dynamic obstacle detection using AI/deep learning.
- Improve sensor fusion and real-time decision making.
- Test on larger and outdoor environments.
- Explore multi-robot coordination.

## Research Publication

**Adaptive Hybrid Navigation for Autonomous Mobile Robots in Unknown Dynamic Environments Using Multi-Sensor SLAM**

IEEE International Conference on Robotics and Automation in Industry (ICRAI), 2026.

DOI: 10.1109/ICRAI70912.2026.11551961
