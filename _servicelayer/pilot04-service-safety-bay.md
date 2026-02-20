---
title: "Top View Safety Evaluation"
weight: 99
description: "AI-powered drone safety analysis for construction sites - automatically detects unsafe material stacking"
license: "https://img.shields.io/badge/License-Apache%202.0-yellowgreen"
trl: "https://img.shields.io/badge/TRL-9-green"
github: "https://github.com/COGNIMANEU/pilot04-service-safety-evaluation-top-view"
---

Automatically detect unsafe material stacking on construction sites from drone imagery—prevent accidents before they happen.

## Name
Top View Safety Evaluation — AI-powered construction site safety analysis

## Overview
This tool analyzes aerial drone images of construction sites to automatically detect material stacks and evaluate their safety. Using advanced AI segmentation, it identifies whether stacks have adequate support structures and classifies them as SAFE or UNSAFE in real-time. Built for safety inspectors, site managers, and construction supervisors who need to monitor material storage compliance across large sites efficiently.

## Key Features

- **Automated Safety Assessment**: Analyze hundreds of drone images automatically without manual inspection—reduces safety audit time from days to hours
- **Visual Safety Reports**: Generates color-coded images showing SAFE stacks in blue and UNSAFE stacks in red with support structures highlighted in green
- **Smart Caching**: 100x faster reprocessing of the same site—perfect for continuous monitoring with daily drone flights
- **Flexible Integration**: Simple API for integration with existing HMI systems and safety management platforms
- **Multi-Model Support**: Choose between speed and accuracy with SAM 2 model variants optimized for your hardware
- **Configurable Thresholds**: Adapt detection parameters to match your specific safety requirements and site conditions

## What Goes In / What Comes Out

### Input
- Aerial drone images (JPG/PNG) captured from top-down view of construction sites
- Configuration parameters for detection sensitivity and safety criteria
- Optional: Previously analyzed images (for caching benefits)

### Output
- **Visual annotations**: Images with color-coded SAFE (blue) / UNSAFE (red) classifications and detected support structures (green)
- **JSON results**: Structured safety data including status, number of supports, and batch center coordinates
- **CSV reports**: Batch processing summaries for compliance documentation
- **Processing logs**: Human-readable analysis details for audit trails

## How It Works
Think of this tool as an automated safety inspector that never gets tired. Just as a human inspector would look at a material stack and count the support blocks touching it, this system uses AI to "see" the stack and its supports from drone photos. It filters out the ground and background, identifies material stacks, then counts how many support structures touch each stack in the critical top and bottom zones. If a stack has enough supports in both zones, it's marked SAFE—preventing potential collapses before they occur.

## Use Cases

- **Daily Safety Audits**: A construction site manager flies a drone over the material storage area each morning. Within minutes, they receive a complete safety report highlighting any stacks that need additional support before work begins.
- **Compliance Monitoring**: A safety officer needs to document material storage compliance for regulatory reporting. They process weeks of drone footage in a single batch, generating timestamped safety classifications for each stack.
- **Incident Prevention**: After a near-miss with a stack collapse on a previous project, a site supervisor implements automated daily scanning. The system flags an unsafe stack arrangement, allowing the crew to add supports before any incident occurs.

## Partners
- NORCE
- Montimage

## Pilot
This tool is deployed in **COGNIMAN Pilot 4** (Construction), where it performs automated safety evaluation of material stacks from drone imagery. It enables continuous safety monitoring of construction sites without requiring manual inspections, supporting safer work environments and regulatory compliance.

## License
[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)

## TRL
**TRL 9** — The tool has been proven in operational environments with comprehensive documentation, benchmarking capabilities, model validation frameworks, and production-ready APIs. It includes advanced features like result caching, configurable safety criteria, and integration interfaces suitable for industrial deployment.

## References
[1] Meta AI Research. [Segment Anything Model (SAM)](https://github.com/facebookresearch/segment-anything)
