---
title: IMDB-BINARY
slug: imdb-binary
benchmark: TU Dortmund
task_type: graph_classification
short_description: Binary graph classification of movie collaboration networks (action
  vs. romance).
description: '**2-class graph classification** Binary graph classification of movie
  collaboration networks (action vs. romance). Uses the released node/edge labels
  or attributes; several social datasets are featureless. Evaluated by Accuracy.'
detailed_description:
  task: Binary graph classification of movie collaboration networks (action vs. romance).
    The primary catalog metric is Accuracy.
  data: Binary graph classification of movie collaboration networks (action vs. romance).
    The cataloged artifact reports 1,000 graphs, 2 target classes or tasks.
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
- title: PyTorch Geometric IMDB-BINARY loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
stats:
  num_graphs: 1000
  avg_nodes: 19.8
  avg_edges: 96.5
  num_classes: 2
result_count: 217
best_model:
  model: GCFL
  value: 0.8299
  metric: Accuracy
  arxiv_id: '2106.13423'
  paper_title: Federated Graph Classification over Non-IID Graphs
papers:
- arxiv_id: '2510.03987'
  title: 'ICEPool: Enhancing Graph Pooling Networks with Inter-cluster Connectivity'
  date_iso: '2025-10-05'
  venue: ''
- arxiv_id: '2508.20597'
  title: Local Virtual Nodes for Alleviating Over-Squashing in Graph Neural Networks
  date_iso: '2025-08-28'
  venue: ''
- arxiv_id: '2506.06571'
  title: Graph Persistence goes Spectral
  date_iso: '2025-06-06'
  venue: NeurIPS 2025
- arxiv_id: '2503.01079'
  title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
  date_iso: '2025-03-03'
  venue: KDD 2025
- arxiv_id: '2501.09821'
  title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
  date_iso: '2025-01-16'
  venue: TMLR 2025
- arxiv_id: '2410.06746'
  title: Cluster-wise Graph Transformer with Dual-granularity Kernelized Attention
  date_iso: '2024-10-09'
  venue: NeurIPS 2024
- arxiv_id: '2407.04236'
  title: Graph Pooling via Ricci Flow
  date_iso: '2024-07-05'
  venue: TMLR 2024
- arxiv_id: '2402.16402'
  title: Graph Learning with Distributional Edge Layouts
  date_iso: '2024-02-26'
  venue: ''
- arxiv_id: '2402.16346'
  title: Boosting Graph Pooling with Persistent Homology
  date_iso: '2024-02-26'
  venue: NeurIPS 2024
- arxiv_id: '2402.15270'
  title: Smoothed Graph Contrastive Learning via Seamless Proximity Integration
  date_iso: '2024-02-23'
  venue: ''
- arxiv_id: '2401.03638'
  title: Unifying Graph Contrastive Learning via Graph Message Augmentation
  date_iso: '2024-01-08'
  venue: ''
- arxiv_id: '2311.01038'
  title: 'Better with Less: A Data-Active Perspective on Pre-Training Graph Neural
    Networks'
  date_iso: '2023-11-02'
  venue: NeurIPS 2023
- arxiv_id: '2310.01668'
  title: Locality-Aware Graph Rewiring in GNNs
  date_iso: '2023-10-02'
  venue: ICLR 2023
- arxiv_id: '2306.04004'
  title: Randomized Schur Complement Views for Graph Contrastive Learning
  date_iso: '2023-06-06'
  venue: ICML 2023
- arxiv_id: '2306.03698'
  title: Fine-grained Expressivity of Graph Neural Networks
  date_iso: '2023-06-06'
  venue: NeurIPS 2023
- arxiv_id: '2305.19903'
  title: Improving Expressivity of GNNs with Subgraph-specific Factor Embedded Normalization
  date_iso: '2023-05-31'
  venue: KDD 2023
- arxiv_id: '2302.08671'
  title: Search to Capture Long-range Dependency with Stacking GNNs for Graph Classification
  date_iso: '2023-02-17'
  venue: WWW 2023
- arxiv_id: '2210.11790'
  title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing in GNNs'
  date_iso: '2022-10-21'
  venue: ICLR 2022
- arxiv_id: '2208.06651'
  title: Revisiting Adversarial Attacks on Graph Neural Networks for Graph Classification
  date_iso: '2022-08-13'
  venue: ''
- arxiv_id: '2206.13510'
  title: Structural Entropy Guided Graph Hierarchical Pooling
  date_iso: '2022-06-26'
  venue: ICML 2022
- arxiv_id: '2202.13248'
  title: Automated Data Augmentations for Graph Classification
  date_iso: '2022-02-26'
  venue: ICLR 2022
- arxiv_id: '2111.03220'
  title: 'Augmentations in Graph Contrastive Learning: Current Methodological Flaws
    & Towards Better Practices'
  date_iso: '2021-11-05'
  venue: WWW 2021
- arxiv_id: '2108.10587'
  title: Pooling Architecture Search for Graph Classification
  date_iso: '2021-08-24'
  venue: ''
- arxiv_id: '2106.13423'
  title: Federated Graph Classification over Non-IID Graphs
  date_iso: '2021-06-25'
  venue: NeurIPS 2021
- arxiv_id: '2103.11155'
  title: Recognizing Predictive Substructures with Subgraph Information Bottleneck
  date_iso: '2021-03-20'
  venue: ''
- arxiv_id: '2010.05563'
  title: Graph Information Bottleneck for Subgraph Recognition
  date_iso: '2020-10-12'
  venue: ICLR 2020
- arxiv_id: '2006.05582'
  title: Contrastive Multi-View Representation Learning on Graphs
  date_iso: '2020-06-01'
  venue: ICML 2020
- arxiv_id: '2005.01214'
  title: Graph Homomorphism Convolution
  date_iso: '2020-05-03'
  venue: ICML 2020
- arxiv_id: '1805.08090'
  title: Graph Capsule Convolutional Neural Networks
  date_iso: '2018-05-21'
  venue: ICML 2018
variants:
- slug: 10-fold-cv
  name: 10-fold CV
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 1000
    avg_nodes: 19.8
    avg_edges: 96.5
    num_classes: 2
  metrics:
  - Accuracy
  - F1
  - ROC-AUC
  - epochs
  metric_display_names:
  - Accuracy
  - F1
  - ROC-AUC
  - epochs
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GCFL
    model_plain: GCFL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13423'
    title: Federated Graph Classification over Non-IID Graphs
    date: Jun 25, 2021
    date_iso: '2021-06-25'
    date_display: Jun 2021
    codebase_url: ''
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8299
    - null
    - null
    - null
    metric_stds:
    - 0.052
    - null
    - null
    - null
  - model: ID-GNN+BEC
    model_plain: ID-GNN+BEC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_iso: '2025-03-03'
    date_display: Mar 2025
    codebase_url: ''
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.815
    - null
    - null
    - null
    metric_stds:
    - 0.024
    - null
    - null
    - null
  - model: GIN+BEC
    model_plain: GIN+BEC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_iso: '2025-03-03'
    date_display: Mar 2025
    codebase_url: ''
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.808
    - null
    - null
    - null
    metric_stds:
    - 0.033
    - null
    - null
    - null
  - model: GCN+BEC
    model_plain: GCN+BEC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_iso: '2025-03-03'
    date_display: Mar 2025
    codebase_url: ''
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.799
    - null
    - null
    - null
    metric_stds:
    - 0.034
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
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_iso: '2025-03-03'
    date_display: Mar 2025
    codebase_url: ''
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.798
    - null
    - null
    - null
    metric_stds:
    - 0.023
    - null
    - null
    - null
  - model: NC-GNN+BEC
    model_plain: NC-GNN+BEC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_iso: '2025-03-03'
    date_display: Mar 2025
    codebase_url: ''
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.796
    - null
    - null
    - null
    metric_stds:
    - 0.036
    - null
    - null
    - null
  - model: GraphSNN+BEC
    model_plain: GraphSNN+BEC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_iso: '2025-03-03'
    date_display: Mar 2025
    codebase_url: ''
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.794
    - null
    - null
    - null
    metric_stds:
    - 0.027
    - null
    - null
    - null
  - model: ID-GNN
    model_plain: ID-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_iso: '2025-03-03'
    date_display: Mar 2025
    codebase_url: ''
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.793
    - null
    - null
    - null
    metric_stds:
    - 0.029
    - null
    - null
    - null
  - model: GAT +DEL-F
    model_plain: GAT +DEL-F
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7863
    - null
    - null
    - null
    metric_stds:
    - 0.0054
    - null
    - null
    - null
  - model: GraphSNN
    model_plain: GraphSNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_iso: '2025-03-03'
    date_display: Mar 2025
    codebase_url: ''
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.785
    - null
    - null
    - null
    metric_stds:
    - 0.023
    - null
    - null
    - null
  - model: EdgeDroppingDegree
    model_plain: EdgeDroppingDegree
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.04004'
    title: Randomized Schur Complement Views for Graph Contrastive Learning
    date: Jun 6, 2023
    date_iso: '2023-06-06'
    date_display: Jun 2023
    codebase_url: https://github.com/kvignesh1420/rlap
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.785
    - null
    - null
    - null
    metric_stds:
    - 0.0632
    - null
    - null
    - null
  - model: NC-GNN
    model_plain: NC-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_iso: '2025-03-03'
    date_display: Mar 2025
    codebase_url: ''
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.784
    - null
    - null
    - null
    metric_stds:
    - 0.04
    - null
    - null
    - null
  - model: EdgeDropping
    model_plain: EdgeDropping
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.04004'
    title: Randomized Schur Complement Views for Graph Contrastive Learning
    date: Jun 6, 2023
    date_iso: '2023-06-06'
    date_display: Jun 2023
    codebase_url: https://github.com/kvignesh1420/rlap
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.783
    - null
    - null
    - null
    metric_stds:
    - 0.1083
    - null
    - null
    - null
  - model: Graph Transformer +DEL-F
    model_plain: Graph Transformer +DEL-F
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7828
    - null
    - null
    - null
    metric_stds:
    - 0.0027
    - null
    - null
    - null
  - model: Graph Transformer + DEL-K
    model_plain: Graph Transformer + DEL-K
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7765
    - null
    - null
    - null
    metric_stds:
    - 0.0049
    - null
    - null
    - null
  - model: GPS(DEL-F)
    model_plain: GPS(DEL-F)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.775
    - null
    - null
    - null
    metric_stds:
    - 0.0065
    - null
    - null
    - null
  - model: FedProx
    model_plain: FedProx
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13423'
    title: Federated Graph Classification over Non-IID Graphs
    date: Jun 25, 2021
    date_iso: '2021-06-25'
    date_display: Jun 2021
    codebase_url: ''
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7746
    - null
    - null
    - null
    metric_stds:
    - 0.048
    - null
    - null
    - null
  - model: GNTK
    model_plain: GNTK
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    arxiv_id: '2005.01214'
    title: Graph Homomorphism Convolution
    date: May 3, 2020
    date_iso: '2020-05-03'
    date_display: May 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.769
    - null
    - null
    - null
    metric_stds:
    - 0.036
    - null
    - null
    - null
  - model: GAT + DEL-K
    model_plain: GAT + DEL-K
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7686
    - null
    - null
    - null
    metric_stds:
    - 0.0058
    - null
    - null
    - null
  - model: EdgeDroppingPR
    model_plain: EdgeDroppingPR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.04004'
    title: Randomized Schur Complement Views for Graph Contrastive Learning
    date: Jun 6, 2023
    date_iso: '2023-06-06'
    date_display: Jun 2023
    codebase_url: https://github.com/kvignesh1420/rlap
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.768
    - null
    - null
    - null
    metric_stds:
    - 0.0748
    - null
    - null
    - null
  - model: GSN
    model_plain: GSN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.16346'
    title: Boosting Graph Pooling with Persistent Homology
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: https://github.com/LOGO-CUHKSZ/TIP
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.768
    - null
    - null
    - null
    metric_stds:
    - 0.02
    - null
    - null
    - null
  - model: TOGL
    model_plain: TOGL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.16346'
    title: Boosting Graph Pooling with Persistent Homology
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: https://github.com/LOGO-CUHKSZ/TIP
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7665
    - null
    - null
    - null
    metric_stds:
    - 0.0275
    - null
    - null
    - null
  - model: self-train
    model_plain: self-train
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.13423'
    title: Federated Graph Classification over Non-IID Graphs
    date: Jun 25, 2021
    date_iso: '2021-06-25'
    date_display: Jun 2021
    codebase_url: ''
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7654
    - null
    - null
    - null
    metric_stds:
    - 0.057
    - null
    - null
    - null
  - model: Graph Transformer + MPNN
    model_plain: Graph Transformer + MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7651
    - null
    - null
    - null
    metric_stds:
    - 0.0039
    - null
    - null
    - null
  - model: DiffPool-TIP
    model_plain: DiffPool-TIP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.16346'
    title: Boosting Graph Pooling with Persistent Homology
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: https://github.com/LOGO-CUHKSZ/TIP
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.764
    - null
    - null
    - null
    metric_stds:
    - 0.0313
    - null
    - null
    - null
  - model: GraphAug
    model_plain: GraphAug
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.13248'
    title: Automated Data Augmentations for Graph Classification
    date: Feb 26, 2022
    date_iso: '2022-02-26'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.762
    - null
    - null
    - null
    metric_stds:
    - 0.004
    - null
    - null
    - null
  - model: Full B8C1
    model_plain: Full B8C1
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.08671'
    title: Search to Capture Long-range Dependency with Stacking GNNs for Graph Classification
    date: Feb 17, 2023
    date_iso: '2023-02-17'
    date_display: Feb 2023
    codebase_url: https://github.com/LARS-research/LRGNN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.762
    - null
    - null
    - null
    metric_stds:
    - 0.0518
    - null
    - null
    - null
  - model: EdgeAddition
    model_plain: EdgeAddition
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.04004'
    title: Randomized Schur Complement Views for Graph Contrastive Learning
    date: Jun 6, 2023
    date_iso: '2023-06-06'
    date_display: Jun 2023
    codebase_url: https://github.com/kvignesh1420/rlap
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.761
    - null
    - null
    - null
    metric_stds:
    - 0.0563
    - null
    - null
    - null
  - model: GAT + Random distance
    model_plain: GAT + Random distance
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7608
    - null
    - null
    - null
    metric_stds:
    - 0.0048
    - null
    - null
    - null
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.06571'
    title: Graph Persistence goes Spectral
    date: Jun 6, 2025
    date_iso: '2025-06-06'
    date_display: Jun 2025
    codebase_url: https://github.com/Aalto-QuML/SpectRe
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.76
    - null
    - null
    - null
    metric_stds:
    - 0.0283
    - null
    - null
    - null
  - model: SPECTRE
    model_plain: SPECTRE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.06571'
    title: Graph Persistence goes Spectral
    date: Jun 6, 2025
    date_iso: '2025-06-06'
    date_display: Jun 2025
    codebase_url: https://github.com/Aalto-QuML/SpectRe
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.76
    - null
    - null
    - null
    metric_stds:
    - 0.0
    - null
    - null
    - null
  - model: FedAvg
    model_plain: FedAvg
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13423'
    title: Federated Graph Classification over Non-IID Graphs
    date: Jun 25, 2021
    date_iso: '2021-06-25'
    date_display: Jun 2021
    codebase_url: ''
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7596
    - null
    - null
    - null
    metric_stds:
    - 0.049
    - null
    - null
    - null
  - model: GAT + MPNN
    model_plain: GAT + MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7585
    - null
    - null
    - null
    metric_stds:
    - 0.0048
    - null
    - null
    - null
  - model: EdgeDroppingEVC
    model_plain: EdgeDroppingEVC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.04004'
    title: Randomized Schur Complement Views for Graph Contrastive Learning
    date: Jun 6, 2023
    date_iso: '2023-06-06'
    date_display: Jun 2023
    codebase_url: https://github.com/kvignesh1420/rlap
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.758
    - null
    - null
    - null
    metric_stds:
    - 0.0626
    - null
    - null
    - null
  - model: SGCL-D
    model_plain: SGCL-D
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.15270'
    title: Smoothed Graph Contrastive Learning via Seamless Proximity Integration
    date: Feb 23, 2024
    date_iso: '2024-02-23'
    date_display: Feb 2024
    codebase_url: https://github.com/maysambehmanesh/SGCL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.758
    - null
    - null
    - null
    metric_stds:
    - 0.019
    - null
    - null
    - null
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.756
    - null
    - null
    - null
    metric_stds:
    - 0.0317
    - null
    - null
    - null
  - model: CGRA
    model_plain: CGRA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.15270'
    title: Smoothed Graph Contrastive Learning via Seamless Proximity Integration
    date: Feb 23, 2024
    date_iso: '2024-02-23'
    date_display: Feb 2024
    codebase_url: https://github.com/maysambehmanesh/SGCL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.756
    - null
    - null
    - null
    metric_stds:
    - 0.005
    - null
    - null
    - null
  - model: GraphMAE
    model_plain: GraphMAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7552
    - null
    - null
    - null
    metric_stds:
    - 0.0066
    - null
    - null
    - null
  - model: GPS+FastSpectRe
    model_plain: GPS+FastSpectRe
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.06571'
    title: Graph Persistence goes Spectral
    date: Jun 6, 2025
    date_iso: '2025-06-06'
    date_display: Jun 2025
    codebase_url: https://github.com/Aalto-QuML/SpectRe
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.755
    - null
    - null
    - null
    metric_stds:
    - 0.0071
    - null
    - null
    - null
  - model: MarkovDiffusion
    model_plain: MarkovDiffusion
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.04004'
    title: Randomized Schur Complement Views for Graph Contrastive Learning
    date: Jun 6, 2023
    date_iso: '2023-06-06'
    date_display: Jun 2023
    codebase_url: https://github.com/kvignesh1420/rlap
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.753
    - null
    - null
    - null
    metric_stds:
    - 0.0836
    - null
    - null
    - null
  - model: Graph Transformer + Random distance
    model_plain: Graph Transformer + Random distance
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
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
    metric_stds:
    - 0.0065
    - null
    - null
    - null
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.752
    - null
    - null
    - null
    metric_stds:
    - 0.0404
    - null
    - null
    - null
  - model: SGCL-T
    model_plain: SGCL-T
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.15270'
    title: Smoothed Graph Contrastive Learning via Seamless Proximity Integration
    date: Feb 23, 2024
    date_iso: '2024-02-23'
    date_display: Feb 2024
    codebase_url: https://github.com/maysambehmanesh/SGCL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.752
    - null
    - null
    - null
    metric_stds:
    - 0.028
    - null
    - null
    - null
  - model: MinCutPool-TIP
    model_plain: MinCutPool-TIP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.16346'
    title: Boosting Graph Pooling with Persistent Homology
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: https://github.com/LOGO-CUHKSZ/TIP
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.752
    - null
    - null
    - null
    metric_stds:
    - 0.0267
    - null
    - null
    - null
  - model: GIN-0
    model_plain: GIN-0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.05582'
    title: Contrastive Multi-View Representation Learning on Graphs
    date: Jun 1, 2020
    date_iso: '2020-06-01'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.751
    - null
    - null
    - null
    metric_stds:
    - 0.051
    - null
    - null
    - null
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
    - 0.751
    - null
    - null
    - null
    metric_stds:
    - 0.0416
    - null
    - null
    - null
  - model: PAS
    model_plain: PAS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2108.10587'
    title: Pooling Architecture Search for Graph Classification
    date: Aug 24, 2021
    date_iso: '2021-08-24'
    date_display: Aug 2021
    codebase_url: https://github.com/GraphNAS/GraphNAS
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.751
    - null
    - null
    - null
    metric_stds:
    - 0.0532
    - null
    - null
    - null
  - model: Cluster-GT
    model_plain: Cluster-GT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2410.06746'
    title: Cluster-wise Graph Transformer with Dual-granularity Kernelized Attention
    date: Oct 9, 2024
    date_iso: '2024-10-09'
    date_display: Oct 2024
    codebase_url: https://github.com/LUMIA-Group/Cluster-wise-Graph-Transformer
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.751
    - null
    - null
    - null
    metric_stds:
    - 0.0084
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
    arxiv_id: '2005.01214'
    title: Graph Homomorphism Convolution
    date: May 3, 2020
    date_iso: '2020-05-03'
    date_display: May 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.751
    - null
    - null
    - null
    metric_stds:
    - 0.051
    - null
    - null
    - null
  - model: RePHINE
    model_plain: RePHINE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2506.06571'
    title: Graph Persistence goes Spectral
    date: Jun 6, 2025
    date_iso: '2025-06-06'
    date_display: Jun 2025
    codebase_url: https://github.com/Aalto-QuML/SpectRe
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.75
    - null
    - null
    - null
    metric_stds:
    - 0.0283
    - null
    - null
    - null
  row_count: 217
  rows_json: /data/datasets/imdb-binary/10-fold-cv-rows.json
  chart_json: /data/datasets/imdb-binary/10-fold-cv-chart.json
  arch_counts:
    gnn: 123
    hybrid: 40
    graph_transformer: 1
    llm: 0
    walk: 4
    traditional: 41
  metric_counts:
  - 188
  - 13
  - 6
  - 10
  milestones: &id001
  - value: 0.7169
    std: 0.034
    model: GCNNs
    arxiv_id: '1805.08090'
    title: Graph Capsule Convolutional Neural Networks
    date: '2018-05-21'
  - value: 0.769
    std: 0.036
    model: GNTK
    arxiv_id: '2005.01214'
    title: Graph Homomorphism Convolution
    date: '2020-05-03'
  - value: 0.8299
    std: 0.052
    model: GCFL
    arxiv_id: '2106.13423'
    title: Federated Graph Classification over Non-IID Graphs
    date: '2021-06-25'
  milestones_by_metric:
    Accuracy: *id001
    F1:
    - value: 0.767
      std: 0.0101
      model: APT-P (fine-tune)
      arxiv_id: '2311.01038'
      title: 'Better with Less: A Data-Active Perspective on Pre-Training Graph Neural
        Networks'
      date: '2023-11-02'
    ROC-AUC:
    - value: 0.7983
      std: 0.0075
      model: GraphSNN
      arxiv_id: '2305.19903'
      title: Improving Expressivity of GNNs with Subgraph-specific Factor Embedded
        Normalization
      date: '2023-05-31'
    epochs:
    - value: 620.0
      std: 151.0
      model: kmis
      arxiv_id: '2501.09821'
      title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
      date: '2025-01-16'
---

