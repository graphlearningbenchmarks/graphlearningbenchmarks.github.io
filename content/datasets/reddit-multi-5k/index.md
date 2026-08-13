---
title: REDDIT-MULTI-5K
slug: reddit-multi-5k
benchmark: TU Dortmund
task_type: graph_classification
short_description: Multi-class graph classification of Reddit discussion threads (5
  subreddits).
description: '**5-class graph classification** Multi-class graph classification of
  Reddit discussion threads (5 subreddits). Uses the released node/edge labels or
  attributes; several social datasets are featureless. Evaluated by Accuracy.'
detailed_description:
  task: Multi-class graph classification of Reddit discussion threads (5 subreddits).
    The primary catalog metric is Accuracy.
  data: Multi-class graph classification of Reddit discussion threads (5 subreddits).
    The cataloged artifact reports 4,999 graphs, 5 target classes or tasks.
  features: The TU text format may contain discrete node or edge labels and optional
    continuous attributes. Social-network datasets commonly have no intrinsic node
    attributes, so papers often add constant or degree features; that choice changes
    the input.
  splits_and_evaluation: 'The catalog records these protocols or variants: 10-fold
    CV. Evaluation uses Accuracy (higher is better). Exact masks or folds must come
    from the cited release.'
  quirks_and_pitfalls: TU datasets have no canonical train/test split. Report cross-validation
    folds, seeds, feature construction, and whether duplicate or isomorphic graphs
    were removed; published results can otherwise differ for protocol rather than
    model quality.
sources:
- title: TU Dortmund benchmark
  arxiv_id: '2007.08663'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric REDDIT-MULTI-5K loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
stats:
  num_graphs: 4999
  avg_nodes: 508.52
  avg_edges: 594.87
  num_classes: 5
result_count: 42
best_model:
  model: SpeGCL
  value: 0.5944
  metric: Accuracy
  arxiv_id: '2410.10365'
  paper_title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without
    Positive Samples'
papers:
- arxiv_id: '2509.22100'
  title: 'SHAKE-GNN: Scalable Hierarchical Kirchhoff-Forest Graph Neural Network'
  date_iso: '2025-09-26'
  venue: ''
- arxiv_id: '2410.10365'
  title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
    Samples'
  date_iso: '2024-10-14'
  venue: ''
- arxiv_id: '2401.16011'
  title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
    pooling'
  date_iso: '2024-01-29'
  venue: ''
- arxiv_id: '2401.03638'
  title: Unifying Graph Contrastive Learning via Graph Message Augmentation
  date_iso: '2024-01-08'
  venue: ''
- arxiv_id: '2305.17437'
  title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
  date_iso: '2023-05-27'
  venue: ''
- arxiv_id: '2204.11028'
  title: Reinforced Causal Explainer for Graph Neural Networks
  date_iso: '2022-04-23'
  venue: ''
variants:
- slug: 10-fold-cv
  name: 10-fold CV
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 4999
    avg_nodes: 508.52
    avg_edges: 594.87
    num_classes: 5
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: SpeGCL
    model_plain: SpeGCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2410.10365'
    title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
      Samples'
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.5944
    metric_stds:
    - 0.0018
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.16011'
    title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
      pooling'
    date: Jan 29, 2024
    date_iso: '2024-01-29'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.576
    metric_stds:
    - 0.015
  - model: LAMP-Soft
    model_plain: LAMP-Soft
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10365'
    title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
      Samples'
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5738
    metric_stds:
    - 0.0041
  - model: GCS
    model_plain: GCS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10365'
    title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
      Samples'
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5704
    metric_stds:
    - 0.0049
  - model: GMCL-M
    model_plain: GMCL-M
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.5681
    metric_stds:
    - 0.025
  - model: AutoGCL
    model_plain: AutoGCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5675
    metric_stds:
    - 0.0018
  - model: GMCL-D
    model_plain: GMCL-D
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5663
    metric_stds:
    - 0.0186
  - model: GMCL-P
    model_plain: GMCL-P
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5635
    metric_stds:
    - 0.0231
  - model: GPS-TopK
    model_plain: GPS-TopK
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2401.16011'
    title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
      pooling'
    date: Jan 29, 2024
    date_iso: '2024-01-29'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.563
    metric_stds:
    - 0.002
  - model: SEGA
    model_plain: SEGA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10365'
    title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
      Samples'
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5613
    metric_stds:
    - 0.003
  - model: GraphCL
    model_plain: GraphCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5599
    metric_stds:
    - 0.0028
  - model: SimGRACE
    model_plain: SimGRACE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.16011'
    title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
      pooling'
    date: Jan 29, 2024
    date_iso: '2024-01-29'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.559
    metric_stds:
    - 0.004
  - model: GPS-Cluster
    model_plain: GPS-Cluster
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2401.16011'
    title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
      pooling'
    date: Jan 29, 2024
    date_iso: '2024-01-29'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.559
    metric_stds:
    - 0.004
  - model: GRACE
    model_plain: GRACE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5571
    metric_stds:
    - 0.0083
  - model: JOAO
    model_plain: JOAO
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.16011'
    title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
      pooling'
    date: Jan 29, 2024
    date_iso: '2024-01-29'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.557
    metric_stds:
    - 0.006
  - model: AD-GCL
    model_plain: AD-GCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.16011'
    title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
      pooling'
    date: Jan 29, 2024
    date_iso: '2024-01-29'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.549
    metric_stds:
    - 0.004
  - model: GIMM-Un-Fit
    model_plain: GIMM-Un-Fit
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.17437'
    title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    date: May 27, 2023
    date_iso: '2023-05-27'
    date_display: May 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5396
    metric_stds:
    - 0.0051
  - model: Infomax
    model_plain: Infomax
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5361
    metric_stds:
    - 0.0031
  - model: AD-GCL
    model_plain: AD-GCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.17437'
    title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    date: May 27, 2023
    date_iso: '2023-05-27'
    date_display: May 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5349
    metric_stds:
    - 0.0028
  - model: InfoGraph
    model_plain: InfoGraph
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5346
    metric_stds:
    - 0.0103
  - model: JOAOv2
    model_plain: JOAOv2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.17437'
    title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    date: May 27, 2023
    date_iso: '2023-05-27'
    date_display: May 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5271
    metric_stds:
    - 0.0028
  - model: AutoGCL
    model_plain: AutoGCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.17437'
    title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    date: May 27, 2023
    date_iso: '2023-05-27'
    date_display: May 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4991
    metric_stds:
    - 0.027
  - model: Original
    model_plain: Original
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.22100'
    title: 'SHAKE-GNN: Scalable Hierarchical Kirchhoff-Forest Graph Neural Network'
    date: Sep 26, 2025
    date_iso: '2025-09-26'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.492
    metric_stds:
    - null
  - model: Coarsened
    model_plain: Coarsened
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.22100'
    title: 'SHAKE-GNN: Scalable Hierarchical Kirchhoff-Forest Graph Neural Network'
    date: Sep 26, 2025
    date_iso: '2025-09-26'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.481
    metric_stds:
    - null
  - model: GraphCL
    model_plain: GraphCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.17437'
    title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    date: May 27, 2023
    date_iso: '2023-05-27'
    date_display: May 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4809
    metric_stds:
    - 0.0174
  - model: graph2vec
    model_plain: graph2vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4786
    metric_stds:
    - 0.0026
  - model: RC-Explainer
    model_plain: RC-Explainer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2204.11028'
    title: Reinforced Causal Explainer for Graph Neural Networks
    date: Apr 23, 2022
    date_iso: '2022-04-23'
    date_display: Apr 2022
    codebase_url: https://github.com/xiangwang1223/reinforced_causal_explainer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.472
    metric_stds:
    - null
  - model: WL
    model_plain: WL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4606
    metric_stds:
    - 0.0021
  - model: JOAOv2
    model_plain: JOAOv2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10365'
    title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
      Samples'
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4557
    metric_stds:
    - 0.0286
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.16011'
    title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
      pooling'
    date: Jan 29, 2024
    date_iso: '2024-01-29'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.438
    metric_stds:
    - 0.032
  - model: DGK
    model_plain: DGK
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4127
    metric_stds:
    - 0.0018
  - model: GL
    model_plain: GL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4101
    metric_stds:
    - 0.0017
  - model: GK
    model_plain: GK
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    arxiv_id: '2401.16011'
    title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
      pooling'
    date: Jan 29, 2024
    date_iso: '2024-01-29'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.41
    metric_stds:
    - 0.002
  - model: SP
    model_plain: SP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.16011'
    title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
      pooling'
    date: Jan 29, 2024
    date_iso: '2024-01-29'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.396
    metric_stds:
    - 0.002
  - model: Sub2Vec
    model_plain: Sub2Vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: Jan 8, 2024
    date_iso: '2024-01-08'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3668
    metric_stds:
    - 0.0042
  - model: GCA
    model_plain: GCA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.17437'
    title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    date: May 27, 2023
    date_iso: '2023-05-27'
    date_display: May 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: true
    metric_values:
    - 0.3295
    metric_stds:
    - 0.1089
  - model: PGM-Explainer
    model_plain: PGM-Explainer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2204.11028'
    title: Reinforced Causal Explainer for Graph Neural Networks
    date: Apr 23, 2022
    date_iso: '2022-04-23'
    date_display: Apr 2022
    codebase_url: https://github.com/xiangwang1223/reinforced_causal_explainer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3
    metric_stds:
    - null
  - model: CXPlain
    model_plain: CXPlain
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2204.11028'
    title: Reinforced Causal Explainer for Graph Neural Networks
    date: Apr 23, 2022
    date_iso: '2022-04-23'
    date_display: Apr 2022
    codebase_url: https://github.com/xiangwang1223/reinforced_causal_explainer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.279
    metric_stds:
    - null
  - model: PGExplainer
    model_plain: PGExplainer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2204.11028'
    title: Reinforced Causal Explainer for Graph Neural Networks
    date: Apr 23, 2022
    date_iso: '2022-04-23'
    date_display: Apr 2022
    codebase_url: https://github.com/xiangwang1223/reinforced_causal_explainer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.175
    metric_stds:
    - null
  - model: SA
    model_plain: SA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2204.11028'
    title: Reinforced Causal Explainer for Graph Neural Networks
    date: Apr 23, 2022
    date_iso: '2022-04-23'
    date_display: Apr 2022
    codebase_url: https://github.com/xiangwang1223/reinforced_causal_explainer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.158
    metric_stds:
    - null
  - model: Grad-CAM
    model_plain: Grad-CAM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2204.11028'
    title: Reinforced Causal Explainer for Graph Neural Networks
    date: Apr 23, 2022
    date_iso: '2022-04-23'
    date_display: Apr 2022
    codebase_url: https://github.com/xiangwang1223/reinforced_causal_explainer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.158
    metric_stds:
    - null
  - model: GNNExplainer
    model_plain: GNNExplainer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2204.11028'
    title: Reinforced Causal Explainer for Graph Neural Networks
    date: Apr 23, 2022
    date_iso: '2022-04-23'
    date_display: Apr 2022
    codebase_url: https://github.com/xiangwang1223/reinforced_causal_explainer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.125
    metric_stds:
    - null
  row_count: 42
  rows_json: ''
  chart_json: /data/datasets/reddit-multi-5k/10-fold-cv-chart.json
  arch_counts:
    gnn: 25
    hybrid: 6
    graph_transformer: 0
    llm: 0
    walk: 2
    traditional: 7
  metric_counts:
  - 42
  milestones: &id001
  - value: 0.472
    std: null
    model: RC-Explainer
    arxiv_id: '2204.11028'
    title: Reinforced Causal Explainer for Graph Neural Networks
    date: '2022-04-23'
  - value: 0.5396
    std: 0.0051
    model: GIMM-Un-Fit
    arxiv_id: '2305.17437'
    title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    date: '2023-05-27'
  - value: 0.5681
    std: 0.025
    model: GMCL-M
    arxiv_id: '2401.03638'
    title: Unifying Graph Contrastive Learning via Graph Message Augmentation
    date: '2024-01-08'
  - value: 0.576
    std: 0.015
    model: GIN
    arxiv_id: '2401.16011'
    title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
      pooling'
    date: '2024-01-29'
  - value: 0.5944
    std: 0.0018
    model: SpeGCL
    arxiv_id: '2410.10365'
    title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
      Samples'
    date: '2024-10-14'
  milestones_by_metric:
    Accuracy: *id001
---

