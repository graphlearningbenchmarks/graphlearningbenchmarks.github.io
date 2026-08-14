---
title: Tc-Ribo
slug: tc-ribo
benchmark: DualEquiNet RNA Benchmarks
task_type: graph_regression
short_description: Predict one sequence-level expression shift induced by tetracycline
  binding on RNA graphs.
description: '**Graph regression** on RNA graphs, predicting one sequence-level expression
  shift induced by tetracycline binding. Evaluated by RMSE.'
detailed_description:
  task: Thermostable ribosome structure prediction (graph regression, RMSE metric).
    The primary catalog metric is RMSE.
  data: Thermostable ribosome structure prediction (graph regression, RMSE metric).
    The cataloged artifact reports 355 graphs.
  features: RNA samples include nucleotide identity, predicted or experimental 3D
    atomic coordinates as specified by the dataset, and task-specific scalar targets.
    Euclidean cutoff edges and spherical-harmonic neighborhoods are model construction,
    not additional measurements.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses RMSE (lower is better). Exact masks or folds must come
    from the cited release.'
  quirks_and_pitfalls: Predicted structures must not be described as experimental
    ground truth. Random sequence splits can place close motifs in train and test,
    circular angles require periodic losses, and experimental targets have assay-specific
    noise and missingness.
sources:
- title: DualEquiNet RNA Benchmarks benchmark
  arxiv_id: '2506.19862'
  kind: benchmark_or_upstream_source
primary_metric: RMSE
higher_is_better: false
pyg_url: ''
stats:
  num_graphs: 355
  avg_nodes: 216.0
  avg_edges: null
  num_classes: null
  extra_stats:
    edge_feature_dim: 0
    feature_type: RNA nucleotide identity plus predicted 3D atomic coordinates
    node_count_range: 66--75 nucleotides; 216 atoms on average
    num_targets: 1
    statistic_notes: 'DualEquiNet Table: 355 sequences; graph-level tetracycline switching-factor
      target.'
result_count: 17
best_model:
  model: G-Heyna
  value: 0.548
  metric: RMSE
  arxiv_id: '2505.22560'
  paper_title: Geometric Hyena Networks for Large-scale Equivariant Learning
papers:
- arxiv_id: '2506.19862'
  title: DualEquiNet RNA Benchmarks
  date_iso: '2025-06-10'
  venue: ''
- arxiv_id: '2505.22560'
  title: Geometric Hyena Networks for Large-scale Equivariant Learning
  date_iso: '2025-05-28'
  venue: ICML 2025
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: RMSE
  default_metric: RMSE
  higher_is_better: false
  stats:
    num_graphs: 355
    avg_nodes: 216.0
    avg_edges: null
    num_classes: null
    extra_stats:
      edge_feature_dim: 0
      feature_type: RNA nucleotide identity plus predicted 3D atomic coordinates
      node_count_range: 66--75 nucleotides; 216 atoms on average
      num_targets: 1
      statistic_notes: 'DualEquiNet Table: 355 sequences; graph-level tetracycline
        switching-factor target.'
  metrics:
  - RMSE
  metric_display_names:
  - RMSE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: G-Heyna
    model_plain: G-Heyna
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.548
    metric_stds:
    - 0.008
  - model: Equiformer
    model_plain: Equiformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.55
    metric_stds:
    - 0.009
  - model: Transformer
    model_plain: Transformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.553
    metric_stds:
    - 0.002
  - model: G-Transformer
    model_plain: G-Transformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.553
    metric_stds:
    - 0.001
  - model: Hyena
    model_plain: Hyena
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.56
    metric_stds:
    - 0.002
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.636
    metric_stds:
    - 0.049
  - model: SchNet
    model_plain: SchNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.691
    metric_stds:
    - 0.018
  - model: FastEGNN
    model_plain: FastEGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.704
    metric_stds:
    - 0.005
  - model: TFN
    model_plain: TFN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.71
    metric_stds:
    - 0.009
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
    - 0.718
    metric_stds:
    - 0.002
  - model: EGNN
    model_plain: EGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.728
    metric_stds:
    - 0.001
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
    - 0.729
    metric_stds:
    - 0.007
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
    - 0.731
    metric_stds:
    - 0.006
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
    - 0.736
    metric_stds:
    - 0.003
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
    - 0.737
    metric_stds:
    - 0.002
  - model: LEFTNet
    model_plain: LEFTNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.749
    metric_stds:
    - 0.006
  - model: TMD-ET
    model_plain: TMD-ET
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.75
    metric_stds:
    - 0.004
  row_count: 17
  rows_json: ''
  chart_json: /data/datasets/tc-ribo/standard-split-chart.json
  arch_counts:
    gnn: 12
    hybrid: 2
    graph_transformer: 2
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 17
  milestones: &id001
  - value: 0.548
    std: 0.008
    model: G-Heyna
    arxiv_id: '2505.22560'
    title: Geometric Hyena Networks for Large-scale Equivariant Learning
    date: '2025-05-28'
  milestones_by_metric:
    RMSE: *id001
---

