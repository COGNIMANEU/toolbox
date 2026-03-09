---
title: "Manufacturing Assistant System (MAS)"
weight: 99
description: "Manage metal 3D printing end-to-end — from job prep to robotic post-processing and quality"
license: "https://img.shields.io/badge/License-Copyright%20%C2%A9-red"
trl: "https://img.shields.io/badge/TRL-7-green"
github: "https://github.com/COGNIMANEU/pilot03-interface-additive-manufacturing-process-management"
---

Gives additive manufacturing operators a single screen to manage every step of metal 3D printing — uploading job cards, monitoring the build in real time, dispatching robots for post-processing, and reviewing quality across every part and layer.

## Name

MAS — Manufacturing Assistant System

## Overview

Metal additive manufacturing involves dozens of handoffs between job preparation, the printing process itself, robotic post-processing, and quality inspection. MAS brings all of these stages into one web-based control panel so operators never lose track of where a session stands. Upload a paper job card, watch the build progress layer by layer, send robots to remove parts from the build plate, and review quality dashboards — all without switching tools.

## Key Features

- **Guided 4-Stage Workflow**: Walk each manufacturing session through pre-printing, printing, post-printing, and termination with enforced step-by-step transitions — so nothing gets skipped or done out of order.
- **Paperless Job Card Intake**: Upload a scanned job card PDF and get structured job data back automatically — barcodes, QR codes, and text in English, French, German, or Spanish are all recognized.
- **Intelligent Build Plan Review**: Upload a build plan CSV and receive a full statistical analysis with interactive 2D and 3D visualizations of part placement on the build plate, then approve or re-upload before production begins.
- **Real-Time Print Monitoring**: Follow the printing process layer by layer with live progress updates, alerts, and per-layer quality metrics — catch problems while there is still time to act.
- **Robotic Post-Processing Control**: Assign a robot to a session and orchestrate part removal, support removal, inspection, and storage operations for each part — with live progress, automatic error recovery, and detailed operation logs.
- **Quality Dashboards**: Review quality at every level — session overview, layer-by-layer defect analysis, and individual part scoring — to make informed accept/reject decisions.
- **Operations Analytics**: Track how many operations each part went through, identify repeat operations, and view summary metrics across the entire session.
- **Alert Management**: Create, track, and resolve alerts (informational, warning, or error) scoped to each session stage, so issues are visible to everyone on the team.
- **Role-Based Access**: Admins, operators, and read-only service accounts each see exactly what they need — no more, no less.

## What Goes In / What Comes Out

### Input

- **Job card PDFs** — scanned paper job cards from the shop floor, in any of four supported languages
- **Build plan CSVs** — machine-generated build plan files describing part positions, layer counts, and thicknesses
- **Robot status updates** — real-time presence, progress, and event messages from robot controllers on the shop floor
- **Operator decisions** — build plan approvals, robot assignments, alert resolutions, and quality accept/reject actions

### Output

- **Structured job data** — automatically extracted job numbers, quantities, delivery dates, and operations from scanned job cards
- **Build plan analysis** — statistical summaries, quality maps, and interactive 3D visualizations of the build plate
- **Robot commands** — prepare, start, pause, and stop instructions sent to robot controllers for each post-processing operation
- **Quality reports** — per-session, per-layer, and per-part quality scores, defect metrics, and operation history
- **Operational dashboards** — real-time printing progress, operations analytics, and alert summaries accessible from any browser

## How It Works

Think of MAS as a digital clipboard that follows a manufacturing job from start to finish. When an operator creates a new session, MAS guides them through a checklist: first upload the job card (the system reads it automatically using optical character recognition), then upload the build plan (a digital twin analyzes it and shows a 3D preview of what will be printed). Once the operator approves the plan, MAS switches to a live monitoring view during printing. After printing finishes, the operator assigns a robot and MAS orchestrates the post-processing steps — removing parts from the build plate, stripping supports, inspecting, and storing — while streaming progress back to the dashboard in real time. At any point, quality dashboards let the team drill into layer-level or part-level metrics.

## Use Cases

- **Pre-shift job setup**: A morning-shift operator receives a stack of paper job cards. Instead of manually entering data, they scan each card as a PDF and upload it to MAS. Within seconds, the system extracts job numbers, quantities, and delivery dates — ready for the supervisor to review and approve the build plan in 3D before the machine starts.

- **Unattended print monitoring**: During an overnight build, MAS tracks layer-by-layer progress and fires alerts when quality metrics drift. The on-call engineer checks the dashboard from a tablet and sees exactly which layer triggered the warning, without walking to the machine.

- **Robotic post-processing coordination**: After a 200-part build completes, the post-processing operator assigns a robot through MAS and starts operations part by part. MAS sends commands to the robot, streams live progress, and automatically schedules recovery if the robot encounters an error — turning a complex multi-hour process into a supervised, step-by-step workflow.

## Partners

Montimage, CROOM, IRT, NORCE

## Pilot

Pilot 03 — Additive Manufacturing Process Management. MAS serves as the primary operator interface for Pilot 03, providing the human-machine interaction layer through which operators prepare jobs, monitor builds, coordinate robotic post-processing, and assess part quality across the full metal additive manufacturing workflow.

## License

Montimage Proprietary License — Copyright (c) 2024 Montimage. All rights reserved. See [LICENSE](LICENSE) for full terms.

## TRL

**TRL 7** — System prototype demonstrated in an operational environment. MAS is a fully functional web application tested in realistic additive manufacturing scenarios with end-to-end workflows: job card OCR, digital twin build plan analysis, real-time print monitoring, robotic post-processing with live MQTT communication, quality dashboards, and comprehensive end-to-end test coverage.

## References

