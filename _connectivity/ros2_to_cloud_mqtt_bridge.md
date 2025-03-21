---
title: "ROS2 to Cloud MQTT Bridge"
date: 2025-03-21T12:00:00+00:00
weight: 2
description: "Software to bridge edge-cloud ROS2 and MQTT messages"
license: "https://img.shields.io/badge/License-MIT-yellow"
trl: "https://img.shields.io/badge/TRL-9-green"
link: "https://github.com/COGNIMANEU/pilot02-connectivity-bridge-ros2-mqtt"
github: "https://github.com/COGNIMANEU/pilot02-connectivity-bridge-ros2-mqtt"
---

## Name
ROS2 to Cloud MQTT Bridge

## Description
This repository provides a software solution designed to bridge edge-cloud ROS2 and MQTT messages (GOIMEK pilot). The component is generic and aimed at facilitating the technological integration between edge-based developments using ROS2 (Robot Operating System 2) and cloud-based software systems, via an Event-Driven Architecture (EDA). The solution leverages MQTT as an intermediary broker, allowing seamless communication between local ROS2 applications running on edge devices and cloud-based platforms.

By using this bridge, developers can easily integrate edge robotics systems that rely on ROS2 for communication with cloud-based services, data analytics platforms, or other distributed systems, enabling advanced functionalities such as remote monitoring, cloud processing, and machine learning. The MQTT protocol acts as a lightweight, scalable communication layer, ensuring reliable and efficient message delivery between the edge and cloud components.

This component provides:
- A flexible architecture for integrating ROS2 and MQTT with minimal configuration.
- Scalable, event-driven communication between edge and cloud systems.
- Seamless data exchange between local robots and remote platforms in real-time.

Configuration and launch files may be customized and adapted for each use case.

## Type
Tool

## Layer
Connectivity

## HRL
2.8

## Partners
ITA

## Pilot
To be used in all pilots that employ ROS2 for robot integration with the digital twin, specifically the GOIMEK pilot. This component ensures smooth interaction between edge robotics running on ROS2 and their digital twin counterparts, enabling more efficient remote operations and monitoring.
