---
title: Extraction Anomalies
type: dev
description: Post-extraction anomaly checks over stored results
dev_table_json: /data/development/extraction-anomalies.json
---

## Post-Extraction Anomalies

This page flags suspicious stored results after overrides are applied.

Checks currently included:

- bounded metrics such as Accuracy/AP/AUC/F1/MRR/Hits@K must not exceed 1
- values roughly 20x away from the dataset-metric median are flagged as likely scale issues

**Flagged papers:** 44
**Flagged rows:** 104


Detailed table: 104 rows (loaded below).
