---
title: "Face Blurring"
weight: 2
description: "A modular face anonymization system for ROS2"
license: "https://img.shields.io/badge/License-AGPL%20v3-blue.svg"
trl: "https://img.shields.io/badge/TRL-7-green"
link: "https://github.com/COGNIMANEU/pilot02-ssh-faceblurring"
github: "https://github.com/COGNIMANEU/pilot02-ssh-faceblurring"
---

## Name
Face Blurring

## Description

This component provides a modular and configurable face anonymization system for use in ROS2 environments. It ensures privacy by detecting and blurring faces in video streams using various supported backends. Designed for flexibility, it enables switching between different face detection algorithms and anonymization styles based on the performance and accuracy needs of the deployment.

## Features

- Modular face detection and anonymization pipeline.
- ROS2 integration for processing image topics in real time.
- Supports video files, live streams, and raw image frames.
- Dockerized setup for easy deployment and testing.
- Graceful fallback to original frames on failure.

## Supported Blurring Methods

- **Haar Cascades (OpenCV)**  
  Classical real-time face detection suitable for low-resource systems.

- **YOLOv5 (Ultralytics)**  
  Deep-learning detector offering high accuracy and performance.  
  [GitHub →](https://github.com/ultralytics/yolov5)

- **MTCNN**  
  A multi-task cascaded convolutional network optimized for face detection.  
  [GitHub →](https://github.com/ipazc/mtcnn)

- **deface**  
  Command-line anonymization tool supporting multiple filter modes (blur, mosaic, solid).  
  [GitHub →](https://github.com/ORB-HD/deface)

![Face Blurring Demo](/images/ita/pilot02-ssh-faceblurring.gif)

## Type
Tool

## Layer
Connectivity

## HRL
2.8

## Partners
![ITA Logo](/images/ita/italogo.jpg)

## Pilot
This component enables face anonymization for images and videos captured by sensors before being sent to the cloud's digital twin. It uses various techniques to ensure privacy, applying different face detection and anonymization methods to blur or obscure facial features, guaranteeing that sensitive personal data is protected in the digital representation.