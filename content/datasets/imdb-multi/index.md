---
title: IMDB-MULTI
slug: imdb-multi
benchmark: TU Dortmund
task_type: graph_classification
short_description: Multi-class graph classification of movie collaboration networks
  (3 genres).
description: '**3-class graph classification** Multi-class graph classification of
  movie collaboration networks (3 genres). Uses the released node/edge labels or attributes;
  several social datasets are featureless. Evaluated by Accuracy.'
detailed_description:
  task: Multi-class graph classification of movie collaboration networks (3 genres).
    The primary catalog metric is Accuracy.
  data: Multi-class graph classification of movie collaboration networks (3 genres).
    The cataloged artifact reports 1,500 graphs, 3 target classes or tasks.
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
- title: PyTorch Geometric IMDB-MULTI loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
stats:
  num_graphs: 1500
  avg_nodes: 13.0
  avg_edges: 65.9
  num_classes: 3
  extra_stats:
    edge_feature_dim: 0
    edge_feature_type: no edge attributes in the standard TU artifact
    node_feature_dim: 0
    node_feature_type: no intrinsic node features
    statistic_notes: The TU benchmark reports 1,500 graphs, 13.00 nodes, and 65.94
      undirected edges per graph
result_count: 123
best_model:
  model: GraphSNN
  value: 0.779
  metric: Accuracy
  arxiv_id: '2206.02059'
  paper_title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
papers:
- arxiv_id: '2510.03987'
  title: 'ICEPool: Enhancing Graph Pooling Networks with Inter-cluster Connectivity'
  date_iso: '2025-10-05'
  venue: ''
- arxiv_id: '2410.06746'
  title: Cluster-wise Graph Transformer with Dual-granularity Kernelized Attention
  date_iso: '2024-10-09'
  venue: NeurIPS 2024
- arxiv_id: '2408.13471'
  title: Disentangled Generative Graph Representation Learning
  date_iso: '2024-08-24'
  venue: ''
- arxiv_id: '2406.17251'
  title: 'TopoGCL: Topological Graph Contrastive Learning'
  date_iso: '2024-03-24'
  venue: AAAI 2024
- arxiv_id: '2402.16402'
  title: Graph Learning with Distributional Edge Layouts
  date_iso: '2024-02-26'
  venue: ''
- arxiv_id: '2306.06788'
  title: Graph Mixup with Soft Alignments
  date_iso: '2023-06-11'
  venue: ICML 2023
- arxiv_id: '2306.04004'
  title: Randomized Schur Complement Views for Graph Contrastive Learning
  date_iso: '2023-06-06'
  venue: ICML 2023
- arxiv_id: '2306.03698'
  title: Fine-grained Expressivity of Graph Neural Networks
  date_iso: '2023-06-06'
  venue: NeurIPS 2023
- arxiv_id: '2304.01575'
  title: The expressive power of pooling in Graph Neural Networks
  date_iso: '2023-04-04'
  venue: NeurIPS 2023
- arxiv_id: '2206.13510'
  title: Structural Entropy Guided Graph Hierarchical Pooling
  date_iso: '2022-06-26'
  venue: ICML 2022
- arxiv_id: '2206.02059'
  title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
  date_iso: '2022-06-04'
  venue: TMLR 2022
- arxiv_id: '2112.01064'
  title: 'AutoGEL: An Automated Graph Neural Network with Explicit Link Information'
  date_iso: '2021-12-02'
  venue: NeurIPS 2021
- arxiv_id: '2110.07875'
  title: Graph Neural Networks with Learnable Structural and Positional Representations
  date_iso: '2021-10-15'
  venue: ICLR 2021
- arxiv_id: '2108.10587'
  title: Pooling Architecture Search for Graph Classification
  date_iso: '2021-08-24'
  venue: ''
- arxiv_id: '2102.07835'
  title: Topological Graph Neural Networks
  date_iso: '2021-02-15'
  venue: ICLR 2021
- arxiv_id: '2010.15116'
  title: On Graph Neural Networks versus Graph-Augmented MLPs
  date_iso: '2020-10-28'
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
    num_graphs: 1500
    avg_nodes: 13.0
    avg_edges: 65.9
    num_classes: 3
    extra_stats:
      edge_feature_dim: 0
      edge_feature_type: no edge attributes in the standard TU artifact
      node_feature_dim: 0
      node_feature_type: no intrinsic node features
      statistic_notes: The TU benchmark reports 1,500 graphs, 13.00 nodes, and 65.94
        undirected edges per graph
  metrics:
  - Accuracy
  - equivalence classes
  metric_display_names:
  - Accuracy
  - equivalence classes
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GraphSNN
    model_plain: GraphSNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02059'
    title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
    date: Jun 4, 2022
    date_iso: '2022-06-04'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.779
    - null
    metric_stds:
    - 0.036
    - null
  - model: SIN
    model_plain: SIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02059'
    title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
    date: Jun 4, 2022
    date_iso: '2022-06-04'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.756
    - null
    metric_stds:
    - 0.032
    - null
  - model: CIN
    model_plain: CIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02059'
    title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
    date: Jun 4, 2022
    date_iso: '2022-06-04'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.756
    - null
    metric_stds:
    - 0.037
    - null
  - model: Empowering GNNs
    model_plain: Empowering GNNs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.02059'
    title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
    date: Jun 4, 2022
    date_iso: '2022-06-04'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.752
    - null
    metric_stds:
    - 0.045
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
    arxiv_id: '2206.02059'
    title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
    date: Jun 4, 2022
    date_iso: '2022-06-04'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.751
    - null
    metric_stds:
    - 0.051
    - null
  - model: GNN-AK+
    model_plain: GNN-AK+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02059'
    title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
    date: Jun 4, 2022
    date_iso: '2022-06-04'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.75
    - null
    metric_stds:
    - 0.042
    - null
  - model: PPGN
    model_plain: PPGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02059'
    title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
    date: Jun 4, 2022
    date_iso: '2022-06-04'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.73
    - null
    metric_stds:
    - 0.058
    - null
  - model: rLap
    model_plain: rLap
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5947
    - null
    metric_stds:
    - 0.0742
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5907
    - null
    metric_stds:
    - 0.05
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.59
    - null
    metric_stds:
    - 0.0958
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.578
    - null
    metric_stds:
    - 0.0996
    - null
  - model: RandomWalkSubgraph
    model_plain: RandomWalkSubgraph
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.578
    - null
    metric_stds:
    - 0.0947
    - null
  - model: NodeDropping
    model_plain: NodeDropping
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5753
    - null
    metric_stds:
    - 0.085
    - null
  - model: PPRDiffusion
    model_plain: PPRDiffusion
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5713
    - null
    metric_stds:
    - 0.0772
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.568
    - null
    metric_stds:
    - 0.0771
    - null
  - model: AutoGEL
    model_plain: AutoGEL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2112.01064'
    title: 'AutoGEL: An Automated Graph Neural Network with Explicit Link Information'
    date: Dec 2, 2021
    date_iso: '2021-12-02'
    date_display: Dec 2021
    codebase_url: https://github.com/zwangeo/AutoGEL
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.568
    - null
    metric_stds:
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5613
    - null
    metric_stds:
    - 0.0831
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.55
    - null
    metric_stds:
    - 0.0701
    - null
  - model: H_d
    model_plain: H_d
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_iso: '2024-08-24'
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
    - 0.5477
    - null
    metric_stds:
    - 0.0263
    - null
  - model: H_d + H_g
    model_plain: H_d + H_g
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_iso: '2024-08-24'
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
    - 0.5469
    - null
    metric_stds:
    - 0.0206
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5354
    - null
    metric_stds:
    - 0.0027
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5339
    - null
    metric_stds:
    - 0.0033
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5327
    - null
    metric_stds:
    - 0.0099
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5295
    - null
    metric_stds:
    - 0.0064
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
    - 0.5286
    - null
    metric_stds:
    - 0.0033
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
    - 0.5286
    - null
    metric_stds:
    - 0.0029
    - null
  - model: TopoGCL
    model_plain: TopoGCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.17251'
    title: 'TopoGCL: Topological Graph Contrastive Learning'
    date: Mar 24, 2024
    date_iso: '2024-03-24'
    date_display: Mar 2024
    codebase_url: https://github.com/topogclaaai24/TopoGCL
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5281
    - null
    metric_stds:
    - 0.0031
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
    - 0.5281
    - null
    metric_stds:
    - 0.0025
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.528
    - null
    metric_stds:
    - 0.046
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
    - 0.526
    - null
    metric_stds:
    - 0.0058
    - null
  - model: SEP-G ICE
    model_plain: SEP-G ICE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.03987'
    title: 'ICEPool: Enhancing Graph Pooling Networks with Inter-cluster Connectivity'
    date: Oct 5, 2025
    date_iso: '2025-10-05'
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
    - 0.5247
    - null
    metric_stds:
    - 0.01
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
    - 0.5231
    - null
    metric_stds:
    - 0.0045
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.523
    - null
    metric_stds:
    - 0.028
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.523
    - null
    metric_stds:
    - 0.028
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.522
    - null
    metric_stds:
    - 0.0373
    - null
  - model: GCL-TAGS
    model_plain: GCL-TAGS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.17251'
    title: 'TopoGCL: Topological Graph Contrastive Learning'
    date: Mar 24, 2024
    date_iso: '2024-03-24'
    date_display: Mar 2024
    codebase_url: https://github.com/topogclaaai24/TopoGCL
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5216
    - null
    metric_stds:
    - 0.0072
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
    - 0.5213
    - null
    metric_stds:
    - 0.0078
    - null
  - model: GIN-ε
    model_plain: GIN-ε
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.521
    - null
    metric_stds:
    - 0.036
    - null
  - model: GCN-1-TOGL-1
    model_plain: GCN-1-TOGL-1
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2102.07835'
    title: Topological Graph Neural Networks
    date: Feb 15, 2021
    date_iso: '2021-02-15'
    date_display: Feb 2021
    codebase_url: https://github.com/BorgwardtLab/TOGL
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.52
    - null
    metric_stds:
    - 0.04
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.519
    - null
    metric_stds:
    - 0.038
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
    - 0.5163
    - null
    metric_stds:
    - 0.0052
    - null
  - model: H_g
    model_plain: H_g
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_iso: '2024-08-24'
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
    - 0.5162
    - null
    metric_stds:
    - 0.0061
    - null
  - model: SEP-G
    model_plain: SEP-G
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.13510'
    title: Structural Entropy Guided Graph Hierarchical Pooling
    date: Jun 26, 2022
    date_iso: '2022-06-26'
    date_display: Jun 2022
    codebase_url: https://github.com/Wu-Junran/SEP
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5153
    - null
    metric_stds:
    - 0.0065
    - null
  - model: AWL kernel
    model_plain: AWL kernel
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.515
    - null
    metric_stds:
    - 0.036
    - null
  - model: MI
    model_plain: MI
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.512
    - null
    metric_stds:
    - 0.005
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.509
    - null
    metric_stds:
    - 0.022
    - null
  - model: GIN-JK
    model_plain: GIN-JK
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.508
    - null
    metric_stds:
    - 0.0302
    - null
  - model: S-Mixup
    model_plain: S-Mixup
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2306.06788'
    title: Graph Mixup with Soft Alignments
    date: Jun 11, 2023
    date_iso: '2023-06-11'
    date_display: Jun 2023
    codebase_url: https://github.com/divelab/DIG
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5073
    - null
    metric_stds:
    - 0.0366
    - null
  - model: GMT
    model_plain: GMT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.13510'
    title: Structural Entropy Guided Graph Hierarchical Pooling
    date: Jun 26, 2022
    date_iso: '2022-06-26'
    date_display: Jun 2022
    codebase_url: https://github.com/Wu-Junran/SEP
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5066
    - null
    metric_stds:
    - 0.0082
    - null
  - model: AD-GCL
    model_plain: AD-GCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.17251'
    title: 'TopoGCL: Topological Graph Contrastive Learning'
    date: Mar 24, 2024
    date_iso: '2024-03-24'
    date_display: Mar 2024
    codebase_url: https://github.com/topogclaaai24/TopoGCL
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.506
    - null
    metric_stds:
    - 0.007
    - null
  row_count: 123
  rows_json: /data/datasets/imdb-multi/10-fold-cv-rows.json
  chart_json: /data/datasets/imdb-multi/10-fold-cv-chart.json
  arch_counts:
    gnn: 74
    hybrid: 14
    graph_transformer: 2
    llm: 0
    walk: 4
    traditional: 22
  metric_counts:
  - 121
  - 2
  milestones: &id001
  - value: 0.485
    std: 0.041
    model: GCNNs
    arxiv_id: '1805.08090'
    title: Graph Capsule Convolutional Neural Networks
    date: '2018-05-21'
  - value: 0.528
    std: 0.046
    model: GNTK
    arxiv_id: '2005.01214'
    title: Graph Homomorphism Convolution
    date: '2020-05-03'
  - value: 0.568
    std: null
    model: AutoGEL
    arxiv_id: '2112.01064'
    title: 'AutoGEL: An Automated Graph Neural Network with Explicit Link Information'
    date: '2021-12-02'
  - value: 0.779
    std: 0.036
    model: GraphSNN
    arxiv_id: '2206.02059'
    title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
    date: '2022-06-04'
  milestones_by_metric:
    Accuracy: *id001
    equivalence classes:
    - value: 387.0
      std: null
      model: GNN
      arxiv_id: '2010.15116'
      title: On Graph Neural Networks versus Graph-Augmented MLPs
      date: '2020-10-28'
---

