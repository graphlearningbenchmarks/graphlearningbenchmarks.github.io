---
title: HSG-topology
slug: hsg-topology
benchmark: HSG-12M
task_type: graph_classification
short_description: Classify each topology-deduplicated Hamiltonian spectral graph
  into one of 1,401 characteristic-polynomial classes.
description: '**1,401-class graph classification** Classify each topology-deduplicated
  Hamiltonian spectral graph into one of 1,401 characteristic-polynomial classes.
  The variant is designed around unique connectivity patterns. Evaluated by Accuracy.'
detailed_description:
  task: Classify each topology-deduplicated Hamiltonian spectral graph into one of
    1,401 characteristic-polynomial classes.
  data: HSG-topology retains one representative of every graph-isomorphism class within
    each polynomial class, leaving 1,812,325 spatial multigraphs with a largest-to-
    smallest class-size ratio of 660.2.
  features: The variant is designed around unique connectivity patterns. Spatial multi-edge
    information remains available in the HSG representation, but topology-only models
    can deliberately omit it for the combinatorial experiment.
  splits_and_evaluation: The official stratified random split is 80/10/10 and evaluation
    reports accuracy averaged over three seeds.
  quirks_and_pitfalls: This is the only deliberately imbalanced HSG static variant.
    Plain accuracy is dominated by large classes; balanced metrics are useful diagnostics
    but are not the published headline. Isomorphism filtering must be performed within
    each class.
sources:
- title: HSG-12M benchmark
  arxiv_id: '2506.08618'
  kind: benchmark_or_upstream_source
primary_metric: Accuracy
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 1812325
  avg_nodes: null
  avg_edges: null
  num_classes: 1401
  extra_stats:
    edge_feature_dim: 6
    edge_feature_type: same six-dimensional spatial edge summaries as HSG-12M
    edge_semantics: spatial_multigraph
    feature_type: same spatial node representation as HSG-12M
    label_imbalance: largest/smallest class ratio 660.2
    node_feature_dim: 4
    statistic_notes: Topology variant keeps one representative per connectivity isomorphism
      class within each polynomial class.
result_count: 8
best_model:
  model: GraphSAGE
  value: 0.62
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
    num_graphs: 1812325
    avg_nodes: null
    avg_edges: null
    num_classes: 1401
    extra_stats:
      edge_feature_dim: 6
      edge_feature_type: same six-dimensional spatial edge summaries as HSG-12M
      edge_semantics: spatial_multigraph
      feature_type: same spatial node representation as HSG-12M
      label_imbalance: largest/smallest class ratio 660.2
      node_feature_dim: 4
      statistic_notes: Topology variant keeps one representative per connectivity
        isomorphism class within each polynomial class.
  metrics:
  - Accuracy
  - Loss
  - Macro F1
  - Top-10 Acc.
  - Top-5 Accuracy
  metric_display_names:
  - Accuracy
  - Loss
  - Macro F1
  - Top-10 Acc.
  - Top-5 Accuracy
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
    - 0.62
    - 1.019
    - 0.622
    - 0.958
    - 0.898
    metric_stds:
    - 0.003
    - 0.002
    - 0.001
    - 0.001
    - 0.002
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
    - 0.566
    - 1.191
    - 0.563
    - 0.94
    - 0.87
    metric_stds:
    - 0.016
    - 0.065
    - 0.018
    - 0.005
    - 0.008
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
    - 0.533
    - 1.316
    - 0.531
    - 0.927
    - 0.848
    metric_stds:
    - 0.017
    - 0.057
    - 0.011
    - 0.008
    - 0.013
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
    - 0.434
    - 1.825
    - 0.431
    - 0.855
    - 0.752
    metric_stds:
    - 0.015
    - 0.053
    - 0.011
    - 0.01
    - 0.014
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
    - 0.401
    - 1.968
    - 0.397
    - 0.833
    - 0.723
    metric_stds:
    - 0.003
    - 0.025
    - 0.001
    - 0.005
    - 0.005
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
    - 0.397
    - 2.062
    - 0.392
    - 0.825
    - 0.715
    metric_stds:
    - 0.009
    - 0.062
    - 0.011
    - 0.006
    - 0.007
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
    - 0.348
    - 2.222
    - 0.343
    - 0.793
    - 0.673
    metric_stds:
    - 0.012
    - 0.051
    - 0.012
    - 0.01
    - 0.011
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
    - 0.095
    - 4.179
    - 0.082
    - 0.39
    - 0.276
    metric_stds:
    - 0.059
    - 0.612
    - 0.06
    - 0.148
    - 0.127
  row_count: 8
  rows_json: ''
  chart_json: /data/datasets/hsg-topology/standard-split-chart.json
  arch_counts:
    gnn: 8
    hybrid: 0
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 8
  - 8
  - 8
  - 8
  - 8
  milestones: &id001
  - value: 0.62
    std: 0.003
    model: GraphSAGE
    arxiv_id: '2506.08618'
    title: HSG-12M
    date: '2025-06-10'
  milestones_by_metric:
    Accuracy: *id001
    Loss:
    - value: 1.019
      std: 0.002
      model: GraphSAGE
      arxiv_id: '2506.08618'
      title: HSG-12M
      date: '2025-06-10'
    Macro F1:
    - value: 0.622
      std: 0.001
      model: GraphSAGE
      arxiv_id: '2506.08618'
      title: HSG-12M
      date: '2025-06-10'
    Top-10 Acc.:
    - value: 0.958
      std: 0.001
      model: GraphSAGE
      arxiv_id: '2506.08618'
      title: HSG-12M
      date: '2025-06-10'
    Top-5 Accuracy:
    - value: 0.898
      std: 0.002
      model: GraphSAGE
      arxiv_id: '2506.08618'
      title: HSG-12M
      date: '2025-06-10'
---

