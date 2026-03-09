---
title: "Barcode Detection and Batch Positioning"
weight: 99
description: "Automatically identify and map stacked objects from video footage into a structured digital layout"
license: "https://img.shields.io/badge/License-MIT-yellow"
trl: "https://img.shields.io/badge/TRL-7-green"
github: "https://github.com/COGNIMANEU/pilot04-service-barcode-detection"
---

Automatically identify and map every marked object in a stack — from a simple camera scan to a complete spatial inventory.

## Name

Barcode Detection and Batch Positioning

## Overview

When stacked objects like timber logs or pipes carry DataMatrix barcodes, keeping track of what is where is a time-consuming manual task. This tool automates it: point a camera at the stack, record a video (or take photos), and receive a complete spatial map showing each object's identity, position, and neighbors. The result is a machine-readable "Digital Twin" of the physical stack that downstream systems can use for logistics, quality control, or inventory management.

## Key Features

- **Hands-free inventory from video**: Walk along a stack with a camera and get a complete object map — no manual barcode scanning required
- **Works in tough conditions**: Multiple image processing strategies adapt to varying lighting, worn-out labels, and curved surfaces typical of industrial environments
- **Understands stack geometry**: Automatically distinguishes between rectangular grids and staggered pyramid arrangements, producing accurate position data for either layout
- **Fast parallel processing**: Leverages all available CPU cores to scan multiple regions simultaneously, keeping up with real-time video input
- **Flexible input options**: Accepts live video files, pre-captured image sets, or individual photos — fits into existing capture workflows
- **Visual verification**: Produces annotated frames with detection overlays so operators can visually confirm results before acting on them

## What Goes In / What Comes Out

### Input

- **Video footage** of a stack of marked objects (e.g., an operator walking along a timber log stack with a handheld or mounted camera)
- **Photographs** of marked objects — either a single image or a folder of images captured from different angles
- Objects must carry **DataMatrix barcodes** that are visible in the footage

### Output

- **Spatial inventory file** (`output.json`): A structured file listing every detected object with its unique barcode ID, logical grid position (column and row), and links to all neighboring objects (up, down, left, right, and diagonals for pyramid stacks)
- **Annotated frames** (`frames/`): Images from the video with green markers highlighting each detected barcode and its ID — ready for operator review
- **Debug visualizations** (optional): Logical grid diagram, binary detection masks, and per-frame performance metrics for quality assurance

## How It Works

The tool processes video frame by frame. For each frame, it identifies bright regions that may contain barcodes, then sends each region to a parallel decoding pipeline that tries multiple image enhancement techniques to read the DataMatrix code — even under poor lighting or on curved surfaces. As new frames arrive, the tool builds up a growing map of which objects sit next to which. Once all frames are processed, it uses this neighbor information to determine whether the stack is a rectangular grid or a staggered pyramid, then assigns logical coordinates to every object. The final output is a structured file that any warehouse system, ERP, or visualization tool can consume.

## Use Cases

- **Timber yard inventory**: A forestry logistics operator records a slow pan along a stack of timber logs, each stamped with a DataMatrix code. Within minutes, the tool produces a complete spatial map of the stack — identifying every log and its exact position — eliminating hours of manual scanning and data entry.

- **Quality inspection of pipe stacks**: A quality engineer photographs a shipment of industrial pipes arranged in a pyramid stack. The tool detects each pipe's barcode and reconstructs the pyramid layout, enabling the engineer to cross-reference positions against the shipping manifest and flag any misplaced items.

- **Automated warehouse cataloguing**: A camera mounted on a forklift continuously captures footage as it moves through a storage area. The tool processes the video and generates per-stack inventory files that feed directly into the warehouse management system, keeping digital records in sync with physical reality.

## Partners

NORCE

## Pilot

**Pilot 4** — Timber and log stack processing. This tool serves as the barcode detection and spatial mapping service within the Pilot 4 workflow, converting raw camera footage of marked timber stacks into structured digital inventory data that downstream planning and logistics services can consume.

## License

[MIT License](LICENSE) (project code) | [BSD 2-Clause](LICENSE) (libdmtx dependency)

## TRL

**TRL 7** — System prototype demonstrated in an operational environment. The tool includes cross-platform automated installers (Windows, Linux, macOS), handles real-world video input with adaptive detection strategies, and produces production-ready structured output.

## References

[1] A. Belbachir, A. M. Ortiz, E. T. Hauge, A. N. Belbachir, G. Bonanno, E. Ciccia, G. Felline, "Drone Technology for Efficient Warehouse Product Localization," ICINCO (2), pp. 357-364, 2024.

[2] A. Belbachir, A. M. Ortiz, E. T. Hauge et al., "Outdoor Warehouse Management: UAS-Driven Precision Tracking of Stacked Steel Bars," SN Computer Science, vol. 6, 701, 2025. https://doi.org/10.1007/s42979-025-04206-8
