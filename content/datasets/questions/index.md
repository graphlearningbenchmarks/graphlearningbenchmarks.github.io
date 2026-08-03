---
title: Questions
slug: questions
benchmark: Heterophilic Graphs
task_type: node_classification
description: Yandex Q&A expert network binary node classification from the heterophilic
  benchmark.
primary_metric: ROC-AUC
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.HeterophilousGraphDataset.html
stats: null
result_count: 266
best_model:
  model: MLP
  value: 0.9733
  metric: ROC-AUC
  arxiv_id: '2405.20445'
  paper_title: Fully-inductive Node Classification on Arbitrary Graphs
papers:
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
- arxiv_id: '2506.15448'
  title: Semi-supervised Graph Anomaly Detection via Robust Homophily Learning
  date_iso: '2025-06-18'
  venue: NeurIPS 2025
- arxiv_id: '2506.14291'
  title: 'Equivariance Everywhere All At Once: A Recipe for Graph Foundation Models'
  date_iso: '2025-06-17'
  venue: ''
- arxiv_id: '2505.14033'
  title: 'Partition-wise Graph Filtering: A Unified Perspective Through the Lens of
    Graph Coarsening'
  date_iso: '2025-05-20'
  venue: KDD 2025
- arxiv_id: '2504.19785'
  title: Heterophily-informed Message Passing
  date_iso: '2025-04-28'
  venue: TMLR 2025
- arxiv_id: '2411.16278'
  title: Even Sparser Graph Transformers
  date_iso: '2024-11-25'
  venue: NeurIPS 2024
- arxiv_id: '2411.06427'
  title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
  date_iso: '2024-11-10'
  venue: NeurIPS 2024
- arxiv_id: '2411.05274'
  title: Distributed-Order Fractional Graph Operating Network
  date_iso: '2024-11-08'
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
- arxiv_id: '2404.17099'
  title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
    with FROND
  date_iso: '2024-04-26'
  venue: ICLR 2024
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
  metric_display_names:
  - ROC-AUC
  - Accuracy
  - Average Precision
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9733
    - null
    - null
    metric_stds:
    - 0.0006
    - null
    - null
  - model: AGS-GNN
    model_plain: AGS-GNN
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9727
    - null
    - null
    metric_stds:
    - 0.0004
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
    - 0.9715
    - null
    - null
    metric_stds:
    - 0.0004
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
    - 0.9711
    - null
    - null
    metric_stds:
    - 0.0002
    - null
    - null
  - model: GraphAny
    model_plain: GraphAny
    is_baseline: false
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
    - 0.971
    - null
    - null
    metric_stds:
    - 0.0001
    - null
    - null
  - model: LINKX
    model_plain: LINKX
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
    - 0.9706
    - null
    - null
    metric_stds:
    - 0.0003
    - null
    - null
  - model: ACM-GCN
    model_plain: ACM-GCN
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9702
    - null
    - null
    metric_stds:
    - 0.0167
    - null
    - null
  - model: BWGNN
    model_plain: BWGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06427'
    title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    date: Nov 10, 2024
    date_iso: '2024-11-10'
    date_display: Nov 2024
    codebase_url: https://github.com/lllyyq1121/UniGAD
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9603
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: AMNet
    model_plain: AMNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06427'
    title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    date: Nov 10, 2024
    date_iso: '2024-11-10'
    date_display: Nov 2024
    codebase_url: https://github.com/lllyyq1121/UniGAD
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9358
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: BernNet
    model_plain: BernNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06427'
    title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    date: Nov 10, 2024
    date_iso: '2024-11-10'
    date_display: Nov 2024
    codebase_url: https://github.com/lllyyq1121/UniGAD
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9237
    - null
    - null
    metric_stds:
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
    arxiv_id: '2411.06427'
    title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    date: Nov 10, 2024
    date_iso: '2024-11-10'
    date_display: Nov 2024
    codebase_url: https://github.com/lllyyq1121/UniGAD
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.906
    - null
    - null
    metric_stds:
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
    arxiv_id: '2411.06427'
    title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    date: Nov 10, 2024
    date_iso: '2024-11-10'
    date_display: Nov 2024
    codebase_url: https://github.com/lllyyq1121/UniGAD
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8643
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GraphSAGE + UniGAP
    model_plain: GraphSAGE + UniGAP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.8421
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
  - model: H2GCN + UniGAP
    model_plain: H2GCN + UniGAP
    is_baseline: false
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
    - 0.8359
    - null
    - null
    metric_stds:
    - 0.007
    - null
    - null
  - model: GCN + UniGAP
    model_plain: GCN + UniGAP
    is_baseline: false
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
    - 0.8273
    - null
    - null
    metric_stds:
    - 0.009
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
    metric_stds:
    - 0.007
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
    metric_stds:
    - 0.008
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
    metric_stds:
    - 0.01
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
    metric_stds:
    - 0.011
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
    metric_stds:
    - 0.008
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
    metric_stds:
    - 0.006
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
    metric_stds:
    - 0.002
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
    metric_stds:
    - 0.019
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
    metric_stds:
    - 0.006
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
    - 0.7892
    - null
    metric_stds:
    - 0.0089
    - 0.0089
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
    - 0.7888
    - null
    - null
    metric_stds:
    - 0.0094
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
    metric_stds:
    - 0.0092
    - null
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
    - 0.788
    - null
    - null
    metric_stds:
    - 0.011
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
    metric_stds:
    - 0.017
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
    arxiv_id: '2411.06427'
    title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    date: Nov 10, 2024
    date_iso: '2024-11-10'
    date_display: Nov 2024
    codebase_url: https://github.com/lllyyq1121/UniGAD
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7816
    - null
    - null
    metric_stds:
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
    metric_stds:
    - 0.0032
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
    metric_stds:
    - 0.0032
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
    metric_stds:
    - 0.0093
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
    - 0.7795
    - null
    metric_stds:
    - 0.0106
    - 0.0106
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
    metric_stds:
    - 0.0068
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
    - 0.7795
    - null
    - null
    metric_stds:
    - 0.0068
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
    metric_stds:
    - 0.0045
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
    metric_stds:
    - 0.0043
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
    metric_stds:
    - 0.0063
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
    metric_stds:
    - 0.0035
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
    metric_stds:
    - 0.0035
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
    - 0.7743
    - null
    - null
    metric_stds:
    - 0.012
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
    metric_stds:
    - 0.0018
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
    metric_stds:
    - 0.0018
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
    metric_stds:
    - 0.0031
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
    metric_stds:
    - 0.0047
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
    metric_stds:
    - 0.0126
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
    metric_stds:
    - 0.0036
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
    metric_stds:
    - 0.0036
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
    metric_stds:
    - 0.0149
    - null
    - null
  row_count: 266
  rows_json: /data/datasets/questions/standard-split-rows.json
  chart_json: /data/datasets/questions/standard-split-chart.json
  arch_counts:
    gnn: 172
    hybrid: 32
    graph_transformer: 19
    llm: 10
    walk: 0
    traditional: 12
  metric_counts:
  - 207
  - 49
  - 12
  milestones: &id001
  - value: 0.9727
    std: 0.0004
    model: AGS-GNN
    arxiv_id: '2202.07082'
    title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    date: '2022-02-14'
  - value: 0.9733
    std: 0.0006
    model: MLP
    arxiv_id: '2405.20445'
    title: Fully-inductive Node Classification on Arbitrary Graphs
    date: '2024-05-30'
  milestones_by_metric:
    ROC-AUC: *id001
    Accuracy:
    - value: 0.7517
      std: 0.0099
      model: CDE-GRAND-GAT
      arxiv_id: '2305.16780'
      title: Graph Neural Convection-Diffusion with Heterophily
      date: '2023-05-26'
    - value: 0.7892
      std: 0.0089
      model: Polynormer-r
      arxiv_id: '2403.01232'
      title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
      date: '2024-03-02'
    - value: 0.9716
      std: 0.0006
      model: MeanGNN
      arxiv_id: '2506.14291'
      title: 'Equivariance Everywhere All At Once: A Recipe for Graph Foundation Models'
      date: '2025-06-17'
    - value: 0.9733
      std: 0.0006
      model: MLP
      arxiv_id: '2604.19028'
      title: Learning Posterior Predictive Distributions for Node Classification from
        Synthetic Graph Priors
      date: '2026-04-21'
    Average Precision:
    - value: 0.2276
      std: 0.0055
      model: GraphPFN
      arxiv_id: '2509.21489'
      title: 'GraphPFN: A Prior-Data Fitted Graph Foundation Model'
      date: '2025-09-25'
---

