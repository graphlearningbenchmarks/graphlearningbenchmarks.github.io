---
title: Questions
slug: questions
benchmark: Heterophily Benchmark
task_type: node_classification
short_description: Yandex Q&A expert network binary node classification from the heterophilic
  benchmark.
description: '**Binary node classification** Yandex Q&A expert network binary node
  classification from the heterophilic benchmark. Uses the corrected benchmark features
  and ten official splits. Low homophily and class imbalance make split and metric
  choice important. Evaluated by ROC-AUC.'
detailed_description:
  task: Yandex Q&A expert network binary node classification from the heterophilic
    benchmark. The primary catalog metric is ROC-AUC.
  data: Yandex Q&A expert network binary node classification from the heterophilic
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
- title: PyTorch Geometric Questions loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.HeterophilousGraphDataset.html
  kind: implementation_documentation
primary_metric: ROC-AUC
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.HeterophilousGraphDataset.html
stats: null
result_count: 265
best_model:
  model: UniGAP
  value: 0.8421
  metric: ROC-AUC
  arxiv_id: '2407.19420'
  paper_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
    Over-Smoothing in Node Classification Tasks'
papers:
- arxiv_id: '2606.05046'
  title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for Structure-Aware
    Graph Machine Learning'
  date_iso: '2026-06-03'
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
- arxiv_id: '2605.11749'
  title: Learning Feature Encoder with Synthetic Anomalies for Weakly Supervised Graph
    Anomaly Detection
  date_iso: '2026-04-01'
  venue: ''
- arxiv_id: '2603.26178'
  title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
    Learning via Ricci Flow'
  date_iso: '2026-03-27'
  venue: ''
- arxiv_id: '2512.12642'
  title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural Networks'
  date_iso: '2025-12-14'
  venue: ''
- arxiv_id: '2510.21267'
  title: Relieving the Over-Aggregating Effect in Graph Transformers
  date_iso: '2025-10-24'
  venue: NeurIPS 2025
- arxiv_id: '2509.21489'
  title: 'GraphPFN: A Prior-Data Fitted Graph Foundation Model'
  date_iso: '2025-09-25'
  venue: ''
- arxiv_id: '2508.20906'
  title: Turning Tabular Foundation Models into Graph Foundation Models
  date_iso: '2025-08-28'
  venue: ''
- arxiv_id: '2508.17531'
  title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
  date_iso: '2025-08-24'
  venue: ''
- arxiv_id: '2506.19343'
  title: Discrepancy-Aware Graph Mask Auto-Encoder
  date_iso: '2025-06-24'
  venue: KDD 2025
- arxiv_id: '2506.15448'
  title: Semi-supervised Graph Anomaly Detection via Robust Homophily Learning
  date_iso: '2025-06-18'
  venue: NeurIPS 2025
- arxiv_id: '2506.14291'
  title: 'Equivariance Everywhere All At Once: A Recipe for Graph Foundation Models'
  date_iso: '2025-06-17'
  venue: ''
- arxiv_id: '2504.19785'
  title: Heterophily-informed Message Passing
  date_iso: '2025-04-28'
  venue: TMLR 2025
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
- arxiv_id: '2410.02158'
  title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation Learning'
  date_iso: '2024-10-03'
  venue: TMLR 2024
- arxiv_id: '2409.05755'
  title: Re-evaluating the Advancements of Heterophilic Graph Learning
  date_iso: '2024-09-09'
  venue: ''
- arxiv_id: '2408.07191'
  title: Joint Graph Rewiring and Feature Denoising via Spectral Resonance
  date_iso: '2024-08-13'
  venue: ICLR 2024
- arxiv_id: '2407.19420'
  title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate Over-Smoothing
    in Node Classification Tasks'
  date_iso: '2024-07-28'
  venue: ''
- arxiv_id: '2405.20445'
  title: Fully-inductive Node Classification on Arbitrary Graphs
  date_iso: '2024-05-30'
  venue: ICLR 2024
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
- arxiv_id: '2312.17679'
  title: Data Augmentation for Supervised Graph Outlier Detection via Latent Diffusion
    Models
  date_iso: '2023-12-29'
  venue: LoG 2023
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
  - Average Precision
  - macro-F1
  metric_display_names:
  - ROC-AUC
  - Accuracy
  - Average Precision
  - macro-F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: UniGAP
    model_plain: UniGAP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_iso: '2024-07-28'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8421
    - null
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
    - null
  - model: H2GCN + AdaEdge
    model_plain: H2GCN + AdaEdge
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_iso: '2024-07-28'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8134
    - null
    - null
    - null
    metric_stds:
    - 0.007
    - null
    - null
    - null
  - model: GCN +AdaEdge
    model_plain: GCN +AdaEdge
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_iso: '2024-07-28'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8085
    - null
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
    - null
  - model: GraphSAGE + AdaEdge
    model_plain: GraphSAGE + AdaEdge
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_iso: '2024-07-28'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8017
    - null
    - null
    - null
    metric_stds:
    - 0.01
    - null
    - null
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
    - 0.8014
    - null
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
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
    - 0.8001
    - null
    - null
    - null
    metric_stds:
    - 0.0043
    - null
    - null
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
    - 0.8001
    - null
    - null
    - null
    metric_stds:
    - 0.0043
    - null
    - null
    - null
  - model: GCN + HalfHop
    model_plain: GCN + HalfHop
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_iso: '2024-07-28'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.796
    - null
    - null
    - null
    metric_stds:
    - 0.011
    - null
    - null
    - null
  - model: H2GCN
    model_plain: H2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_iso: '2024-07-28'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7928
    - null
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
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
    - 0.7921
    - null
    - null
    - null
    metric_stds:
    - 0.0079
    - null
    - null
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
    - 0.7921
    - null
    - null
    - null
    metric_stds:
    - 0.0079
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
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_iso: '2024-07-28'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7902
    - null
    - null
    - null
    metric_stds:
    - 0.006
    - null
    - null
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
    - 0.79
    - null
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
    - null
  - model: H2GCN + HalfHop
    model_plain: H2GCN + HalfHop
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_iso: '2024-07-28'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7896
    - null
    - null
    - null
    metric_stds:
    - 0.019
    - null
    - null
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
    - 0.7896
    - null
    - null
    - null
    metric_stds:
    - 0.006
    - null
    - null
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
    - 0.7892
    - null
    - null
    - null
    metric_stds:
    - 0.0089
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
    - 0.7886
    - null
    - null
    - null
    metric_stds:
    - 0.0092
    - null
    - null
    - null
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7875
    - null
    - null
    - null
    metric_stds:
    - 0.0109
    - null
    - null
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
    - 0.7869
    - null
    - null
    - null
    metric_stds:
    - 0.0024
    - null
    - null
    - null
  - model: GraphSAGE + HalfHop
    model_plain: GraphSAGE + HalfHop
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_iso: '2024-07-28'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7862
    - null
    - null
    - null
    metric_stds:
    - 0.017
    - null
    - null
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
    - 0.7812
    - null
    - null
    - null
    metric_stds:
    - 0.0032
    - null
    - null
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
    - 0.7812
    - null
    - null
    - null
    metric_stds:
    - 0.0032
    - null
    - null
    - null
  - model: GT-sep
    model_plain: GT-sep
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    - 0.7805
    - null
    - null
    - null
    metric_stds:
    - 0.0093
    - null
    - null
    - null
  - model: Graphtransformer
    model_plain: Graphtransformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    - 0.7795
    - null
    - null
    - null
    metric_stds:
    - 0.0068
    - null
    - null
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
    - 0.7795
    - null
    - null
    - null
    metric_stds:
    - 0.0106
    - null
    - null
    - null
  - model: GT
    model_plain: GT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7795
    - null
    - null
    - null
    metric_stds:
    - 0.0068
    - null
    - null
    - null
  - model: DGMAE
    model_plain: DGMAE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2506.19343'
    title: Discrepancy-Aware Graph Mask Auto-Encoder
    date: Jun 24, 2025
    date_iso: '2025-06-24'
    date_display: Jun 2025
    codebase_url: https://github.com/zhengziyu77/DGMAE
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7793
    - null
    - null
    - null
    metric_stds:
    - 0.0098
    - null
    - null
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
    - 0.7785
    - null
    - null
    - null
    metric_stds:
    - 0.0045
    - null
    - null
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
    - 0.7782
    - null
    - null
    - null
    metric_stds:
    - 0.0043
    - null
    - null
    - null
  - model: GCN+JDR
    model_plain: GCN+JDR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2408.07191'
    title: Joint Graph Rewiring and Feature Denoising via Spectral Resonance
    date: Aug 13, 2024
    date_iso: '2024-08-13'
    date_display: Aug 2024
    codebase_url: https://github.com/jlinki/JDR
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7752
    - null
    - null
    - null
    metric_stds:
    - 0.0063
    - null
    - null
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
    - 0.775
    - null
    - null
    - null
    metric_stds:
    - 0.0035
    - null
    - null
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
    - 0.775
    - null
    - null
    - null
    metric_stds:
    - 0.0035
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
    - 0.7743
    - null
    - null
    - null
    metric_stds:
    - 0.012
    - null
    - null
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
    - 0.7738
    - null
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
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
    - 0.7738
    - null
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
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
    - 0.7732
    - null
    - null
    - null
    metric_stds:
    - 0.0031
    - null
    - null
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
    - 0.773
    - null
    - null
    - null
    metric_stds:
    - 0.0047
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
    - 0.7724
    - null
    - null
    - null
    metric_stds:
    - 0.0126
    - null
    - null
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
    - 0.7723
    - null
    - null
    - null
    metric_stds:
    - 0.0036
    - null
    - null
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
    - 0.7723
    - null
    - null
    - null
    metric_stds:
    - 0.0036
    - null
    - null
    - null
  - model: GPS GAT+Performer
    model_plain: GPS GAT+Performer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.7714
    - null
    - null
    - null
    metric_stds:
    - 0.0149
    - null
    - null
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
    - 0.7697
    - null
    - null
    - null
    metric_stds:
    - 0.0045
    - null
    - null
    - null
  - model: SGFormer + Wideformer
    model_plain: SGFormer + Wideformer
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
    - 0.7694
    - null
    - null
    - null
    metric_stds:
    - 0.0005
    - null
    - null
    - null
  - model: GODM
    model_plain: GODM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.17679'
    title: Data Augmentation for Supervised Graph Outlier Detection via Latent Diffusion
      Models
    date: Dec 29, 2023
    date_iso: '2023-12-29'
    date_display: Dec 2023
    codebase_url: https://github.com/kayzliu/godm
    published_conference: LoG 2023
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7684
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: SGFormer + Entropy Reg
    model_plain: SGFormer + Entropy Reg
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
    - 0.7683
    - null
    - null
    - null
    metric_stds:
    - 0.0018
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
    - 0.7681
    - null
    - null
    - null
    metric_stds:
    - 0.0009
    - null
    - null
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
    - 0.7679
    - null
    - null
    - null
    metric_stds:
    - 0.0071
    - null
    - null
    - null
  - model: Gumbel-MPNN
    model_plain: Gumbel-MPNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.17531'
    title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    date: Aug 24, 2025
    date_iso: '2025-08-24'
    date_display: Aug 2025
    codebase_url: https://github.com/Bobowner/Gumbel-Softmax-MPNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7661
    - null
    - null
    - null
    metric_stds:
    - 0.0012
    - null
    - null
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
    - 0.7655
    - null
    - null
    - null
    metric_stds:
    - 0.0033
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
    - 0.7644
    - null
    - null
    - null
    metric_stds:
    - 0.0062
    - null
    - null
    - null
  row_count: 265
  rows_json: /data/datasets/questions/standard-split-rows.json
  chart_json: /data/datasets/questions/standard-split-chart.json
  arch_counts:
    gnn: 154
    hybrid: 34
    graph_transformer: 32
    llm: 10
    walk: 0
    traditional: 11
  metric_counts:
  - 198
  - 68
  - 12
  - 14
  milestones: &id001
  - value: 0.7886
    std: 0.0092
    model: FSGNN
    arxiv_id: '2306.12943'
    title: Evolving Computation Graphs
    date: '2023-06-22'
  - value: 0.7892
    std: 0.0089
    model: Polynormer-r
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: '2024-03-02'
  - value: 0.7896
    std: 0.006
    model: DC-GNN
    arxiv_id: '2405.16185'
    title: Differentiable Cluster Graph Neural Network
    date: '2024-05-25'
  - value: 0.8421
    std: 0.008
    model: UniGAP
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: '2024-07-28'
  milestones_by_metric:
    ROC-AUC: *id001
    Accuracy:
    - value: 0.9727
      std: null
      model: AGS-GNN
      arxiv_id: '2202.07082'
      title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
      date: '2022-02-14'
    - value: 0.9733
      std: null
      model: MLP
      arxiv_id: '2405.20445'
      title: Fully-inductive Node Classification on Arbitrary Graphs
      date: '2024-05-30'
    Average Precision:
    - value: 0.2276
      std: 0.0055
      model: GraphPFN
      arxiv_id: '2509.21489'
      title: 'GraphPFN: A Prior-Data Fitted Graph Foundation Model'
      date: '2025-09-25'
    macro-F1:
    - value: 0.543
      std: null
      model: CR-TAS
      arxiv_id: '2606.05046'
      title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for Structure-Aware
        Graph Machine Learning'
      date: '2026-06-03'
---

