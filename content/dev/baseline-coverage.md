---
title: Baseline Coverage Gaps
type: dev
description: Datasets missing common GNN or MLP baseline families
dev_table_json: /data/development/baseline-coverage.json
---

## Baseline Coverage Gaps

Datasets in this report are missing one of the baseline families we usually want on the leaderboard for context.

### No GCN/GIN/GraphSAGE Baseline (36)

| Benchmark | Dataset | Task | Metric | Results | Present Families |
|-----------|---------|------|--------|--------:|------------------|
| CosmoBench | CAMELS-SAM | graph_regression | R^2 | 0 | — |
| CosmoBench | CS-Trees | graph_regression | R2 | 0 | — |
| CosmoBench | CS-Trees-200 | graph_classification | Accuracy | 0 | — |
| CosmoBench | Quijote | graph_regression | R^2 | 0 | — |
| DualEquiNet RNA Benchmarks | COVID | node_regression | RMSE | 32 | — |
| DualEquiNet RNA Benchmarks | Ribonanza | node_regression | RMSE | 20 | — |
| DualEquiNet RNA Benchmarks | Tc-Ribo | graph_regression | RMSE | 19 | — |
| GraphBench | Algorithmic Reasoning | graph_classification | Accuracy | 8 | — |
| GraphBench | BlueSky | node_regression | MAE | 0 | — |
| GraphBench | Bridges | edge_classification | F1 | 5 | — |
| GraphBench | Chip Design | graph_generation | Accuracy | 0 | — |
| GraphBench | Combinatorial Optimization | graph_regression | MAE | 0 | — |
| GraphBench | Electronic Circuits | graph_regression | MAE | 0 | — |
| GraphBench | Flow | graph_regression | MAE | 5 | — |
| GraphBench | MST | edge_classification | F1 | 5 | — |
| GraphBench | Max Clique | node_classification | F1 | 0 | — |
| GraphBench | Max Matching | edge_classification | F1 | 0 | — |
| GraphBench | Steiner Trees | edge_classification | F1 | 0 | — |
| GraphBench | Topological Sorting | node_regression | MAE | 0 | — |
| GraphBench | Weather Forecasting | node_regression | MAE | 0 | — |
| Heterogeneous Graph Benchmarks | RCDD | link_prediction | MRR | 0 | — |
| Hypergraph Benchmarks | BAT | node_classification | F1 | 99 | — |
| Hypergraph Benchmarks | Congress | node_classification | Accuracy | 13 | — |
| Hypergraph Benchmarks | DBLP-CA | node_classification | Accuracy | 27 | mlp |
| Hypergraph Benchmarks | EAT | node_classification | F1 | 74 | — |
| Hypergraph Benchmarks | House | node_classification | Accuracy | 74 | mlp |
| Hypergraph Benchmarks | LEN | node_classification | Accuracy | 0 | — |
| Hypergraph Benchmarks | Senate | node_classification | Accuracy | 14 | — |
| Hypergraph Benchmarks | UAT | node_classification | F1 | 137 | — |
| Hypergraph Benchmarks | Walmart | node_classification | Accuracy | 23 | mlp |
| Knowledge Graphs | WN18 | link_prediction | MRR | 22 | — |
| OGB | ogbl-biokg | link_prediction | MRR | 29 | — |
| Other Graph Benchmarks | MovieLens Film | node_classification | Micro-F1 | 7 | — |
| Power Flow Benchmarks | Case 1 | graph_regression | Accuracy | 17 | — |
| Power Flow Benchmarks | Case 2 | graph_regression | Accuracy | 4 | — |
| Quantum Chemistry | MD17 | graph_regression | MAE | 404 | — |

### No MLP Baseline (77)


Detailed table: 77 rows (loaded below).
