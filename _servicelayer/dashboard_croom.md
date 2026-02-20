---
title: Job Card Extractor
weight: 99
description: Extracts job numbers and operations from manufacturing PDFs automatically
license: https://img.shields.io/badge/license-Apache--2.0-blue
trl: https://img.shields.io/badge/TRL-7-blue
github: https://github.com/COGNIMANEU/pilot03-service-job-card-extractor
---

## One-line Value Proposition

Automates the extraction of critical production data from paper job cards, eliminating manual data entry errors and accelerating order processing in manufacturing plants.

## Name

**Job Card Extractor** — Automated manufacturing document data extraction tool

## Overview

Manufacturing plants rely on paper job cards to track production orders, but manually transferring this data to digital systems is time-consuming and error-prone. The Job Card Extractor uses OCR and barcode detection to automatically read job numbers, quantities, delivery dates, and operation details from scanned PDF job cards. Plants can process hundreds of job cards per hour with near-perfect accuracy, enabling real-time production tracking without clerical overhead.

## Key Features

- **Automated Data Extraction**: Reads job numbers, quantities, delivery dates, and operation details without manual intervention
- **Multi-format Support**: Handles multi-page PDFs with parallel processing for faster batch operations
- **Barcode Recognition**: Detects and decodes barcodes printed on job cards for instant job identification
- **Visual Debugging**: Generates annotated images showing exactly what was detected, building trust in the extraction results
- **Confidence Scoring**: Flags low-confidence extractions so supervisors can review only uncertain entries
- **Flexible Output**: Produces structured JSON ready for integration with MES, ERP, or production tracking systems
- **Multi-language OCR**: Supports English and French job cards out of the box

## What Goes In / What Comes Out

### Input

- Scanned PDF job cards from the production floor
- Images (PNG, JPEG) of job cards
- Batch folders containing multiple documents for bulk processing

### Output

- **Structured JSON** containing:
  - Job number and quantity
  - Delivery date
  - Operation list with names and sequence numbers
  - Confidence scores for each extracted field
- **Raw extraction data** for debugging and verification
- **Annotated images** highlighting detected text regions and barcodes
- **Extraction logs** with processing timestamps and performance metrics

## How It Works

The tool converts PDF pages to images, then applies computer vision algorithms to locate text regions and barcodes. EasyOCR reads the textual content while PyZbar decodes any embedded barcodes. A custom extraction engine parses the recognized text to identify job numbers, dates, and operation sequences using pattern matching. The entire process runs locally—no data leaves the plant—making it suitable for sensitive manufacturing environments.

## Use Cases

### Scenario 1: Production Planning Manager
A plant receives 200 job cards daily from the assembly line. Before the extractor, clerks spent 6 hours manually typing each card into the MES. With Job Card Extractor, the system processes all 200 cards in 15 minutes, flagging 5 that need manual review due to poor print quality. The planning team now has accurate job data by 8 AM instead of noon.

### Scenario 2: Quality Assurance Supervisor
After a production defect, the QA team needs to trace which job batch was affected. Instead of searching through filing cabinets, they run the extractor on archived job cards and immediately retrieve the exact job number, date, and operations performed—reducing traceability investigation from hours to minutes.

### Scenario 3: Logistics Coordinator
Daily delivery schedules depend on knowing which jobs are complete and which are pending. The coordinator runs the extractor on the morning batch of job cards and imports the structured JSON directly into the scheduling software, ensuring trucks load the right orders on time.

## Partners

- **Croom** — System architecture and integration
- **Montimage** — OCR optimization and validation
- **IRT** — Technical contribution and validation


## Pilot

**Pilot 3** — The Job Card Extractor serves as the primary data ingestion layer for Pilot 3's digital workflow, enabling automated capture of production orders from legacy paper-based processes.

## License

[Apache License 2.0](https://opensource.org/licenses/Apache-2.0)

## TRL

**TRL 7** — System prototype has been tested in operational environment. The tool has reached version 1.1.0 with semantic versioning, includes a comprehensive test suite, multiple documentation guides (user, API, architecture, troubleshooting), and is actively used in the COGNIMAN pilot workflow.

## References

[1] COGNIMAN Project — https://cogniman.eu