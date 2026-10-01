# e-waste-classifier
Multimodal E-Waste Assessment AI — Research and production-oriented development of a multimodal device assessment system combining structured functional diagnostics, cosmetic computer vision, and multimodal fusion for automated e-waste/device condition assessment.

# Multimodal E-Waste Assessment AI

A research and production-oriented AI system for automated assessment of electronic devices using **structured functional diagnostics** and **cosmetic computer vision**, with a planned multimodal fusion layer for generating a unified device assessment.

The project is being developed with a clear separation between:

- Existing trained model artifacts
- Model inference and validation
- Multimodal fusion
- Production inference architecture
- Android integration
- Deployment

---

## Project Objective

The objective is to build a reliable multimodal assessment pipeline that can combine:

1. **Functional device diagnostics**
2. **Cosmetic/device-condition images**
3. **Multimodal fusion**

to produce a unified assessment of an electronic device.

The system is intended to support future integration with an Android application for real-world device assessment.

---

## High-Level Architecture

```text
                    DEVICE
                       │
          ┌────────────┴────────────┐
          │                         │
          ▼                         ▼
 Functional Diagnostics          Photos
          │                         │
          ▼                         ▼
 Functional Model             Cosmetic Model
          │                         │
          ▼                         ▼
 Functional Result            Cosmetic Result
          │                         │
          └────────────┬────────────┘
                       ▼
                 Fusion Engine
                       │
                       ▼
              Final Assessment
                       │
                       ▼
                Android / API
