---
title: "DepthAI ROS2 Camera Driver for OAK Camera Sensors"
date: 2025-03-20T12:00:00+00:00
weight: 2
description: "OAK Camera sensor (DepthAI ROS Integration)"
license: "https://img.shields.io/badge/License-MIT-yellowgreen"
trl: "https://img.shields.io/badge/TRL-9-green"
link: "https://github.com/COGNIMANEU/pilot02-physical-oak-camera"
github: "https://github.com/COGNIMANEU/pilot02-physical-oak-camera"
---
## Name
Spinnaker ROS2 Camera Driver for Blackfly Camera Sensors

## Description

The **DepthAI ROS2 Camera Driver** is a package that provides seamless integration of the **Pilot02-Physical OAK Camera** into the ROS 2 ecosystem. Built on top of the open-source [`depthai_ros_driver`](https://github.com/luxonis/depthai-ros) by Luxonis, this driver bridges the [OAK (OpenCV AI Kit)](https://docs.luxonis.com/en/latest/) hardware with ROS 2, enabling powerful camera and depth perception features for robotics applications.

The driver includes all the necessary configurations, launch files, and a Docker setup, providing an easy and containerized deployment of the OAK camera in a ROS 2-based environment.

### Key Features:
- **ROS 2 Support:** This driver allows integration of OAK camera sensors into ROS 2 systems, enabling seamless camera integration and control.
- **SDK Compatibility:** Built upon the `depthai_ros_driver`, it leverages DepthAI's SDK for integration into ROS 2.
- **Supported Features:**
  - Synchronized RGB and depth streaming
  - Real-time point cloud generation
  - IMU data publishing
  - TF tree publishing from calibration
  - ROS 2 composition for optimized intra-process communication
- **Point Cloud and Depth Information:** Provides depth perception capabilities and generates point clouds, critical for tasks like 3D mapping and SLAM.
- **Camera Streams:** Exposes camera streams, including both RGB and depth data, as standard ROS topics.

### Platforms:
- ROS 2 Humble/Iron under Ubuntu 22.04 LTS
- ROS 2 Rolling/Jazzy under Ubuntu 24.04 LTS
- DepthAI SDK version 2.15.0 (other versions may work but are not guaranteed)

This driver is ideal for robotics applications that require real-time depth sensing, 3D perception, and AI vision processing. It is particularly useful in research, prototyping, and production environments, supporting a wide range of robotic platforms requiring high-quality depth data and camera inputs.

## Type
Device

## Layer
Physical

## HRL
- 2.3 Autonomous navigation
- 2.6 Context & safety awareness
- 2.7 Semantic map generation

## Partners
![ITA Logo](/images/ita/italogo.jpg)

## Pilot

This component integrates high-resolution OAK cameras to enhance the AGV’s visual perception capabilities. These cameras deliver essential image and depth data, supporting a range of autonomous functions and ensuring reliability, accuracy, and situational awareness in diverse operational environments.

### 2.3 Autonomous Navigation  
The OAK cameras contribute to precise visual and depth feedback, helping the robot to perceive and navigate autonomously through complex environments. These cameras provide essential data in areas where LiDAR or other sensors may have limitations.

### 2.6 Context & Safety Awareness  
High-quality image and depth streams from the OAK cameras enable the detection of obstacles, dynamic elements, and environmental changes. This ensures the AGV maintains real-time awareness, improving safety and responsiveness in unpredictable or changing environments.

### 2.7 Semantic Map Generation  
The image and depth data from the OAK cameras serve as input for AI-driven perception pipelines, supporting object recognition, scene understanding, and semantic segmentation. This facilitates the creation of detailed semantic maps, enhancing decision-making and allowing the AGV to adapt to context-specific tasks.