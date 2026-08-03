---
title: SAT Solving
slug: sat-solving
benchmark: GraphBench
task_type: node_classification
description: 'SAT problem instances represented as graphs. Multi-level node/edge/graph-level
  tasks across 11 solvers and 3 instance-size scales.

  '
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://graphbench.github.io/website/datasets.html
stats:
  num_graphs: 208788
  avg_nodes: 10400.5
  avg_edges: 2054969.0
  num_classes: null
result_count: 6
best_model:
  model: PR
  value: 0.51
  metric: Accuracy
  arxiv_id: '2512.04475'
  paper_title: GraphBench
papers:
- arxiv_id: '2512.04475'
  title: GraphBench
  date_iso: '2025-12-04'
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
    num_graphs: 208788
    avg_nodes: 10400.5
    avg_edges: 2054969.0
    num_classes: null
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: PR
    model_plain: PR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.04475'
    title: GraphBench
    date: Dec 4, 2025
    date_iso: '2025-12-04'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.51
    metric_stds:
    - 0.01
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.04475'
    title: GraphBench
    date: Dec 4, 2025
    date_iso: '2025-12-04'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.45
    metric_stds:
    - 0.0
  - model: Gated GCN+
    model_plain: Gated GCN+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.04475'
    title: GraphBench
    date: Dec 4, 2025
    date_iso: '2025-12-04'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4
    metric_stds:
    - 0.04
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.04475'
    title: GraphBench
    date: Dec 4, 2025
    date_iso: '2025-12-04'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.31
    metric_stds:
    - 0.0
  - model: PC
    model_plain: PC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.04475'
    title: GraphBench
    date: Dec 4, 2025
    date_iso: '2025-12-04'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.21
    metric_stds:
    - 0.01
  - model: MC
    model_plain: MC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.04475'
    title: GraphBench
    date: Dec 4, 2025
    date_iso: '2025-12-04'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - -0.05
    metric_stds:
    - 0.01
  row_count: 6
  rows_json: ''
  chart_json: /data/datasets/sat-solving/standard-split-chart.json
  arch_counts:
    gnn: 3
    hybrid: 0
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 3
  metric_counts:
  - 6
  milestones: &id001
  - value: 0.51
    std: 0.01
    model: PR
    arxiv_id: '2512.04475'
    title: GraphBench
    date: '2025-12-04'
  milestones_by_metric:
    Accuracy: *id001
---

