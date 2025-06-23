---
title: "Semantic Map Generator"
weight: 2
description: "Generation of geometric & semantic map (3D) from previously recorded data"
license: "https://img.shields.io/badge/License-Copyright%20%C2%A9-red"
trl: "TRL https://img.shields.io/badge/TRL-7-green"
link: ""
github: ""
---

## Name
Generation of geometric & semantic map (3D) from previously recorded data

## Description
This component serves to create a 3D model of the environment from previously recorded sensor data (bag files). This includes both geometric and semantic representations of the environment, enabling subsequent tasks such as navigation.

### Key Features:
- Creates a metric-semantic 3D model of the environment
- Supports heterogeneous sensor data
- Robust to different sensor setups
- Configurable via YAML parameter files

## Type
Tool

## Layer
Service

## HRL
-	2.3 Autonomous navigation
-	2.6 Context & safety awareness
-	2.7 Semantic map generation


## Partners
![ITA Logo](/images/ita/italogo.jpg)

## Pilot

This component builds metric-semantic maps of the environment from raw sensory data. These maps can later be used for subsequent tasks, such as navigation and obstacle avoidance. It is a crucial part of the system that is responsible for understanding the space observed by the agent.
