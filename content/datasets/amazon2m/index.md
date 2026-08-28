---
title: Amazon2M
slug: amazon2m
benchmark: Other Graph Benchmarks
task_type: node_classification
short_description: Predict each product’s category on a roughly two-million-node co-purchase
  graph.
description: '**Node classification** on a roughly two-million-node co-purchase graph,
  predicting each product’s category. Evaluated by Accuracy.'
detailed_description:
  task: Large-scale Amazon co-purchase graph with ~2M nodes. Node classification (product
    category). Used to benchmark scalable GNNs and graph transformers. The primary
    catalog metric is Accuracy.
  data: Large-scale Amazon co-purchase graph with ~2M nodes. Node classification (product
    category). Used to benchmark scalable GNNs and graph transformers. The cataloged
    artifact reports 1 graphs.
  features: 'Input construction is dataset-specific and follows the cited release:
    program call graphs, 3D point coordinates, text-derived vectors, product attributes,
    or movie metadata. Added edges, neighborhood graphs, and feature normalization
    are preprocessing choices.'
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses Accuracy (higher is better). Exact masks or folds must
    come from the cited release.'
  quirks_and_pitfalls: These entries come from unrelated upstream benchmarks and have
    no shared protocol. Report the exact graph construction, split, feature pipeline,
    and label granularity; similarly named Film, Actor, IMDB, or Amazon artifacts
    are not interchangeable.
sources:
- title: Cluster-GCN
  arxiv_id: '1905.07953'
  kind: benchmark_or_upstream_source
primary_metric: Accuracy
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 1
  avg_nodes: 2449029.0
  avg_edges: 61859140.0
  num_classes: 47
  extra_stats:
    avg_degree: 50.52
    edge_feature_dim: 0
    feature_type: bag_of_words
    node_feature_dim: 100
    statistic_notes: 'Cluster-GCN release: 2,449,029 products, 61,859,140 co-purchase
      edges, 47 top-level classes, and 100-dimensional product-description features.'
result_count: 244
best_model:
  model: MA-GCL
  value: 0.8883
  metric: Accuracy
  arxiv_id: '2212.07035'
  paper_title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
papers:
- arxiv_id: '2605.11749'
  title: Learning Feature Encoder with Synthetic Anomalies for Weakly Supervised Graph
    Anomaly Detection
  date_iso: '2026-04-01'
  venue: ''
- arxiv_id: '2510.22451'
  title: 'GraphTOP: Graph Topology-Oriented Prompting for Graph Neural Networks'
  date_iso: '2025-10-25'
  venue: NeurIPS 2025
- arxiv_id: '2508.20906'
  title: Turning Tabular Foundation Models into Graph Foundation Models
  date_iso: '2025-08-28'
  venue: ''
- arxiv_id: '2508.07117'
  title: 'From Nodes to Narratives: Explaining Graph Neural Networks with LLMs and
    Graph Context'
  date_iso: '2025-08-09'
  venue: ''
- arxiv_id: '2506.15448'
  title: Semi-supervised Graph Anomaly Detection via Robust Homophily Learning
  date_iso: '2025-06-18'
  venue: NeurIPS 2025
- arxiv_id: '2505.19762'
  title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
    Graph Learning'
  date_iso: '2025-05-26'
  venue: ''
- arxiv_id: '2505.17660'
  title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
    for Node Classification'
  date_iso: '2025-05-23'
  venue: ''
- arxiv_id: '2412.19106'
  title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized Rational
    Graph Filters'
  date_iso: '2024-12-26'
  venue: ''
- arxiv_id: '2412.00020'
  title: Partitioning Message Passing for Graph Fraud Detection
  date_iso: '2024-11-16'
  venue: ICLR 2024
- arxiv_id: '2410.02158'
  title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation Learning'
  date_iso: '2024-10-03'
  venue: TMLR 2024
- arxiv_id: '2408.07654'
  title: 'Graph Triple Attention Network: A Decoupled Perspective'
  date_iso: '2024-08-14'
  venue: ''
- arxiv_id: '2406.19249'
  title: 'NTFormer: A Composite Node Tokenized Graph Transformer for Node Classification'
  date_iso: '2024-06-27'
  venue: ''
- arxiv_id: '2406.06642'
  title: 'TopoBench: A Framework for Benchmarking Topological Deep Learning'
  date_iso: '2024-06-09'
  venue: ''
- arxiv_id: '2405.15564'
  title: Rethinking Independent Cross-Entropy Loss For Graph-Structured Data
  date_iso: '2024-05-24'
  venue: ICML 2024
- arxiv_id: '2306.12251'
  title: 'GADBench: Revisiting and Benchmarking Supervised Graph Anomaly Detection'
  date_iso: '2023-06-21'
  venue: NeurIPS 2023
- arxiv_id: '2305.12677'
  title: Tokenized Graph Transformer with Neighborhood Augmentation for Node Classification
    in Large Graphs
  date_iso: '2023-05-22'
  venue: ''
- arxiv_id: '2305.14000'
  title: Node-wise Diffusion for Scalable Graph Learning
  date_iso: '2023-04-30'
  venue: WWW 2023
- arxiv_id: '2212.07035'
  title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
  date_iso: '2022-12-14'
  venue: AAAI 2022
- arxiv_id: '2206.12547'
  title: Geometry Contrastive Learning on Heterogeneous Graphs
  date_iso: '2022-06-25'
  venue: ''
- arxiv_id: '2205.15508'
  title: Rethinking Graph Neural Networks for Anomaly Detection
  date_iso: '2022-05-31'
  venue: ICML 2022
- arxiv_id: '2203.06389'
  title: 'GRAND+: Scalable Graph Random Neural Networks'
  date_iso: '2022-03-12'
  venue: WWW 2022
- arxiv_id: '2203.00949'
  title: 'GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation'
  date_iso: '2022-03-02'
  venue: ''
- arxiv_id: '2104.07477'
  title: Lorentzian Graph Convolutional Networks
  date_iso: '2021-04-15'
  venue: WWW 2021
- arxiv_id: '2008.08692'
  title: Enhancing Graph Neural Network-based Fraud Detectors against Camouflaged
    Fraudsters
  date_iso: '2020-08-19'
  venue: ''
- arxiv_id: '1907.04931'
  title: 'GraphSAINT: mpling Based ductive Learning Me hod'
  date_iso: '2019-07-10'
  venue: ICLR 2019
- arxiv_id: '1905.07953'
  title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph Convolutional
    Networks'
  date_iso: '2019-05-20'
  venue: KDD 2019
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
    avg_nodes: 2449029.0
    avg_edges: 61859140.0
    num_classes: 47
    extra_stats:
      avg_degree: 50.52
      edge_feature_dim: 0
      feature_type: bag_of_words
      node_feature_dim: 100
      statistic_notes: 'Cluster-GCN release: 2,449,029 products, 61,859,140 co-purchase
        edges, 47 top-level classes, and 100-dimensional product-description features.'
  metrics:
  - Accuracy
  - AUC
  - AUPRC
  - AUROC
  - F1
  - F1-macro
  - F1-micro
  - Fidelity
  - Macro-F1
  - micro-F1
  metric_display_names:
  - Accuracy
  - AUC
  - AUPRC
  - AUROC
  - F1
  - F1-macro
  - F1-micro
  - Fidelity
  - Macro-F1
  - micro-F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: MA-GCL
    model_plain: MA-GCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8883
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: CCA-SSG
    model_plain: CCA-SSG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8842
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ARIEL
    model_plain: ARIEL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8827
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
  - model: BGRL
    model_plain: BGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8823
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GCA
    model_plain: GCA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8785
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Base Model
    model_plain: Base Model
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8765
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8752
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GRACE
    model_plain: GRACE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8746
    - null
    - null
    - null
    - null
    - null
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
    - null
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
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8693
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8651
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.005
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SimGRACE
    model_plain: SimGRACE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8604
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
  - model: DGI
    model_plain: DGI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8395
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.005
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GAP-EDP
    model_plain: GAP-EDP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2203.00949'
    title: 'GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation'
    date: Mar 2, 2022
    date_iso: '2022-03-02'
    date_display: Mar 2022
    codebase_url: https://github.com/sisaman/GAP
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.838
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
  - model: COLES
    model_plain: COLES
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: Dec 14, 2022
    date_iso: '2022-12-14'
    date_display: Dec 2022
    codebase_url: https://github.com/GXM1141/MA-GCL
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7964
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DAM-GT
    model_plain: DAM-GT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_iso: '2025-05-23'
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
    - 0.7892
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0033
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DeGTA
    model_plain: DeGTA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2408.07654'
    title: 'Graph Triple Attention Network: A Decoupled Perspective'
    date: Aug 14, 2024
    date_iso: '2024-08-14'
    date_display: Aug 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7849
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0029
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: NTFormer
    model_plain: NTFormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.19249'
    title: 'NTFormer: A Composite Node Tokenized Graph Transformer for Node Classification'
    date: Jun 27, 2024
    date_iso: '2024-06-27'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7803
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0044
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: NAGphormer
    model_plain: NAGphormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.12677'
    title: Tokenized Graph Transformer with Neighborhood Augmentation for Node Classification
      in Large Graphs
    date: May 22, 2023
    date_iso: '2023-05-22'
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
    - 0.7798
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
  - model: NAGphormer
    model_plain: NAGphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.19249'
    title: 'NTFormer: A Composite Node Tokenized Graph Transformer for Node Classification'
    date: Jun 27, 2024
    date_iso: '2024-06-27'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7743
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
  - model: GAP-NDP
    model_plain: GAP-NDP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2203.00949'
    title: 'GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation'
    date: Mar 2, 2022
    date_iso: '2022-03-02'
    date_display: Mar 2022
    codebase_url: https://github.com/sisaman/GAP
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.774
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0007
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ANS-GT
    model_plain: ANS-GT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.19249'
    title: 'NTFormer: A Composite Node Tokenized Graph Transformer for Node Classification'
    date: Jun 27, 2024
    date_iso: '2024-06-27'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7632
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0038
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GRAND+ (S)
    model_plain: GRAND+ (S)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2203.06389'
    title: 'GRAND+: Scalable Graph Random Neural Networks'
    date: Mar 12, 2022
    date_iso: '2022-03-12'
    date_display: Mar 2022
    codebase_url: https://github.com/THUDM/GRAND-plus
    published_conference: WWW 2022
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.762
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.006
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: VCR-Graphormer
    model_plain: VCR-Graphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_iso: '2025-05-23'
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
    - 0.7609
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
  - model: GraphSAINT
    model_plain: GraphSAINT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2203.06389'
    title: 'GRAND+: Scalable Graph Random Neural Networks'
    date: Mar 12, 2022
    date_iso: '2022-03-12'
    date_display: Mar 2022
    codebase_url: https://github.com/THUDM/GRAND-plus
    published_conference: WWW 2022
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.759
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.013
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GRAND
    model_plain: GRAND
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2408.07654'
    title: 'Graph Triple Attention Network: A Decoupled Perspective'
    date: Aug 14, 2024
    date_iso: '2024-08-14'
    date_display: Aug 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7583
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0021
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GRAND
    model_plain: GRAND
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.12677'
    title: Tokenized Graph Transformer with Neighborhood Augmentation for Node Classification
      in Large Graphs
    date: May 22, 2023
    date_iso: '2023-05-22'
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
    - 0.7549
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0011
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2203.06389'
    title: 'GRAND+: Scalable Graph Random Neural Networks'
    date: Mar 12, 2022
    date_iso: '2022-03-12'
    date_display: Mar 2022
    codebase_url: https://github.com/THUDM/GRAND-plus
    published_conference: WWW 2022
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.749
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.005
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SGFormer
    model_plain: SGFormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.19249'
    title: 'NTFormer: A Composite Node Tokenized Graph Transformer for Node Classification'
    date: Jun 27, 2024
    date_iso: '2024-06-27'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7422
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0036
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: MLP-DP
    model_plain: MLP-DP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2203.00949'
    title: 'GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation'
    date: Mar 2, 2022
    date_iso: '2022-03-02'
    date_display: Mar 2022
    codebase_url: https://github.com/sisaman/GAP
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.736
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0005
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: FastGCN
    model_plain: FastGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2203.06389'
    title: 'GRAND+: Scalable Graph Random Neural Networks'
    date: Mar 12, 2022
    date_iso: '2022-03-12'
    date_display: Mar 2022
    codebase_url: https://github.com/THUDM/GRAND-plus
    published_conference: WWW 2022
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.729
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
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
    arxiv_id: '2203.06389'
    title: 'GRAND+: Scalable Graph Random Neural Networks'
    date: Mar 12, 2022
    date_iso: '2022-03-12'
    date_display: Mar 2022
    codebase_url: https://github.com/THUDM/GRAND-plus
    published_conference: WWW 2022
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.723
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
  - model: NodeFormer
    model_plain: NodeFormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.19249'
    title: 'NTFormer: A Composite Node Tokenized Graph Transformer for Node Classification'
    date: Jun 27, 2024
    date_iso: '2024-06-27'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7156
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0042
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GBP
    model_plain: GBP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2203.06389'
    title: 'GRAND+: Scalable Graph Random Neural Networks'
    date: Mar 12, 2022
    date_iso: '2022-03-12'
    date_display: Mar 2022
    codebase_url: https://github.com/THUDM/GRAND-plus
    published_conference: WWW 2022
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.701
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.009
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SAGE-EDP
    model_plain: SAGE-EDP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2203.00949'
    title: 'GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation'
    date: Mar 2, 2022
    date_iso: '2022-03-02'
    date_display: Mar 2022
    codebase_url: https://github.com/sisaman/GAP
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.683
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0099
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PPRGo
    model_plain: PPRGo
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2203.06389'
    title: 'GRAND+: Scalable Graph Random Neural Networks'
    date: Mar 12, 2022
    date_iso: '2022-03-12'
    date_display: Mar 2022
    codebase_url: https://github.com/THUDM/GRAND-plus
    published_conference: WWW 2022
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.676
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.005
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PPRGo
    model_plain: PPRGo
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.12677'
    title: Tokenized Graph Transformer with Neighborhood Augmentation for Node Classification
      in Large Graphs
    date: May 22, 2023
    date_iso: '2023-05-22'
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
    - 0.6612
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
  - model: Polynormer
    model_plain: Polynormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    - 0.5481
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0049
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ERGNN
    model_plain: ERGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.19106'
    title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized Rational
      Graph Filters'
    date: Dec 26, 2024
    date_iso: '2024-12-26'
    date_display: Dec 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5369
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
  - model: FSGNN
    model_plain: FSGNN
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
    - 0.5274
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0083
    - null
    - null
    - null
    - null
    - null
    - null
    - null
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
    - 0.5257
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0042
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: CWN
    model_plain: CWN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.06642'
    title: 'TopoBench: A Framework for Benchmarking Topological Deep Learning'
    date: Jun 9, 2024
    date_iso: '2024-06-09'
    date_display: Jun 2024
    codebase_url: https://github.com/geometric-intelligence/topobench
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.519
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0015
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: AST
    model_plain: AST
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.06642'
    title: 'TopoBench: A Framework for Benchmarking Topological Deep Learning'
    date: Jun 9, 2024
    date_iso: '2024-06-09'
    date_display: Jun 2024
    codebase_url: https://github.com/geometric-intelligence/topobench
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.505
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0027
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: CCCN
    model_plain: CCCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.06642'
    title: 'TopoBench: A Framework for Benchmarking Topological Deep Learning'
    date: Jun 9, 2024
    date_iso: '2024-06-09'
    date_display: Jun 2024
    codebase_url: https://github.com/geometric-intelligence/topobench
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5025999999999999
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0017000000000000001
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2406.06642'
    title: 'TopoBench: A Framework for Benchmarking Topological Deep Learning'
    date: Jun 9, 2024
    date_iso: '2024-06-09'
    date_display: Jun 2024
    codebase_url: https://github.com/geometric-intelligence/topobench
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5017
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
  - model: GloGNN
    model_plain: GloGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.19106'
    title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized Rational
      Graph Filters'
    date: Dec 26, 2024
    date_iso: '2024-12-26'
    date_display: Dec 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4988
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0044
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2406.06642'
    title: 'TopoBench: A Framework for Benchmarking Topological Deep Learning'
    date: Jun 9, 2024
    date_iso: '2024-06-09'
    date_display: Jun 2024
    codebase_url: https://github.com/geometric-intelligence/topobench
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.49560000000000004
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0055000000000000005
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2412.19106'
    title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized Rational
      Graph Filters'
    date: Dec 26, 2024
    date_iso: '2024-12-26'
    date_display: Dec 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4956
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0047
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: OptBasis
    model_plain: OptBasis
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.19106'
    title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized Rational
      Graph Filters'
    date: Dec 26, 2024
    date_iso: '2024-12-26'
    date_display: Dec 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4948
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0036
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ChebNetII
    model_plain: ChebNetII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.19106'
    title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized Rational
      Graph Filters'
    date: Dec 26, 2024
    date_iso: '2024-12-26'
    date_display: Dec 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4943
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0041
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2406.06642'
    title: 'TopoBench: A Framework for Benchmarking Topological Deep Learning'
    date: Jun 9, 2024
    date_iso: '2024-06-09'
    date_display: Jun 2024
    codebase_url: https://github.com/geometric-intelligence/topobench
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4916
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0102
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  row_count: 244
  rows_json: /data/datasets/amazon2m/standard-split-rows.json
  chart_json: /data/datasets/amazon2m/standard-split-chart.json
  arch_counts:
    gnn: 185
    hybrid: 16
    graph_transformer: 13
    llm: 5
    walk: 4
    traditional: 16
  metric_counts:
  - 109
  - 31
  - 25
  - 26
  - 9
  - 12
  - 8
  - 7
  - 14
  - 3
  milestones: &id001
  - value: 0.838
    std: 0.0026
    model: GAP-EDP
    arxiv_id: '2203.00949'
    title: 'GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation'
    date: '2022-03-02'
  - value: 0.8883
    std: 0.003
    model: MA-GCL
    arxiv_id: '2212.07035'
    title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
    date: '2022-12-14'
  milestones_by_metric:
    Accuracy: *id001
    AUC:
    - value: 0.8973
      std: null
      model: CARE-GNN
      arxiv_id: '2008.08692'
      title: Enhancing Graph Neural Network-based Fraud Detectors against Camouflaged
        Fraudsters
      date: '2020-08-19'
    - value: 0.964
      std: 0.011
      model: LGCN
      arxiv_id: '2104.07477'
      title: Lorentzian Graph Convolutional Networks
      date: '2021-04-15'
    - value: 0.9757
      std: 0.0012
      model: GFD
      arxiv_id: '2412.00020'
      title: Partitioning Message Passing for Graph Fraud Detection
      date: '2024-11-16'
    AUPRC:
    - value: 0.9333
      std: null
      model: XGB-Graph
      arxiv_id: '2306.12251'
      title: 'GADBench: Revisiting and Benchmarking Supervised Graph Anomaly Detection'
      date: '2023-06-21'
    AUROC:
    - value: 0.9443
      std: null
      model: GGAD
      arxiv_id: '2506.15448'
      title: Semi-supervised Graph Anomaly Detection via Robust Homophily Learning
      date: '2025-06-18'
    - value: 0.969
      std: 0.01
      model: weakly supervised graph anomaly detection method
      arxiv_id: '2605.11749'
      title: Learning Feature Encoder with Synthetic Anomalies for Weakly Supervised
        Graph Anomaly Detection
      date: '2026-04-01'
    F1:
    - value: 0.9041
      std: null
      model: Cluster-GCN
      arxiv_id: '1905.07953'
      title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph
        Convolutional Networks'
      date: '2019-05-20'
    F1-macro:
    - value: 0.9229
      std: 0.0044
      model: BWGNN (Homo)
      arxiv_id: '2205.15508'
      title: Rethinking Graph Neural Networks for Anomaly Detection
      date: '2022-05-31'
    F1-micro:
    - value: 0.815
      std: 0.001
      model: GraphSAINT-RW
      arxiv_id: '1907.04931'
      title: 'GraphSAINT: mpling Based ductive Learning Me hod'
      date: '2019-07-10'
    Fidelity:
    - value: 0.945
      std: 0.015
      model: GNNExplainer
      arxiv_id: '2508.07117'
      title: 'From Nodes to Narratives: Explaining Graph Neural Networks with LLMs
        and Graph Context'
      date: '2025-08-09'
    Macro-F1:
    - value: 0.765
      std: 0.0122
      model: GCL
      arxiv_id: '2206.12547'
      title: Geometry Contrastive Learning on Heterogeneous Graphs
      date: '2022-06-25'
    micro-F1:
    - value: 0.8022
      std: 0.0004
      model: SIGN
      arxiv_id: '2405.15564'
      title: Rethinking Independent Cross-Entropy Loss For Graph-Structured Data
      date: '2024-05-24'
---

