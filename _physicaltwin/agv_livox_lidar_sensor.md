---
title: "Livox ROS 2 Driver for Lidar Sensors"
weight: 2
description: "AGV Lidar sensor (GOIMEK pilot)"
license: "https://img.shields.io/badge/License-Apache%202.0-yellowgreen"
trl: "https://img.shields.io/badge/TRL-9-green"
link: "https://github.com/COGNIMANEU/pilot02-physical-livox-lidar"
github: "https://github.com/COGNIMANEU/pilot02-physical-livox-lidar"
---

## Name
Livox ROS 2 Driver for Lidar Sensors

## Description

The Livox ROS 2 Driver is a package designed to integrate Livox LiDAR devices into the ROS 2 ecosystem. This driver enables seamless communication between ROS 2 and Livox LiDAR sensors, providing an efficient solution for perception-based applications.

Key Features:
- **ROS 2 Compatibility:** Supports integration with ROS 2-based systems for real-time LiDAR data processing.
- **Pilot02-Physical Support:** Specifically designed for the Pilot02-Physical Livox LiDAR.
- **Configuration Options:** Allows setup via JSON configuration files and RViz visualization.
- **Launch Files:** Predefined ROS 2 launch files for streamlined deployment.
- **Docker Support:** Includes a Docker setup for containerized execution, simplifying environment management.
- **Testing Environment:** Provides a `docker-compose`-based test setup for verifying published LiDAR topics (requires LiDAR hardware).

Platforms:
- **ROS 2 Humble/Iron** on **Ubuntu 22.04 LTS**
- **ROS 2 Rolling/Jazzy** on **Ubuntu 24.04 LTS**

This package enables easy integration of Livox LiDAR devices into ROS 2, offering a fully configurable, containerized solution for various robotics and perception applications.

## Type
Device

## Layer
Physical

## HRL
- 2.3 Autonomous navigation
- 2.6 Context & safety awareness
- 2.7 Semantic map generation

## Partners
ITA

## Pilot

This component integrates high-resolution Blackfly cameras to enhance the AGV’s visual perception capabilities. These cameras provide critical image data that supports a range of autonomous functions, ensuring reliability, precision, and situational awareness across various operational scenarios.

### 2.3 Autonomous Navigation  
The Blackfly cameras contribute to accurate visual feedback, assisting the robot in interpreting its environment and navigating autonomously through complex spaces where LiDAR or other sensors may have limitations.

### 2.6 Context & Safety Awareness  
High-quality image streams from the Blackfly cameras enable detection of obstacles, dynamic elements, and changes in the environment. This ensures the AGV maintains real-time awareness, enhancing safety and responsiveness in unpredictable surroundings.

### 2.7 Semantic Map Generation  
The image data serves as input for computer vision and AI-based perception pipelines, supporting object recognition and scene understanding. This enables the creation of rich semantic maps, improving decision-making and enabling the AGV to adapt to context-specific tasks.