---
title: Manufacturing Assistant System (MAS)
weight: 99
description: Real-time monitoring and control system for additive manufacturing with digital twin integration
license: Apache-2.0
license_url: https://opensource.org/licenses/Apache-2.0
trl: 7
trl_url: https://creativecommons.org/licenses/by/4.0/
link: 
github_url: https://github.com/COGNIMANEU/pilot03-interface-additive-manufacturing-process-management
---

## One-line Value Proposition

Enables real-time monitoring and control of additive manufacturing processes, integrating job card OCR, digital twin predictions, and robot operations in a single dashboard for plant operators.

## Name

**Manufacturing Assistant System (MAS)** — A web-based monitoring and control interface for additive manufacturing workflows.

## Overview

MAS provides plant operators with a unified dashboard to monitor, control, and optimize 3D printing operations in real-time. The system extracts job specifications from scanned documents using OCR, correlates them with live sensor data, and presents actionable insights through an intuitive web interface. By bridging the gap between physical printing and digital twin predictions, operators can make informed decisions to reduce waste and improve yield.

## Key Features

- **4-Stage Workflow Management** — Guide operators through setup, printing, cooling, and extraction phases with clear status indicators and step-by-step instructions
- **Job Card Digitization** — Automatically extract print specifications from PDF documents and barcodes, eliminating manual data entry errors
- **Live Build Monitoring** — Track temperature, chamber conditions, and print progress in real-time with visual dashboards
- **Robot Command Interface** — Send and receive commands to the 3D printer robot arm directly from the control panel
- **Digital Twin Integration** — Compare actual print progress against ML-predicted outcomes to detect anomalies early
- **Quality Analytics** — View historical performance metrics and identify patterns that impact product quality

## What Goes In / What Comes Out

### Input

- **PDF Job Cards** — Scanned manufacturing orders containing print parameters, material specs, and part designs
- **Barcode Data** — Machine-readable identifiers linking physical print jobs to digital records
- **Sensor Streams** — Real-time temperature, pressure, and position data from the 3D printer
- **MQTT Commands** — Control messages from external systems or robot controllers

### Output

- **Operator Dashboard** — Visual display of current job status, next steps, and alerts
- **Job Status Reports** — Summary of completed prints with quality metrics and timestamps
- **Robot Commands** — Start, pause, resume, and stop instructions sent to the printer
- **Analytics Views** — Historical trends, yield statistics, and anomaly alerts

## How It Works

The system acts as a central hub connecting physical manufacturing equipment with digital workflows. When a job card arrives, the OCR service reads the specifications and creates a digital job record. As printing begins, sensor data flows via MQTT to the server, where it's stored in MongoDB and displayed on the React dashboard. The digital twin module runs predictions in Python, comparing expected vs. actual progress and flagging deviations. Operators interact through the web interface to monitor progress, acknowledge alerts, and send commands back to the robot.

## Use Cases

### Use Case 1: New Operator Running First Print
**Who:** A plant operator with limited experience  
**Situation:** Received a new job card for a complex aerospace component  
**Outcome:** The system walks them through each workflow stage, displays the extracted parameters on screen, and highlights when the digital twin predicts potential issues — preventing a failed print worth €2,000 in materials.

### Use Case 2: Night Shift Anomaly Detection
**Who:** Remote monitoring supervisor  
**Situation:** Overnight printing session with no staff on site  
**Outcome:** MAS sends alerts when temperature exceeds thresholds, logs all events for post-incident review, and automatically pauses the print to prevent damage until the on-call team responds.

### Use Case 3: Process Optimization Review
**Who:** Production manager  
**Situation:** Quarterly review of manufacturing efficiency  
**Outcome:** The analytics dashboard reveals that 15% of delays occur during the cooling phase, enabling targeted workflow improvements that increase overall throughput by 8%.

## Partners

- **Montimage** — Core system development, React frontend, Node.js backend
- **Croom** — Digital twin integration, ML model development
- **IRT** — Technical contribution and validation

## Pilot

**Pilot 3 — Additive Manufacturing**  
MAS serves as the primary operator interface for the additive manufacturing cell, providing real-time visibility into print processes and enabling direct robot control from a centralized dashboard.

## License

**Apache License 2.0**  
See the [LICENSE](https://github.com/COGNIMANEU/pilot03-interface-additive-manufacturing-process-management/blob/main/LICENSE) file for details.

## TRL

**Level 7 — System Prototype Operational**  
The system has been demonstrated in an operational environment (real manufacturing setting). It includes full workflow integration with robot control, OCR processing, and digital twin predictions running in a representative production scenario.

## References

[1] COGNIMAN Project — https://cogniman.eu

