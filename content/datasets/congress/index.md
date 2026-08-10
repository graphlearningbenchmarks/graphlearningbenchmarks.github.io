---
title: Congress
slug: congress
benchmark: Hypergraph Benchmarks
task_type: node_classification
description: US Congress bill co-sponsorship hypergraph node classification (2 classes).
primary_metric: Accuracy
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 1
  avg_nodes: null
  avg_edges: null
  num_classes: 2
result_count: 13
best_model:
  model: HealHGNN
  value: 0.9345
  metric: Accuracy
  arxiv_id: '2603.00599'
  paper_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local
    Exchanger
papers:
- arxiv_id: '2603.00599'
  title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
  date_iso: '2026-02-28'
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
    num_graphs: 1
    avg_nodes: null
    avg_edges: null
    num_classes: 2
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: HealHGNN
    model_plain: HealHGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9345
    metric_stds:
    - 0.0079
  - model: ED-HNN
    model_plain: ED-HNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9328
    metric_stds:
    - 0.0059
  - model: KHGNN
    model_plain: KHGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9255
    metric_stds:
    - 0.0103
  - model: Deep-HGNN
    model_plain: Deep-HGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9247
    metric_stds:
    - 0.0106
  - model: UniGCNII
    model_plain: UniGCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9243
    metric_stds:
    - 0.0071
  - model: AllSetTransformer
    model_plain: AllSetTransformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9216
    metric_stds:
    - 0.0105
  - model: SheafHyperGNN
    model_plain: SheafHyperGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9181
    metric_stds:
    - 0.016
  - model: AllDeepSets
    model_plain: AllDeepSets
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.918
    metric_stds:
    - 0.0153
  - model: HGNN
    model_plain: HGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9126
    metric_stds:
    - 0.0115
  - model: HNHN
    model_plain: HNHN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9089
    metric_stds:
    - 0.0031
  - model: HCHA
    model_plain: HCHA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9043
    metric_stds:
    - 0.012
  - model: PhenomNN
    model_plain: PhenomNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8824
    metric_stds:
    - 0.0147
  - model: HyperGCN
    model_plain: HyperGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8743
    metric_stds:
    - 0.0146
  row_count: 13
  rows_json: ''
  chart_json: /data/datasets/congress/standard-split-chart.json
  arch_counts:
    gnn: 12
    hybrid: 0
    graph_transformer: 1
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 13
  milestones: &id001
  - value: 0.9345
    std: 0.0079
    model: HealHGNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: '2026-02-28'
  milestones_by_metric:
    Accuracy: *id001
---

