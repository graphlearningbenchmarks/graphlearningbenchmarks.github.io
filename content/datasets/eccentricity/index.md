---
title: Eccentricity
slug: eccentricity
benchmark: Algorithmic Graph Tasks
task_type: node_regression
short_description: Predict each node’s maximum shortest-path distance to any other
  node on synthetic graphs.
description: '**Node regression** on synthetic graphs, predicting each node’s maximum
  shortest-path distance to any other node. Uses synthetic topology plus task-specific
  source indicators or random node features. Evaluated by MSE.'
detailed_description:
  task: Graph eccentricity prediction — node-level task predicting max distance to
    any other node. The primary catalog metric is MSE.
  data: 'The release has 7,040 synthetic graphs with 25--35 nodes sampled from multiple
    graph generators: 5,120 train, 640 validation, and 1,280 test graphs.'
  features: Synthetic graphs provide task-specific structural inputs such as a designated
    source. Targets are numeric node quantities computed by the reference algorithm;
    positional encodings or extra structural features are model additions.
  splits_and_evaluation: The fixed split is 5,120/640/1,280 graphs. The paper selects
    models by validation MSE and reports mean log10(MSE) over 20 runs; lower is better.
  quirks_and_pitfalls: Targets are deterministic functions of generated topology,
    so generator overlap and size range determine difficulty. Random splits test interpolation;
    claims about algorithmic generalization require held-out sizes or graph families.
sources:
- title: Algorithmic Graph Tasks benchmark
  arxiv_id: '2312.16560'
  kind: benchmark_or_upstream_source
primary_metric: MSE
higher_is_better: false
pyg_url: ''
stats:
  num_graphs: 7040
  avg_nodes: null
  avg_edges: null
  num_classes: null
result_count: 19
best_model:
  model: GCN-SSM + k-hop
  value: -4.2652
  metric: MSE
  arxiv_id: '2502.10818'
  paper_title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs:
    Bridging Recurrent and Graph Learning'
papers:
- arxiv_id: '2505.18728'
  title: 'Message-Passing State-Space Models: Improving Graph Learning with Modern
    Sequence Modeling'
  date_iso: '2025-05-24'
  venue: ''
- arxiv_id: '2502.10818'
  title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
    Recurrent and Graph Learning'
  date_iso: '2025-02-15'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: MSE
  default_metric: MSE
  higher_is_better: false
  stats:
    num_graphs: 7040
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - MSE
  metric_display_names:
  - MSE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GCN-SSM + k-hop
    model_plain: GCN-SSM + k-hop
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - -4.2652
    metric_stds:
    - 0.1776
  - model: MP-SSM
    model_plain: MP-SSM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.18728'
    title: 'Message-Passing State-Space Models: Improving Graph Learning with Modern
      Sequence Modeling'
    date: May 24, 2025
    date_iso: '2025-05-24'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -2.9724
    metric_stds:
    - 0.0271
  - model: GCN-SSM + eig(Lambda) approx 1
    model_plain: GCN-SSM + eig(Lambda) approx 1
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -2.2583
    metric_stds:
    - 0.0085
  - model: GCN-SSM
    model_plain: GCN-SSM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -2.2446
    metric_stds:
    - 0.0027
  - model: DRew-GCN
    model_plain: DRew-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -2.1004
    metric_stds:
    - 0.0256
  - model: DRew-GCN + delay
    model_plain: DRew-GCN + delay
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -2.0291
    metric_stds:
    - 0.024
  - model: PH-DGN
    model_plain: PH-DGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -0.9348
    metric_stds:
    - 0.2097
  - model: SWAN
    model_plain: SWAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -0.0739
    metric_stds:
    - 0.219
  - model: ADGN
    model_plain: ADGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4296
    metric_stds:
    - 0.1003
  - model: A-DGN
    model_plain: A-DGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.18728'
    title: 'Message-Passing State-Space Models: Improving Graph Learning with Modern
      Sequence Modeling'
    date: May 24, 2025
    date_iso: '2025-05-24'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4296
    metric_stds:
    - 0.1003
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6077
    metric_stds:
    - 0.0282
  - model: GRAND
    model_plain: GRAND
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6602
    metric_stds:
    - 0.1393
  - model: GraphCON
    model_plain: GraphCON
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6833
    metric_stds:
    - 0.0074
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.764
    metric_stds:
    - 0.0355
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7863
    metric_stds:
    - 0.0207
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7909
    metric_stds:
    - 0.0222
  - model: DGC
    model_plain: DGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8261
    metric_stds:
    - 0.0032
  - model: GCN
    model_plain: GCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8468
    metric_stds:
    - 0.0028
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9504
    metric_stds:
    - 0.0007
  row_count: 19
  rows_json: ''
  chart_json: /data/datasets/eccentricity/standard-split-chart.json
  arch_counts:
    gnn: 15
    hybrid: 2
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 19
  milestones: &id001
  - value: -4.2652
    std: 0.1776
    model: GCN-SSM + k-hop
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: '2025-02-15'
  milestones_by_metric:
    MSE: *id001
---

