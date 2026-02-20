---
title: "AM Printing Process Digital Twin"
weight: 99
description: "AI-powered quality monitoring for additive manufacturing detecting defects in powder and melt layers"
license: "https://img.shields.io/badge/License-Apache%202.0-yellowgreen"
trl: "https://img.shields.io/badge/TRL-7-green"
github: "https://github.com/COGNIMANEU/pilot03-digitaltwin-am-printing-process"
---

Detects and classifies defects in 3D printed parts before they become costly failures, reducing scrap rates and rework.

## Name

AM Printing Process Digital Twin — Comprehensive Additive Manufacturing Analysis System

## Overview

This digital twin enables manufacturing engineers to monitor and analyze the quality of additive manufacturing (3D printing) processes in real time. By automatically detecting defects such as porosity, balling, and fusion issues in each printing layer, operators can identify problems early and take corrective action before wasting expensive materials. The system processes images from powder coating and laser melting stages, combining traditional image analysis with advanced AI models to provide comprehensive quality assurance.

## Key Features

- **Automated Defect Detection**: Identifies porosity, balling, and fusion defects in powder and melted layer images within seconds, enabling immediate corrective action
- **AI-Powered Analysis**: Uses deep learning models (Multi-Modal ConvLSTM) to detect anomalies that traditional methods may miss, improving detection accuracy
- **Part Quality Mapping**: Links quality metrics to individual parts based on build plan data, helping pinpoint which specific components failed
- **Hybrid Powder Coverage Analysis**: Combines image segmentation with coordinate-based mapping to ensure 100% part coverage analysis
- **Real-Time and Offline Modes**: Supports both batch analysis of completed builds and live monitoring of ongoing printing sessions
- **Comprehensive Reporting**: Generates detailed layer-by-layer reports and executive summaries for quality teams and management

## What Goes In / What Comes Out

### Input

- Powder layer images from the powder spreading station (JPEG format)
- Melted layer images from the laser melting process (JPEG format)
- Laser packet data files containing power and speed parameters
- Build plan CSV files with part placement and configuration data

### Output

- Defect classification reports for each layer (Porosity, Balling, Fusion, or No Defect)
- Quality scores and severity ratings for each printed part
- Visual maps showing defect locations across the build plate
- Statistical summaries comparing quality across layers and builds
- Executive reports suitable for management review

## How It Works

The system acts as a virtual quality inspector that watches every layer of a 3D print job. It captures images at two critical stages: after powder is spread but before melting, and after the laser has melted the powder. These images are analyzed using both traditional computer vision techniques and AI models trained to recognize common defect patterns. The system correlates findings with laser processing data to understand why defects occurred. Results are organized by individual parts using the build plan, so operators know exactly which components need inspection or rework.

## Use Cases

- **Scenario**: A quality engineer at an aerospace additive manufacturing facility needs to verify the integrity of 3D-printed turbine components before expensive post-processing.
- **Outcome**: The system scans all 200+ layers of the build, flags three layers with elevated porosity risk, and identifies the specific parts affected. The engineer can focus inspection efforts on those parts, reducing inspection time by 70%.

- **Scenario**: A production manager wants to understand why recent builds have shown increasing failure rates to adjust printer parameters.
- **Outcome**: The system provides statistical trend analysis across multiple builds, showing that powder coverage uniformity has degraded over the past two weeks, suggesting the powder recycling process needs attention.

- **Scenario**: An operator running a 48-hour metal printing job needs to know immediately if something goes wrong.
- **Outcome**: The online monitoring mode detects an anomaly in layer 156, alerts the operator, and generates a detailed report before the build completes—saving potentially thousands of euros in wasted material.

## Partners

- Montimage
- CROOM

## Pilot

Pilot 3 — Additive Manufacturing Printing Process. This tool serves as the core quality monitoring system for the AM printing pilot, providing real-time defect detection and comprehensive analysis capabilities that enable the pilot to demonstrate closed-loop quality control in metal additive manufacturing.

## License

Apache 2.0 — [LICENSE](https://github.com/COGNIMANEU/pilot03-digitaltwin-am-printing-process/blob/main/LICENSE)

## TRL

TRL 7 — System prototype has been demonstrated in an operational environment. The project includes comprehensive test suites, automated quality gates (linting, security scanning), pre-commit hooks, and fully functional AI models with both statistical and deep learning analysis modes.


