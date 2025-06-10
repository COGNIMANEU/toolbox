---
title: "Real-Time ROS2 Lichtblick Visualizer"
weight: 2
description: "Real-Time viewer of ROS2 in a web-based fully customizable user interface"
license: "https://img.shields.io/badge/License-MPL%202.0-brightgreen"
trl: "https://img.shields.io/badge/TRL-7-green"
link: "https://github.com/COGNIMANEU/pilot02-digitaltwin-lichtblick"
github: "https://github.com/COGNIMANEU/pilot02-digitaltwin-lichtblick"
---

## Name
Real-Time ROS2 Lichtblick Visualizer

## Description

This component provides a Docker-based version of Lichtblick (https://github.com/lichtblick-suite/lichtblick), adapted as a real-time visualization tool for robotics solutions based on ROS 2. It leverages the capabilities of Foxglove (https://foxglove.dev/) to provide an intuitive and interactive interface for monitoring and analyzing robotic systems in real time.

### Features

- Dockerized deployment: Easy to set up and run in isolated environments without complex installation.
- Real-time visualization: Leverages Foxglove for monitoring live ROS 2 data streams (topics, transforms, logs, etc.).
- ROS 2 compatibility: Natively supports ROS 2 message types and tools for robotic system integration.
- 3D visualization: View robot models, environments, and sensor data (e.g., LIDAR, cameras) in an interactive 3D scene.
- Customizable panels: Flexible UI with panels for plotting, logging, time-series data, and more.
- Bag file playback support: Visualize and debug recorded `.db3` or `.mcap` data alongside live streams.
- Isolated environment: Ensures consistent behavior across different systems using containerization.
- Web-based interface: Access the visualization tool through a browser, no local GUI required.
- Multi-topic inspection: Subscribe to and inspect multiple ROS 2 topics in parallel.
- Easy configuration: Supports loading custom layouts and configurations at startup.

![Board Demo](./images/ita/pilot02-digitaltwin-lichtblick.gif)

[See at](https://toolbox.cogniman.eu/images/ita/pilot02-digitaltwin-lichtblick.gif)

## Type
Tool

## Layer
Digital Twin Representation

## HRL
2.3, 2.4, 2.8

## Partners
![ITA Logo](/images/ita/italogo.jpg)

## Pilot
This component enables remote monitoring of all ROS2 topics in the pilot, allowing users to visualize data—whether textual, point clouds, images, or others, directly from a web browser. Additionally, it can be reused in any other pilot project that includes developments based on ROS.