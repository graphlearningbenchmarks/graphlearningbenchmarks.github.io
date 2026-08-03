---
title: Problematic Papers
type: dev
description: LaTeX table-parser blind spots requiring re-extraction
---

## Problematic Papers (LaTeX table coverage)

Papers whose LaTeX source may have benchmark tables that were invisible to the extractor: `wraptable`, `sidewaystable`, or tabular rows with multiple `&` separators outside parsed table environments.

Regenerate this list on the server with:

```bash
uv run python scripts/scan_latex_table_issues.py --write-list --export-json
uv run python -m backend.export_to_hugo
```

Re-extraction runbook: `config/latex_table_reextract_server.txt` in the repo.

**Last scan:** 2026-07-01T12:14:57.545366+00:00
**Flagged papers:** 1

| ArXiv | Title | Issues | Explanation | Sample unparsed line |
|-------|-------|--------|-------------|----------------------|
| [Distributed-Order Fractional Graph Operating Network](/papers/2411.05274/) | Distributed-Order Fractional Graph Operating Network | unparsed_tabular_lines, wraptable | Contains 2 wraptable environment(s); parsed 2. Papers processed before wraptable support need full LLM re-extraction. Found lines with two or more '&' column separators outside parsed table environments (possible standalone tabular or unsupported... | y_j(0)= \begin{cases}y_0^{[j / M]}, & \text { if } j / M... |
