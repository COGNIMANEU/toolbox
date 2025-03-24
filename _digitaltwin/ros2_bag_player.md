---
title: "Real-Time ROS2 Log Bag Player"
weight: 4
description: "Real-Time Log Player for ROS2"
license: "https://img.shields.io/badge/License-Apache%202.0-yellowgreen"
trl: "https://img.shields.io/badge/TRL-9-green"
link: "https://github.com/COGNIMANEU/pilot02-digitaltwin-rosbag-player"
github: "https://github.com/COGNIMANEU/pilot02-digitaltwin-rosbag-player"
---

## Name
Real-Time ROS2 Log Bag Player

## Description

The ROS 2 Bag Player is a software component that facilitates the playback of data stored in ROS 2 bag files. This component is designed to allow users to replay sensor data, messages, and topics that were previously recorded within a ROS 2 environment. The component reads the bag file, which contains serialized message data, and publishes the messages to the corresponding ROS 2 topics as they were originally recorded.

The primary function of the ROS 2 Bag Player is to simulate real-time behavior by replaying recorded messages at their original timestamps. It is useful in scenarios such as testing, debugging, and developing applications that require the replay of real-world data without needing to interact with physical hardware or sensors.

Features:
- Plays back multiple topics stored within a bag file.
- Preserves the timing and order of messages as recorded.
- Supports different serialization formats, including CDR (Common Data Representation).
- Integrated with the ROS 2 ecosystem, utilizing the `ros2 bag` command-line tool for playback.
- Ideal for end-to-end testing and simulating robotic systems or applications.

## Type
Tool

## Layer
Digital Twin Representation

## HRL
2.3, 2.4, 2.8

## Partners
ITA

## Pilot
To be used in all pilots that employ ROS2 for robot integration with the digital twin, specifically the GOIMEK pilot. 

Use cases:
- **Testing**: Verifying algorithms and behaviors with recorded data.
- **Debugging**: Investigating issues without requiring live data from hardware.
- **Development**: Using real-world data for creating and refining ROS 2 applications.