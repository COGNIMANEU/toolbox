---
title: "Top-View Safety Evaluation"
weight: 99
description: "Automated drone-based safety assessment of material stacks in industrial warehouses"
license: "https://img.shields.io/badge/License-Copyright%20%C2%A9-red"
trl: "https://img.shields.io/badge/TRL-7-green"
github: "https://github.com/COGNIMANEU/pilot04-service-safety-evaluation-top-view"
---

Automatically verify that material stacks in industrial warehouses are properly supported -- using drone images and videos instead of manual walkarounds.

## Name

Top-View Safety Evaluation Service

## Overview

Industrial warehouses store heavy material stacks -- steel beams, timber bundles, pipe packs -- that must be held in place by support structures to prevent collapse. Verifying these supports today means sending inspectors on foot, a process that is slow, subjective, and sometimes hazardous. This service replaces that manual check with an AI-powered analysis of top-down drone data, delivering a clear SAFE or UNSAFE verdict for every stack in view.

## Key Features

- **Instant safety verdicts**: Get a SAFE/UNSAFE classification for each material stack, so warehouse managers can act immediately rather than waiting for inspection reports.
- **Image and video support**: Analyse individual drone images or full video recordings of a drone flyover -- each frame is evaluated and the results are compiled into a single overview.
- **Works from standard drone cameras**: No specialised sensors needed -- any commercial drone capturing top-down data is sufficient.
- **Configurable safety rules**: Adjust how many support structures are required and where they must be located, matching your warehouse's specific safety standards.
- **Visual evidence**: Every verdict comes with colour-coded annotations overlaid on the original image or video, making it easy to see exactly which supports were detected and where.
- **Runs without cloud access**: All processing happens locally on your own hardware, keeping warehouse data private and eliminating network dependencies.

## What Goes In / What Comes Out

### Input

Top-down drone images or videos of material stacks in an industrial warehouse. The data should be captured from directly above, showing the stack and its surrounding support structures.

### Output

- A **SAFE or UNSAFE verdict** for each material stack indicating whether it has adequate support.
- **Annotated images** with colour-coded overlays: blue for safe stacks, red for unsafe stacks, green for detected support structures.
- **Annotated videos** where each frame carries the same colour-coded safety overlay, providing a continuous visual record of the entire flyover.
- A **structured result** with the verdict and number of supports detected -- ready for integration with warehouse management dashboards.
- A **batch summary** when processing multiple images, giving a quick overview of the entire survey.

## How It Works

The service takes a drone image or video and uses an AI vision model to identify every distinct object in each frame. It filters out the ground and background, isolates the main material stack, and searches for support structures nearby -- recognising them by their characteristic size and position relative to the stack. Each frame is divided into a top zone and a bottom zone, and the system counts how many supports appear in each. If both zones have enough supports, the stack is classified as safe; otherwise, it is flagged as unsafe. For videos, the process runs frame by frame and the annotated results are reassembled into an output video.

## Use Cases

- **Daily warehouse inspection**: A warehouse safety officer flies a drone over the storage yard each morning. The footage is processed automatically, producing an annotated video and summary report that highlights any stacks needing attention before work begins.
- **Post-delivery verification**: After a new batch of steel beams is delivered and stored, the logistics coordinator captures a quick overhead image and checks the verdict to confirm the supports were placed correctly before signing off the delivery.
- **Ongoing compliance monitoring**: A warehouse manager schedules weekly drone surveys. The system processes each survey and flags only the stacks whose safety status has changed, saving hours of manual re-inspection.

## Partners

NORCE

## Pilot

**Pilot 04 -- Industrial Warehouse Safety**: This tool is the core safety evaluation service for Pilot 04, responsible for automated assessment of material stack stability from aerial data captured by drones at the industrial warehouse.

## License

NORCE -- All rights reserved.

## TRL

**TRL 7** -- System prototype demonstrated in an operational environment. The tool has been validated with real drone data from industrial warehouses and features a production-ready architecture with comprehensive documentation and cross-platform support.

## References

[1] Assia Belbachir, Antonio M. Ortiz, Ahmed Nabil Belbachir, Emanuele Ciccia: Safety-Centric Monitoring of Structural Configurations in Outdoor Warehouse Using an UAV. ICINCO (2) 2025: 471-478
