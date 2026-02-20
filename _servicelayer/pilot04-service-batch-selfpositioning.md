---
title: "DataMatrix Decoder & Digital Twin Generator"
weight: 99
description: "Automatically detect and track DataMatrix-coded objects in video to create a digital inventory twin"
license: "https://img.shields.io/badge/License-Apache%202.0-yellowgreen"
trl: "https://img.shields.io/badge/TRL-7-green"
github: "https://github.com/COGNIMANEU/pilot04-service-barcode-detection.git"
---

One-line value proposition: Transform video footage of stacked, barcoded inventory into a structured digital twin that tells you exactly what you have and where it is.

## Name
**DataMatrix Decoder & Digital Twin Generator**

## Overview
This tool automatically detects DataMatrix codes on objects in video footage—such as stacked timber logs or pipes—and reconstructs their spatial relationships into a logical "Digital Twin." Designed for warehouse managers and logistics operators, it eliminates manual inventory counting and provides immediate visibility into your stock layout, even when objects are stacked in complex grid or pyramid formations.

## Key Features
- **High-Speed Parallel Processing**: Analyzes multiple regions simultaneously using all CPU cores, enabling rapid processing of large video files
- **Robust Camera Tracking**: Compensates for camera movement (pan, tilt, zoom) using optical flow tracking, ensuring consistent object identification across the entire video sequence
- **Automatic Layout Detection**: Intelligently determines whether your stack follows a grid or pyramid pattern and assigns logical row/column coordinates to each item
- **Visual Verification**: Generates annotated frames and stitched panoramas so you can visually confirm detection accuracy
- **Resilient Tracking**: Seamlessly handles objects that temporarily disappear or new items that enter the frame mid-scan

## What Goes In / What Comes Out

### Input
- Video footage showing stacked objects marked with DataMatrix codes (timber logs, pipes, boxes, etc.)
- Optional: Directory of sequential images instead of video

### Output
- **Digital Twin JSON**: Structured data file containing every detected object with its unique ID, logical position (row/column), and neighbor relationships
- **Annotated Visual Frames**: Images with detection overlays for manual verification
- **Debug Visualizations** (optional): Stitched panorama, spatial graph, and logical grid representations

## How It Works
Think of it like a smart scanner that watches a video of your inventory and creates a map. As the camera moves across your stack, the tool tracks each frame's position, reads the DataMatrix codes it can see, and figures out how items relate to each other spatially. It then builds a logical coordinate system—like a spreadsheet grid—showing exactly where each item sits in the stack, even if you can't see all the codes at once.

## Use Cases
- **Timber Yard Inventory**: A logistics operator scans a video of stacked logs to automatically generate a complete inventory list with each log's position in the stack, eliminating manual counting and reducing errors
- **Warehouse Auditing**: A warehouse manager verifies stock levels by walking through aisles with a camera; the tool reconstructs the complete inventory layout for comparison against the warehouse management system
- **Shipping Verification**: Before dispatch, a supervisor scans loaded pallets to confirm all items are present and correctly positioned, catching misplacements before they leave the facility

## Partners
Montimage, NORCE, IBM, ABS

## Pilot
**Pilot 04 (Timber/Logistics)** — This tool is deployed for tracking timber logs marked with DataMatrix codes. It enables accurate inventory management of stacked logs in storage yards by automatically reading barcodes and determining each log's position within the stack structure.

## License
[Apache License 2.0](LICENSE)

## TRL
**TRL 7 — System prototype demonstration in operational environment**

The tool has been developed as a complete, functional prototype with automated installation scripts for Windows, Linux, and macOS. It has been tested with real video data and produces validated digital twin outputs, demonstrating readiness for deployment in operational timber and logistics scenarios.


