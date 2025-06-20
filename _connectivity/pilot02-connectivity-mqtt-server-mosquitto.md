---
title: "Mosquitto MQTT Broker"
weight: 2
description: "Open source MQTT broker"
license: "https://img.shields.io/badge/License-EPL%202.0-red"
trl: "https://img.shields.io/badge/TRL-9-green"
link: "https://github.com/COGNIMANEU/pilot02-connectivity-mqtt-server-mosquitto"
github: "https://github.com/COGNIMANEU/pilot02-connectivity-mqtt-server-mosquitto"
---

## Name
Mosquitto MQTT Broker

## Description
This repository provides a software solution designed to deploy and manage a **Mosquitto MQTT Broker**. The component acts as a lightweight, high-performance message broker that enables secure and efficient communication between edge and cloud systems using the MQTT protocol. It is specifically designed to support distributed software architectures, where it functions as the central message mediator for all MQTT communications.

The **Mosquitto MQTT Broker** ensures seamless communication between local edge devices running **ROS2** (Robot Operating System 2) and cloud-based platforms. It leverages MQTT as the messaging protocol to facilitate real-time data exchange, providing a reliable and scalable communication layer for IoT applications and robotics systems.

By using Mosquitto as the MQTT broker, developers can create scalable, event-driven systems that allow local robots and cloud-based services to communicate in a decoupled and efficient manner. The broker ensures secure message delivery, supports multiple clients, and handles a variety of message delivery options to meet the needs of edge-cloud integrations.

This component provides:
- A fully functional **Mosquitto MQTT Broker** for lightweight, scalable communication.
- Real-time message exchange between edge devices running ROS2 and cloud platforms.
- High availability and reliability with support for multiple clients and message persistence.
- Flexible configuration options for various use cases and deployment environments.

Configuration and setup files can be customized to meet specific deployment requirements, ensuring the solution is adaptable to different scenarios and systems.

## Type
Tool

## Layer
Connectivity

## HRL
2.8

## Partners
![ITA Logo](/images/ita/italogo.jpg)

## Pilot
To be used in all pilots that employ ROS2 for robot integration with the digital twin, specifically the GOIMEK pilot. This component acts as an MQTT broker to build a distributed software architecture, serving as a message mediator between the edge ROS2 components and the cloud-based digital twin components.
