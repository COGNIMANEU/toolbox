---
title: "Batch identification"
date: 2024-10-24T10:59:53+00:00
weight: 4
description: "The system must be able to acquire the batch 'code' at least in the 90% of cases (ABS Pilot)"
license: "https://img.shields.io/badge/License-Unlicense-lightgrey"
trl: "https://img.shields.io/badge/TRL-6-red"
link: ""
github: ""
---

## Name
Batch identification

## Description
This tool is developed to automatically identify the batch code associated with stacked materials—such as steel bars—in the ABS Pilot. The batch code is a critical identifier used for tracking, traceability, and quality assurance within the industrial workflow.

The system processes image data captured from cameras positioned above or near the material stacks. It detects and extracts the batch code, which may be printed, tagged, or embedded via QR/2D codes. The detection pipeline is designed to achieve at least 90% successful identification under realistic conditions, including variable lighting, partial occlusion, and material placement inconsistencies.

By automating batch identification, the system reduces the need for manual input, lowers the risk of data entry errors, and ensures that materials are correctly logged and traced throughout the production and logistics process. This functionality plays a key role in maintaining end-to-end visibility and compliance in the ABS Pilot scenario.

## Type
Tool

## Layer
DTR

## HRL
4.1.3

## Partners
NORCE, MI

## Pilot
To be used in Pilot 4 (ABS pilot)
