---
title: Penn94
slug: penn94
benchmark: LINKX Benchmarks
task_type: node_classification
description: Facebook100 Penn94 social network node classification (binary gender).
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.LINKXDataset.html
stats:
  num_graphs: 1
  avg_nodes: 41554.0
  avg_edges: 1362229.0
  num_classes: 2
result_count: 106
best_model:
  model: ChebNet2D
  value: 0.8762
  metric: Accuracy
  arxiv_id: '2404.04559'
  paper_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
papers:
- arxiv_id: '2604.15699'
  title: Frequency-Corrupt Based Graph Self-Supervised Learning
  date_iso: '2026-04-17'
  venue: WWW 2026
- arxiv_id: '2504.20430'
  title: Learning Laplacian Positional Encodings for Heterophilous Graphs
  date_iso: '2025-04-29'
  venue: ''
- arxiv_id: '2411.17296'
  title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
  date_iso: '2024-11-26'
  venue: ICML 2024
- arxiv_id: '2408.07191'
  title: Joint Graph Rewiring and Feature Denoising via Spectral Resonance
  date_iso: '2024-08-13'
  venue: ICLR 2024
- arxiv_id: '2406.01249'
  title: Equivariant Machine Learning on Graphs with Nonlinear Spectral Filters
  date_iso: '2024-06-03'
  venue: NeurIPS 2024
- arxiv_id: '2405.20652'
  title: 'Sign is Not a Remedy: Multiset-to-Multiset Message Passing for Learning
    on Heterophilic Graphs'
  date_iso: '2024-05-31'
  venue: ICML 2024
- arxiv_id: '2405.16185'
  title: Differentiable Cluster Graph Neural Network
  date_iso: '2024-05-25'
  venue: ''
- arxiv_id: '2405.12474'
  title: 'How Universal Polynomial Bases Enhance Spectral Graph Neural Networks: Heterophily,
    Over-smoothing, and Over-squashing'
  date_iso: '2024-05-21'
  venue: ICML 2024
- arxiv_id: '2404.04559'
  title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
  date_iso: '2024-04-06'
  venue: ''
- arxiv_id: '2403.07954'
  title: 'Optimizing Polynomial Graph Filters: A Novel Adaptive Krylov Subspace Approach'
  date_iso: '2024-03-12'
  venue: WWW 2024
- arxiv_id: '2403.03676'
  title: Simplified PCNet with Robustness
  date_iso: '2024-03-06'
  venue: ''
- arxiv_id: '2312.14438'
  title: 'PC-Conv: Unifying Homophily and Heterophily with Two-fold Filtering'
  date_iso: '2023-12-22'
  venue: AAAI 2023
- arxiv_id: '2311.05185'
  title: Mixture of Weak & Strong Experts on Graphs
  date_iso: '2023-11-09'
  venue: ICLR 2023
- arxiv_id: '2310.10064'
  title: Shape-aware Graph Spectral Learning
  date_iso: '2023-10-16'
  venue: ''
- arxiv_id: '2306.02285'
  title: Clarify Confused Nodes via Separated Learning
  date_iso: '2023-06-04'
  venue: ''
- arxiv_id: '2303.06344'
  title: Graph Contrastive Learning under Heterophily via Graph Filters
  date_iso: '2023-03-11'
  venue: ''
- arxiv_id: '2302.12432'
  title: Graph Neural Networks with Learnable and Optimal Polynomial Bases
  date_iso: '2023-02-24'
  venue: ICML 2023
- arxiv_id: '2206.03601'
  title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
  date_iso: '2022-06-07'
  venue: ''
- arxiv_id: '2205.07308'
  title: Finding Global Homophily in Graph Neural Networks When Meeting Heterophily
  date_iso: '2022-05-15'
  venue: ICML 2022
- arxiv_id: '2202.03580'
  title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
  date_iso: '2022-02-04'
  venue: NeurIPS 2022
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
    avg_nodes: 41554.0
    avg_edges: 1362229.0
    num_classes: 2
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: ChebNet2D
    model_plain: ChebNet2D
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.04559'
    title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    date: Apr 6, 2024
    date_iso: '2024-04-06'
    date_display: Apr 2024
    codebase_url: https://github.com/jianhao2016/GPRGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8762
    metric_stds:
    - 0.002
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
    - 0.8669
    metric_stds:
    - 0.0022
  - model: M2M-GNN
    model_plain: M2M-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.20652'
    title: 'Sign is Not a Remedy: Multiset-to-Multiset Message Passing for Learning
      on Heterophilic Graphs'
    date: May 31, 2024
    date_iso: '2024-05-31'
    date_display: May 2024
    codebase_url: https://github.com/Jinx-byebye/m2mgnn
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8594
    metric_stds:
    - 0.004
  - model: GloGNN
    model_plain: GloGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07308'
    title: Finding Global Homophily in Graph Neural Networks When Meeting Heterophily
    date: May 15, 2022
    date_iso: '2022-05-15'
    date_display: May 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8557
    metric_stds:
    - null
  - model: att-Node-level NLSFs
    model_plain: att-Node-level NLSFs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.01249'
    title: Equivariant Machine Learning on Graphs with Nonlinear Spectral Filters
    date: Jun 3, 2024
    date_iso: '2024-06-03'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8519
    metric_stds:
    - 0.003
  - model: AdaptKry
    model_plain: AdaptKry
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.07954'
    title: 'Optimizing Polynomial Graph Filters: A Novel Adaptive Krylov Subspace
      Approach'
    date: Mar 12, 2024
    date_iso: '2024-03-12'
    date_display: Mar 2024
    codebase_url: https://github.com/kkhuang81/AdaptKry
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8497
    metric_stds:
    - 0.0036
  - model: GloGNN
    model_plain: GloGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.10064'
    title: Shape-aware Graph Spectral Learning
    date: Oct 16, 2023
    date_iso: '2023-10-16'
    date_display: Oct 2023
    codebase_url: https://github.com/junjie-xu/NewtonNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8494
    metric_stds:
    - 0.002
  - model: FavardGNN
    model_plain: FavardGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.8492
    metric_stds:
    - 0.0041
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
    - 0.8486
    metric_stds:
    - 0.0033
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
    - 0.8485
    metric_stds:
    - 0.0039
  - model: OptBasis
    model_plain: OptBasis
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.04559'
    title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    date: Apr 6, 2024
    date_iso: '2024-04-06'
    date_display: Apr 2024
    codebase_url: https://github.com/jianhao2016/GPRGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8482
    metric_stds:
    - 0.006
  - model: PCNet
    model_plain: PCNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.14438'
    title: 'PC-Conv: Unifying Homophily and Heterophily with Two-fold Filtering'
    date: Dec 22, 2023
    date_iso: '2023-12-22'
    date_display: Dec 2023
    codebase_url: https://github.com/uestclbh/PC-Conv
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8475
    metric_stds:
    - 0.0051
  - model: SPCNet-D
    model_plain: SPCNet-D
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.03676'
    title: Simplified PCNet with Robustness
    date: Mar 6, 2024
    date_iso: '2024-03-06'
    date_display: Mar 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8475
    metric_stds:
    - 0.0027
  - model: LINKX
    model_plain: LINKX
    is_baseline: true
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
    - 0.8471
    metric_stds:
    - 0.0052
  - model: MoE-GIN
    model_plain: MoE-GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8456
    metric_stds:
    - 0.0031
  - model: NewtonNet
    model_plain: NewtonNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.10064'
    title: Shape-aware Graph Spectral Learning
    date: Oct 16, 2023
    date_iso: '2023-10-16'
    date_display: Oct 2023
    codebase_url: https://github.com/junjie-xu/NewtonNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8456
    metric_stds:
    - 0.001
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_iso: '2023-06-04'
    date_display: Jun 2023
    codebase_url: https://github.com/GISec-Team/NCGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8455
    metric_stds:
    - 0.0054
  - model: UniFilter
    model_plain: UniFilter
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.12474'
    title: 'How Universal Polynomial Bases Enhance Spectral Graph Neural Networks:
      Heterophily, Over-smoothing, and Over-squashing'
    date: May 21, 2024
    date_iso: '2024-05-21'
    date_display: May 2024
    codebase_url: https://github.com/kkhuang81/UniFilter
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8446
    metric_stds:
    - 0.0033
  - model: Specformer
    model_plain: Specformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_iso: '2024-11-26'
    date_display: Nov 2024
    codebase_url: https://github.com/GGA23/GrokFormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8432
    metric_stds:
    - 0.0032
  - model: GOAL
    model_plain: GOAL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.20652'
    title: 'Sign is Not a Remedy: Multiset-to-Multiset Message Passing for Learning
      on Heterophilic Graphs'
    date: May 31, 2024
    date_iso: '2024-05-31'
    date_display: May 2024
    codebase_url: https://github.com/Jinx-byebye/m2mgnn
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8418
    metric_stds:
    - 0.003
  - model: NodeFormer
    model_plain: NodeFormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2404.04559'
    title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    date: Apr 6, 2024
    date_iso: '2024-04-06'
    date_display: Apr 2024
    codebase_url: https://github.com/jianhao2016/GPRGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8371
    metric_stds:
    - 0.003
  - model: Ord. GNN
    model_plain: Ord. GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.20652'
    title: 'Sign is Not a Remedy: Multiset-to-Multiset Message Passing for Learning
      on Heterophilic Graphs'
    date: May 31, 2024
    date_iso: '2024-05-31'
    date_display: May 2024
    codebase_url: https://github.com/Jinx-byebye/m2mgnn
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8365
    metric_stds:
    - 0.006
  - model: GrokFormer
    model_plain: GrokFormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_iso: '2024-11-26'
    date_display: Nov 2024
    codebase_url: https://github.com/GGA23/GrokFormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8359
    metric_stds:
    - 0.0026
  - model: GPR-GNN
    model_plain: GPR-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.0921
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
    - 0.8354
    metric_stds:
    - 0.0032
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.01249'
    title: Equivariant Machine Learning on Graphs with Nonlinear Spectral Filters
    date: Jun 3, 2024
    date_iso: '2024-06-03'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8354
    metric_stds:
    - 0.003
  - model: ChebNetII
    model_plain: ChebNetII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.10064'
    title: Shape-aware Graph Spectral Learning
    date: Oct 16, 2023
    date_iso: '2023-10-16'
    date_display: Oct 2023
    codebase_url: https://github.com/junjie-xu/NewtonNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8352
    metric_stds:
    - 0.002
  - model: MixHop
    model_plain: MixHop
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
    - 0.8347
    metric_stds:
    - 0.0071
  - model: MoE-H2GCN
    model_plain: MoE-H2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8339
    metric_stds:
    - 0.0043
  - model: JacobiConv
    model_plain: JacobiConv
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.10064'
    title: Shape-aware Graph Spectral Learning
    date: Oct 16, 2023
    date_iso: '2023-10-16'
    date_display: Oct 2023
    codebase_url: https://github.com/junjie-xu/NewtonNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8328
    metric_stds:
    - 0.001
  - model: BernNet
    model_plain: BernNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.0921
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
    - 0.8326
    metric_stds:
    - 0.0029
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.10064'
    title: Shape-aware Graph Spectral Learning
    date: Oct 16, 2023
    date_iso: '2023-10-16'
    date_display: Oct 2023
    codebase_url: https://github.com/junjie-xu/NewtonNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8323
    metric_stds:
    - 0.002
  - model: H2GCN
    model_plain: H2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_iso: '2023-06-04'
    date_display: Jun 2023
    codebase_url: https://github.com/GISec-Team/NCGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.832
    metric_stds:
    - 0.0055
  - model: MoE-GCN
    model_plain: MoE-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8319
    metric_stds:
    - 0.0043
  - model: GloGNN
    model_plain: GloGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_iso: '2023-06-04'
    date_display: Jun 2023
    codebase_url: https://github.com/GISec-Team/NCGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8307
    metric_stds:
    - 0.0135
  - model: ACM-GCN
    model_plain: ACM-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_iso: '2023-06-04'
    date_display: Jun 2023
    codebase_url: https://github.com/GISec-Team/NCGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8298
    metric_stds:
    - 0.0063
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
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
    - 0.8292
    metric_stds:
    - 0.0059
  - model: SPCNet-L
    model_plain: SPCNet-L
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.03676'
    title: Simplified PCNet with Robustness
    date: Mar 6, 2024
    date_iso: '2024-03-06'
    date_display: Mar 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8269
    metric_stds:
    - 0.0022
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8268
    metric_stds:
    - 0.0032
  - model: ChebNet
    model_plain: ChebNet
    is_baseline: true
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
    - 0.8259
    metric_stds:
    - 0.0031
  - model: BernNet
    model_plain: BernNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_iso: '2024-11-26'
    date_display: Nov 2024
    codebase_url: https://github.com/GGA23/GrokFormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8247
    metric_stds:
    - 0.0021
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.0921
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
    - 0.8247
    metric_stds:
    - 0.0027
  - model: AERO-GNN
    model_plain: AERO-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.20652'
    title: 'Sign is Not a Remedy: Multiset-to-Multiset Message Passing for Learning
      on Heterophilic Graphs'
    date: May 31, 2024
    date_iso: '2024-05-31'
    date_display: May 2024
    codebase_url: https://github.com/Jinx-byebye/m2mgnn
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8247
    metric_stds:
    - 0.007
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
    - 0.823
    metric_stds:
    - 0.0061
  - model: H_A
    model_plain: H_A
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07308'
    title: Finding Global Homophily in Graph Neural Networks When Meeting Heterophily
    date: May 15, 2022
    date_iso: '2022-05-15'
    date_display: May 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8225
    metric_stds:
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
    arxiv_id: '2403.07954'
    title: 'Optimizing Polynomial Graph Filters: A Novel Adaptive Krylov Subspace
      Approach'
    date: Mar 12, 2024
    date_iso: '2024-03-12'
    date_display: Mar 2024
    codebase_url: https://github.com/kkhuang81/AdaptKry
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8213
    metric_stds:
    - 0.0028
  - model: GraphMoE-GCN
    model_plain: GraphMoE-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8161
    metric_stds:
    - 0.0027
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8153
    metric_stds:
    - 0.0055
  - model: SGC
    model_plain: SGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.07954'
    title: 'Optimizing Polynomial Graph Filters: A Novel Adaptive Krylov Subspace
      Approach'
    date: Mar 12, 2024
    date_iso: '2024-03-12'
    date_display: Mar 2024
    codebase_url: https://github.com/kkhuang81/AdaptKry
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8144
    metric_stds:
    - 0.0015
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.14438'
    title: 'PC-Conv: Unifying Homophily and Heterophily with Two-fold Filtering'
    date: Dec 22, 2023
    date_iso: '2023-12-22'
    date_display: Dec 2023
    codebase_url: https://github.com/uestclbh/PC-Conv
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8138
    metric_stds:
    - 0.0016
  - model: GPR-GNN
    model_plain: GPR-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8138
    metric_stds:
    - 0.0016
  row_count: 106
  rows_json: /data/datasets/penn94/standard-split-rows.json
  chart_json: /data/datasets/penn94/standard-split-chart.json
  arch_counts:
    gnn: 79
    hybrid: 14
    graph_transformer: 8
    llm: 0
    walk: 3
    traditional: 2
  metric_counts:
  - 106
  milestones: &id001
  - value: 0.8486
    std: 0.0033
    model: ChebNetII
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: '2022-02-04'
  - value: 0.856
    std: 0.004
    model: GloGNN
    arxiv_id: '2303.06344'
    title: Graph Contrastive Learning under Heterophily via Graph Filters
    date: '2023-03-11'
  - value: 0.8574
    std: 0.0042
    model: GloGNN
    arxiv_id: '2312.14438'
    title: 'PC-Conv: Unifying Homophily and Heterophily with Two-fold Filtering'
    date: '2023-12-22'
  - value: 0.8762
    std: 0.002
    model: ChebNet2D
    arxiv_id: '2404.04559'
    title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    date: '2024-04-06'
  milestones_by_metric:
    Accuracy: *id001
---

