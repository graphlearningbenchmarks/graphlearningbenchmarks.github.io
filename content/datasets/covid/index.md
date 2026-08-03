---
title: COVID
slug: covid
benchmark: DualEquiNet RNA Benchmarks
task_type: graph_regression
description: RNA structure prediction on the COVID-19 dataset from the EternaFold/Kaggle
  Ribonanza challenge (RMSE metric, lower is better).
primary_metric: RMSE
higher_is_better: false
pyg_url: ''
stats:
  num_graphs: 4082
  avg_nodes: null
  avg_edges: null
  num_classes: null
result_count: 8
best_model:
  model: DualEquiNet
  value: 0.353
  metric: Avg.
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
  primary_metric: Avg.
  default_metric: Avg.
  higher_is_better: false
  stats:
    num_graphs: 4082
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - Avg.
  - Mg pH10
  - Reactivity
  - pH10
  metric_display_names:
  - Avg.
  - Mg pH10
  - Reactivity
  - pH10
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
    - 0.353
    - 0.34
    - 0.272
    - 0.448
    metric_stds:
    - 0.006
    - 0.005
    - 0.004
    - 0.01
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.475
    - 0.455
    - 0.388
    - 0.582
    metric_stds:
    - 0.009
    - 0.008
    - 0.002
    - 0.011
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
    - 0.478
    - 0.463
    - 0.39
    - 0.582
    metric_stds:
    - 0.031
    - 0.027
    - 0.019
    - 0.029
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.531
    - 0.515
    - 0.448
    - 0.631
    metric_stds:
    - 0.011
    - 0.009
    - 0.006
    - 0.012
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
    - 0.533
    - 0.517
    - 0.45
    - 0.632
    metric_stds:
    - 0.011
    - 0.009
    - 0.005
    - 0.012
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.534
    - 0.518
    - 0.451
    - 0.633
    metric_stds:
    - 0.011
    - 0.01
    - 0.006
    - 0.012
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.535
    - 0.52
    - 0.453
    - 0.634
    metric_stds:
    - 0.011
    - 0.01
    - 0.006
    - 0.013
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
    - 0.535
    - 0.52
    - 0.453
    - 0.634
    metric_stds:
    - 0.011
    - 0.01
    - 0.006
    - 0.012
  row_count: 8
  rows_json: ''
  chart_json: /data/datasets/covid/standard-split-chart.json
  arch_counts:
    gnn: 7
    hybrid: 1
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 8
  - 8
  - 8
  - 8
  milestones: &id001
  - value: 0.353
    std: 0.006
    model: DualEquiNet
    arxiv_id: '2506.19862'
    title: DualEquiNet RNA Benchmarks
    date: '2025-06-10'
  milestones_by_metric:
    Avg.: *id001
    Mg pH10:
    - value: 0.34
      std: 0.005
      model: DualEquiNet
      arxiv_id: '2506.19862'
      title: DualEquiNet RNA Benchmarks
      date: '2025-06-10'
    Reactivity:
    - value: 0.272
      std: 0.004
      model: DualEquiNet
      arxiv_id: '2506.19862'
      title: DualEquiNet RNA Benchmarks
      date: '2025-06-10'
    pH10:
    - value: 0.448
      std: 0.01
      model: DualEquiNet
      arxiv_id: '2506.19862'
      title: DualEquiNet RNA Benchmarks
      date: '2025-06-10'
---

