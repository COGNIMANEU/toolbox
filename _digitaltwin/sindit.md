---
title: "SINDIT"
date: 2024-01-16T12:00:00+00:00
weight: 1
description: "Knowledge Graph Based Digital Twin Framework."
license: "https://img.shields.io/badge/license-MIT-blue"
trl: "https://img.shields.io/badge/TRL-4-yellow"
link: "https://sindit.sintef.cloud/"
github: "https://github.com/SINTEF-9012/SINDIT"
---

Knowledge Graph Based Digital Twin Framework

## Name
SINDIT - **SIN**TEF **Di**gital **T**win 

## Defined in Task
Task 2.2 - COGNIMAN Toolbox and Architectural Framework

## Description
SINDIT covers aspects related to Digital Twin data representation (graph-based data structures for assets data and processes), data storage (assets and time-series data), and support for discrete/continuous simulation (e.g., estimation of production capacity).

The purpose of the framework is to provide the mechanisms to represent and store data in a way that can capture assets and time-series data, while at the same time can offer efficient access to the data and ability to use the stored data for various types of simulations (discrete/flow).

The framework is meant to help factories IT personnel in the process of representing assets and processes within factories and storing data about them, and combining the information with real-time sensor data, to facilitate analytics tasks such as simulations.

Figure 1 provides illustration of the four-layer software architecture of SINDIT along with various technologies deployed in the stack. The data layer contains all persistent storage back-ends – both those managed by SINDIT as well as those managed by third parties. The business layer contains (i) descriptions of machines and processes, (ii) services for event detection and capacity estimation, and (iii) ingestion of and federated access to relevant data sources. The application layer exposes the relevant outputs of the business logic. These can be consumed either by SINDIT’s own presentation layer or by authorized third parties. The physical assets comprise the physical layer which is not discussed here.

![SINDITArchitecture](images/sindit/SINDIT_software_architecture.png)

## License
MIT License

## Pilot
To be used in Pilot 1 and 4.

## References
