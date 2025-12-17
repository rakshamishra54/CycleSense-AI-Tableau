## Alert Rules — PCOSense Actionable Analytics Layer

This document defines alerting logic built on top of Tableau calculated fields.
Alerts convert passive insights into real-time, actionable signals.

---

## Alert Philosophy

PCOSense alerts are designed to be:
- Preventive, not diagnostic
- Explainable and non-alarming
- Triggered only when meaningful thresholds are crossed
- Aligned with ethical healthcare analytics

---

## Alert 1: Elevated PCOS Risk Alert

### Trigger Condition
```tableau
[PCOS Risk Index] > 60
