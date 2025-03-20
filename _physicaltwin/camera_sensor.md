---
title: "Spinnaker ROS2 Camera Driver for Blackfly Camera Sensors"
date: 2025-03-20T12:00:00+00:00
weight: 2
description: "AGV Camera sensor (GOIMEK pilot)"
license: "https://img.shields.io/badge/License-Apache%202.0-yellowgreen"
trl: "https://img.shields.io/badge/TRL-9-green"
link: "https://github.com/COGNIMANEU/pilot02-physical-blackfly-camera"
github: "https://github.com/COGNIMANEU/pilot02-physical-blackfly-camera"
---

## Name
Spinnaker ROS2 Camera Driver for Blackfly Camera Sensors

## Description

The **Spinnaker ROS 2 Camera Driver** is a package that provides integration for Teledyne/FLIR cameras into the ROS 2 ecosystem using the Spinnaker SDK. For synchronized camera configurations, the Spinnaker synchronized camera driver is available, allowing precise hardware synchronization.

Note: This driver is not officially written or supported by FLIR.

### Key Features:
- **ROS 2 Support:** This driver allows users to integrate FLIR cameras into ROS 2-based systems, enabling seamless camera integration and control within ROS 2 environments.
- **SDK Compatibility:** Compatible with Spinnaker SDK for integration of FLIR cameras with ROS 2.
- **Supported Camera Models:**
  - Blackfly S (USB3, GigE)
  - Blackfly (GigE)
  - Grasshopper (USB3)
  - Oryx (Reported working)
  - Chameleon (USB3, tested with firmware v1.13.3.00)
  - FLIR AX5 (GigE)
- **Supported Firmware Versions:**
  - Blackfly S, Blackfly: 3.8.0 and above
  - Grasshopper: 3.7.0 and above
  - Oryx: 3.7.0 and above
  - Chameleon: 1.13.3.00 and above
  - FLIR AX5: 3.7.0 and above

### Platforms:
- ROS 2 Humble/Iron under Ubuntu 22.04 LTS
- ROS 2 Rolling/Jazzy under Ubuntu 24.04 LTS
- Spinnaker 3.1.0.79 (other versions may work as well but this is the version used in continuous integration builds)

This driver facilitates the integration of Teledyne/FLIR cameras with ROS 2, providing complete functionality for supported camera models within the ROS 2 environment, including image streaming, calibration, and synchronization.

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
