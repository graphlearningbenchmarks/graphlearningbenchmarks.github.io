---
title: Paper Extraction Status
type: dev
description: Overview of extraction status
dev_table_json: /data/development/paper-status.json
---

## Paper Extraction Status

**Total:** 2740 papers

This page tracks the extraction pipeline status for all papers in the benchmarking dataset. Each paper goes through several stages: first it must be downloaded from arXiv, then the full text is extracted and parsed (either from HTML, LaTeX source, or PDF), and finally results are extracted using an LLM. The extraction model shown indicates which LLM (if any) was used to extract results.

### Downloaded (38)

Papers that have been downloaded but not yet processed for extraction.

| ArXiv | Title | Model |
|-------|-------|-------|
| 1409.4842 | arXiv:1409.4842 | — |
| 1704.07912 | arXiv:1704.07912 | — |
| 1706.02216 | Inductive Representation Learning on Large Graphs | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 1710.10361 | arXiv:1710.10361 | — |
| 1805.10437 | arXiv:1805.10437 | — |
| 1904.07090 | arXiv:1904.07090 | — |
| 1905.05494 | arXiv:1905.05494 | — |
| 1907.04943 | arXiv:1907.04943 | — |
| 1910.00967 | arXiv:1910.00967 | — |
| 1910.11436 | Hierarchical Representation Learning in Graph Neural Networks with... | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2002.09605 | arXiv:2002.09605 | — |
| 2004.11197 | arXiv:2004.11197 | — |
| 2006.09957 | arXiv:2006.09957 | — |
| 2009.08012 | arXiv:2009.08012 | — |
| 2012.03173 | arXiv:2012.03173 | — |
| 2103.04559 | arXiv:2103.04559 | — |
| 2105.09336 | arXiv:2105.09336 | — |
| 2106.03386 | arXiv:2106.03386 | — |
| 2106.06760 | arXiv:2106.06760 | — |
| 2107.02285 | arXiv:2107.02285 | — |
| 2107.02802 | arXiv:2107.02802 | — |
| 2110.05950 | arXiv:2110.05950 | — |
| 2111.15099 | arXiv:2111.15099 | — |
| 2202.01129 | arXiv:2202.01129 | — |
| 2202.02292 | arXiv:2202.02292 | — |
| 2202.05184 | arXiv:2202.05184 | — |
| 2203.05496 | arXiv:2203.05496 | — |
| 2203.10555 | arXiv:2203.10555 | — |
| 2206.06281 | arXiv:2206.06281 | — |
| 2208.06050 | arXiv:2208.06050 | — |
| 2305.17311 | arXiv:2305.17311 | — |
| 2403.06560 | arXiv:2403.06560 | — |
| 2404.19288 | Training-free Graph Neural Networks and the Power of... | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2407.09709 | GOFA: A Generative One-For-All Model for Joint Graph... | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2408.05391 | arXiv:2408.05391 | — |
| 2502.00806 | UniGraph2: Learning a Unified Embedding Space to Bind... | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2512.08274 | arXiv:2512.08274 | — |
| 2604.00199 | arXiv:2604.00199 | — |

### Extracted (1504)

Papers with successfully extracted results. These papers contribute to the leaderboards.


Detailed table: 1504 rows (loaded below).


### Failed (318)

Papers where extraction failed. These may have parsing errors, missing datasets, or LLM errors.


Detailed table: 318 rows (loaded below).


### Quarantined_extraction_quality (590)


Detailed table: 590 rows (loaded below).


### Quarantined_method_name (279)


Detailed table: 279 rows (loaded below).


### Quarantined_yaml_parse (11)

| ArXiv | Title | Model |
|-------|-------|-------|
| 1707.03815 | arXiv:1707.03815 | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 1806.01242 | arXiv:1806.01242 | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 1910.14356 | arXiv:1910.14356 | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2007.13681 | arXiv:2007.13681 | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2102.13085 | arXiv:2102.13085 | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2206.09144 | arXiv:2206.09144 | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2312.12477 | arXiv:2312.12477 | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2409.08023 | arXiv:2409.08023 | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2410.00626 | arXiv:2410.00626 | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2502.12412 | arXiv:2502.12412 | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |
| 2505.02247 | arXiv:2505.02247 | cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit |