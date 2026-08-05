---
title: ogbn-arxiv
slug: ogbn-arxiv
benchmark: OGB
task_type: node_classification
description: Node classification on arXiv citation network (40 subject areas).
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.OGBNodePropPredDataset.html
stats:
  num_graphs: 169343
  avg_nodes: 1166243.0
  avg_edges: null
  num_classes: 40
result_count: 171
best_model:
  model: OFA
  value: 0.7764
  metric: Accuracy
  arxiv_id: '2407.19941'
  paper_title: Boosting Cross-Domain and Cross-Task Generalization for Text-Attributed
    Graphs from Structural Perspective
papers:
- arxiv_id: '2606.00757'
  title: 'RADE: Random Add-Drop Edge as a Regularizer'
  date_iso: '2026-05-30'
  venue: ICML 2026
- arxiv_id: '2603.26178'
  title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
    Learning via Ricci Flow'
  date_iso: '2026-03-27'
  venue: ''
- arxiv_id: '2601.07419'
  title: 'Position: Don''t be Afraid of Over-Smoothing And Over-Squashing'
  date_iso: '2026-01-12'
  venue: ''
- arxiv_id: '2510.07755'
  title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
    and Inter-domain Knowledge Modeling'
  date_iso: '2025-10-09'
  venue: ''
- arxiv_id: '2501.19089'
  title: Resolving Oversmoothing with Opinion Dissensus
  date_iso: '2025-01-31'
  venue: ''
- arxiv_id: '2412.04064'
  title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
  date_iso: '2024-12-05'
  venue: NeurIPS 2024
- arxiv_id: '2410.02158'
  title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation Learning'
  date_iso: '2024-10-03'
  venue: TMLR 2024
- arxiv_id: '2407.19941'
  title: Boosting Cross-Domain and Cross-Task Generalization for Text-Attributed Graphs
    from Structural Perspective
  date_iso: '2024-07-29'
  venue: ''
- arxiv_id: '2407.04236'
  title: Graph Pooling via Ricci Flow
  date_iso: '2024-07-05'
  venue: TMLR 2024
- arxiv_id: '2405.20445'
  title: Fully-inductive Node Classification on Arbitrary Graphs
  date_iso: '2024-05-30'
  venue: ICLR 2024
- arxiv_id: '2405.13806'
  title: A General Graph Spectral Wavelet Convolution via Chebyshev Order Decomposition
  date_iso: '2024-05-22'
  venue: ICML 2024
- arxiv_id: '2403.12529'
  title: Contextualized Messages Boost Graph Representations
  date_iso: '2024-03-19'
  venue: TMLR 2024
- arxiv_id: '2312.02619'
  title: Rethinking and Simplifying Bootstrapped Graph Latents
  date_iso: '2023-12-05'
  venue: ''
- arxiv_id: '2311.17781'
  title: 'Propagate & Distill: Towards Effective Graph Learners Using Propagation-Embracing
    MLPs'
  date_iso: '2023-11-29'
  venue: LoG 2023
- arxiv_id: '2309.14907'
  title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
    Graphs against Learning Bias
  date_iso: '2023-09-26'
  venue: ''
- arxiv_id: '2306.10466'
  title: 'Graph Ladling: Shockingly Simple Parallel GNN Training without Intermediate
    Communication'
  date_iso: '2023-06-18'
  venue: ICML 2023
- arxiv_id: '2212.03654'
  title: Node-oriented Spectral Filtering for Graph Neural Networks
  date_iso: '2022-12-07'
  venue: ''
- arxiv_id: '2212.02483'
  title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
  date_iso: '2022-12-05'
  venue: ICML 2022
- arxiv_id: '2210.03930'
  title: Hierarchical Graph Transformer with Adaptive Node Sampling
  date_iso: '2022-10-08'
  venue: NeurIPS 2022
- arxiv_id: '2206.09166'
  title: 'NAS-Bench-Graph: Benchmarking Graph Neural Architecture Search'
  date_iso: '2022-06-18'
  venue: NeurIPS 2022
- arxiv_id: '2111.12128'
  title: On the Unreasonable Effectiveness of Feature Propagation in Learning on Graphs
    with Missing Node Features
  date_iso: '2021-11-23'
  venue: ''
- arxiv_id: '2111.00064'
  title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
  date_iso: '2021-10-29'
  venue: ICLR 2021
- arxiv_id: '2110.15174'
  title: On Provable Benefits of Depth in Training Graph Convolutional Networks
  date_iso: '2021-10-28'
  venue: NeurIPS 2021
- arxiv_id: '2106.09078'
  title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical Analysis of
    GNN Explanation Methods'
  date_iso: '2021-06-16'
  venue: ''
- arxiv_id: '2106.02466'
  title: 'Graph Barlow Twins: A self-supervised representation learning framework
    for graphs'
  date_iso: '2021-06-04'
  venue: ''
- arxiv_id: '2102.06986'
  title: How Framelets Enhance Graph Neural Networks
  date_iso: '2021-02-13'
  venue: ICML 2021
- arxiv_id: '2102.03147'
  title: Learning Conjoint Attentions for Graph Neural Nets
  date_iso: '2021-02-05'
  venue: NeurIPS 2021
- arxiv_id: '2012.15024'
  title: Adaptive Graph Diffusion Networks
  date_iso: '2020-12-30'
  venue: ''
- arxiv_id: '2010.00238'
  title: Multi-grained Semantics-aware Graph Neural Networks
  date_iso: '2020-10-01'
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
    num_graphs: 169343
    avg_nodes: 1166243.0
    avg_edges: null
    num_classes: 40
  metrics:
  - Accuracy
  - F1
  - Instability
  - Unfaithfulness
  metric_display_names:
  - Accuracy
  - F1
  - Instability
  - Unfaithfulness
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: OFA
    model_plain: OFA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2407.19941'
    title: Boosting Cross-Domain and Cross-Task Generalization for Text-Attributed
      Graphs from Structural Perspective
    date: Jul 29, 2024
    date_iso: '2024-07-29'
    date_display: Jul 2024
    codebase_url: https://github.com/cy623/BooG
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7764
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: GIANT-XRT
    model_plain: GIANT-XRT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: https://github.com/amzn/pecos
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7612
    - null
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
    - null
  - model: GEGCN
    model_plain: GEGCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.26178'
    title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
      Learning via Ricci Flow'
    date: Mar 27, 2026
    date_iso: '2026-03-27'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7576
    - null
    - null
    - null
    metric_stds:
    - 0.0064
    - null
    - null
    - null
  - model: AGDN
    model_plain: AGDN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.26178'
    title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
      Learning via Ricci Flow'
    date: Mar 27, 2026
    date_iso: '2026-03-27'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7522
    - null
    - null
    - null
    metric_stds:
    - 0.0007
    - null
    - null
    - null
  - model: CNA
    model_plain: CNA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_iso: '2024-12-05'
    date_display: Dec 2024
    codebase_url: https://github.com/ml-research/cna_modules
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7464
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: UniMP
    model_plain: UniMP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2603.26178'
    title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
      Learning via Ricci Flow'
    date: Mar 27, 2026
    date_iso: '2026-03-27'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.745
    - null
    - null
    - null
    metric_stds:
    - 0.0005
    - null
    - null
    - null
  - model: BERT+GAE
    model_plain: BERT+GAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: https://github.com/amzn/pecos
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7448
    - null
    - null
    - null
    metric_stds:
    - 0.0015
    - null
    - null
    - null
  - model: OGB-feat
    model_plain: OGB-feat
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: https://github.com/amzn/pecos
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7426
    - null
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
    - null
  - model: RevGAT
    model_plain: RevGAT
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
    - 0.7426
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: OGB-feat+GAE
    model_plain: OGB-feat+GAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: https://github.com/amzn/pecos
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7406
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    - null
  - model: OGB-feat+VGAE
    model_plain: OGB-feat+VGAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: https://github.com/amzn/pecos
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7395
    - null
    - null
    - null
    metric_stds:
    - 0.0009
    - null
    - null
    - null
  - model: UniMP-v2
    model_plain: UniMP-v2
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
    - 0.7392
    - null
    - null
    - null
    metric_stds:
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
    - 0.7391
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: OGB-feat+DGI
    model_plain: OGB-feat+DGI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: https://github.com/amzn/pecos
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.739
    - null
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
    - null
  - model: FGSSL
    model_plain: FGSSL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7377
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
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
    - 0.7371
    - null
    - null
    - null
    metric_stds:
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
    arxiv_id: '2405.20445'
    title: Fully-inductive Node Classification on Arbitrary Graphs
    date: May 30, 2024
    date_iso: '2024-05-30'
    date_display: May 2024
    codebase_url: https://github.com/DeepGraphLearning/GraphAny
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7365
    - null
    - null
    - null
    metric_stds:
    - 0.0011
    - null
    - null
    - null
  - model: BERT+DGI
    model_plain: BERT+DGI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: https://github.com/amzn/pecos
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.736
    - null
    - null
    - null
    metric_stds:
    - 0.0021
    - null
    - null
    - null
  - model: BERT
    model_plain: BERT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: https://github.com/amzn/pecos
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7359
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    - null
  - model: FedTAD
    model_plain: FedTAD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7352
    - null
    - null
    - null
    metric_stds:
    - 0.0039
    - null
    - null
    - null
  - model: AGDN
    model_plain: AGDN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.15024'
    title: Adaptive Graph Diffusion Networks
    date: Dec 30, 2020
    date_iso: '2020-12-30'
    date_display: Dec 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7341
    - null
    - null
    - null
    metric_stds:
    - 0.0025
    - null
    - null
    - null
  - model: FedSage
    model_plain: FedSage
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7333
    - null
    - null
    - null
    metric_stds:
    - 0.0048
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
    arxiv_id: '2603.26178'
    title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
      Learning via Ricci Flow'
    date: Mar 27, 2026
    date_iso: '2026-03-27'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.733
    - null
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
    - null
  - model: FedGTA
    model_plain: FedGTA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.732
    - null
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
    - null
  - model: FED-PUB
    model_plain: FED-PUB
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7319
    - null
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
    - null
  - model: UniGraph
    model_plain: UniGraph
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2407.19941'
    title: Boosting Cross-Domain and Cross-Task Generalization for Text-Attributed
      Graphs from Structural Perspective
    date: Jul 29, 2024
    date_iso: '2024-07-29'
    date_display: Jul 2024
    codebase_url: https://github.com/cy623/BooG
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.731
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: WaveGC
    model_plain: WaveGC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13806'
    title: A General Graph Spectral Wavelet Convolution via Chebyshev Order Decomposition
    date: May 22, 2024
    date_iso: '2024-05-22'
    date_display: May 2024
    codebase_url: https://github.com/liun-online/WaveGC
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7301
    - null
    - null
    - null
    metric_stds:
    - 0.0018
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
    arxiv_id: '2603.26178'
    title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
      Learning via Ricci Flow'
    date: Mar 27, 2026
    date_iso: '2026-03-27'
    date_display: Mar 2026
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
    metric_stds:
    - 0.0017
    - null
    - null
    - null
  - model: ANS-GT
    model_plain: ANS-GT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2210.03930'
    title: Hierarchical Graph Transformer with Adaptive Node Sampling
    date: Oct 8, 2022
    date_iso: '2022-10-08'
    date_display: Oct 2022
    codebase_url: https://github.com/zaixizhang/ANS-GT
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7284
    - null
    - null
    - null
    metric_stds:
    - 0.0034
    - null
    - null
    - null
  - model: Node Sampled Soup
    model_plain: Node Sampled Soup
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.10466'
    title: 'Graph Ladling: Shockingly Simple Parallel GNN Training without Intermediate
      Communication'
    date: Jun 18, 2023
    date_iso: '2023-06-18'
    date_display: Jun 2023
    codebase_url: https://github.com/VITA-Group/graph_ladling
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7283
    - null
    - null
    - null
    metric_stds:
    - 0.0021
    - null
    - null
    - null
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.26178'
    title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
      Learning via Ricci Flow'
    date: Mar 27, 2026
    date_iso: '2026-03-27'
    date_display: Mar 2026
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
    metric_stds:
    - 0.0016
    - null
    - null
    - null
  - model: MAGNA
    model_plain: MAGNA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.15024'
    title: Adaptive Graph Diffusion Networks
    date: Dec 30, 2020
    date_iso: '2020-12-30'
    date_display: Dec 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7276
    - null
    - null
    - null
    metric_stds:
    - 0.0014
    - null
    - null
    - null
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2010.00238'
    title: Multi-grained Semantics-aware Graph Neural Networks
    date: Oct 1, 2020
    date_iso: '2020-10-01'
    date_display: Oct 2020
    codebase_url: https://github.com/zhiqiangzhongddu/AdamGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7274
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: AdamGNN
    model_plain: AdamGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2010.00238'
    title: Multi-grained Semantics-aware Graph Neural Networks
    date: Oct 1, 2020
    date_iso: '2020-10-01'
    date_display: Oct 2020
    codebase_url: https://github.com/zhiqiangzhongddu/AdamGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7265
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: SEA-GWNN
    model_plain: SEA-GWNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13806'
    title: A General Graph Spectral Wavelet Convolution via Chebyshev Order Decomposition
    date: May 22, 2024
    date_iso: '2024-05-22'
    date_display: May 2024
    codebase_url: https://github.com/liun-online/WaveGC
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7264
    - null
    - null
    - null
    metric_stds:
    - 0.0021
    - null
    - null
    - null
  - model: SIR-GCN
    model_plain: SIR-GCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.12529'
    title: Contextualized Messages Boost Graph Representations
    date: Mar 19, 2024
    date_iso: '2024-03-19'
    date_display: Mar 2024
    codebase_url: https://github.com/briangodwinlim/SIR-GCN
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7252
    - null
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
    - null
  - model: OGB-feat+GZ
    model_plain: OGB-feat+GZ
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: https://github.com/amzn/pecos
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.725
    - null
    - null
    - null
    metric_stds:
    - 0.0008
    - null
    - null
    - null
  - model: PNA
    model_plain: PNA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2010.00238'
    title: Multi-grained Semantics-aware Graph Neural Networks
    date: Oct 1, 2020
    date_iso: '2020-10-01'
    date_display: Oct 2020
    codebase_url: https://github.com/zhiqiangzhongddu/AdamGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7237
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: Our Data Partition Soup
    model_plain: Our Data Partition Soup
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.10466'
    title: 'Graph Ladling: Shockingly Simple Parallel GNN Training without Intermediate
      Communication'
    date: Jun 18, 2023
    date_iso: '2023-06-18'
    date_display: Jun 2023
    codebase_url: https://github.com/VITA-Group/graph_ladling
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7235
    - null
    - null
    - null
    metric_stds:
    - 0.0019
    - null
    - null
    - null
  - model: BERT+GZ
    model_plain: BERT+GZ
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: https://github.com/amzn/pecos
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7233
    - null
    - null
    - null
    metric_stds:
    - 0.0006
    - null
    - null
    - null
  - model: DeepGCN
    model_plain: DeepGCN
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
    - 0.7232
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: FP
    model_plain: FP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.12128'
    title: On the Unreasonable Effectiveness of Feature Propagation in Learning on
      Graphs with Missing Node Features
    date: Nov 23, 2021
    date_iso: '2021-11-23'
    date_display: Nov 2021
    codebase_url: https://github.com/marblet/GCNmf
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
    metric_stds:
    - null
    - null
    - null
    - null
  - model: EGC-S
    model_plain: EGC-S
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.12529'
    title: Contextualized Messages Boost Graph Representations
    date: Mar 19, 2024
    date_iso: '2024-03-19'
    date_display: Mar 2024
    codebase_url: https://github.com/briangodwinlim/SIR-GCN
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7221
    - null
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
    - null
  - model: JKNet
    model_plain: JKNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.09
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.15024'
    title: Adaptive Graph Diffusion Networks
    date: Dec 30, 2020
    date_iso: '2020-12-30'
    date_display: Dec 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7219
    - null
    - null
    - null
    metric_stds:
    - 0.0021
    - null
    - null
    - null
  - model: Auto-GNN
    model_plain: Auto-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.09166'
    title: 'NAS-Bench-Graph: Benchmarking Graph Neural Architecture Search'
    date: Jun 18, 2022
    date_iso: '2022-06-18'
    date_display: Jun 2022
    codebase_url: https://github.com/THUMNLab/NAS-Bench-Graph
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7213
    - null
    - null
    - null
    metric_stds:
    - 0.0003
    - null
    - null
    - null
  - model: RL
    model_plain: RL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.09166'
    title: 'NAS-Bench-Graph: Benchmarking Graph Neural Architecture Search'
    date: Jun 18, 2022
    date_iso: '2022-06-18'
    date_display: Jun 2022
    codebase_url: https://github.com/THUMNLab/NAS-Bench-Graph
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7213
    - null
    - null
    - null
    metric_stds:
    - 0.0005
    - null
    - null
    - null
  - model: NFGNN
    model_plain: NFGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.03654'
    title: Node-oriented Spectral Filtering for Graph Neural Networks
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7213
    - null
    - null
    - null
    metric_stds:
    - 0.0033
    - null
    - null
    - null
  - model: MOON
    model_plain: MOON
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7212
    - null
    - null
    - null
    metric_stds:
    - 0.0033
    - null
    - null
    - null
  - model: DAGNN
    model_plain: DAGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.04
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.15024'
    title: Adaptive Graph Diffusion Networks
    date: Dec 30, 2020
    date_iso: '2020-12-30'
    date_display: Dec 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7209
    - null
    - null
    - null
    metric_stds:
    - 0.0025
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
    arxiv_id: '2010.00238'
    title: Multi-grained Semantics-aware Graph Neural Networks
    date: Oct 1, 2020
    date_iso: '2020-10-01'
    date_display: Oct 2020
    codebase_url: https://github.com/zhiqiangzhongddu/AdamGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7206
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  row_count: 171
  rows_json: /data/datasets/ogbn-arxiv/standard-split-rows.json
  chart_json: /data/datasets/ogbn-arxiv/standard-split-chart.json
  arch_counts:
    gnn: 125
    hybrid: 14
    graph_transformer: 2
    llm: 6
    walk: 2
    traditional: 20
  metric_counts:
  - 157
  - 5
  - 9
  - 9
  milestones: &id001
  - value: 0.7274
    std: null
    model: GCNII
    arxiv_id: '2010.00238'
    title: Multi-grained Semantics-aware Graph Neural Networks
    date: '2020-10-01'
  - value: 0.7341
    std: 0.0025
    model: AGDN
    arxiv_id: '2012.15024'
    title: Adaptive Graph Diffusion Networks
    date: '2020-12-30'
  - value: 0.7612
    std: 0.0016
    model: GIANT-XRT
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: '2021-10-29'
  - value: 0.7764
    std: null
    model: OFA
    arxiv_id: '2407.19941'
    title: Boosting Cross-Domain and Cross-Task Generalization for Text-Attributed
      Graphs from Structural Perspective
    date: '2024-07-29'
  milestones_by_metric:
    Accuracy: *id001
    F1:
    - value: 0.7263
      std: 0.0012
      model: DGCN
      arxiv_id: '2110.15174'
      title: On Provable Benefits of Depth in Training Graph Convolutional Networks
      date: '2021-10-28'
    Instability:
    - value: 0.125
      std: 0.002
      model: GraphMask
      arxiv_id: '2106.09078'
      title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical Analysis
        of GNN Explanation Methods'
      date: '2021-06-16'
    Unfaithfulness:
    - value: 0.26
      std: 0.003
      model: GraphLIME
      arxiv_id: '2106.09078'
      title: 'Probing GNN Explainers: A Rigorous Theoretical and Empirical Analysis
        of GNN Explanation Methods'
      date: '2021-06-16'
---

