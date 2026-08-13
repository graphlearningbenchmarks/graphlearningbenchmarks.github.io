---
title: ogbn-papers100M
slug: ogbn-papers100m
benchmark: OGB
task_type: node_classification
short_description: Predict a primary arXiv subject area for the approximately 1.5
  million labeled arXiv papers while using the full 111-million-node citation network.
description: '**172-class node classification** Predict a primary arXiv subject area
  for the approximately 1.5 million labeled arXiv papers while using the full 111-million-node
  citation network. Evaluated by Accuracy.'
detailed_description:
  task: Predict a primary arXiv subject area for the approximately 1.5 million labeled
    arXiv papers while using the full 111-million-node citation network. Accuracy
    over 172 classes is the official measure.
  data: Nodes are papers indexed by Microsoft Academic Graph and directed edges are
    citations. Most nodes are not arXiv papers and have no class label, but remain
    available as unlabeled graph context.
  features: As in ogbn-arxiv, every paper has a 128-dimensional average of skip-gram
    embeddings for title and abstract words. The fixed features and graph come from
    the released MAG snapshot.
  splits_and_evaluation: Labeled arXiv papers through 2017 train the model, papers
    from 2018 validate it, and papers from 2019 onward form test. The task is transductive
    because features and topology for all nodes are supplied.
  quirks_and_pitfalls: 'Dataset scale makes full-batch processing impractical and
    often forces sampling or partitioning choices that affect results. The overwhelming
    majority of nodes are unlabeled. This is not simply a scaled ogbn-arxiv: it uses
    172 subjects and a much broader MAG graph.'
sources:
- title: Open Graph Benchmark
  arxiv_id: '2005.00687'
  kind: benchmark_definition
- title: OGB node property prediction documentation
  url: https://ogb.stanford.edu/docs/nodeprop/#ogbn-papers100M
  kind: official_documentation
- title: Microsoft Academic Graph, When experts are not enough
  url: https://doi.org/10.1162/qss_a_00021
  kind: upstream_data_source
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.OGBNodePropPredDataset.html
stats:
  num_graphs: 111059956
  avg_nodes: 1615685872.0
  avg_edges: null
  num_classes: 1
result_count: 141
best_model:
  model: SGC
  value: 0.791
  metric: Accuracy
  arxiv_id: '2403.13268'
  paper_title: 'Unifews: You Need Fewer Operations for Efficient Graph Neural Networks'
papers:
- arxiv_id: '2602.12613'
  title: 'Coden: Efficient Temporal Graph Neural Networks for Continuous Prediction'
  date_iso: '2026-02-13'
  venue: ''
- arxiv_id: '2505.14033'
  title: 'Partition-wise Graph Filtering: A Unified Perspective Through the Lens of
    Graph Coarsening'
  date_iso: '2025-05-20'
  venue: KDD 2025
- arxiv_id: '2504.13266'
  title: 'Graph Learning at Scale: Characterizing and Optimizing Pre-Propagation GNNs'
  date_iso: '2025-04-17'
  venue: ''
- arxiv_id: '2502.19693'
  title: Accurate and Scalable Graph Neural Networks via Message Invariance
  date_iso: '2025-02-27'
  venue: ICLR 2025
- arxiv_id: '2412.19106'
  title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized Rational
    Graph Filters'
  date_iso: '2024-12-26'
  venue: ''
- arxiv_id: '2404.15354'
  title: 'Polynomial Selection in Spectral Graph Neural Networks: An Error-Sum of
    Function Slices Approach'
  date_iso: '2024-04-15'
  venue: WWW 2024
- arxiv_id: '2403.13268'
  title: 'Unifews: You Need Fewer Operations for Efficient Graph Neural Networks'
  date_iso: '2024-03-19'
  venue: ICML 2024
- arxiv_id: '2402.13630'
  title: 'UniGraph: Learning a Unified Cross-Domain Foundation Model for Text-Attributed
    Graphs'
  date_iso: '2024-02-21'
  venue: KDD 2024
- arxiv_id: '2402.06128'
  title: Rethinking Node-wise Propagation for Large-scale Graph Learning
  date_iso: '2024-02-09'
  venue: WWW 2024
- arxiv_id: '2401.11772'
  title: 'LightDiC: A Simple yet Effective Approach for Large-scale Digraph Representation
    Learning'
  date_iso: '2024-01-22'
  venue: ''
- arxiv_id: '2401.12231'
  title: Disentangled Condensation for Large-scale Graphs
  date_iso: '2024-01-18'
  venue: WWW 2024
- arxiv_id: '2312.11109'
  title: Graph Transformers for Large Graphs
  date_iso: '2023-12-18'
  venue: ''
- arxiv_id: '2310.12457'
  title: 'MuseGNN: Forming Scalable, Convergent GNN Layers that Minimize a Sampling-Based
    Energy'
  date_iso: '2023-10-19'
  venue: ICLR 2023
- arxiv_id: '2401.11755'
  title: 'FedGTA: Topology-aware Averaging for Federated Graph Learning'
  date_iso: '2023-09-01'
  venue: ''
- arxiv_id: '2305.14000'
  title: Node-wise Diffusion for Scalable Graph Learning
  date_iso: '2023-04-30'
  venue: WWW 2023
- arxiv_id: '2302.12432'
  title: Graph Neural Networks with Learnable and Optimal Polynomial Bases
  date_iso: '2023-02-24'
  venue: ICML 2023
- arxiv_id: '2210.14709'
  title: Learning on Large-scale Text-attributed Graphs via Variational Inference
  date_iso: 2022-10
  venue: ICLR 2022
- arxiv_id: '2207.09179'
  title: 'SCARA: Scalable Graph Neural Networks with Feature-Oriented Optimization'
  date_iso: '2022-07-01'
  venue: ''
- arxiv_id: '2206.04355'
  title: Graph Attention Multi-Layer Perceptron
  date_iso: '2022-06-09'
  venue: KDD 2022
- arxiv_id: '2206.04361'
  title: Model Degradation Hinders Deep Graph Neural Networks
  date_iso: '2022-06-09'
  venue: KDD 2022
- arxiv_id: '2206.01535'
  title: 'Rethinking and Scaling Up Graph Contrastive Learning: An Extremely Efficient
    Approach with Group Discrimination'
  date_iso: '2022-06-03'
  venue: NeurIPS 2022
- arxiv_id: '2203.06389'
  title: 'GRAND+: Scalable Graph Random Neural Networks'
  date_iso: '2022-03-12'
  venue: WWW 2022
- arxiv_id: '2202.03341'
  title: 'Neighbor2Seq: Deep Learning on Massive Graphs by Transforming Neighbors
    to Sequences'
  date_iso: '2022-02-07'
  venue: ''
- arxiv_id: '2202.03580'
  title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
  date_iso: '2022-02-04'
  venue: NeurIPS 2022
- arxiv_id: '2112.04319'
  title: 'SCR: Training Graph Neural Networks with Consistency Regularization'
  date_iso: '2021-12-08'
  venue: ''
- arxiv_id: '2111.06483'
  title: 'Sequential Aggregation and Rematerialization: Distributed Full-batch Training
    of Graph Neural Networks on Large Graphs'
  date_iso: '2021-11-11'
  venue: ''
- arxiv_id: '2111.00064'
  title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
  date_iso: '2021-10-29'
  venue: ICLR 2021
- arxiv_id: '2110.14377'
  title: Node Dependent Local Smoothing for Scalable Graph Learning
  date_iso: '2021-10-27'
  venue: NeurIPS 2021
- arxiv_id: '2108.10097'
  title: Graph Attention MLP with Reliable Label Utilization
  date_iso: '2021-08-23'
  venue: ''
- arxiv_id: '2108.00955'
  title: Evaluating Deep Graph Neural Networks
  date_iso: '2021-08-02'
  venue: ''
- arxiv_id: '2108.00219'
  title: 'Grain: Improving Data Efficiency of Graph Neural Networks via Diversified
    Influence Maximization'
  date_iso: '2021-07-01'
  venue: ''
- arxiv_id: '2104.09376'
  title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced Training
  date_iso: '2021-04-19'
  venue: ''
- arxiv_id: '2104.06700'
  title: 'DistGNN: Scalable Distributed Training for Large-Scale Graph Neural Networks'
  date_iso: '2021-04-14'
  venue: ''
- arxiv_id: '2004.11198'
  title: 'SIGN: Scalable Inception Graph Neural Networks'
  date_iso: '2020-04-23'
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
    num_graphs: 111059956
    avg_nodes: 1615685872.0
    avg_edges: null
    num_classes: 1
  metrics:
  - Accuracy
  - F1
  metric_display_names:
  - Accuracy
  - F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: SGC
    model_plain: SGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.13268'
    title: 'Unifews: You Need Fewer Operations for Efficient Graph Neural Networks'
    date: Mar 19, 2024
    date_iso: '2024-03-19'
    date_display: Mar 2024
    codebase_url: https://github.com/gdmnl/Unifews
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.791
    - null
    metric_stds:
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
    arxiv_id: '2210.14709'
    title: Learning on Large-scale Text-attributed Graphs via Variational Inference
    date: Oct 2022
    date_iso: 2022-10
    date_display: Oct 2022
    codebase_url: https://github.com/AndyJZhao/GLEM
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7036
    - null
    metric_stds:
    - 0.0002
    - null
  - model: GLEM-GNN
    model_plain: GLEM-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.14709'
    title: Learning on Large-scale Text-attributed Graphs via Variational Inference
    date: Oct 2022
    date_iso: 2022-10
    date_display: Oct 2022
    codebase_url: https://github.com/AndyJZhao/GLEM
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7036
    - null
    metric_stds:
    - 0.0002
    - null
  - model: ShaDow+ATP
    model_plain: ShaDow+ATP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.06128'
    title: Rethinking Node-wise Propagation for Large-scale Graph Learning
    date: Feb 9, 2024
    date_iso: '2024-02-09'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.698
    - null
    metric_stds:
    - 0.001
    - null
  - model: GAMLP+RLU
    model_plain: GAMLP+RLU
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
    - 0.6967
    - null
    metric_stds:
    - 0.0004
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
    - 0.6908
    - null
    metric_stds:
    - 0.0047
    - null
  - model: CPF
    model_plain: CPF
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.14033'
    title: 'Partition-wise Graph Filtering: A Unified Perspective Through the Lens
      of Graph Coarsening'
    date: May 20, 2025
    date_iso: '2025-05-20'
    date_display: May 2025
    codebase_url: https://github.com/vasile-paskardlgm/CPF
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6887
    - null
    metric_stds:
    - 0.003
    - null
  - model: TFGNN
    model_plain: TFGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.15354'
    title: 'Polynomial Selection in Spectral Graph Neural Networks: An Error-Sum of
      Function Slices Approach'
    date: Apr 15, 2024
    date_iso: '2024-04-15'
    date_display: Apr 2024
    codebase_url: https://github.com/vasile-paskardlgm/TFGNN
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6865
    - null
    metric_stds:
    - 0.002
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
    - 0.6842
    - null
    metric_stds:
    - 0.0015
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
    - 0.683
    - null
    metric_stds:
    - 0.0008
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
    - 0.6825
    - null
    metric_stds:
    - 0.0011
    - null
  - model: GAMLP+RLU
    model_plain: GAMLP+RLU
    is_baseline: false
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
    - 0.6825
    - null
    metric_stds:
    - 0.0011
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
    - 0.6816
    - null
    metric_stds:
    - 0.0012
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
    - 0.6814
    - null
    metric_stds:
    - 0.0008
    - null
  - model: GAMLP(JK)
    model_plain: GAMLP(JK)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.04355'
    title: Graph Attention Multi-Layer Perceptron
    date: Jun 9, 2022
    date_iso: '2022-06-09'
    date_display: Jun 2022
    codebase_url: https://github.com/PKU-DAIR/GAMLP
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6807
    - null
    metric_stds:
    - 0.001
    - null
  - model: SAGN+SLE
    model_plain: SAGN+SLE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2104.09376'
    title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced Training
    date: Apr 19, 2021
    date_iso: '2021-04-19'
    date_display: Apr 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.68
    - null
    metric_stds:
    - 0.0015
    - null
  - model: UniGraph
    model_plain: UniGraph
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2402.13630'
    title: 'UniGraph: Learning a Unified Cross-Domain Foundation Model for Text-Attributed
      Graphs'
    date: Feb 21, 2024
    date_iso: '2024-02-21'
    date_display: Feb 2024
    codebase_url: https://github.com/yf-he/UniGraph
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6789
    - null
    metric_stds:
    - 0.0021
    - null
  - model: GAMLP
    model_plain: GAMLP
    is_baseline: false
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
    - 0.6771
    - null
    metric_stds:
    - 0.002
    - null
  - model: SAGN+SLE
    model_plain: SAGN+SLE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.04355'
    title: Graph Attention Multi-Layer Perceptron
    date: Jun 9, 2022
    date_iso: '2022-06-09'
    date_display: Jun 2022
    codebase_url: https://github.com/PKU-DAIR/GAMLP
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6755
    - null
    metric_stds:
    - 0.0015
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
    arxiv_id: '2104.09376'
    title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced Training
    date: Apr 19, 2021
    date_iso: '2021-04-19'
    date_display: Apr 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6736
    - null
    metric_stds:
    - 0.001
    - null
  - model: SGC+AIR
    model_plain: SGC+AIR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.04361'
    title: Model Degradation Hinders Deep Graph Neural Networks
    date: Jun 9, 2022
    date_iso: '2022-06-09'
    date_display: Jun 2022
    codebase_url: https://github.com/PKU-DAIR/AIR
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6723
    - null
    metric_stds:
    - 0.002
    - null
  - model: OptBasisGNN
    model_plain: OptBasisGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.12432'
    title: Graph Neural Networks with Learnable and Optimal Polynomial Bases
    date: Feb 24, 2023
    date_iso: '2023-02-24'
    date_display: Feb 2023
    codebase_url: https://github.com/yuziGuo/FarOptBasis
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6722
    - null
    metric_stds:
    - 0.0015
    - null
  - model: TOP-GCNII
    model_plain: TOP-GCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.19693'
    title: Accurate and Scalable Graph Neural Networks via Message Invariance
    date: Feb 27, 2025
    date_iso: '2025-02-27'
    date_display: Feb 2025
    codebase_url: https://github.com/MIRALab-USTC/TOP
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6721
    - null
    metric_stds:
    - 0.0012
    - null
  - model: GraphSAINT+ATP
    model_plain: GraphSAINT+ATP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.06128'
    title: Rethinking Node-wise Propagation for Large-scale Graph Learning
    date: Feb 9, 2024
    date_iso: '2024-02-09'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.672
    - null
    metric_stds:
    - 0.002
    - null
  - model: ChebNetII
    model_plain: ChebNetII
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6718
    - null
    metric_stds:
    - 0.0032
    - null
  - model: shaDow
    model_plain: shaDow
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.06128'
    title: Rethinking Node-wise Propagation for Large-scale Graph Learning
    date: Feb 9, 2024
    date_iso: '2024-02-09'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.671
    - null
    metric_stds:
    - 0.002
    - null
  - model: SHADOW-GAT
    model_plain: SHADOW-GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.19693'
    title: Accurate and Scalable Graph Neural Networks via Message Invariance
    date: Feb 27, 2025
    date_iso: '2025-02-27'
    date_display: Feb 2025
    codebase_url: https://github.com/MIRALab-USTC/TOP
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6708
    - null
    metric_stds:
    - null
    - null
  - model: AdaptKry
    model_plain: AdaptKry
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.15354'
    title: 'Polynomial Selection in Spectral Graph Neural Networks: An Error-Sum of
      Function Slices Approach'
    date: Apr 15, 2024
    date_iso: '2024-04-15'
    date_display: Apr 2024
    codebase_url: https://github.com/vasile-paskardlgm/TFGNN
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6707
    - null
    metric_stds:
    - 0.002
    - null
  - model: NS-SAGE
    model_plain: NS-SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.19693'
    title: Accurate and Scalable Graph Neural Networks via Message Invariance
    date: Feb 27, 2025
    date_iso: '2025-02-27'
    date_display: Feb 2025
    codebase_url: https://github.com/MIRALab-USTC/TOP
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6706
    - null
    metric_stds:
    - null
    - null
  - model: SIGN-XL
    model_plain: SIGN-XL
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
    - 0.6706
    - null
    metric_stds:
    - 0.0017
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
    arxiv_id: '2404.15354'
    title: 'Polynomial Selection in Spectral Graph Neural Networks: An Error-Sum of
      Function Slices Approach'
    date: Apr 15, 2024
    date_iso: '2024-04-15'
    date_display: Apr 2024
    codebase_url: https://github.com/vasile-paskardlgm/TFGNN
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6703
    - null
    metric_stds:
    - 0.003
    - null
  - model: HOGA
    model_plain: HOGA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.13266'
    title: 'Graph Learning at Scale: Characterizing and Optimizing Pre-Propagation
      GNNs'
    date: Apr 17, 2025
    date_iso: '2025-04-17'
    date_display: Apr 2025
    codebase_url: https://github.com/cornell-zhang/preprop-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6686
    - null
    metric_stds:
    - 0.0011
    - null
  - model: MuseGNN
    model_plain: MuseGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.12457'
    title: 'MuseGNN: Forming Scalable, Convergent GNN Layers that Minimize a Sampling-Based
      Energy'
    date: Oct 19, 2023
    date_iso: '2023-10-19'
    date_display: Oct 2023
    codebase_url: https://github.com/RXPHD/Lazy_GNN
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6682
    - null
    metric_stds:
    - null
    - null
  - model: UniFilter
    model_plain: UniFilter
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.15354'
    title: 'Polynomial Selection in Spectral Graph Neural Networks: An Error-Sum of
      Function Slices Approach'
    date: Apr 15, 2024
    date_iso: '2024-04-15'
    date_display: Apr 2024
    codebase_url: https://github.com/vasile-paskardlgm/TFGNN
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6679
    - null
    metric_stds:
    - 0.003
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
    arxiv_id: '2104.09376'
    title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced Training
    date: Apr 19, 2021
    date_iso: '2021-04-19'
    date_display: Apr 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6675
    - null
    metric_stds:
    - 0.0084
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
    - 0.6673
    - null
    metric_stds:
    - 0.0041
    - null
  - model: GLEM-LM
    model_plain: GLEM-LM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2210.14709'
    title: Learning on Large-scale Text-attributed Graphs via Variational Inference
    date: Oct 2022
    date_iso: 2022-10
    date_display: Oct 2022
    codebase_url: https://github.com/AndyJZhao/GLEM
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6671
    - null
    metric_stds:
    - 0.0025
    - null
  - model: NIGCN
    model_plain: NIGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.14033'
    title: 'Partition-wise Graph Filtering: A Unified Perspective Through the Lens
      of Graph Coarsening'
    date: May 20, 2025
    date_iso: '2025-05-20'
    date_display: May 2025
    codebase_url: https://github.com/vasile-paskardlgm/CPF
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6657
    - null
    metric_stds:
    - 0.002
    - null
  - model: Supervised SGC
    model_plain: Supervised SGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.01535'
    title: 'Rethinking and Scaling Up Graph Contrastive Learning: An Extremely Efficient
      Approach with Group Discrimination'
    date: Jun 3, 2022
    date_iso: '2022-06-03'
    date_display: Jun 2022
    codebase_url: https://github.com/zyzisastudyreallyhardguy/Graph-Group-Discrimination
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.665
    - null
    metric_stds:
    - 0.002
    - null
  - model: GAMLP (FedGTA)
    model_plain: GAMLP (FedGTA)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2401.11755'
    title: 'FedGTA: Topology-aware Averaging for Federated Graph Learning'
    date: Sep 1, 2023
    date_iso: '2023-09-01'
    date_display: Sep 2023
    codebase_url: https://github.com/xkLi-Allen/FedGTA
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.665
    - null
    metric_stds:
    - 0.003
    - null
  - model: Coden
    model_plain: Coden
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.12613'
    title: 'Coden: Efficient Temporal Graph Neural Networks for Continuous Prediction'
    date: Feb 13, 2026
    date_iso: '2026-02-13'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6645
    - null
    metric_stds:
    - 0.0033
    - null
  - model: SAGE
    model_plain: SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.13266'
    title: 'Graph Learning at Scale: Characterizing and Optimizing Pre-Propagation
      GNNs'
    date: Apr 17, 2025
    date_iso: '2025-04-17'
    date_display: Apr 2025
    codebase_url: https://github.com/cornell-zhang/preprop-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6644
    - null
    metric_stds:
    - 0.0017
    - null
  - model: Cluster-GCN+ATP
    model_plain: Cluster-GCN+ATP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.06128'
    title: Rethinking Node-wise Propagation for Large-scale Graph Learning
    date: Feb 9, 2024
    date_iso: '2024-02-09'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.664
    - null
    metric_stds:
    - 0.002
    - null
  - model: NFGNN
    model_plain: NFGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.15354'
    title: 'Polynomial Selection in Spectral Graph Neural Networks: An Error-Sum of
      Function Slices Approach'
    date: Apr 15, 2024
    date_iso: '2024-04-15'
    date_display: Apr 2024
    codebase_url: https://github.com/vasile-paskardlgm/TFGNN
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6638
    - null
    metric_stds:
    - 0.002
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
    arxiv_id: '2504.13266'
    title: 'Graph Learning at Scale: Characterizing and Optimizing Pre-Propagation
      GNNs'
    date: Apr 17, 2025
    date_iso: '2025-04-17'
    date_display: Apr 2025
    codebase_url: https://github.com/cornell-zhang/preprop-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6636
    - null
    metric_stds:
    - 0.0005
    - null
  - model: GraphSage+C&S
    model_plain: GraphSage+C&S
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.06483'
    title: 'Sequential Aggregation and Rematerialization: Distributed Full-batch Training
      of Graph Neural Networks on Large Graphs'
    date: Nov 11, 2021
    date_iso: '2021-11-11'
    date_display: Nov 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.663
    - null
    metric_stds:
    - null
    - null
  - model: GAT (NS)
    model_plain: GAT (NS)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.12457'
    title: 'MuseGNN: Forming Scalable, Convergent GNN Layers that Minimize a Sampling-Based
      Energy'
    date: Oct 19, 2023
    date_iso: '2023-10-19'
    date_display: Oct 2023
    codebase_url: https://github.com/RXPHD/Lazy_GNN
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6628
    - null
    metric_stds:
    - 0.0008
    - null
  - model: GraphMAE2
    model_plain: GraphMAE2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.13630'
    title: 'UniGraph: Learning a Unified Cross-Domain Foundation Model for Text-Attributed
      Graphs'
    date: Feb 21, 2024
    date_iso: '2024-02-21'
    date_display: Feb 2024
    codebase_url: https://github.com/yf-he/UniGraph
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6624
    - null
    metric_stds:
    - 0.0054
    - null
  - model: FreshGNN
    model_plain: FreshGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.12457'
    title: 'MuseGNN: Forming Scalable, Convergent GNN Layers that Minimize a Sampling-Based
      Energy'
    date: Oct 19, 2023
    date_iso: '2023-10-19'
    date_display: Oct 2023
    codebase_url: https://github.com/RXPHD/Lazy_GNN
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6622
    - null
    metric_stds:
    - 0.0007
    - null
  - model: SAGE (NS)
    model_plain: SAGE (NS)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.12457'
    title: 'MuseGNN: Forming Scalable, Convergent GNN Layers that Minimize a Sampling-Based
      Energy'
    date: Oct 19, 2023
    date_iso: '2023-10-19'
    date_display: Oct 2023
    codebase_url: https://github.com/RXPHD/Lazy_GNN
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.662
    - null
    metric_stds:
    - 0.0013
    - null
  row_count: 141
  rows_json: /data/datasets/ogbn-papers100m/standard-split-rows.json
  chart_json: /data/datasets/ogbn-papers100m/standard-split-chart.json
  arch_counts:
    gnn: 100
    hybrid: 19
    graph_transformer: 4
    llm: 3
    walk: 2
    traditional: 12
  metric_counts:
  - 135
  - 6
  milestones: &id001
  - value: 0.6511
    std: 0.0014
    model: SIGN
    arxiv_id: '2004.11198'
    title: 'SIGN: Scalable Inception Graph Neural Networks'
    date: '2020-04-23'
  - value: 0.68
    std: 0.0015
    model: SAGN+SLE
    arxiv_id: '2104.09376'
    title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced Training
    date: '2021-04-19'
  - value: 0.6825
    std: 0.0011
    model: GAMLP+RLU
    arxiv_id: '2108.10097'
    title: Graph Attention MLP with Reliable Label Utilization
    date: '2021-08-23'
  - value: 0.6967
    std: 0.0004
    model: GAMLP+RLU
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: '2021-10-29'
  - value: 0.7036
    std: 0.0002
    model: GAMLP
    arxiv_id: '2210.14709'
    title: Learning on Large-scale Text-attributed Graphs via Variational Inference
    date: '2022-10-01'
  - value: 0.791
    std: null
    model: SGC
    arxiv_id: '2403.13268'
    title: 'Unifews: You Need Fewer Operations for Efficient Graph Neural Networks'
    date: '2024-03-19'
  milestones_by_metric:
    Accuracy: *id001
    F1:
    - value: 0.355
      std: 0.008
      model: SCARA
      arxiv_id: '2207.09179'
      title: 'SCARA: Scalable Graph Neural Networks with Feature-Oriented Optimization'
      date: '2022-07-01'
    - value: 0.4981
      std: 0.011
      model: NIGCN
      arxiv_id: '2305.14000'
      title: Node-wise Diffusion for Scalable Graph Learning
      date: '2023-04-30'
---

