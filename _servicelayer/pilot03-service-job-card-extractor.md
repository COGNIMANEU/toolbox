---
title: "Job Card Extractor"
weight: 99
description: "Automatically digitize paper job cards into structured data — eliminate manual data entry"
license: "https://img.shields.io/badge/License-Montimage-blue"
trl: "https://img.shields.io/badge/TRL-7-green"
github: "https://github.com/COGNIMANEU/pilot03-service-job-card-extractor"
---

Eliminate manual data entry from your shop floor by automatically reading scanned job cards and turning them into structured, machine-readable records.

## Name

Job Card Extractor

## Overview

Manufacturing shops rely on paper job cards to track production orders and operations. Manually keying in job numbers, quantities, and operation sequences from these cards is slow, error-prone, and creates bottlenecks in production planning. Job Card Extractor reads scanned or photographed job card PDFs and automatically produces structured digital records — giving you accurate production data in seconds instead of minutes.

## Key Features

- **Instant digitization of paper job cards**: Feed in a scanned PDF and receive a complete digital record of the job number, quantity, delivery date, and every listed operation — ready for your ERP or planning system.
- **Reliable barcode-to-operation matching**: Each operation is automatically linked to its corresponding barcode using multiple matching strategies, so you can track individual steps through the production floor.
- **Works with low-quality scans**: Advanced image preprocessing handles faded prints, skewed scans, and poor lighting conditions — no need to re-scan or invest in high-end scanning equipment.
- **Multi-language support**: Process job cards written in English, French, German, and 80+ other languages without switching tools.
- **Batch processing**: Process stacks of job cards in one go with built-in parallel processing, keeping up with high-volume production environments.
- **Confidence scoring**: Every extracted field comes with a confidence score, so you can flag uncertain readings for human review instead of trusting bad data.
- **Visual verification**: Generates annotated images highlighting detected areas, text regions, and barcodes — making it easy to spot and diagnose extraction issues.

## What Goes In / What Comes Out

### Input

Scanned or photographed job card PDFs — single-page or multi-page documents as typically found on a manufacturing shop floor. Supports standard barcode formats (Code128, Code39, EAN, UPC) printed on the cards.

### Output

A structured JSON file containing:
- **Job identification**: Job number, order quantity, and delivery date
- **Operation list**: Each manufacturing operation with its number, name, associated barcode value, and a confidence score
- **Quality report**: Processing metrics including barcode detection rate, OCR confidence, and per-operation success indicators

Optionally: annotated images for visual verification and detailed processing logs for auditing.

## How It Works

Think of it as a digital assistant that reads a job card the way an experienced operator would — but faster and without mistakes. The tool first converts each PDF page into an image, then identifies the horizontal dividing lines that separate operations on the card. Within each section, it simultaneously reads any printed barcodes and extracts text using optical character recognition. Finally, it matches each detected operation to its barcode using a smart fallback strategy: first trying an exact match, then looking in the same card section, and finally checking nearby sections. The result is a clean, structured record ready for downstream systems.

## Use Cases

- **Production digitization**: A shop floor supervisor at a metal fabrication plant receives a stack of 50 printed job cards for the week's orders. Instead of manually entering each job into the planning system, they scan the cards to PDF and run the extractor. Within minutes, all job numbers, operations, and barcodes are available as structured data ready for import.

- **Quality traceability**: A quality engineer investigating a defective batch needs to trace which operations were performed and in what order. By extracting the barcode associations from the original job card, they can cross-reference each production step with inspection records — without digging through paper files.

- **Legacy system migration**: A manufacturer transitioning from paper-based to digital job tracking has years of archived job cards. The batch processing capability allows them to digitize their historical records, building a searchable database of past production orders.

## Partners

- [Montimage](https://www.montimage.com/)
- [CROOM](https://croom.com/)

## Pilot

**Pilot 03 — Deburring of large metal parts (CROOM)**: The Job Card Extractor digitizes production job cards at CROOM's manufacturing facility, feeding structured job and operation data into the COGNIMAN service layer. This enables downstream services to automatically associate deburring tasks with specific production orders and track operation progress without manual intervention.

## License

[Montimage License](LICENSE)

## TRL

**TRL 7** — System prototype demonstrated in an operational environment. The tool has been validated with real manufacturing job cards from the Pilot 03 production line, includes comprehensive unit tests, versioned releases, and full documentation.

## References

No publications yet.
