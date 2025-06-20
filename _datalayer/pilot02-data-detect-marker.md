---
title: "Aruco Marker Detection"
weight: 1
description: "Detects ArUco markers from an RGB stream in ROS 2 and provides real-time pose data."
license: "https://img.shields.io/badge/License-Copyright%20%C2%A9-red"
trl: "https://img.shields.io/badge/TRL-9-green"
link: ""
github: ""
---

## Name
Sensor Dataset

## Description
This component enables the detection of Aruco markers from a RGB camera stream in a ROS2 environment. It facilitates the localization of key reference points in the table and the part where the robot is going to work and provides pose estimation data in real time.

### Key Features:
- realTimeDetection: true (boolean) - Real-time detection of Aruco markers
- ros2Integration: true (boolean) - Integration with ROS2 camera topics
- outputs (object)
    - markerId (number) - Detected marker ID
    - position (array[number]) - 3D position of the marker [x, y, z]
    - orientation (array[number]) - Orientation as a quaternion [x, y, z, w]
- configurableDictionaries: true (boolean) - Supports configurable marker dictionaries
- detectionParametersConfigurable: true (boolean) - Detection parameters can be adjusted
- lightweight: true (boolean) - Designed for lightweight, efficient edge deployment

## Type
Tool

## Layer
Data

## HRL
- 	2.3 Autonomous navigation
-	2.6 Context & safety awareness
-	2.7 Semantic map generation

## Partners
![ITA Logo](/images/ita/italogo.jpg)

## Pilot

This component enables real-time detection of ArUco markers to enhance the AGV’s environmental perception and localization capabilities. By processing image streams from onboard cameras, it provides essential spatial cues that support a wide range of autonomous functions with high precision and adaptability.

### 2.3 Autonomous Navigation  
The ArucoMarker component delivers accurate visual markers that assist the robot in localizing itself and interpreting its surroundings. This is especially valuable in environments where GPS is unreliable or LiDAR coverage is limited, allowing the AGV to navigate autonomously through structured or dynamic spaces.

### 2.6 Context & Safety Awareness  
Through continuous detection of ArUco markers embedded in the environment, the component helps the AGV maintain context-awareness. Marker-based cues can signal restricted zones, operational areas, or hazards, enhancing real-time safety monitoring and enabling responsive behavior in changing environments.

### 2.7 Semantic Map Generation  
Detected markers provide reliable reference points that can be used in mapping and scene interpretation pipelines. The component supports the generation of semantic maps by linking marker IDs to known locations, objects, or task-specific zones, thereby improving the AGV’s ability to execute context-sensitive operations and navigate intelligently.
