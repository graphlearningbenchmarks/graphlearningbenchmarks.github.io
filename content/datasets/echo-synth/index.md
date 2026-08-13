---
title: ECHO-Synth
slug: echo-synth
benchmark: ECHO Benchmark
task_type: graph_regression
short_description: Predict graph diameter, node eccentricity, and single-source shortest-path
  distances on synthetic graphs.
description: '**Mixed graph/node regression suite** covering diameter (graph-level),
  eccentricity (node-level), and SSSP (node-level) on synthetic long-range graphs.
  Inputs expose only local graph state while targets require long-range information.
  Evaluated by MAE.'
detailed_description:
  task: ECHO synthetic propagation task — node-level regression on synthetic long-range
    graphs. The primary catalog metric is MAE.
  data: ECHO synthetic propagation task — node-level regression on synthetic long-range
    graphs. The cataloged artifact reports 10,080 graphs.
  features: Each synthetic or physical graph supplies local node/edge state and a
    target created by controlled long-range propagation. The exact signal channels
    and propagation parameters are part of the named ECHO task and should not be mixed
    across variants.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses MAE (lower is better). Exact masks or folds must come from
    the cited release.'
  quirks_and_pitfalls: Performance is sensitive to propagation radius, graph size,
    and train/test distance regime. Randomly mixing configurations can turn a long-range
    extrapolation task into interpolation; report the named variant and fixed generation
    parameters.
sources:
- title: ECHO Benchmark benchmark
  arxiv_id: '2512.17762'
  kind: benchmark_or_upstream_source
primary_metric: MAE
higher_is_better: false
pyg_url: ''
stats:
  num_graphs: 10080
  avg_nodes: null
  avg_edges: null
  num_classes: null
result_count: 13
best_model:
  model: GHR
  value: 0.035
  metric: MAE
  arxiv_id: '2605.18387'
  paper_title: Graph Hierarchical Recurrence for Long-Range Generalization
papers:
- arxiv_id: '2605.18387'
  title: Graph Hierarchical Recurrence for Long-Range Generalization
  date_iso: '2026-05-18'
  venue: ''
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
    num_graphs: 10080
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
  - model: GHR
    model_plain: GHR
    is_baseline: false
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.035
    metric_stds:
    - 0.004
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
    - 0.121
    metric_stds:
    - 0.013
  - model: GHR-GINE
    model_plain: GHR-GINE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.379
    metric_stds:
    - 0.191
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.472
    metric_stds:
    - 0.05
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
    - 0.896
    metric_stds:
    - 0.232
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
    - 1.151
    metric_stds:
    - 0.038
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.243
    metric_stds:
    - 0.047
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
    - 1.323
    metric_stds:
    - 0.485
  - model: GIN/GINE
    model_plain: GIN/GINE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 1.63
    metric_stds:
    - 0.161
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
    - 1.63
    metric_stds:
    - 0.161
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
    - 2.005
    metric_stds:
    - 0.093
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
    - 2.102
    metric_stds:
    - 0.094
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
    - 2.969
    metric_stds:
    - 0.189
  row_count: 13
  rows_json: ''
  chart_json: /data/datasets/echo-synth/standard-split-chart.json
  arch_counts:
    gnn: 9
    hybrid: 2
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 1
  metric_counts:
  - 13
  milestones: &id001
  - value: 0.121
    std: 0.013
    model: GRIT
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: '2025-12-19'
  - value: 0.035
    std: 0.004
    model: GHR
    arxiv_id: '2605.18387'
    title: Graph Hierarchical Recurrence for Long-Range Generalization
    date: '2026-05-18'
  milestones_by_metric:
    MAE: *id001
---

