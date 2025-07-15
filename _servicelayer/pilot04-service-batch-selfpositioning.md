---
title: "Batch Self-positioning Service"
weight: 4
description: "Batch Self-positioning positionning"
license: "https://img.shields.io/badge/License-Copyright%20%C2%A9-red"
trl: "TRL https://img.shields.io/badge/TRL-6-green"
link: ""
github: ""
---

## Name
Batch Self-positioning Service

## Description
This system provides autonomous batch positioning using drones equipped with cameras to capture product positions. It supports QR codes and a novel trust-ability scoring system to ensure precise relative positioning in outdoor warehouse environments.

### Key Features:

- Image-based positioning system
- Infrastructure-free operation (no GPS or external anchors required)
- QR code-based product identification
- Trust-ability scoring to ensure the reliability of position data

## Type
Tool

## Layer
Service

## HRL
- 4.2.1 Real position of batches, introducing the Y dimension (ground clearance of the bar) 

## Partners
NORCE

## Pilot
This component allows positioning of batches in outdoor stacks using front images captured by drones. 
The system autonomously scans a designated area, detects QR codes for product identification, and calculates the spatial relationships between batches. 
