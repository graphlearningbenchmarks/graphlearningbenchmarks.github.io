---
title: Case 2
slug: case-2
benchmark: Power Flow Benchmarks
task_type: graph_regression
description: Power flow analysis on IEEE test case 2 (medium power grid, node-level
  regression).
primary_metric: Accuracy
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 750000
  avg_nodes: null
  avg_edges: null
  num_classes: null
result_count: 4
best_model:
  model: RMGL
  value: 0.9928
  metric: Accuracy
  arxiv_id: '2601.01387'
  paper_title: Power Flow Benchmarks
papers:
- arxiv_id: '2601.01387'
  title: Power Flow Benchmarks
  date_iso: '2026-01-04'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 750000
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: RMGL
    model_plain: RMGL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9928
    metric_stds:
    - null
  - model: MGL
    model_plain: MGL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9607
    metric_stds:
    - null
  - model: GLP
    model_plain: GLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5072
    metric_stds:
    - null
  - model: GLR
    model_plain: GLR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4709
    metric_stds:
    - null
  row_count: 4
  rows_json: ''
  chart_json: /data/datasets/case-2/standard-split-chart.json
  arch_counts:
    gnn: 3
    hybrid: 1
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 4
  milestones: []
  milestones_by_metric:
    Accuracy: []
---

