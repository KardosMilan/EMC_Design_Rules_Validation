# Automotive SEPIC Converter — EMC Design Rules Validation

> **Complete engineering workflow for an automotive-grade SEPIC DC-DC converter, from power-stage dimensioning through iterative EMC filter development to laboratory validation.**

---

## Overview

This project documents the full development and validation cycle of a switching power supply designed to meet demanding automotive EMC requirements. Starting from topology selection and component dimensioning, the work progresses through multiple hardware revisions, EMC-oriented filter design, and systematic laboratory validation — including electrical, frequency-domain, and thermal measurements.

Two contrasting PCB design iterations (SEPIC-A2 and SEPIC-B) are included side by side, demonstrating the measurable EMC impact of layout and filter decisions.

---

## Project Goals

- Design an automotive SEPIC converter power stage with appropriate switching-frequency selection and thermal management
- Identify and characterise conducted and radiated emission sources
- Develop and iteratively optimise LC input/output EMC filters
- Validate all design decisions through laboratory measurements
- Correlate theoretical calculations with experimental results
- Produce a documented engineering process suitable for future design iterations

---

## Engineering Workflow

### 1 — System Design
Component selection, power-stage dimensioning, switching-frequency optimisation, thermal considerations, and initial PCB layout preparation.

### 2 — EMC Filter Development
LC filter calculations, topology comparison, resonance analysis, and iterative optimisation verified against laboratory measurements. All calculation sheets are included in the repository.

### 3 — Prototype Manufacturing
Custom PCB design with microcontroller integration, automotive-grade components, and dedicated measurement interfaces. Two hardware revisions are provided:

| Revision     | Design Intent                                                        |
|---|---|
| **SEPIC-A2** | Reference iteration — poor EMC layout (emission source example)      |
| **SEPIC-B**  | Optimised iteration — improved EMC layout and filter (target design) |

### 4 — Measurement & Validation

| Domain      | Method                                                                               |
|---|---|
| Electrical  | Switching waveform analysis, frequency-domain characterisation, noise quantification |
| EMC         | Conducted emission measurement, filter effectiveness comparison between revisions    |
| Thermal     | FLIR thermal imaging, hotspot identification, thermal performance validation         |
| Correlation | Calculated vs. measured comparison across all key parameters                         |

---

## Repository Structure

```
EMC_Design_Rules_Validation/
├── 01_Documents/
│   ├── Filter design documentation
│   ├── Measurement plans
│   ├── Correlation calculations
│   ├── Thermal analysis results
│   └── Oscilloscope captures
│
├── 02_Pictures/
│   ├── Prototype photos
│   └── Laboratory setup
│
├── 03_Calculations/
│   ├── Design calculations
│   ├── EMC filter calculations
│   └── Validation worksheets
│
├── 04_SEPIC_microcontroller_prototype/
│   ├── Prototype hardware
│   ├── Embedded controller integration
│   └── Supporting component libraries
│
└── 05_HW_design/
    ├── SEPIC-A2/     ← bad EMC design example
    ├── SEPIC-B/      ← optimised EMC design example
    └── PCB design resources
```

---

## Technology Stack

| Area                   | Tools & Methods                         |
|---|---|
| PCB Design             | CAD schematic & layout tools            |
| Calculations           | Excel-based engineering worksheets      |
| Electrical Measurement | Oscilloscope (time & frequency domain)  |
| Thermal Measurement    | FLIR thermal camera                     |
| EMC Measurement        | Conducted emission laboratory equipment |
| Embedded Platform      | Automotive-grade microcontroller        |

---

## Key Outcomes

- Designed and validated two SEPIC converter hardware revisions with measurably different EMC behaviour
- Developed EMC filter solutions grounded in both analytical calculation and experimental iteration
- Demonstrated a systematic correlation methodology between design predictions and laboratory results
- Produced a complete, reproducible engineering workflow applicable to future power electronics and EMC projects

---

## Author

**Kardos Milan**  
Electrical / Electronics Engineer  
*Specialising in Power Electronics, EMC Validation, Hardware Design, and Embedded Systems*

---

## License

This repository is shared for portfolio and reference purposes. All rights reserved.
