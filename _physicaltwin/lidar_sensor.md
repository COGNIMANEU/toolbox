---
title: "Livox ROS 2 Driver for Lidar Sensors"
date: 2025-03-19T12:00:00+00:00
weight: 2
description: "AGV Lidar sensor (GOIMEK pilot)"
license: "https://img.shields.io/badge/License-Apache%202.0-yellowgreen"
trl: "TRL https://img.shields.io/badge/TRL-9-green"
link: "https://github.com/COGNIMANEU/pilot02-physical-livox-lidar"
github: "https://github.com/COGNIMANEU/pilot02-physical-livox-lidar"
---

## Name
Livox ROS 2 Driver for Lidar Sensors

## Description
2xRidbadge Laser 2D (GOIMEK pilot)

The **Livox ROS 2 Driver** is driver package for integrating Livox LiDAR devices into the ROS 2 ecosystem. This driver supports several Livox LiDAR products, enabling users to easily interface with these devices in ROS 2 environments.

Key Features:
- **ROS 2 Support:** it is designed to allow users to utilize Livox LiDAR devices with the ROS 2 framework.
- **SDK Compatibility:** compatible with Livox SDK 2.2.0 and above.
- **Supported Livox LiDAR Models:**
  - MID40
  - MID100
  - Horizon
  - Tele
  - Avia
  - Mid-70
  - HUB
- **Supported Firmware Versions:**
  - MID40/MID100: 3.7.0 and above
  - HUB: 8.8.0 and above
  - Horizon: 6.7.0 and above
  - Tele: 7.10.0 and above
  - Avia: 11.06.0 and above
  - Mid-70: 10.04.0 and above

This driver package facilitates the integration of Livox LiDARs into ROS 2-based robotics systems, providing access to the full functionality of these devices within the ROS 2 environment.

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

This component enables the generation of point clouds that support the autonomous navigation system by detecting objects, preventing collisions, and creating a semantic map. It specifically addresses the following requirements:

### 2.3 Autonomous Navigation
The point clouds generated assist in enabling the robot to navigate autonomously, ensuring safe and efficient movement in various environments.

### 2.6 Context & Safety Awareness
The system uses the point clouds to detect surrounding objects, providing real-time awareness to avoid potential hazards and ensuring safety in dynamic environments.

### 2.7 Semantic Map Generation
The generated point clouds are used to create a detailed semantic map, helping the robot to understand its environment and make informed decisions based on context.
