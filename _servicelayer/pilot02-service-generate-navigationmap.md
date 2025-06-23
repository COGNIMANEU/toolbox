---
title: "Navigation Map Generator"
weight: 2
description: "Generation of navigation map (2D) from geometric map (3D)"
license: "https://img.shields.io/badge/License-Copyright%20%C2%A9-red"
trl: "TRL https://img.shields.io/badge/TRL-7-green"
link: ""
github: ""
---

## Name
Generation of navigation map (2D) from geometric map (3D)

## Description
This component enables 2D geometric maps to be built from 3D metric-semantic models for use in 2D navigation and planning algorithms. This is achieved through a careful flattening process of the geometric information.

### Key Features:
- Creates a 2D geometric navigation map of the environment
- Supports 3D maps in multiple formats as input
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

This component enables navigation features by creating a 2D map of the environment from an existing 3D map, which the agent can then use to compute and execute trajectories in order to fulfil a given goal. This component acts as an intermediary between the full 3D reconstruction of the environment and the necessary navigation features.
