---
title: Skipped Papers
type: dev
description: Papers rejected by LLM screening
dev_table_json: /data/development/skipped-papers.json
---

## Skipped Papers

This page shows papers that were identified but rejected by the LLM screening pipeline. The screening happens in two stages: Stage 1 filters for general relevance to graph neural network research, and Stage 2 checks whether the paper evaluates results on known benchmarks. Papers that pass both stages proceed to full result extraction.

### Stage 1 Rejections: 265

Stage 1 rejects papers that are deemed not relevant to graph neural networks. These are typically papers in unrelated fields that happened to mention GNNs or graph concepts, but don't focus on benchmarking graph neural network models.


Detailed table: 265 rows (loaded below).


### Stage 2 Rejections: 0

Stage 2 rejects papers that are relevant to GNNs but don't evaluate models on any known benchmarks. This includes position papers, theoretical papers, survey papers, or papers that only propose new datasets without evaluating existing models. The 'Datasets Found' column shows how many benchmark datasets the LLM detected in the paper (if any).


### No Datasets/Results Discovered: 0

These papers passed Stage 2 screening (were deemed relevant and benchmarking-focused) but the extraction pipeline was unable to discover any benchmark datasets or results. This could mean: the paper's results are too noisy for extraction, the datasets used have non-standard names, or the extraction model failed to parse the paper format. These papers may still be worth investigating manually.