---
title: "Clearpath Robotic Simulator"
weight: 2
description: "Digital Twin Clearpath Robotic Simulator"
license: "https://img.shields.io/badge/License-BSD%203--Clause-blue"
trl: "https://img.shields.io/badge/TRL-9-green"
link: "https://github.com/COGNIMANEU/pilot02-digitaltwin-clearpath-simulator"
github: "https://github.com/COGNIMANEU/pilot02-digitaltwin-clearpath-simulator"
---

## Name
Clearpath Robotic Simulator

## Description
This component contains a Docker-based version of the Clearpath simulator ([https://github.com/clearpathrobotics/clearpath_simulator/tree/humble](https://github.com/clearpathrobotics/clearpath_simulator/tree/humble)), which includes NoVNC web services for visualization. By running this container, users can access the ClearPath  Simulator's graphical interface through a web browser at [http://localhost:6080/vnc.html](http://localhost:6080/vnc.html), providing an easy way to interact with simulations remotely using a VNC viewer or through the NoVNC web interface. 
The container also allows for configuring the simulation environment and launching different Gazebo worlds or robots by specifying launch files and adjusting the container's environment variables. By default, a simple robot model and its corresponding launch file are included; however, they may be modified for future reuse.

The Clearpath simulator is built using **Gazebo Harmonic** to provide a physics-based environment for Clearpath robot simulation. It enables users to simulate **multiple robots simultaneously**, and is tightly integrated with the **Clearpath Config** system.

Example of a simple AGV model and world:
![Clearpath Simulator Demo](/images/ita/pilot02-digitaltwin-clearpath-simulator.gif)

## Type
Tool

## Layer
Digital Twin Representation

## HRL
2.3, 2.4, 2.8

## Partners
![ITA Logo](/images/ita/italogo.jpg)

## Pilot
Intended for use in all use cases involving ROS 2-based robot integration with the digital twin, particularly for Rockwell Automation robots such as the AGV deployed in the GOIMEK pilot.

Use cases:
- **Testing**: Verifying algorithms and behaviors with recorded data.
- **Debugging**: Investigating issues without requiring live data from hardware.
- **Development**: Using real-world data for creating and refining ROS 2 applications.