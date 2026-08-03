---
title: PPI
slug: ppi
benchmark: Classic
task_type: node_classification
description: Protein-protein interaction node classification (121 GO labels, multi-label).
primary_metric: F1
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.PPI.html
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 121
result_count: 290
best_model:
  model: GAMLP(JK)
  value: 0.9982
  metric: F1
  arxiv_id: '2206.04355'
  paper_title: Graph Attention Multi-Layer Perceptron
papers:
- arxiv_id: '2603.16849'
  title: 'GIST: Gauge-Invariant Spectral Transformers for Scalable Graph Neural Operators'
  date_iso: '2026-03-17'
  venue: ''
- arxiv_id: '2505.02020'
  title: Wide & Deep Learning for Node Classification
  date_iso: '2025-05-04'
  venue: ''
- arxiv_id: '2502.13555'
  title: Democratizing Large Language Model-Based Graph Data Augmentation via Latent
    Knowledge Graphs
  date_iso: '2025-02-19'
  venue: ''
- arxiv_id: '2412.17961'
  title: 'Extending Graph Condensation to Multi-Label Datasets: A Benchmark Study'
  date_iso: '2024-12-23'
  venue: TMLR 2024
- arxiv_id: '2410.21043'
  title: Disentangled and Self-Explainable Node Representation Learning
  date_iso: '2024-10-28'
  venue: TMLR 2024
- arxiv_id: '2408.13471'
  title: Disentangled Generative Graph Representation Learning
  date_iso: '2024-08-24'
  venue: ''
- arxiv_id: '2402.10380'
  title: Subgraph-level Universal Prompt Tuning
  date_iso: '2024-02-16'
  venue: ''
- arxiv_id: '2402.08023'
  title: 'UGMAE: A Unified Framework for Graph Masked Autoencoders'
  date_iso: '2024-02-12'
  venue: ''
- arxiv_id: '2402.07225'
  title: Rethinking Graph Masked Autoencoders through Alignment and Uniformity
  date_iso: '2024-02-11'
  venue: AAAI 2024
- arxiv_id: '2307.00534'
  title: Shared Growth of Graph Neural Networks via Prompted Free-direction Knowledge
    Distillation
  date_iso: '2023-07-02'
  venue: ''
- arxiv_id: '2302.00924'
  title: 'LMC: Fast Training of GNNs via subgraph-wise sampling with Provable Convergence'
  date_iso: '2023-02-02'
  venue: ICLR 2023
- arxiv_id: '2301.12063'
  title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical Adaptive
    Masking and Trainable Corruption'
  date_iso: '2023-01-28'
  venue: ''
- arxiv_id: '2208.10493'
  title: Relational Self-Supervised Learning on Graphs
  date_iso: '2022-08-21'
  venue: ''
- arxiv_id: '2207.12600'
  title: Learning Hierarchical Protein Representations via Complete 3D Graph Networks
  date_iso: '2022-07-26'
  venue: ICLR 2022
- arxiv_id: '2207.11996'
  title: Generative Subgraph Contrast for Self-Supervised Graph Representation Learning
  date_iso: '2022-07-25'
  venue: ''
- arxiv_id: '2206.14418'
  title: Optimization-Induced Graph Implicit Nonlinear Diffusion
  date_iso: '2022-06-29'
  venue: ICML 2022
- arxiv_id: '2206.06561'
  title: 'FreeKD: Free-direction Knowledge Distillation for Graph Neural Networks'
  date_iso: '2022-06-14'
  venue: KDD 2022
- arxiv_id: '2206.04355'
  title: Graph Attention Multi-Layer Perceptron
  date_iso: '2022-06-09'
  venue: KDD 2022
- arxiv_id: '2205.10803'
  title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
  date_iso: '2022-05-22'
  venue: KDD 2022
- arxiv_id: '2202.08333'
  title: Self-Supervised Representation Learning via Latent Graph Prediction
  date_iso: '2022-02-16'
  venue: ICML 2022
- arxiv_id: '2202.02296'
  title: Graph-Coupled Oscillator Networks
  date_iso: '2022-02-04'
  venue: ICML 2022
- arxiv_id: '2201.13410'
  title: 'Weisfeiler and Leman Go Infinite: Spectral and Combinatorial Pre-Colorings'
  date_iso: '2022-01-31'
  venue: TMLR 2022
- arxiv_id: '2201.12843'
  title: Graph Representation Learning via Aggregation Enhancement
  date_iso: '2022-01-30'
  venue: ''
- arxiv_id: '2201.01702'
  title: 'Bringing Your Own View: Graph Contrastive Learning without Prefabricated
    Data Augmentations'
  date_iso: '2022-01-04'
  venue: ''
- arxiv_id: '2111.04964'
  title: On Representation Knowledge Distillation for Graph Neural Networks
  date_iso: '2021-11-09'
  venue: ''
- arxiv_id: '2110.14363'
  title: 'VQ-GNN: A Universal Framework to Scale-up Graph Neural Networks using Vector
    Quantization'
  date_iso: '2021-10-27'
  venue: NeurIPS 2021
- arxiv_id: '2109.12872'
  title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph Neural Networks'
  date_iso: '2021-09-27'
  venue: ''
- arxiv_id: '2106.02466'
  title: 'Graph Barlow Twins: A self-supervised representation learning framework
    for graphs'
  date_iso: '2021-06-04'
  venue: ''
- arxiv_id: '2104.09376'
  title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced Training
  date_iso: '2021-04-19'
  venue: ''
- arxiv_id: '2104.06608'
  title: Search to aggregate neighborhood for graph neural network
  date_iso: '2021-04-01'
  venue: ''
- arxiv_id: '2103.00959'
  title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
  date_iso: '2021-03-01'
  venue: WWW 2021
- arxiv_id: '2103.00111'
  title: 'Graph Self-Supervised Learning: A Survey'
  date_iso: '2021-02-27'
  venue: ''
- arxiv_id: '2102.06514'
  title: Large-Scale Representation Learning on Graphs via Bootstrapping
  date_iso: '2021-02-12'
  venue: ICLR 2021
- arxiv_id: '2011.07057'
  title: 'Learning to Drop: Robust Graph Neural Network via Topological Denoising'
  date_iso: '2020-11-13'
  venue: ''
- arxiv_id: '2009.10273'
  title: Sub-graph Contrast for Scalable Self-Supervised Graph Representation Learning
  date_iso: '2020-09-22'
  venue: ''
- arxiv_id: '2009.03717'
  title: Hierarchical message-passing graph neural networks
  date_iso: '2020-09-08'
  venue: ''
- arxiv_id: '2007.02133'
  title: Simple and Deep Graph Convolutional Networks
  date_iso: '2020-07-04'
  venue: ICML 2020
- arxiv_id: '2006.04131'
  title: Deep Graph Contrastive Representation Learning
  date_iso: '2020-06-07'
  venue: ''
- arxiv_id: '2004.11198'
  title: 'SIGN: Scalable Inception Graph Neural Networks'
  date_iso: '2020-04-23'
  venue: ''
- arxiv_id: '2003.13606'
  title: 'L$^2$-GCN: Layer-Wise and Learned Efficient Training of Graph Convolutional
    Networks'
  date_iso: '2020-03-30'
  venue: ''
- arxiv_id: '2003.10477'
  title: Distilling Knowledge from Graph Convolutional Networks
  date_iso: '2020-03-23'
  venue: ''
- arxiv_id: '2002.01169'
  title: Graph Representation Learning via Graphical Mutual Information Maximization
  date_iso: '2020-02-04'
  venue: WWW 2020
- arxiv_id: '1910.06849'
  title: 'DeepGCNs: Making GCNs Go as Deep as CNNs'
  date_iso: '2019-10-15'
  venue: ''
- arxiv_id: '1910.02370'
  title: 'GraphZoom: A Multi-level Spectral Approach for Accurate and Scalable Graph
    Embedding'
  date_iso: '2019-10-06'
  venue: ICLR 2019
- arxiv_id: '1909.03184'
  title: 'Auto-GNN: Neural Architecture Search of Graph Neural Networks'
  date_iso: '2019-09-07'
  venue: ''
- arxiv_id: '1907.04931'
  title: 'GraphSAINT: mpling Based ductive Learning Me hod'
  date_iso: '2019-07-10'
  venue: ICLR 2019
- arxiv_id: '1905.09550'
  title: 'Revisiting Graph Neural Networks: All We Have is Low-Pass Filters'
  date_iso: '2019-05-23'
  venue: ''
- arxiv_id: '1905.07953'
  title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph Convolutional
    Networks'
  date_iso: '2019-05-20'
  venue: KDD 2019
- arxiv_id: '1812.04202'
  title: 'Deep Learning on Graphs: A Survey'
  date_iso: '2018-12-11'
  venue: ''
- arxiv_id: '1803.07294'
  title: 'GaAN: Gated Attention Networks for Learning on Large and Spatiotemporal
    Graphs'
  date_iso: '2018-03-20'
  venue: ''
- arxiv_id: '1710.03059'
  title: Learning Graph Representations with Embedding Propagation
  date_iso: '2017-10-09'
  venue: NeurIPS 2017
- arxiv_id: '1706.02216'
  title: Inductive Representation Learning on Large Graphs
  date_iso: '2017-06-07'
  venue: NeurIPS 2017
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: F1
  default_metric: F1
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: 121
  metrics:
  - F1
  - AUROC
  - Accuracy
  - Overlap Consistency
  - ROC-AUC
  - Topological Alignment
  metric_display_names:
  - F1
  - AUROC
  - Accuracy
  - Overlap Consistency
  - ROC-AUC
  - Topological Alignment
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9982
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
  - model: GraphCON-GCN
    model_plain: GraphCON-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/tk-rusch/GraphCON
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.996
    - null
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
    - null
  - model: GCNII
    model_plain: GCNII*
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2007.02133'
    title: Simple and Deep Graph Convolutional Networks
    date: Jul 4, 2020
    date_iso: '2020-07-04'
    date_display: Jul 2020
    codebase_url: https://github.com/DropEdge/DropEdge
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9956
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.02
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
    arxiv_id: '2302.00924'
    title: 'LMC: Fast Training of GNNs via subgraph-wise sampling with Provable Convergence'
    date: Feb 2, 2023
    date_iso: '2023-02-02'
    date_display: Feb 2023
    codebase_url: https://github.com/MIRALab-USTC/GNN-LMC
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.995
    - null
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
    - null
  - model: GIST
    model_plain: GIST
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.16849'
    title: 'GIST: Gauge-Invariant Spectral Transformers for Scalable Graph Neural
      Operators'
    date: Mar 17, 2026
    date_iso: '2026-03-17'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.995
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0003
    - null
    - null
    - null
    - null
    - null
  - model: GCNIII
    model_plain: GCNIII
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.02020'
    title: Wide & Deep Learning for Node Classification
    date: May 4, 2025
    date_iso: '2025-05-04'
    date_display: May 2025
    codebase_url: https://github.com/CYCUCAS/GCNIII
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.995
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.03
    - null
    - null
    - null
    - null
    - null
  - model: DenseMRGCN-14
    model_plain: DenseMRGCN-14
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '1910.06849'
    title: 'DeepGCNs: Making GCNs Go as Deep as CNNs'
    date: Oct 15, 2019
    date_iso: '2019-10-15'
    date_display: Oct 2019
    codebase_url: https://github.com/lightaime/deep_gcns_torch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9943
    - null
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
    - null
  - model: Teacher
    model_plain: Teacher
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.06561'
    title: 'FreeKD: Free-direction Knowledge Distillation for Graph Neural Networks'
    date: Jun 14, 2022
    date_iso: '2022-06-14'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9941
    - null
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
    - null
  - model: ResMRGCN-28
    model_plain: ResMRGCN-28
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '1910.06849'
    title: 'DeepGCNs: Making GCNs Go as Deep as CNNs'
    date: Oct 15, 2019
    date_iso: '2019-10-15'
    date_display: Oct 2019
    codebase_url: https://github.com/lightaime/deep_gcns_torch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9941
    - null
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
    - null
  - model: Cluster-GCN
    model_plain: Cluster-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/tk-rusch/GraphCON
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.994
    - null
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
    - null
  - model: GraphCON-GAT
    model_plain: GraphCON-GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/tk-rusch/GraphCON
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.994
    - null
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
    - null
  - model: Cluster-GCN
    model_plain: Cluster-GCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1905.07953'
    title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph
      Convolutional Networks'
    date: May 20, 2019
    date_iso: '2019-05-20'
    date_display: May 2019
    codebase_url: https://github.com/google-research/google-research
    published_conference: KDD 2019
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2019
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9936
    - null
    - 0.9936
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GCNII (GAS)
    model_plain: GCNII (GAS)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.00924'
    title: 'LMC: Fast Training of GNNs via subgraph-wise sampling with Provable Convergence'
    date: Feb 2, 2023
    date_iso: '2023-02-02'
    date_display: Feb 2023
    codebase_url: https://github.com/MIRALab-USTC/GNN-LMC
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9936
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.02
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
    arxiv_id: '2103.00959'
    title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    date: Mar 1, 2021
    date_iso: '2021-03-01'
    date_display: Mar 2021
    codebase_url: https://github.com/THUDM/cogdl
    published_conference: WWW 2021
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2021
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.993
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
  - model: PDE-GCN
    model_plain: PDE-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/tk-rusch/GraphCON
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.992
    - null
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
    - null
  - model: AGNN-with share
    model_plain: AGNN-with share
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.37
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1909.03184'
    title: 'Auto-GNN: Neural Architecture Search of Graph Neural Networks'
    date: Sep 7, 2019
    date_iso: '2019-09-07'
    date_display: Sep 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.991
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
  - model: FreeKD-Prompt (GAT/GAT)
    model_plain: FreeKD-Prompt (GAT/GAT)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.00534'
    title: Shared Growth of Graph Neural Networks via Prompted Free-direction Knowledge
      Distillation
    date: Jul 2, 2023
    date_iso: '2023-07-02'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9896
    - null
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
    - null
  - model: FreeKD
    model_plain: FreeKD
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.06561'
    title: 'FreeKD: Free-direction Knowledge Distillation for Graph Neural Networks'
    date: Jun 14, 2022
    date_iso: '2022-06-14'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9879
    - null
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
    - null
  - model: FreeKD (GAT/GAT)
    model_plain: FreeKD (GAT/GAT)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.00534'
    title: Shared Growth of Graph Neural Networks via Prompted Free-direction Knowledge
      Distillation
    date: Jul 2, 2023
    date_iso: '2023-07-02'
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
    - 0.9879
    - null
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
    - null
  - model: GaAN
    model_plain: GaAN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1803.07294'
    title: 'GaAN: Gated Attention Networks for Learning on Large and Spatiotemporal
      Graphs'
    date: Mar 20, 2018
    date_iso: '2018-03-20'
    date_display: Mar 2018
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9871
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0002
    - null
    - null
    - null
    - null
    - null
  - model: Full Prec.
    model_plain: Full Prec.
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.12872'
    title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph Neural Networks'
    date: Sep 27, 2021
    date_iso: '2021-09-27'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.987
    - null
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
    - null
  - model: VRGCN
    model_plain: VRGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.13606'
    title: 'L$^2$-GCN: Layer-Wise and Learned Efficient Training of Graph Convolutional
      Networks'
    date: Mar 30, 2020
    date_iso: '2020-03-30'
    date_display: Mar 2020
    codebase_url: https://github.com/VITA-Group/L2-GCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.986
    - null
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
    - null
  - model: SANE
    model_plain: SANE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2104.06608'
    title: Search to aggregate neighborhood for graph neural network
    date: Apr 1, 2021
    date_iso: '2021-04-01'
    date_display: Apr 2021
    codebase_url: https://github.com/AutoML-4Paradigm/SANE
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9856
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.012
    - null
    - null
    - null
    - null
    - null
  - model: GeniePath
    model_plain: GeniePath
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1905.07953'
    title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph
      Convolutional Networks'
    date: May 20, 2019
    date_iso: '2019-05-20'
    date_display: May 2019
    codebase_url: https://github.com/google-research/google-research
    published_conference: KDD 2019
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.985
    - null
    - 0.985
    - null
    - null
    - null
    metric_stds:
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
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/tk-rusch/GraphCON
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.985
    - null
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
    - null
  - model: Attention-only
    model_plain: Attention-only
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '1803.07294'
    title: 'GaAN: Gated Attention Networks for Learning on Large and Spatiotemporal
      Graphs'
    date: Mar 20, 2018
    date_iso: '2018-03-20'
    date_display: Mar 2018
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9846
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0009
    - null
    - null
    - null
    - null
    - null
  - model: G-CRD
    model_plain: G-CRD
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.04964'
    title: On Representation Knowledge Distillation for Graph Neural Networks
    date: Nov 9, 2021
    date_iso: '2021-11-09'
    date_display: Nov 2021
    codebase_url: https://github.com/chaitjo/efficient-gnns
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9842
    - null
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
    - null
  - model: GIND
    model_plain: GIND
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.14418'
    title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: https://github.com/7qchen/GIND
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.984
    - null
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
    - null
  - model: Max pooling
    model_plain: Max pooling
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1803.07294'
    title: 'GaAN: Gated Attention Networks for Learning on Large and Spatiotemporal
      Graphs'
    date: Mar 20, 2018
    date_iso: '2018-03-20'
    date_display: Mar 2018
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9839
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
  - model: Pairwise+sigmoid
    model_plain: Pairwise+sigmoid
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1803.07294'
    title: 'GaAN: Gated Attention Networks for Learning on Large and Spatiotemporal
      Graphs'
    date: Mar 20, 2018
    date_iso: '2018-03-20'
    date_display: Mar 2018
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9839
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
  - model: Pairwise+tanh
    model_plain: Pairwise+tanh
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1803.07294'
    title: 'GaAN: Gated Attention Networks for Learning on Large and Spatiotemporal
      Graphs'
    date: Mar 20, 2018
    date_iso: '2018-03-20'
    date_display: Mar 2018
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9832
    - null
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
    - null
  - model: LSP
    model_plain: LSP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.06561'
    title: 'FreeKD: Free-direction Knowledge Distillation for Graph Neural Networks'
    date: Jun 14, 2022
    date_iso: '2022-06-14'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9825
    - null
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
    - null
  - model: GraphSAINT-EDGE
    model_plain: GraphSAINT-EDGE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1907.04931'
    title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    date: Jul 10, 2019
    date_iso: '2019-07-10'
    date_display: Jul 2019
    codebase_url: https://github.com/GraphSAINT/GraphSAINT
    published_conference: ICLR 2019
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.981
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.007
    - null
    - null
    - null
    - null
    - null
  - model: GraphSAINT-RW
    model_plain: GraphSAINT-RW
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1907.04931'
    title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    date: Jul 10, 2019
    date_iso: '2019-07-10'
    date_display: Jul 2019
    codebase_url: https://github.com/GraphSAINT/GraphSAINT
    published_conference: ICLR 2019
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.981
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.004
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
    arxiv_id: '2004.11198'
    title: 'SIGN: Scalable Inception Graph Neural Networks'
    date: Apr 23, 2020
    date_iso: '2020-04-23'
    date_display: Apr 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.981
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.004
    - null
    - null
    - null
    - null
    - null
  - model: GraphSAINT-MRW
    model_plain: GraphSAINT-MRW
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1907.04931'
    title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    date: Jul 10, 2019
    date_iso: '2019-07-10'
    date_display: Jul 2019
    codebase_url: https://github.com/GraphSAINT/GraphSAINT
    published_conference: ICLR 2019
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.98
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
  - model: EIGNN
    model_plain: EIGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.14418'
    title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: https://github.com/7qchen/GIND
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.98
    - null
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
    - 0.98
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
  - model: GAT PTDNet
    model_plain: GAT PTDNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2011.07057'
    title: 'Learning to Drop: Robust Graph Neural Network via Topological Denoising'
    date: Nov 13, 2020
    date_iso: '2020-11-13'
    date_display: Nov 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.98
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.022
    - null
    - null
    - null
    - null
    - null
  - model: Supervised Teacher
    model_plain: Supervised Teacher
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.04964'
    title: On Representation Knowledge Distillation for Graph Neural Networks
    date: Nov 9, 2021
    date_iso: '2021-11-09'
    date_display: Nov 2021
    codebase_url: https://github.com/chaitjo/efficient-gnns
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9795
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
  - model: KD
    model_plain: KD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.04964'
    title: On Representation Knowledge Distillation for Graph Neural Networks
    date: Nov 9, 2021
    date_iso: '2021-11-09'
    date_display: Nov 2021
    codebase_url: https://github.com/chaitjo/efficient-gnns
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9793
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
  - model: Cluster-SAGE
    model_plain: Cluster-SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.00959'
    title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    date: Mar 1, 2021
    date_iso: '2021-03-01'
    date_display: Mar 2021
    codebase_url: https://github.com/THUDM/cogdl
    published_conference: WWW 2021
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.979
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
  - model: StochasticGCN
    model_plain: StochasticGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1812.04202'
    title: 'Deep Learning on Graphs: A Survey'
    date: Dec 11, 2018
    date_iso: '2018-12-11'
    date_display: Dec 2018
    codebase_url: https://github.com/Hanjun-Dai/steady_state_embedding
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.979
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
  - model: Supervised Student
    model_plain: Supervised Student
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.04964'
    title: On Representation Knowledge Distillation for Graph Neural Networks
    date: Nov 9, 2021
    date_iso: '2021-11-09'
    date_display: Nov 2021
    codebase_url: https://github.com/chaitjo/efficient-gnns
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.979
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0045
    - null
    - null
    - null
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
    - 0.979
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
  - model: LSP
    model_plain: LSP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.04964'
    title: On Representation Knowledge Distillation for Graph Neural Networks
    date: Nov 9, 2021
    date_iso: '2021-11-09'
    date_display: Nov 2021
    codebase_url: https://github.com/chaitjo/efficient-gnns
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9781
    - null
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
    - null
  - model: VR-GCN
    model_plain: VR-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1905.07953'
    title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph
      Convolutional Networks'
    date: May 20, 2019
    date_iso: '2019-05-20'
    date_display: May 2019
    codebase_url: https://github.com/google-research/google-research
    published_conference: KDD 2019
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.978
    - null
    - 0.978
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GAT PTDNet-wl
    model_plain: GAT PTDNet-wl
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2011.07057'
    title: 'Learning to Drop: Robust Graph Neural Network via Topological Denoising'
    date: Nov 13, 2020
    date_iso: '2020-11-13'
    date_display: Nov 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.978
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.018
    - null
    - null
    - null
    - null
    - null
  - model: FitNet
    model_plain: FitNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2111.04964'
    title: On Representation Knowledge Distillation for Graph Neural Networks
    date: Nov 9, 2021
    date_iso: '2021-11-09'
    date_display: Nov 2021
    codebase_url: https://github.com/chaitjo/efficient-gnns
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9774
    - null
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
    - null
  - model: GNN-SD
    model_plain: GNN-SD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.06561'
    title: 'FreeKD: Free-direction Knowledge Distillation for Graph Neural Networks'
    date: Jun 14, 2022
    date_iso: '2022-06-14'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9773
    - null
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
    - null
  row_count: 290
  rows_json: /data/datasets/ppi/standard-split-rows.json
  chart_json: /data/datasets/ppi/standard-split-chart.json
  arch_counts:
    gnn: 197
    hybrid: 57
    graph_transformer: 1
    llm: 1
    walk: 6
    traditional: 13
  metric_counts:
  - 233
  - 15
  - 20
  - 2
  - 25
  - 9
  milestones: &id001
  - value: 0.612
    std: null
    model: GraphSAGE-LSTM
    arxiv_id: '1706.02216'
    title: Inductive Representation Learning on Large Graphs
    date: '2017-06-07'
  - value: 0.9871
    std: 0.0002
    model: GaAN
    arxiv_id: '1803.07294'
    title: 'GaAN: Gated Attention Networks for Learning on Large and Spatiotemporal
      Graphs'
    date: '2018-03-20'
  - value: 0.9936
    std: null
    model: Cluster-GCN
    arxiv_id: '1905.07953'
    title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph
      Convolutional Networks'
    date: '2019-05-20'
  - value: 0.9943
    std: null
    model: DenseMRGCN-14
    arxiv_id: '1910.06849'
    title: 'DeepGCNs: Making GCNs Go as Deep as CNNs'
    date: '2019-10-15'
  - value: 0.996
    std: null
    model: GraphCON-GCN
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: '2022-02-04'
  - value: 0.9982
    std: 0.01
    model: GAMLP(JK)
    arxiv_id: '2206.04355'
    title: Graph Attention Multi-Layer Perceptron
    date: '2022-06-09'
  milestones_by_metric:
    F1: *id001
    AUROC:
    - value: 0.7116
      std: 0.0028
      model: LP-InfoBN
      arxiv_id: '2201.01702'
      title: 'Bringing Your Own View: Graph Contrastive Learning without Prefabricated
        Data Augmentations'
      date: '2022-01-04'
    - value: 0.871
      std: null
      model: ProNet-All-Atom
      arxiv_id: '2207.12600'
      title: Learning Hierarchical Protein Representations via Complete 3D Graph Networks
      date: '2022-07-26'
    Accuracy:
    - value: 0.9936
      std: null
      model: Cluster-GCN
      arxiv_id: '1905.07953'
      title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and Large Graph
        Convolutional Networks'
      date: '2019-05-20'
    Overlap Consistency: []
    ROC-AUC:
    - value: 0.8191
      std: null
      model: AttrMasking SUPT_soft
      arxiv_id: '2402.10380'
      title: Subgraph-level Universal Prompt Tuning
      date: '2024-02-16'
    Topological Alignment: []
---

