---
title: "Real-Time ROS2 Board"
weight: 2
description: "Real-Time viewer of ROS2 in a web-based board"
license: "https://img.shields.io/badge/License-BSD%203--Clause-blue"
trl: "https://img.shields.io/badge/TRL-7-green"
link: "https://github.com/COGNIMANEU/pilot02-digitaltwin-rosboard"
github: "https://github.com/COGNIMANEU/pilot02-digitaltwin-rosboard"
---

## Name
Real-Time ROS2 Board

## Description

This component provides a web based visualization tool for ROS2 environments. It builds upon the original ROSboard (https://github.com/dheera/rosboard) project by adding project-specific visual branding and improving error handling during ROS2 message reception. These enhancements allow the component to log exceptions gracefully without interrupting data flow, increasing reliability during runtime.

## Features
- Web-based visualization of ROS1/ROS2 topics
- Mobile-friendly interface
- Lightweight and resource-efficient
- Compatible with live ROS nodes and ROS bag file playback
- Easily extensible with custom .js visualizations

![ROSBoard Demo](/images/ita/pilot02-digitaltwin-rosboard.png)

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