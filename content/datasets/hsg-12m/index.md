---
title: HSG-12M
slug: hsg-12m
benchmark: HSG-12M
task_type: graph_classification
description: Node classification on the HSG-12M large-scale heterogeneous spatial
  graph (~12M edges).
primary_metric: Accuracy
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 11601681
  avg_nodes: null
  avg_edges: null
  num_classes: 1401
result_count: 8
best_model:
  model: GraphSAGE
  value: 0.546
  metric: Accuracy
  arxiv_id: '2506.08618'
  paper_title: HSG-12M
papers:
- arxiv_id: '2506.08618'
  title: HSG-12M
  date_iso: '2025-06-10'
  venue: ICLR 2025
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 11601681
    avg_nodes: null
    avg_edges: null
    num_classes: 1401
  metrics:
  - Accuracy
  - Top-10 Acc.
  metric_display_names:
  - Accuracy
  - Top-10 Acc.
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.08618'
    title: HSG-12M
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: https://github.com/sarinstein-yan/HSG-12M
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.546
    - 0.952
    metric_stds:
    - 0.004
    - 0.001
  - model: CGCNN
    model_plain: CGCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.08618'
    title: HSG-12M
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: https://github.com/sarinstein-yan/HSG-12M
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.531
    - null
    metric_stds:
    - 0.004
    - null
  - model: GINE
    model_plain: GINE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.08618'
    title: HSG-12M
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: https://github.com/sarinstein-yan/HSG-12M
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.46
    - 0.921
    metric_stds:
    - 0.025
    - 0.011
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.08618'
    title: HSG-12M
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: https://github.com/sarinstein-yan/HSG-12M
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.365
    - null
    metric_stds:
    - 0.021
    - null
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.08618'
    title: HSG-12M
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: https://github.com/sarinstein-yan/HSG-12M
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.365
    - null
    metric_stds:
    - 0.01
    - null
  - model: GATv2
    model_plain: GATv2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.08618'
    title: HSG-12M
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: https://github.com/sarinstein-yan/HSG-12M
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.351
    - null
    metric_stds:
    - 0.002
    - null
  - model: MF
    model_plain: MF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.08618'
    title: HSG-12M
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: https://github.com/sarinstein-yan/HSG-12M
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.295
    - null
    metric_stds:
    - 0.01
    - null
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.08618'
    title: HSG-12M
    date: Jun 10, 2025
    date_iso: '2025-06-10'
    date_display: Jun 2025
    codebase_url: https://github.com/sarinstein-yan/HSG-12M
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.063
    - null
    metric_stds:
    - 0.031
    - null
  row_count: 8
  rows_json: ''
  chart_json: /data/datasets/hsg-12m/standard-split-chart.json
  arch_counts:
    gnn: 8
    hybrid: 0
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 8
  - 2
  milestones: &id001
  - value: 0.546
    std: 0.004
    model: GraphSAGE
    arxiv_id: '2506.08618'
    title: HSG-12M
    date: '2025-06-10'
  milestones_by_metric:
    Accuracy: *id001
    Top-10 Acc.:
    - value: 0.952
      std: 0.001
      model: GraphSAGE
      arxiv_id: '2506.08618'
      title: HSG-12M
      date: '2025-06-10'
---

