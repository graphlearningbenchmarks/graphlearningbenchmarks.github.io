---
title: TorsionAngle
slug: torsionangle
benchmark: DualEquiNet RNA Benchmarks
task_type: graph_regression
description: RNA backbone torsion angle prediction (circular regression task, Circular
  MAE metric).
primary_metric: Circular MAE
higher_is_better: false
pyg_url: ''
stats:
  num_graphs: 1018
  avg_nodes: null
  avg_edges: null
  num_classes: null
result_count: 8
best_model:
  model: DualEquiNet
  value: 15.87
  metric: Circular MAE
  arxiv_id: '2506.19862'
  paper_title: DualEquiNet RNA Benchmarks
papers:
- arxiv_id: '2506.19862'
  title: DualEquiNet RNA Benchmarks
  date_iso: '2025-06-10'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Circular MAE
  default_metric: Circular MAE
  higher_is_better: false
  stats:
    num_graphs: 1018
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - Circular MAE
  metric_display_names:
  - Circular MAE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: DualEquiNet
    model_plain: DualEquiNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.19862'
    title: DualEquiNet RNA Benchmarks
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 15.87
    metric_stds:
    - 2.03
  - model: GotenNet
    model_plain: GotenNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.19862'
    title: DualEquiNet RNA Benchmarks
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 16.27
    metric_stds:
    - 1.19
  - model: GVPGNN
    model_plain: GVPGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.19862'
    title: DualEquiNet RNA Benchmarks
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 17.56
    metric_stds:
    - 0.21
  - model: EGNN
    model_plain: EGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.19862'
    title: DualEquiNet RNA Benchmarks
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 17.79
    metric_stds:
    - 0.61
  - model: HEGNN
    model_plain: HEGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.19862'
    title: DualEquiNet RNA Benchmarks
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 18.41
    metric_stds:
    - 0.22
  - model: SchNet
    model_plain: SchNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.19862'
    title: DualEquiNet RNA Benchmarks
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 18.54
    metric_stds:
    - 0.86
  - model: FastEGNN
    model_plain: FastEGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.19862'
    title: DualEquiNet RNA Benchmarks
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 18.89
    metric_stds:
    - 0.22
  - model: TFN
    model_plain: TFN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.19862'
    title: DualEquiNet RNA Benchmarks
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 21.97
    metric_stds:
    - 0.45
  row_count: 8
  rows_json: ''
  chart_json: /data/datasets/torsionangle/standard-split-chart.json
  arch_counts:
    gnn: 7
    hybrid: 1
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 8
  milestones: &id001
  - value: 15.87
    std: 2.03
    model: DualEquiNet
    arxiv_id: '2506.19862'
    title: DualEquiNet RNA Benchmarks
    date: '2025-06-10'
  milestones_by_metric:
    Circular MAE: *id001
---

