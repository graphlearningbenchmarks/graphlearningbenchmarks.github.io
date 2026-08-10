---
title: ogbn-mag
slug: ogbn-mag
benchmark: OGB
task_type: node_classification
description: Heterogeneous academic graph node classification (349 venue classes)
  from OGB.
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.OGB_MAG.html
stats:
  num_graphs: 1939743
  avg_nodes: 21111007.0
  avg_edges: null
  num_classes: 1
result_count: 105
best_model:
  model: LMSPS+LP+MS
  value: 0.5784
  metric: Accuracy
  arxiv_id: '2307.08430'
  paper_title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
papers:
- arxiv_id: '2604.27387'
  title: 'Robust Learning on Heterogeneous Graphs with Heterophily: A Graph Structure
    Learning Approach'
  date_iso: '2026-04-30'
  venue: ''
- arxiv_id: '2503.19666'
  title: 'Towards Efficient Training of Graph Neural Networks: A Multiscale Approach'
  date_iso: '2025-03-25'
  venue: TMLR 2025
- arxiv_id: '2410.02158'
  title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation Learning'
  date_iso: '2024-10-03'
  venue: TMLR 2024
- arxiv_id: '2312.02619'
  title: Rethinking and Simplifying Bootstrapped Graph Latents
  date_iso: '2023-12-05'
  venue: ''
- arxiv_id: '2310.14481'
  title: Efficient Heterogeneous Graph Learning via Random Projection
  date_iso: '2023-10-23'
  venue: ''
- arxiv_id: '2307.08430'
  title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
  date_iso: '2023-07-17'
  venue: NeurIPS 2023
- arxiv_id: '2305.19903'
  title: Improving Expressivity of GNNs with Subgraph-specific Factor Embedded Normalization
  date_iso: '2023-05-31'
  venue: KDD 2023
- arxiv_id: '2207.02547'
  title: Simple and Efficient Heterogeneous Graph Neural Network
  date_iso: '2022-07-06'
  venue: AAAI 2022
- arxiv_id: '2205.15653'
  title: Label-Enhanced Graph Neural Network for Semi-supervised Node Classification
  date_iso: '2022-05-31'
  venue: ''
- arxiv_id: '2112.04319'
  title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
  date_iso: '2021-12-08'
  venue: ''
- arxiv_id: '2108.13555'
  title: Adaptive Label Smoothing To Regularize Large-Scale Graph Training
  date_iso: '2021-08-30'
  venue: ''
- arxiv_id: '2108.10097'
  title: Graph Attention MLP with Reliable Label Utilization
  date_iso: '2021-08-23'
  venue: ''
- arxiv_id: '2106.09078'
  title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical Analysis of
    GNN Explanation Methods'
  date_iso: '2021-06-16'
  venue: ''
- arxiv_id: '2105.11122'
  title: Heterogeneous Graph Representation Learning with Relation Awareness
  date_iso: '2021-05-24'
  venue: ''
- arxiv_id: '2105.08330'
  title: 'Residual Network and Embedding Usage: New Tricks of Node Classification
    with Graph Convolutional Networks'
  date_iso: '2021-05-18'
  venue: ''
- arxiv_id: '2104.09376'
  title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced Training
  date_iso: '2021-04-19'
  venue: ''
- arxiv_id: '2011.09679'
  title: Scalable Graph Neural Networks for Heterogeneous Graphs
  date_iso: '2020-11-19'
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
    num_graphs: 1939743
    avg_nodes: 21111007.0
    avg_edges: null
    num_classes: 1
  metrics:
  - Accuracy
  - Instability
  - Unfaithfulness
  metric_display_names:
  - Accuracy
  - Instability
  - Unfaithfulness
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: LMSPS+LP+MS
    model_plain: LMSPS+LP+MS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.5784
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
  - model: SeHGNN+emb+ms
    model_plain: SeHGNN+emb+ms
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5719
    - null
    - null
    metric_stds:
    - 0.0012
    - null
    - null
  - model: SeHGNN+ms
    model_plain: SeHGNN+ms
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5671
    - null
    - null
    metric_stds:
    - 0.0014
    - null
    - null
  - model: SeHGNN+LP+MS
    model_plain: SeHGNN+LP+MS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5671
    - null
    - null
    metric_stds:
    - 0.0014
    - null
    - null
  - model: RLU+SCR
    model_plain: RLU+SCR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2112.04319'
    title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
    date: Dec 8, 2021
    date_iso: '2021-12-08'
    date_display: Dec 2021
    codebase_url: https://github.com/THUDM/SCR
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5631
    - null
    - null
    metric_stds:
    - 0.0021
    - null
    - null
  - model: RLU
    model_plain: RLU
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.04319'
    title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
    date: Dec 8, 2021
    date_iso: '2021-12-08'
    date_display: Dec 2021
    codebase_url: https://github.com/THUDM/SCR
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.559
    - null
    - null
    metric_stds:
    - 0.0027
    - null
    - null
  - model: GAMLP+emb+ms
    model_plain: GAMLP+emb+ms
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.559
    - null
    - null
    metric_stds:
    - 0.0027
    - null
    - null
  - model: NARS-GAMLP+RLU
    model_plain: NARS-GAMLP+RLU
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2108.10097'
    title: Graph Attention MLP with Reliable Label Utilization
    date: Aug 23, 2021
    date_iso: '2021-08-23'
    date_display: Aug 2021
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
    - null
    - null
    metric_stds:
    - 0.0027
    - null
    - null
  - model: LMSPS+LP
    model_plain: LMSPS+LP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.551
    - null
    - null
    metric_stds:
    - 0.0011
    - null
    - null
  - model: LMSPS
    model_plain: LMSPS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5483
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
  - model: SeHGNN+emb
    model_plain: SeHGNN+emb
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5478
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
  - model: SCR-m
    model_plain: SCR-m
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2112.04319'
    title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
    date: Dec 8, 2021
    date_iso: '2021-12-08'
    date_display: Dec 2021
    codebase_url: https://github.com/THUDM/SCR
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5451
    - null
    - null
    metric_stds:
    - 0.0019
    - null
    - null
  - model: SLE
    model_plain: SLE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.04319'
    title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
    date: Dec 8, 2021
    date_iso: '2021-12-08'
    date_display: Dec 2021
    codebase_url: https://github.com/THUDM/SCR
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.544
    - null
    - null
    metric_stds:
    - 0.0015
    - null
    - null
  - model: SAGN+emb+ms
    model_plain: SAGN+emb+ms
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.544
    - null
    - null
    metric_stds:
    - 0.0015
    - null
    - null
  - model: NARS-SAGN+2-SLE
    model_plain: NARS-SAGN+2-SLE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2108.10097'
    title: Graph Attention MLP with Reliable Label Utilization
    date: Aug 23, 2021
    date_iso: '2021-08-23'
    date_display: Aug 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.544
    - null
    - null
    metric_stds:
    - 0.0015
    - null
    - null
  - model: SCR
    model_plain: SCR
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2112.04319'
    title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
    date: Dec 8, 2021
    date_iso: '2021-12-08'
    date_display: Dec 2021
    codebase_url: https://github.com/THUDM/SCR
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5432
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
  - model: HGUL
    model_plain: HGUL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.27387'
    title: 'Robust Learning on Heterogeneous Graphs with Heterophily: A Graph Structure
      Learning Approach'
    date: Apr 30, 2026
    date_iso: '2026-04-30'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5421
    - null
    - null
    metric_stds:
    - 0.0027
    - null
    - null
  - model: SeHGNN
    model_plain: SeHGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5399
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
  - model: SeHGNN+LP
    model_plain: SeHGNN+LP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5399
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
  - model: NARS_GAMLP
    model_plain: NARS_GAMLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.04319'
    title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
    date: Dec 8, 2021
    date_iso: '2021-12-08'
    date_display: Dec 2021
    codebase_url: https://github.com/THUDM/SCR
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5396
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
  - model: GAMLP+emb
    model_plain: GAMLP+emb
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5396
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
  - model: NARS-GAMLP
    model_plain: NARS-GAMLP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2108.10097'
    title: Graph Attention MLP with Reliable Label Utilization
    date: Aug 23, 2021
    date_iso: '2021-08-23'
    date_display: Aug 2021
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
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
  - model: LEGNN + AS-Train
    model_plain: LEGNN + AS-Train
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15653'
    title: Label-Enhanced Graph Neural Network for Semi-supervised Node Classification
    date: May 31, 2022
    date_iso: '2022-05-31'
    date_display: May 2022
    codebase_url: https://github.com/yule-BUAA/LEGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5378
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
  - model: LEGNN
    model_plain: LEGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.02158'
    title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation Learning'
    date: Oct 3, 2024
    date_iso: '2024-10-03'
    date_display: Oct 2024
    codebase_url: https://github.com/joshem163/SCNode
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5378
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: LEGNN with SuperNorm
    model_plain: LEGNN with SuperNorm
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19903'
    title: Improving Expressivity of GNNs with Subgraph-specific Factor Embedded Normalization
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/chenchkx/SuperNorm
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5324
    - null
    - null
    metric_stds:
    - 0.0013
    - null
    - null
  - model: H2G-former
    model_plain: H2G-former
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2604.27387'
    title: 'Robust Learning on Heterogeneous Graphs with Heterophily: A Graph Structure
      Learning Approach'
    date: Apr 30, 2026
    date_iso: '2026-04-30'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5312
    - null
    - null
    metric_stds:
    - 0.0032
    - null
    - null
  - model: SIGN
    model_plain: SIGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19903'
    title: Improving Expressivity of GNNs with Subgraph-specific Factor Embedded Normalization
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/chenchkx/SuperNorm
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5289
    - null
    - null
    metric_stds:
    - 0.0011
    - null
    - null
  - model: LEGNN
    model_plain: LEGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.15653'
    title: Label-Enhanced Graph Neural Network for Semi-supervised Node Classification
    date: May 31, 2022
    date_iso: '2022-05-31'
    date_display: May 2022
    codebase_url: https://github.com/yule-BUAA/LEGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5276
    - null
    - null
    metric_stds:
    - 0.0014
    - null
    - null
  - model: NARS+emb
    model_plain: NARS+emb
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.524
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
  - model: NARS
    model_plain: NARS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2108.10097'
    title: Graph Attention MLP with Reliable Label Utilization
    date: Aug 23, 2021
    date_iso: '2021-08-23'
    date_display: Aug 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.524
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
  - model: NARS_SAGN
    model_plain: NARS_SAGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.04319'
    title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
    date: Dec 8, 2021
    date_iso: '2021-12-08'
    date_display: Dec 2021
    codebase_url: https://github.com/THUDM/SCR
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5232
    - null
    - null
    metric_stds:
    - 0.0025
    - null
    - null
  - model: NARS-SAGN+0-SLE
    model_plain: NARS-SAGN+0-SLE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2108.10097'
    title: Graph Attention MLP with Reliable Label Utilization
    date: Aug 23, 2021
    date_iso: '2021-08-23'
    date_display: Aug 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5232
    - null
    - null
    metric_stds:
    - 0.0025
    - null
    - null
  - model: RpHGNN
    model_plain: RpHGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.14481'
    title: Efficient Heterogeneous Graph Learning via Random Projection
    date: Oct 23, 2023
    date_iso: '2023-10-23'
    date_display: Oct 2023
    codebase_url: https://github.com/CrawlScript/RpHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5207
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
  - model: R-HGNN
    model_plain: R-HGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2105.11122'
    title: Heterogeneous Graph Representation Learning with Relation Awareness
    date: May 24, 2021
    date_iso: '2021-05-24'
    date_display: May 2021
    codebase_url: https://github.com/yule-BUAA/R-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5204
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GAMLP
    model_plain: GAMLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5163
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
  - model: GAMLP+LP
    model_plain: GAMLP+LP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5163
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
  - model: Hetero2Net
    model_plain: Hetero2Net
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.27387'
    title: 'Robust Learning on Heterogeneous Graphs with Heterophily: A Graph Structure
      Learning Approach'
    date: Apr 30, 2026
    date_iso: '2026-04-30'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.516
    - null
    - null
    metric_stds:
    - 0.0033
    - null
    - null
  - model: SeHGNN
    model_plain: SeHGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5145
    - null
    - null
    metric_stds:
    - 0.0029
    - null
    - null
  - model: SAGN
    model_plain: SAGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5117
    - null
    - null
    metric_stds:
    - 0.0032
    - null
    - null
  - model: SAGN+LP
    model_plain: SAGN+LP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5117
    - null
    - null
    metric_stds:
    - 0.0032
    - null
    - null
  - model: R-GraphSAGE
    model_plain: R-GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.27387'
    title: 'Robust Learning on Heterogeneous Graphs with Heterophily: A Graph Structure
      Learning Approach'
    date: Apr 30, 2026
    date_iso: '2026-04-30'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5094
    - null
    - null
    metric_stds:
    - 0.0044
    - null
    - null
  - model: NARS
    model_plain: NARS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5088
    - null
    - null
    metric_stds:
    - 0.0012
    - null
    - null
  - model: HGConv
    model_plain: HGConv
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2108.10097'
    title: Graph Attention MLP with Reliable Label Utilization
    date: Aug 23, 2021
    date_iso: '2021-08-23'
    date_display: Aug 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5045
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
  - model: R-GSN
    model_plain: R-GSN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2108.10097'
    title: Graph Attention MLP with Reliable Label Utilization
    date: Aug 23, 2021
    date_iso: '2021-08-23'
    date_display: Aug 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5032
    - null
    - null
    metric_stds:
    - 0.0037
    - null
    - null
  - model: HGT
    model_plain: HGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2604.27387'
    title: 'Robust Learning on Heterogeneous Graphs with Heterophily: A Graph Structure
      Learning Approach'
    date: Apr 30, 2026
    date_iso: '2026-04-30'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5023
    - null
    - null
    metric_stds:
    - 0.0048
    - null
    - null
  - model: SCNode
    model_plain: SCNode
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2410.02158'
    title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation Learning'
    date: Oct 3, 2024
    date_iso: '2024-10-03'
    date_display: Oct 2024
    codebase_url: https://github.com/joshem163/SCNode
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5003
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: HGT+emb
    model_plain: HGT+emb
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4982
    - null
    - null
    metric_stds:
    - 0.0013
    - null
    - null
  - model: GraphSAINT + metapath2vec
    model_plain: GraphSAINT + metapath2vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2105.08330'
    title: 'Residual Network and Embedding Usage: New Tricks of Node Classification
      with Graph Convolutional Networks'
    date: May 18, 2021
    date_iso: '2021-05-18'
    date_display: May 2021
    codebase_url: https://github.com/ytchx1999/PyG-OGB-Tricks
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4969
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
  - model: HGT
    model_plain: HGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2105.11122'
    title: Heterogeneous Graph Representation Learning with Relation Awareness
    date: May 24, 2021
    date_iso: '2021-05-24'
    date_display: May 2021
    codebase_url: https://github.com/yule-BUAA/R-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4921
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: HDHGR
    model_plain: HDHGR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.27387'
    title: 'Robust Learning on Heterogeneous Graphs with Heterophily: A Graph Structure
      Learning Approach'
    date: Apr 30, 2026
    date_iso: '2026-04-30'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4921
    - null
    - null
    metric_stds:
    - 0.0038
    - null
    - null
  row_count: 105
  rows_json: /data/datasets/ogbn-mag/standard-split-rows.json
  chart_json: /data/datasets/ogbn-mag/standard-split-chart.json
  arch_counts:
    gnn: 70
    hybrid: 18
    graph_transformer: 5
    llm: 0
    walk: 1
    traditional: 9
  metric_counts:
  - 96
  - 9
  - 9
  milestones: &id001
  - value: 0.481
    std: 0.001
    model: SIGN
    arxiv_id: '2011.09679'
    title: Scalable Graph Neural Networks for Heterogeneous Graphs
    date: '2020-11-19'
  - value: 0.4969
    std: 0.0022
    model: GraphSAINT + metapath2vec
    arxiv_id: '2105.08330'
    title: 'Residual Network and Embedding Usage: New Tricks of Node Classification
      with Graph Convolutional Networks'
    date: '2021-05-18'
  - value: 0.5204
    std: null
    model: R-HGNN
    arxiv_id: '2105.11122'
    title: Heterogeneous Graph Representation Learning with Relation Awareness
    date: '2021-05-24'
  - value: 0.559
    std: 0.0027
    model: NARS-GAMLP+RLU
    arxiv_id: '2108.10097'
    title: Graph Attention MLP with Reliable Label Utilization
    date: '2021-08-23'
  - value: 0.5631
    std: 0.0021
    model: RLU+SCR
    arxiv_id: '2112.04319'
    title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
    date: '2021-12-08'
  - value: 0.5719
    std: 0.0012
    model: SeHGNN+emb+ms
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: '2022-07-06'
  - value: 0.5784
    std: 0.0022
    model: LMSPS+LP+MS
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: '2023-07-17'
  milestones_by_metric:
    Accuracy: *id001
    Instability:
    - value: 0.222
      std: 0.006
      model: PGMExplainer
      arxiv_id: '2106.09078'
      title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical Analysis
        of GNN Explanation Methods'
      date: '2021-06-16'
    Unfaithfulness:
    - value: 0.001
      std: 0.0
      model: GraphLIME
      arxiv_id: '2106.09078'
      title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical Analysis
        of GNN Explanation Methods'
      date: '2021-06-16'
---

