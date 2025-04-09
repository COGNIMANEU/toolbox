---
title: "ROS2 to Cloud JSON MQTT Bridge"
weight: 2
description: "Software to bridge edge-cloud ROS2 and MQTT including a json serialization/deserializacion of messages"
license: "https://img.shields.io/badge/License-Apache%202.0-yellowgreen"
trl: "https://img.shields.io/badge/TRL-7-green"
link: "https://github.com/COGNIMANEU/pilot02-connectivity-bridge-ros2-json-mqtt"
github: "https://github.com/COGNIMANEU/pilot02-connectivity-bridge-ros2-json-mqtt"
---

## Name
ROS2MQTTJsonBridge ROS2 to Cloud MQTT Bridge

## Description
This repository provides a bidirectional bridge between ROS2 and MQTT, enabling message exchange between ROS2 systems and other distributed systems through MQTT brokers using JSON serialization.

Traditional ROS2 systems use binary message formats, which are not easily consumable by many cloud-based or non-ROS systems. Existing solutions like [`mqtt_bridge`](https://github.com/groove-x/mqtt_bridge) are no longer actively maintained. An alternative, [`mqtt_client`](https://github.com/ika-rwth-aachen/mqtt_client), supports bidirectional MQTT communication but transmits messages in a binary format, limiting interoperability.

**ROS2MQTTJsonBridge** provides a lightweight, extensible, and container-ready solution that enables:
- **Bidirectional communication** between ROS2 nodes and MQTT clients.
- **Automatic serialization and deserialization** of ROS2 messages into **JSON** format for improved interoperability.
- Seamless integration with edge devices running ROS2 and cloud-based MQTT ecosystems.

Features:
- Bidirectional bridging (ROS2 ↔ MQTT)
- Automatic JSON serialization/deserialization for ROS2 messages
- Configurable topic mapping (ROS ↔ MQTT)
- Docker support for containerized deployments

The repository includes the following components:
- Configuration files (how to address the bridge from ROS->MQTT and MQTT->ROS including the automatic serializer and deserializer)
- Docker setup for easy containerization
- A Docker Compose-based test environment to verify end-to-end functionality: ROS publisher → MQTT bridge → MQTT broker → Python MQTT client; Python MQTT client → MQTT broker → MQTT bridge → ROS subscriber.

## Type
Tool

## Layer
Connectivity

## HRL
2.8

## Partners
![ITA Logo](/images/ita/italogo.jpg)

## Pilot
To be used in all pilots involving ROS2 for robot integration with the digital twin—particularly the GOIMEK pilot—this component plays a critical role in bridging ROS2-based edge robotics with distributed systems in the cloud. By automatically converting ROS2 messages to and from JSON, it enables seamless interoperability with non-ROS2 components, such as cloud services, monitoring tools, or digital twin platforms. This ensures smooth bidirectional communication and enhances the efficiency of remote supervision and operations.