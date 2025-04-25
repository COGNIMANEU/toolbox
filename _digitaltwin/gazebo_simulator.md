---
title: "Gazebo Robotic Simulator"
weight: 2
description: "Digital Twin Robotic Simulator"
license: "https://img.shields.io/badge/License-Apache%202.0-yellowgreen"
trl: "https://img.shields.io/badge/TRL-9-green"
link: "https://github.com/COGNIMANEU/pilot02-digitaltwin-gazebo-simulator"
github: "https://github.com/COGNIMANEU/pilot02-digitaltwin-gazebo-simulator"
---

## Name
Gazebo Robotic Simulator

## Description
This component contains a Docker-based version of the Gazebo Simulator ([https://github.com/gazebosim/gz-sim](https://github.com/gazebosim/gz-sim)), which includes NoVNC web services for visualization. By running this container, users can access the Gazebo Simulator's graphical interface through a web browser at [http://localhost:6080/vnc.html](http://localhost:6080/vnc.html), providing an easy way to interact with simulations remotely using a VNC viewer or through the NoVNC web interface. The container also allows for configuring the simulation environment and launching different Gazebo worlds or robots by specifying launch files and adjusting the container's environment variables.

Gazebo Sim is an open-source robotics simulator that offers high-fidelity physics, rendering, and sensor models, providing a realistic environment for robotics research and development. It supports multiple points of entry for interaction, including a graphical user interface, plugins, and asynchronous message passing, giving users and developers flexibility in controlling simulations. Derived from over 16 years of development, Gazebo Sim enables advanced dynamics simulations, 3D graphics, and various sensor models like cameras, laser range finders, and IMUs, making it a powerful tool for both academic and commercial robotics projects.

Example of a simple AGV model and world:
![Gazebo Demo](/images/ita/)

## Type
Tool

## Layer
Digital Twin Representation

## HRL
2.3, 2.4, 2.8

## Partners
![ITA Logo](/images/ita/pilot02-digitaltwin-gazebo-simulator.png)

## Pilot
To be used in all pilots that employ ROS2 for robot integration with the digital twin, specifically the GOIMEK pilot. 

Use cases:
- **Testing**: Verifying algorithms and behaviors with recorded data.
- **Debugging**: Investigating issues without requiring live data from hardware.
- **Development**: Using real-world data for creating and refining ROS 2 applications.
