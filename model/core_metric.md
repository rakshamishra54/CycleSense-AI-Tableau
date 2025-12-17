## Core Metric: PCOS Risk Index (PRI)

### Metric Purpose
The PCOS Risk Index (PRI) is a composite, non-clinical indicator designed to surface potential PCOS-related risk patterns using observable lifestyle, physiological, and symptom-based variables.

This metric is **not a diagnostic tool** and is intended strictly for analytics, awareness, and preventive insights.

---

### Why a Composite Metric?
Individual health indicators often fail to provide context in isolation. PRI combines multiple signals into a single, interpretable score that allows:

- Early risk awareness
- Trend tracking over time
- Population-level comparison
- Actionable alerts without medical claims

---

### PRI Scale Definition

| PRI Score Range | Risk Band        | Interpretation                     |
|-----------------|------------------|-------------------------------------|
| 0 – 30          | Low              | No significant observed risk        |
| 31 – 60         | Moderate         | Emerging patterns worth monitoring  |
| 61 – 100        | Elevated         | Strong correlation signals detected |

---

### Core Contributing Factors

Each factor contributes a weighted component to the final PRI score:

| Factor Category       | Example Variables                        |
|-----------------------|------------------------------------------|
| Menstrual Irregularity| Cycle length, missed periods             |
| Metabolic Indicators | BMI, weight fluctuation                  |
| Hormonal Signals     | Acne, hair growth, hair thinning         |
| Lifestyle Factors    | Physical activity, stress levels         |
| Reproductive History | Fertility-related indicators (if present)|

Weights are configurable and adjustable for future research validation.

---

### Explainability Principle

Each PRI score must be decomposable into:
- Contributing variables
- Weight influence
- Time-based change

This enables transparent analytics and avoids “black-box” scoring.

---

### Tableau Implementation Concept

In Tableau:
- PRI will be implemented as a calculated field
- Risk bands will be visualized using color semantics
- Tooltips will show factor-level breakdowns
- Dashboards will emphasize **trend movement**, not static scores

---

### Ethical & Compliance Considerations

- No medical diagnosis or prediction claims
- Educational and informational usage only
- Clear disclaimers present in dashboards
- Designed to complement, not replace, clinical judgment
