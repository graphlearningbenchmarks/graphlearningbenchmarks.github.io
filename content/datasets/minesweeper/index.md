---
title: Minesweeper
slug: minesweeper
benchmark: Heterophily Benchmark
task_type: node_classification
short_description: Synthetic Minesweeper grid graph binary node classification from
  the heterophilic benchmark.
description: '**Binary node classification** Synthetic Minesweeper grid graph binary
  node classification from the heterophilic benchmark. Uses the corrected benchmark
  features and ten official splits. Evaluated by ROC-AUC.'
detailed_description:
  task: Synthetic Minesweeper grid graph binary node classification from the heterophilic
    benchmark. The primary catalog metric is ROC-AUC.
  data: Synthetic Minesweeper grid graph binary node classification from the heterophilic
    benchmark.
  features: The benchmark provides one fixed graph, node features, labels, and ten
    official splits per dataset. Features are dataset-specific and include text-derived,
    product, synthetic-grid, or platform-account attributes described by the release.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses ROC-AUC (higher is better). Exact masks or folds must come
    from the cited release.'
  quirks_and_pitfalls: Use the corrected release and its ten masks. Several tasks
    are imbalanced and use ROC-AUC rather than accuracy; treating missing relationships
    as negative evidence or tuning on the test masks invalidates comparison.
sources:
- title: Heterophily Benchmark benchmark
  arxiv_id: '2302.11640'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric Minesweeper loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.HeterophilousGraphDataset.html
  kind: implementation_documentation
primary_metric: ROC-AUC
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.HeterophilousGraphDataset.html
stats: null
result_count: 274
best_model:
  model: BuNN
  value: 0.9899
  metric: ROC-AUC
  arxiv_id: '2405.15540'
  paper_title: Bundle Neural Networks for message diffusion on graphs
papers:
- arxiv_id: '2605.20248'
  title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
    Classification'
  date_iso: '2026-05-18'
  venue: ''
- arxiv_id: '2605.13383'
  title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
  date_iso: '2026-05-13'
  venue: ''
- arxiv_id: '2604.19028'
  title: Learning Posterior Predictive Distributions for Node Classification from
    Synthetic Graph Priors
  date_iso: '2026-04-21'
  venue: ICLR 2026
- arxiv_id: '2604.08980'
  title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware Graph
    Learning'
  date_iso: '2026-04-10'
  venue: ''
- arxiv_id: '2603.26178'
  title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
    Learning via Ricci Flow'
  date_iso: '2026-03-27'
  venue: ''
- arxiv_id: '2602.07256'
  title: 'Graph homophily booster: Reimagining the role of discrete features in heterophilic
    graph learning'
  date_iso: '2026-02-06'
  venue: ICLR 2026
- arxiv_id: '2512.12642'
  title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural Networks'
  date_iso: '2025-12-14'
  venue: ''
- arxiv_id: '2510.22451'
  title: 'GraphTOP: Graph Topology-Oriented Prompting for Graph Neural Networks'
  date_iso: '2025-10-25'
  venue: NeurIPS 2025
- arxiv_id: '2510.21267'
  title: Relieving the Over-Aggregating Effect in Graph Transformers
  date_iso: '2025-10-24'
  venue: NeurIPS 2025
- arxiv_id: '2510.21207'
  title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised Learning on Diverse
    Graphs with Heterogeneous Specialization'
  date_iso: '2025-10-24'
  venue: ''
- arxiv_id: '2509.12530'
  title: 'Graph Homophily Booster: Rethinking the Role of Discrete Features on Heterophilic
    Graphs'
  date_iso: '2025-09-16'
  venue: ''
- arxiv_id: '2508.17531'
  title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
  date_iso: '2025-08-24'
  venue: ''
- arxiv_id: '2507.14484'
  title: 'ReDiSC: A Reparameterized Masked Diffusion Model for Scalable Node Classification
    with Structured Predictions'
  date_iso: '2025-07-19'
  venue: ''
- arxiv_id: '2506.19343'
  title: Discrepancy-Aware Graph Mask Auto-Encoder
  date_iso: '2025-06-24'
  venue: KDD 2025
- arxiv_id: '2505.15015'
  title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
  date_iso: '2025-05-21'
  venue: ''
- arxiv_id: '2504.19785'
  title: Heterophily-informed Message Passing
  date_iso: '2025-04-28'
  venue: TMLR 2025
- arxiv_id: '2502.10818'
  title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
    Recurrent and Graph Learning'
  date_iso: '2025-02-15'
  venue: ''
- arxiv_id: '2411.16278'
  title: Even Sparser Graph Transformers
  date_iso: '2024-11-25'
  venue: NeurIPS 2024
- arxiv_id: '2411.05274'
  title: Distributed-Order Fractional Graph Operating Network
  date_iso: '2024-11-08'
  venue: NeurIPS 2024
- arxiv_id: '2410.05499'
  title: Unitary convolutions for learning on graphs and groups
  date_iso: '2024-10-07'
  venue: NeurIPS 2024
- arxiv_id: '2409.05755'
  title: Re-evaluating the Advancements of Heterophilic Graph Learning
  date_iso: '2024-09-09'
  venue: ''
- arxiv_id: '2407.11596'
  title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
  date_iso: '2024-06-30'
  venue: ''
- arxiv_id: '2406.06642'
  title: 'TopoBench: A Framework for Benchmarking Topological Deep Learning'
  date_iso: '2024-06-09'
  venue: ''
- arxiv_id: '2405.16185'
  title: Differentiable Cluster Graph Neural Network
  date_iso: '2024-05-25'
  venue: ''
- arxiv_id: '2405.15540'
  title: Bundle Neural Networks for message diffusion on graphs
  date_iso: '2024-05-24'
  venue: ''
- arxiv_id: '2403.12529'
  title: Contextualized Messages Boost Graph Representations
  date_iso: '2024-03-19'
  venue: TMLR 2024
- arxiv_id: '2403.01232'
  title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
  date_iso: '2024-03-02'
  venue: ICLR 2024
- arxiv_id: '2402.08678'
  title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
  date_iso: '2024-02-13'
  venue: KDD 2024
- arxiv_id: '2306.12943'
  title: Evolving Computation Graphs
  date_iso: '2023-06-22'
  venue: ICML 2023
- arxiv_id: '2305.16780'
  title: Graph Neural Convection-Diffusion with Heterophily
  date_iso: '2023-05-26'
  venue: IJCAI 2023
- arxiv_id: '2202.07082'
  title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
  date_iso: '2022-02-14'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: ROC-AUC
  default_metric: ROC-AUC
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - ROC-AUC
  - Accuracy
  metric_display_names:
  - ROC-AUC
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: BuNN
    model_plain: BuNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.15540'
    title: Bundle Neural Networks for message diffusion on graphs
    date: May 24, 2024
    date_iso: '2024-05-24'
    date_display: May 2024
    codebase_url: https://github.com/jacobbamberger/BuNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9899
    - null
    metric_stds:
    - 0.0016
    - null
  - model: DC-GNN
    model_plain: DC-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.16185'
    title: Differentiable Cluster Graph Neural Network
    date: May 25, 2024
    date_iso: '2024-05-25'
    date_display: May 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.985
    - null
    metric_stds:
    - 0.0021
    - null
  - model: Polynormer-r
    model_plain: Polynormer-r
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/cornell-zhang/Polynormer
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9746
    - null
    metric_stds:
    - 0.0036
    - null
  - model: Polynormer + Wideformer
    model_plain: Polynormer + Wideformer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_iso: '2025-10-24'
    date_display: Oct 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9726
    - null
    metric_stds:
    - 0.0001
    - null
  - model: Polynormer + Entropy Reg
    model_plain: Polynormer + Entropy Reg
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_iso: '2025-10-24'
    date_display: Oct 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.972
    - null
    metric_stds:
    - 0.0032
    - null
  - model: Polynormer
    model_plain: Polynormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/cornell-zhang/Polynormer
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9696
    - null
    metric_stds:
    - 0.0052
    - null
  - model: Polynormer-v1
    model_plain: Polynormer-v1
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/cornell-zhang/Polynormer
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9696
    - null
    metric_stds:
    - 0.0052
    - null
  - model: Polynormer-v2
    model_plain: Polynormer-v2
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/cornell-zhang/Polynormer
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9648
    - null
    metric_stds:
    - 0.0037
    - null
  - model: D-CDE
    model_plain: D-CDE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.05274'
    title: Distributed-Order Fractional Graph Operating Network
    date: Nov 8, 2024
    date_iso: '2024-11-08'
    date_display: Nov 2024
    codebase_url: https://github.com/zknus/NeurIPS-2024-DRAGON
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9647
    - null
    metric_stds:
    - 0.0189
    - null
  - model: Schrödinger
    model_plain: Schrödinger
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_iso: '2026-05-13'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9631
    - null
    metric_stds:
    - 0.0049
    - null
  - model: Lie Unitary GCN
    model_plain: Lie Unitary GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.478
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.05499'
    title: Unitary convolutions for learning on graphs and groups
    date: Oct 7, 2024
    date_iso: '2024-10-07'
    date_display: Oct 2024
    codebase_url: https://github.com/Weber-GeoML/Unitary_Convolutions
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9611
    - null
    metric_stds:
    - 0.001
    - null
  - model: Lie UniGCN
    model_plain: Lie UniGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_iso: '2026-05-13'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9611
    - null
    metric_stds:
    - 0.001
    - null
  - model: F-CDE
    model_plain: F-CDE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.05274'
    title: Distributed-Order Fractional Graph Operating Network
    date: Nov 8, 2024
    date_iso: '2024-11-08'
    date_display: Nov 2024
    codebase_url: https://github.com/zknus/NeurIPS-2024-DRAGON
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9604
    - null
    metric_stds:
    - 0.0025
    - null
  - model: GCN-SSM (Optimal L)
    model_plain: GCN-SSM (Optimal L)
    is_baseline: false
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
    - 0.9602
    - null
    metric_stds:
    - 0.0052
    - null
  - model: CDE-GRAND-GAT
    model_plain: CDE-GRAND-GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.16780'
    title: Graph Neural Convection-Diffusion with Heterophily
    date: May 26, 2023
    date_iso: '2023-05-26'
    date_display: May 2023
    codebase_url: https://github.com/zknus/Graph-Diffusion-CDE
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.955
    - null
    metric_stds:
    - 0.0523
    - null
  - model: CDE
    model_plain: CDE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.05274'
    title: Distributed-Order Fractional Graph Operating Network
    date: Nov 8, 2024
    date_iso: '2024-11-08'
    date_display: Nov 2024
    codebase_url: https://github.com/zknus/NeurIPS-2024-DRAGON
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.955
    - null
    metric_stds:
    - 0.0523
    - null
  - model: CDE-GRAND
    model_plain: CDE-GRAND
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.16780'
    title: Graph Neural Convection-Diffusion with Heterophily
    date: May 26, 2023
    date_iso: '2023-05-26'
    date_display: May 2023
    codebase_url: https://github.com/zknus/Graph-Diffusion-CDE
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.955
    - null
    metric_stds:
    - 0.0523
    - null
  - model: Graphite
    model_plain: Graphite
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.12530'
    title: 'Graph Homophily Booster: Rethinking the Role of Discrete Features on Heterophilic
      Graphs'
    date: Sep 16, 2025
    date_iso: '2025-09-16'
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
    - 0.9478
    - null
    metric_stds:
    - 0.0041
    - null
  - model: ECG-GAT-sep
    model_plain: ECG-GAT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9452
    - null
    metric_stds:
    - 0.002
    - null
  - model: MLP-ECG-GAT-sep
    model_plain: MLP-ECG-GAT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9452
    - null
    metric_stds:
    - 0.002
    - null
  - model: MLPBGRL-GAT-sep
    model_plain: MLPBGRL-GAT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9439
    - null
    metric_stds:
    - 0.002
    - null
  - model: Unitary GCN
    model_plain: Unitary GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.05499'
    title: Unitary convolutions for learning on graphs and groups
    date: Oct 7, 2024
    date_iso: '2024-10-07'
    date_display: Oct 2024
    codebase_url: https://github.com/Weber-GeoML/Unitary_Convolutions
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9427
    - null
    metric_stds:
    - 0.0058
    - null
  - model: UniGCN
    model_plain: UniGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_iso: '2026-05-13'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9427
    - null
    metric_stds:
    - 0.0058
    - null
  - model: BGRL-ECG-GAT-sep
    model_plain: BGRL-ECG-GAT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9424
    - null
    metric_stds:
    - 0.0015
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
    - 0.9412
    - null
    metric_stds:
    - 0.0042
    - null
  - model: ECG-SAGE
    model_plain: ECG-SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9411
    - null
    metric_stds:
    - 0.0007
    - null
  - model: BGRL-ECG-SAGE
    model_plain: BGRL-ECG-SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9411
    - null
    metric_stds:
    - 0.0007
    - null
  - model: MLP-ECG-SAGE
    model_plain: MLP-ECG-SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.941
    - null
    metric_stds:
    - 0.0008
    - null
  - model: PD-GNN
    model_plain: PD-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.07082'
    title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    date: Feb 14, 2022
    date_iso: '2022-02-14'
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
    - 0.9403
    - null
    metric_stds:
    - 0.0045
    - null
  - model: MLPBGRL-ECG-SAGE
    model_plain: MLPBGRL-ECG-SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9401
    - null
    metric_stds:
    - 0.0007
    - null
  - model: CDE-GraphBel
    model_plain: CDE-GraphBel
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.16780'
    title: Graph Neural Convection-Diffusion with Heterophily
    date: May 26, 2023
    date_iso: '2023-05-26'
    date_display: May 2023
    codebase_url: https://github.com/zknus/Graph-Diffusion-CDE
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9398
    - null
    metric_stds:
    - 0.0057
    - null
  - model: MLP->GNN-ECG-GAT-sep
    model_plain: MLP->GNN-ECG-GAT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9397
    - null
    metric_stds:
    - 0.0019
    - null
  - model: GAT-sep
    model_plain: GAT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9391
    - null
    metric_stds:
    - 0.0035
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
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_iso: '2025-10-24'
    date_display: Oct 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9391
    - null
    metric_stds:
    - 0.0035
    - null
  - model: MLP->GNN-ECG-SAGE
    model_plain: MLP->GNN-ECG-SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9377
    - null
    metric_stds:
    - 0.0012
    - null
  - model: ECG-GT-sep
    model_plain: ECG-GT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9362
    - null
    metric_stds:
    - 0.0027
    - null
  - model: MLP-ECG-GT-sep
    model_plain: MLP-ECG-GT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9362
    - null
    metric_stds:
    - 0.0027
    - null
  - model: BGRL-ECG-GT-sep
    model_plain: BGRL-ECG-GT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9355
    - null
    metric_stds:
    - 0.0018
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
    arxiv_id: '2305.16780'
    title: Graph Neural Convection-Diffusion with Heterophily
    date: May 26, 2023
    date_iso: '2023-05-26'
    date_display: May 2023
    codebase_url: https://github.com/zknus/Graph-Diffusion-CDE
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9353
    - null
    metric_stds:
    - 0.005
    - null
  - model: MLPBGRL-GT-sep
    model_plain: MLPBGRL-GT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9352
    - null
    metric_stds:
    - 0.0025
    - null
  - model: GraphGPS + Wideformer
    model_plain: GraphGPS + Wideformer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_iso: '2025-10-24'
    date_display: Oct 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9352
    - null
    metric_stds:
    - 0.0007
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
    arxiv_id: '2202.07082'
    title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    date: Feb 14, 2022
    date_iso: '2022-02-14'
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
    - 0.9351
    - null
    metric_stds:
    - 0.0057
    - null
  - model: GraphGPS+Entropy Reg
    model_plain: GraphGPS+Entropy Reg
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_iso: '2025-10-24'
    date_display: Oct 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9335
    - null
    metric_stds:
    - 0.0023
    - null
  - model: GraphGPS
    model_plain: GraphGPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_iso: '2025-10-24'
    date_display: Oct 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9326
    - null
    metric_stds:
    - 0.001
    - null
  - model: MLP->GNN-ECG-GT-sep
    model_plain: MLP->GNN-ECG-GT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9269
    - null
    metric_stds:
    - 0.0034
    - null
  - model: ECG-GCN
    model_plain: ECG-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9263
    - null
    metric_stds:
    - 0.001
    - null
  - model: MLP-ECG-GCN
    model_plain: MLP-ECG-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9263
    - null
    metric_stds:
    - 0.001
    - null
  - model: MLP->GNN-ECG-GCN
    model_plain: MLP->GNN-ECG-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9256
    - null
    metric_stds:
    - 0.0023
    - null
  - model: MLPBGRL-ECG-GCN
    model_plain: MLPBGRL-ECG-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9247
    - null
    metric_stds:
    - 0.005
    - null
  - model: BGRL-ECG-GCN
    model_plain: BGRL-ECG-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: Jun 22, 2023
    date_iso: '2023-06-22'
    date_display: Jun 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9235
    - null
    metric_stds:
    - 0.001
    - null
  row_count: 274
  rows_json: /data/datasets/minesweeper/standard-split-rows.json
  chart_json: /data/datasets/minesweeper/standard-split-chart.json
  arch_counts:
    gnn: 163
    hybrid: 40
    graph_transformer: 38
    llm: 0
    walk: 0
    traditional: 11
  metric_counts:
  - 179
  - 95
  milestones: &id001
  - value: 0.9403
    std: 0.0045
    model: PD-GNN
    arxiv_id: '2202.07082'
    title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    date: '2022-02-14'
  - value: 0.955
    std: 0.0523
    model: CDE-GRAND-GAT
    arxiv_id: '2305.16780'
    title: Graph Neural Convection-Diffusion with Heterophily
    date: '2023-05-26'
  - value: 0.9746
    std: 0.0036
    model: Polynormer-r
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: '2024-03-02'
  - value: 0.9899
    std: 0.0016
    model: BuNN
    arxiv_id: '2405.15540'
    title: Bundle Neural Networks for message diffusion on graphs
    date: '2024-05-24'
  milestones_by_metric:
    ROC-AUC: *id001
    Accuracy:
    - value: 0.8872
      std: 0.0052
      model: GCN
      arxiv_id: '2407.11596'
      title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
      date: '2024-06-30'
    - value: 0.9478
      std: 0.0064
      model: MSH-GNN
      arxiv_id: '2505.15015'
      title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
      date: '2025-05-21'
    - value: 0.9792
      std: 0.0028
      model: NT*
      arxiv_id: '2604.08980'
      title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
        Graph Learning'
      date: '2026-04-10'
    - value: 0.9903
      std: 0.0019
      model: GraphTARIF
      arxiv_id: '2605.20248'
      title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
        Classification'
      date: '2026-05-18'
---

