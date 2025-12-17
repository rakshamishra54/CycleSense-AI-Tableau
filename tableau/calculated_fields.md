## Tableau Calculated Fields — Semantic Modeling Layer

This document defines the semantic layer for PCOSense built using Tableau Calculated Fields.
The goal is to translate raw health and lifestyle data into meaningful, reusable business metrics.

---

## Semantic Modeling Philosophy

PCOSense follows a **metrics-first semantic design**:
- Raw signals → Interpreted features → Composite risk metrics
- No direct exposure of raw medical indicators
- Fully explainable, reusable logic across dashboards and alerts

This aligns with modern analytics practices encouraged by Tableau.

---

## Core Semantic Metrics

### 1. PCOS Risk Index (Primary KPI)

```tableau
(
IF [Cycle Irregularity] = 1 THEN 25 ELSE 0 END +
IF [Androgen Indicators] = 1 THEN 25 ELSE 0 END +
IF [Metabolic Risk Score] = 1 THEN 25 ELSE 0 END +
IF [Lifestyle Stress Score] = 1 THEN 25 ELSE 0 END
)
