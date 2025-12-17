## Feature Engineering Logic for PCOS Risk Index (PRI)

### Objective
Translate raw dataset variables into standardized, interpretable signals that contribute to the PCOS Risk Index.

Each feature is normalized into a **risk contribution score** between 0 and 1.

---

## Feature Groups & Logic

### 1. Menstrual Regularity Score
**Input Variables**
- Cycle length (days)
- Missed periods (yes/no)

**Logic**
- Regular cycle (21–35 days): score = 0
- Mild irregularity (36–45 days): score = 0.5
- Severe irregularity (>45 days or missed): score = 1

---

### 2. Metabolic Risk Score
**Input Variables**
- BMI
- Weight gain in last 6–12 months

**Logic**
- BMI < 25 and stable weight: score = 0
- BMI 25–30 or recent weight gain: score = 0.5
- BMI > 30 and weight gain: score = 1

---

### 3. Androgenic Symptom Score
**Input Variables**
- Acne severity
- Hair growth (hirsutism)
- Hair thinning

**Logic**
- No symptoms: score = 0
- One symptom present: score = 0.5
- Multiple symptoms present: score = 1

---

### 4. Lifestyle Stress Score
**Input Variables**
- Physical activity frequency
- Self-reported stress levels

**Logic**
- Active lifestyle + low stress: score = 0
- Moderate activity or stress: score = 0.5
- Sedentary + high stress: score = 1

---

### Feature Normalization Principle
All feature scores are scaled between **0 and 1** to:
- Maintain comparability
- Enable flexible weighting
- Support explainable scoring

---

### Tableau Implementation Notes
Each feature score will be:
- Implemented as a Tableau calculated field
- Independently visualized
- Used in PRI aggregation logic

