---
title: Problematic Papers
type: dev
description: LaTeX table-parser blind spots requiring re-extraction
dev_table_json: /data/development/problematic-papers.json
---

## Problematic Papers (LaTeX table coverage)

Papers whose LaTeX source may have benchmark tables that were invisible to the extractor: `wraptable`, `sidewaystable`, or tabular rows with multiple `&` separators outside parsed table environments.

Regenerate this list on the server with:

```bash
uv run python scripts/scan_latex_table_issues.py --write-list --export-json
uv run python -m backend.export_to_hugo
```

Re-extraction runbook: `config/latex_table_reextract_server.txt` in the repo.

**Last scan:** 2026-07-01T12:19:26.517465+00:00
**Flagged papers:** 1486


Detailed table: 1486 rows (loaded below).
