---
title: "Semantic Map Data Recorder"
weight: 2
description: "Records ROS 2 data streams for semantic map generation"
license: "https://img.shields.io/badge/License-Copyright%20%C2%A9-red"
trl: "TRL https://img.shields.io/badge/TRL-7-green"
link: ""
github: ""
---

## Name
Semantic Map Data Recorder

## Description
This service records data streams from ROS2 topics (e.g., RGB, depth, LiDAR, and pose) required for the generation of a semantic map. It enables controlled data acquisition in ROS2 environments, allowing operators to initiate and stop recording through service calls. The data gathered by this application will be able to be processed later by another application to generate the map.

### Key Features:
- Records synchronized multimodal data for semantic mapping
- Supports RGB, depth, LiDAR, and robot pose topics
- Configurable start/stop via ROS2 service interface
- Data stored in ROS bag format for post-processing
- Compatible with offline and real-time mapping workflows

## Type
Tool

## Layer
Service

## HRL
-	2.1 Navigation planning
-	2.3 Autonomous navigation
-	2.6 Context & safety awareness
-	2.7 Semantic map generation


## Partners
![ITA Logo](/images/ita/italogo.jpg)

## Pilot

Used during exploration phases in the pilot to capture the necessary data for building accurate semantic maps. The component enables targeted recording, minimizing unnecessary data collection while maximizing map quality.
