## PCOS Risk Index (PRI) Scoring Logic

### Formula Overview

PRI is calculated as a weighted sum of normalized feature scores:

PRI = (
  Menstrual_Score * 0.30 +
  Metabolic_Score * 0.25 +
  Androgenic_Score * 0.25 +
  Lifestyle_Score * 0.20
) * 100

---

### Weighting Rationale

| Feature Group        | Weight | Reasoning |
|----------------------|--------|-----------|
| Menstrual Regularity | 30%    | Primary diagnostic indicator |
| Metabolic Factors   | 25%    | Strong PCOS correlation |
| Androgenic Symptoms | 25%    | Hallmark clinical signal |
| Lifestyle Stress    | 20%    | Modifiable risk contributor |

Weights are configurable and adjustable for future iterations.

---

### Risk Band Mapping

| PRI Range | Risk Label  | Tableau Color |
|----------|-------------|---------------|
| 0–30     | Low         | Green         |
| 31–60    | Moderate    | Amber         |
| 61–100   | Elevated    | Red           |

---

### Explainability Output

Each dashboard must expose:
- Individual feature contributions
- Weight applied
- Change over time

This ensures trust, transparency, and ethical analytics.
