# Document Template Validator

A document validation and comparison system that compares a submitted document against a reference template and generates an automated verification report.

## Overview

The system is designed to identify differences between a reference document and a submitted document.

It supports:

- PDF documents
- DOCX documents
- Text extraction
- OCR-based processing for document images
- Heading/section detection
- Section-level comparison
- Match, mismatch, and missing-content classification
- Word-overlap based accuracy calculation
- Automated PDF verification reports

## Workflow

```text
Reference Document
        |
        v
Document Extraction
        |
        v
OCR / Text Processing
        |
        v
Section Detection
        |
        +----------------------+
        |                      |
        v                      v
Reference Sections       Submitted Sections
        |                      |
        +----------+-----------+
                   |
                   v
          Section Comparison
                   |
          +--------+--------+
          |        |        |
          v        v        v
        MATCH   MISMATCH  MISSING
                   |
                   v
          Accuracy Calculation
                   |
                   v
        Verification Report
