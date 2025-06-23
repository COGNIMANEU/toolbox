---
title: "Navigation Route Generator"
weight: 2
description: "Generation of Navigation Route"
license: "https://img.shields.io/badge/License-Copyright%20%C2%A9-red"
trl: "TRL https://img.shields.io/badge/TRL-7-green"
link: ""
github: ""
---

## Name
Generation of Navigation Route

## Description
This component generates a route from a starting pose to a goal one, given a 2D geometric map of the environment. The route is optimized according to different configuration parameters, and guarantees collision avoidance along the movement with static obstacles present in the map.

### Key Features:
- Based in ROS2 route planning strategies
- Computes a collision-free trajectory in 2D
- Configurable via YAML parameter files
- Compatible with static obstacles of different shapes and sizes

## Type
Tool

## Layer
Service

## HRL
- 2.1 Navigation planning
- 2.3 Autonomous navigation

## Partners
![ITA Logo](/images/ita/italogo.jpg)

## Pilot

In the framework of the pilot, this module allows the user to check the navigation trajectory of the platfform before executing it. It also enables the configuration of different optimization parameters for modifying the geometry if the resulting trajectory.
