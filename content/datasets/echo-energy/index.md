---
title: ECHO-Energy
slug: echo-energy
benchmark: ECHO Benchmark
task_type: graph_regression
description: ECHO energy propagation task — predicting energy distribution on physical
  graphs.
primary_metric: MAE
higher_is_better: false
pyg_url: ''
stats:
  num_graphs: 196000
  avg_nodes: null
  avg_edges: null
  num_classes: null
result_count: 11
best_model:
  model: GPS
  value: 0.053
  metric: MAE
  arxiv_id: '2512.17762'
  paper_title: ECHO Benchmark
papers:
- arxiv_id: '2512.17762'
  title: ECHO Benchmark
  date_iso: '2025-12-19'
  venue: ICLR 2025
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: MAE
  default_metric: MAE
  higher_is_better: false
  stats:
    num_graphs: 196000
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - MAE
  metric_display_names:
  - MAE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_iso: '2025-12-19'
    date_display: Dec 2025
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.053
    metric_stds:
    - 0.008
  - model: DRew
    model_plain: DRew
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_iso: '2025-12-19'
    date_display: Dec 2025
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.113
    metric_stds:
    - 0.024
  - model: A-DGN
    model_plain: A-DGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_iso: '2025-12-19'
    date_display: Dec 2025
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.125
    metric_stds:
    - 0.016
  - model: SWAN
    model_plain: SWAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_iso: '2025-12-19'
    date_display: Dec 2025
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.126
    metric_stds:
    - 0.012
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_iso: '2025-12-19'
    date_display: Dec 2025
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.132
    metric_stds:
    - 0.026
  - model: GraphCON
    model_plain: GraphCON
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_iso: '2025-12-19'
    date_display: Dec 2025
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.143
    metric_stds:
    - 0.008
  - model: PH-DGN
    model_plain: PH-DGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_iso: '2025-12-19'
    date_display: Dec 2025
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.161
    metric_stds:
    - 0.011
  - model: GINE
    model_plain: GINE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_iso: '2025-12-19'
    date_display: Dec 2025
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.236
    metric_stds:
    - 0.076
  - model: GRIT
    model_plain: GRIT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_iso: '2025-12-19'
    date_display: Dec 2025
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.255
    metric_stds:
    - 0.025
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_iso: '2025-12-19'
    date_display: Dec 2025
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.281
    metric_stds:
    - 0.012
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_iso: '2025-12-19'
    date_display: Dec 2025
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.479
    metric_stds:
    - 0.102
  row_count: 11
  rows_json: ''
  chart_json: /data/datasets/echo-energy/standard-split-chart.json
  arch_counts:
    gnn: 9
    hybrid: 1
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 1
  metric_counts:
  - 11
  milestones: &id001
  - value: 0.053
    std: 0.008
    model: GPS
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: '2025-12-19'
  milestones_by_metric:
    MAE: *id001
---

