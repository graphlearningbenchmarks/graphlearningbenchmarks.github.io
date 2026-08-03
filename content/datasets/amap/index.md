---
title: AMAP
slug: amap
benchmark: Hypergraph Benchmarks
task_type: node_classification
description: Amazon Photography co-purchase hypergraph node classification (8 categories).
primary_metric: F1
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.Amazon.html
stats:
  num_graphs: 1
  avg_nodes: null
  avg_edges: null
  num_classes: 8
result_count: 126
best_model:
  model: GANN
  value: 0.9405
  metric: F1
  arxiv_id: '2303.07778'
  paper_title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
papers:
- arxiv_id: '2507.20127'
  title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph Message-passing'
  date_iso: '2025-07-27'
  venue: ''
- arxiv_id: '2508.14097'
  title: Non-Dissipative Graph Propagation for Non-Local Community Detection
  date_iso: '2025-06-30'
  venue: ''
- arxiv_id: '2403.03670'
  title: 'CDC: A Simple Framework for Complex Data Clustering'
  date_iso: '2024-03-06'
  venue: ''
- arxiv_id: '2403.03666'
  title: Provable Filter for Real-world Graph Clustering
  date_iso: '2024-03-06'
  venue: ''
- arxiv_id: '2308.08963'
  title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
  date_iso: '2023-08-17'
  venue: ''
- arxiv_id: '2308.06827'
  title: Reinforcement Graph Clustering with Unknown Cluster Number
  date_iso: '2023-08-13'
  venue: ''
- arxiv_id: '2307.14613'
  title: Self-Contrastive Graph Diffusion Network
  date_iso: '2023-07-27'
  venue: ''
- arxiv_id: '2303.07778'
  title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
  date_iso: '2023-03-14'
  venue: ''
- arxiv_id: '2212.08665'
  title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
  date_iso: '2022-12-16'
  venue: AAAI 2022
- arxiv_id: '2212.03559'
  title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
  date_iso: '2022-12-07'
  venue: ''
- arxiv_id: '2205.07865'
  title: Simple Contrastive Graph Clustering
  date_iso: '2022-05-11'
  venue: ''
- arxiv_id: '2202.12533'
  title: Improved Dual Correlation Reduction Network
  date_iso: '2022-02-25'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: F1
  default_metric: F1
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: null
    avg_edges: null
    num_classes: 8
  metrics:
  - F1
  - ACC
  - ARI
  - Conductance
  - NMI
  metric_display_names:
  - F1
  - ACC
  - ARI
  - Conductance
  - NMI
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GANN
    model_plain: GANN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9405
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0037
    - null
    - null
    - null
    - null
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9308
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
    - null
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
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9238
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0014
    - null
    - null
    - null
    - null
  - model: JK-Net
    model_plain: JK-Net
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9168
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0082
    - null
    - null
    - null
    - null
  - model: GCN-Cheby
    model_plain: GCN-Cheby
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9156
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0075
    - null
    - null
    - null
    - null
  - model: GWNN
    model_plain: GWNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9075
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0126
    - null
    - null
    - null
    - null
  - model: SGC
    model_plain: SGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9017
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0075
    - null
    - null
    - null
    - null
  - model: FAGCN
    model_plain: FAGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9006
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0104
    - null
    - null
    - null
    - null
  - model: MixupForGraph
    model_plain: MixupForGraph
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8728
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0108
    - null
    - null
    - null
    - null
  - model: PPNP
    model_plain: PPNP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8627
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0074
    - null
    - null
    - null
    - null
  - model: APPNP
    model_plain: APPNP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8602
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0076
    - null
    - null
    - null
    - null
  - model: IDCRN
    model_plain: IDCRN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_iso: '2022-02-25'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8208
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
    - null
    - null
  - model: V. GCN
    model_plain: V. GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8141
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0147
    - null
    - null
    - null
    - null
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    date: Mar 14, 2023
    date_iso: '2023-03-14'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8115
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0105
    - null
    - null
    - null
    - null
  - model: DCRN
    model_plain: DCRN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_iso: '2022-02-25'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7966
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0025
    - null
    - null
    - null
    - null
  - model: DFCN
    model_plain: DFCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_iso: '2022-02-25'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.76
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
    - null
    - null
  - model: SCGDN
    model_plain: SCGDN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.14613'
    title: Self-Contrastive Graph Diffusion Network
    date: Jul 27, 2023
    date_iso: '2023-07-27'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7527
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
    - null
    - null
  - model: CONVERT
    model_plain: CONVERT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.08963'
    title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    date: Aug 17, 2023
    date_iso: '2023-08-17'
    date_display: Aug 2023
    codebase_url: https://github.com/xihongyang1999/CONVERT
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7403
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.01
    - null
    - null
    - null
    - null
  - model: NACL
    model_plain: NACL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.08963'
    title: 'CONVERT: Contrastive Graph Clustering with Reliable Augmentation'
    date: Aug 17, 2023
    date_iso: '2023-08-17'
    date_display: Aug 2023
    codebase_url: https://github.com/xihongyang1999/CONVERT
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7304
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0108
    - null
    - null
    - null
    - null
  - model: GraphLearner
    model_plain: GraphLearner
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7302
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0234
    - null
    - null
    - null
    - null
  - model: CDC
    model_plain: CDC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2403.03670'
    title: 'CDC: A Simple Framework for Complex Data Clustering'
    date: Mar 6, 2024
    date_iso: '2024-03-06'
    date_display: Mar 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.73
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
  - model: SCAGC
    model_plain: SCAGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7277
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
    - null
    - null
  - model: SCGC
    model_plain: SCGC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7222
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0097
    - null
    - null
    - null
    - null
  - model: AGE
    model_plain: AGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7174
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0093
    - null
    - null
    - null
    - null
  - model: DFCN
    model_plain: DFCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7125
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0031
    - null
    - null
    - null
    - null
  - model: HSAN
    model_plain: HSAN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7115
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
    - null
    - null
  - model: AGC-DRR
    model_plain: AGC-DRR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7103
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0064
    - null
    - null
    - null
    - null
  - model: DCRN
    model_plain: DCRN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7086
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
    - null
    - null
  - model: AFGRL
    model_plain: AFGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6999
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0034
    - null
    - null
    - null
    - null
  - model: DEAGC
    model_plain: DEAGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6987
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0054
    - null
    - null
    - null
    - null
  - model: DAEGC
    model_plain: DAEGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6987
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0054
    - null
    - null
    - null
    - null
  - model: AGE
    model_plain: AGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6973
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0024
    - null
    - null
    - null
    - null
  - model: DFCN
    model_plain: DFCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.695
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
    - null
    - null
  - model: MCGC
    model_plain: MCGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.03670'
    title: 'CDC: A Simple Framework for Complex Data Clustering'
    date: Mar 6, 2024
    date_iso: '2024-03-06'
    date_display: Mar 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.686
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
  - model: AGC-DRR
    model_plain: AGC-DRR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6832
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0183
    - null
    - null
    - null
    - null
  - model: GAE
    model_plain: GAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6808
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0176
    - null
    - null
    - null
    - null
  - model: MGAE
    model_plain: MGAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.14613'
    title: Self-Contrastive Graph Diffusion Network
    date: Jul 27, 2023
    date_iso: '2023-07-27'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6808
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0176
    - null
    - null
    - null
    - null
  - model: SDCN
    model_plain: SDCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_iso: '2022-02-25'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6805
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0181
    - null
    - null
    - null
    - null
  - model: DMoN
    model_plain: DMoN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.14097'
    title: Non-Dissipative Graph Propagation for Non-Local Community Detection
    date: Jun 30, 2025
    date_iso: '2025-06-30'
    date_display: Jun 2025
    codebase_url: https://github.com/willleeney/ugle
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: true
    metric_values:
    - 0.67
    - null
    - null
    - 0.6
    - 0.61
    metric_stds:
    - 0.1
    - null
    - null
    - 0.49
    - 0.08
  - model: AutoSSL
    model_plain: AutoSSL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6676
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0067
    - null
    - null
    - null
    - null
  - model: GDCL
    model_plain: GDCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6639
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0065
    - null
    - null
    - null
    - null
  - model: ProGCL
    model_plain: ProGCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6592
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
    - null
    - null
  - model: SDCN_Q
    model_plain: SDCN_Q
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_iso: '2022-02-25'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6574
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0134
    - null
    - null
    - null
    - null
  - model: SUBLIME
    model_plain: SUBLIME
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.14097'
    title: Non-Dissipative Graph Propagation for Non-Local Community Detection
    date: Jun 30, 2025
    date_iso: '2025-06-30'
    date_display: Jun 2025
    codebase_url: https://github.com/willleeney/ugle
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.65
    - null
    - null
    - 0.23
    - 0.6
    metric_stds:
    - 0.07
    - null
    - null
    - 0.18
    - 0.04
  - model: ARGA
    model_plain: ARGA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_iso: '2022-02-25'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6483
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0059
    - null
    - null
    - null
    - null
  - model: DAEGC
    model_plain: DAEGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6454
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0139
    - null
    - null
    - null
    - null
  - model: MvAGC
    model_plain: MvAGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.03670'
    title: 'CDC: A Simple Framework for Complex Data Clustering'
    date: Mar 6, 2024
    date_iso: '2024-03-06'
    date_display: Mar 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.64
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
  - model: MVGRL
    model_plain: MVGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6283
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0159
    - null
    - null
    - null
    - null
  - model: DAEGC
    model_plain: DAEGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: Feb 25, 2022
    date_iso: '2022-02-25'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6205
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0048
    - null
    - null
    - null
    - null
  - model: MGAE
    model_plain: MGAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6135
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
    - null
    - null
  row_count: 126
  rows_json: /data/datasets/amap/standard-split-rows.json
  chart_json: /data/datasets/amap/standard-split-chart.json
  arch_counts:
    gnn: 110
    hybrid: 7
    graph_transformer: 0
    llm: 0
    walk: 2
    traditional: 7
  metric_counts:
  - 81
  - 26
  - 19
  - 8
  - 50
  milestones: &id001
  - value: 0.8208
    std: 0.0018
    model: IDCRN
    arxiv_id: '2202.12533'
    title: Improved Dual Correlation Reduction Network
    date: '2022-02-25'
  milestones_by_metric:
    F1: *id001
    ACC:
    - value: 0.7994
      std: null
      model: DCRN
      arxiv_id: '2403.03666'
      title: Provable Filter for Real-world Graph Clustering
      date: '2024-03-06'
    ARI:
    - value: 0.6015
      std: 0.0156
      model: AGC-DRR
      arxiv_id: '2308.06827'
      title: Reinforcement Graph Clustering with Unknown Cluster Number
      date: '2023-08-13'
    Conductance:
    - value: 0.23
      std: 0.18
      model: SUBLIME
      arxiv_id: '2508.14097'
      title: Non-Dissipative Graph Propagation for Non-Local Community Detection
      date: '2025-06-30'
    NMI:
    - value: 0.6961
      std: 0.0036
      model: RGC
      arxiv_id: '2308.06827'
      title: Reinforcement Graph Clustering with Unknown Cluster Number
      date: '2023-08-13'
    - value: 0.737
      std: null
      model: DCRN
      arxiv_id: '2403.03666'
      title: Provable Filter for Real-world Graph Clustering
      date: '2024-03-06'
---

