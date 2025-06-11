---
title: "BlackBox Service"
weight: 2
description: "BlackBox service for auditing"
license: "https://img.shields.io/badge/License-Apache%202.0-yellowgreen"
trl: "https://img.shields.io/badge/TRL-7-green"
link: "https://github.com/COGNIMANEU/pilot02-service-blackbox"
github: "https://github.com/COGNIMANEU/pilot02-service-blackbox"
---

## Name
BlackBox Service for auditing

## Description
The Blackbox component is a ROS 2 node designed to passively monitor specified topics and persist recent messages to disk upon request. This is particularly useful for post-mortem analysis, debugging, or system auditing.

## Features
- Passive message capture on configurable ROS 2 topics.
- Crash service that dumps buffered messages to disk.
- Supports CSV, SQLite (DB3), and MCAP output formats.
- Configurable limits for: maximum number of recent messages (max_messages) and maximum message age in seconds (max_seconds).

## Type
Tool

## Layer
Service 

## HRL
All 

## Partners
![ITA Logo](/images/ita/italogo.jpg)

## Pilot
This component enables blackbox-style logging of all configured ROS 2 topics, allowing for post-event analysis and system auditing. It captures the most recent messages prior to a failure or crash, making it easier to diagnose root causes and improve system reliability. The component is designed to be reusable across different ROS-based pilot projects that require traceability and fault investigation.