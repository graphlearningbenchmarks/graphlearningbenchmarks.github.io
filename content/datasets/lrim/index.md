---
title: LRIM
slug: lrim
benchmark: LRIM Graph Benchmark
task_type: node_regression
description: Long-Range Ising Model benchmark for per-node energy prediction on periodic
  2D grid graphs with controllable long-range interactions.
primary_metric: log-MSE
higher_is_better: false
pyg_url: https://lrim-graphbenchmark.com/
stats:
  num_graphs: 10000
  avg_nodes: 256.0
  avg_edges: 512.0
  num_classes: null
result_count: 8
best_model:
  model: GPS-RWSE
  value: -4.345
  metric: log-MSE
  arxiv_id: '2605.12358'
  paper_title: From Message-Passing to Linearized Graph Sequence Models
papers:
- arxiv_id: '2605.18387'
  title: Graph Hierarchical Recurrence for Long-Range Generalization
  date_iso: '2026-05-18'
  venue: ''
- arxiv_id: '2605.12358'
  title: From Message-Passing to Linearized Graph Sequence Models
  date_iso: '2026-05-12'
  venue: ''
variants:
- slug: lrim-16-hard
  name: LRIM-16-hard
  notes: ''
  is_standard: true
  primary_metric: log-MSE
  default_metric: log-MSE
  higher_is_better: false
  stats:
    num_graphs: 10000
    avg_nodes: 256.0
    avg_edges: 512.0
    num_classes: null
  metrics:
  - log-MSE
  metric_display_names:
  - log-MSE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GPS-RWSE
    model_plain: GPS-RWSE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - -4.345
    metric_stds:
    - 0.065
  - model: GPS-Base
    model_plain: GPS-Base
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - -4.34
    metric_stds:
    - 0.101
  - model: LGSM
    model_plain: LGSM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - -4.284
    metric_stds:
    - 0.133
  - model: GPS-LapPE
    model_plain: GPS-LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - -4.248
    metric_stds:
    - 0.11
  - model: GHR-GatedGCN
    model_plain: GHR-GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2605.18387'
    title: Graph Hierarchical Recurrence for Long-Range Generalization
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -4.195
    metric_stds:
    - 0.061
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -3.919
    metric_stds:
    - 0.223
  - model: GatedGCN-VN_G
    model_plain: GatedGCN-VN_G
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -3.756
    metric_stds:
    - 0.063
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -2.406
    metric_stds:
    - 0.148
  row_count: 8
  rows_json: ''
  chart_json: /data/datasets/lrim/lrim-16-hard-chart.json
  arch_counts:
    gnn: 3
    hybrid: 3
    graph_transformer: 1
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 8
  milestones: &id001
  - value: -4.345
    std: 0.065
    model: GPS-RWSE
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: '2026-05-12'
  milestones_by_metric:
    log-MSE: *id001
- slug: lrim-16-easy
  name: LRIM-16-easy
  notes: ''
  is_standard: false
  primary_metric: log-MSE
  higher_is_better: false
  stats:
    num_graphs: 10000
    avg_nodes: 256.0
    avg_edges: 512.0
    num_classes: null
  metrics:
  - log-MSE
  rows: []
  milestones: []
- slug: lrim-32-easy
  name: LRIM-32-easy
  notes: ''
  is_standard: false
  primary_metric: log-MSE
  higher_is_better: false
  stats:
    num_graphs: 10000
    avg_nodes: 1024.0
    avg_edges: 2048.0
    num_classes: null
  metrics:
  - log-MSE
  rows: []
  milestones: []
- slug: lrim-32-hard
  name: LRIM-32-hard
  notes: ''
  is_standard: false
  primary_metric: log-MSE
  higher_is_better: false
  stats:
    num_graphs: 10000
    avg_nodes: 1024.0
    avg_edges: 2048.0
    num_classes: null
  metrics:
  - log-MSE
  rows: []
  milestones: []
- slug: lrim-64-easy
  name: LRIM-64-easy
  notes: ''
  is_standard: false
  primary_metric: log-MSE
  higher_is_better: false
  stats:
    num_graphs: 10000
    avg_nodes: 4096.0
    avg_edges: 8192.0
    num_classes: null
  metrics:
  - log-MSE
  rows: []
  milestones: []
- slug: lrim-64-hard
  name: LRIM-64-hard
  notes: ''
  is_standard: false
  primary_metric: log-MSE
  higher_is_better: false
  stats:
    num_graphs: 10000
    avg_nodes: 4096.0
    avg_edges: 8192.0
    num_classes: null
  metrics:
  - log-MSE
  rows: []
  milestones: []
- slug: lrim-128-easy
  name: LRIM-128-easy
  notes: ''
  is_standard: false
  primary_metric: log-MSE
  higher_is_better: false
  stats:
    num_graphs: 10000
    avg_nodes: 16384.0
    avg_edges: 32768.0
    num_classes: null
  metrics:
  - log-MSE
  rows: []
  milestones: []
- slug: lrim-128-hard
  name: LRIM-128-hard
  notes: ''
  is_standard: false
  primary_metric: log-MSE
  higher_is_better: false
  stats:
    num_graphs: 10000
    avg_nodes: 16384.0
    avg_edges: 32768.0
    num_classes: null
  metrics:
  - log-MSE
  rows: []
  milestones: []
- slug: lrim-256-easy
  name: LRIM-256-easy
  notes: ''
  is_standard: false
  primary_metric: log-MSE
  higher_is_better: false
  stats:
    num_graphs: 10000
    avg_nodes: 65536.0
    avg_edges: 131072.0
    num_classes: null
  metrics:
  - log-MSE
  rows: []
  milestones: []
- slug: lrim-256-hard
  name: LRIM-256-hard
  notes: ''
  is_standard: false
  primary_metric: log-MSE
  higher_is_better: false
  stats:
    num_graphs: 10000
    avg_nodes: 65536.0
    avg_edges: 131072.0
    num_classes: null
  metrics:
  - log-MSE
  rows: []
  milestones: []
---

