---
title: ZINC
slug: zinc
benchmark: Classic
task_type: graph_regression
description: Molecular property regression (constrained solubility).
primary_metric: MAE
higher_is_better: false
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.ZINC.html
stats:
  num_graphs: 249456
  avg_nodes: 23.2
  avg_edges: 24.9
  num_classes: null
result_count: 150
best_model:
  model: TIGT
  value: 0.014
  metric: MAE
  arxiv_id: '2402.02005'
  paper_title: Topology-Informed Graph Transformer
papers:
- arxiv_id: '2601.19094'
  title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
  date_iso: '2026-01-27'
  venue: ''
- arxiv_id: '2510.12369'
  title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive Graph Representation
    Learning
  date_iso: '2025-10-14'
  venue: ''
- arxiv_id: '2509.02803'
  title: A Graph Laplacian Eigenvector-based Pre-training Method for Graph Neural
    Networks
  date_iso: '2025-09-02'
  venue: ''
- arxiv_id: '2506.05814'
  title: Positional Encoding meets Persistent Homology on Graphs
  date_iso: '2025-06-06'
  venue: ICML 2025
- arxiv_id: '2502.02479'
  title: Using Random Noise Equivariantly to Boost Graph Neural Networks Universally
  date_iso: '2025-02-04'
  venue: ''
- arxiv_id: '2501.18739'
  title: 'Beyond Message Passing: Neural Graph Pattern Machine'
  date_iso: '2025-01-30'
  venue: ICML 2025
- arxiv_id: '2407.00696'
  title: Graph in Graph Neural Network
  date_iso: '2024-06-30'
  venue: ''
- arxiv_id: '2406.09291'
  title: A Flexible, Equivariant Framework for Subgraph GNNs via Graph Products and
    Graph Coarsening
  date_iso: '2024-06-13'
  venue: NeurIPS 2024
- arxiv_id: '2406.05815'
  title: What Can We Learn from State Space Models for Machine Learning on Graphs?
  date_iso: '2024-06-09'
  venue: ''
- arxiv_id: '2405.02795'
  title: Graph as Point Set
  date_iso: '2024-05-05'
  venue: ICML 2024
- arxiv_id: '2402.08450'
  title: 'Subgraphormer: Unifying Subgraph GNNs and Graph Transformers via Graph Products'
  date_iso: '2024-02-13'
  venue: ICML 2024
- arxiv_id: '2402.02005'
  title: Topology-Informed Graph Transformer
  date_iso: '2024-02-03'
  venue: ''
- arxiv_id: '2401.10119'
  title: Towards Principled Graph Transformers
  date_iso: '2024-01-18'
  venue: NeurIPS 2024
- arxiv_id: '2401.08514'
  title: 'Beyond Weisfeiler-Lehman: A Quantitative Framework for GNN Expressiveness'
  date_iso: '2024-01-16'
  venue: ICLR 2024
- arxiv_id: '2310.20519'
  title: Enhancing Graph Neural Networks with Quantum Computed Encodings
  date_iso: '2023-10-31'
  venue: ''
- arxiv_id: '2310.19142'
  title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
  date_iso: '2023-10-29'
  venue: NeurIPS 2023
- arxiv_id: '2309.04941'
  title: Distance-Restricted Folklore Weisfeiler-Leman GNNs with Provable Cycle Counting
    Power
  date_iso: '2023-09-10'
  venue: NeurIPS 2023
- arxiv_id: '2308.08235'
  title: 'The Expressive Power of Graph Neural Networks: A Survey'
  date_iso: '2023-08-16'
  venue: ''
- arxiv_id: '2306.10767'
  title: 'P-tensors: a General Framework for Higher Order Message Passing in Subgraph
    Neural Networks'
  date_iso: '2023-06-19'
  venue: ''
- arxiv_id: '2306.03561'
  title: 'CIN++: Enhancing Topological Message Passing'
  date_iso: '2023-06-06'
  venue: ''
- arxiv_id: '2305.15747'
  title: Union Subgraph Neural Networks
  date_iso: '2023-05-25'
  venue: AAAI 2023
- arxiv_id: '2304.10933'
  title: 'Self-Attention in Colors: Another Take on Encoding Graph Structure in Transformers'
  date_iso: '2023-04-21'
  venue: TMLR 2023
- arxiv_id: '2302.11556'
  title: Equivariant Polynomials for Graph Neural Networks
  date_iso: '2023-02-22'
  venue: ICML 2023
- arxiv_id: '2210.13978'
  title: Boosting the Cycle Counting Power of Graph Neural Networks with I$^2$-GNNs
  date_iso: '2022-10-22'
  venue: ICLR 2022
- arxiv_id: '2210.05274'
  title: Equivariant 3D-Conditional Diffusion Models for Molecular Linker Design
  date_iso: '2022-10-11'
  venue: ''
- arxiv_id: '2201.09332'
  title: How Expressive are Transformers in Spectral Domain for Graphs?
  date_iso: '2022-01-23'
  venue: TMLR 2022
- arxiv_id: '2109.12872'
  title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph Neural Networks'
  date_iso: '2021-09-27'
  venue: ''
- arxiv_id: '2106.12575'
  title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
  date_iso: '2021-06-23'
  venue: NeurIPS 2021
- arxiv_id: '1910.12892'
  title: Hyperbolic Graph Neural Networks
  date_iso: '2019-10-28'
  venue: NeurIPS 2019
- arxiv_id: '1802.08786'
  title: Syntax-Directed Variational Autoencoder for Structured Data
  date_iso: '2018-02-15'
  venue: ICLR 2018
variants:
- slug: full
  name: Full
  notes: 250,000 train molecules. Much better quality expected compared to 12k subset.
  is_standard: true
  primary_metric: MAE
  default_metric: MAE
  higher_is_better: false
  stats:
    num_graphs: 249456
    avg_nodes: 23.2
    avg_edges: 24.9
    num_classes: null
  metrics:
  - MAE
  - QED
  - RMSD
  - RMSE
  - Recovery
  - SA
  metric_display_names:
  - MAE
  - QED
  - RMSD
  - RMSE
  - Recovery
  - SA
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: TIGT
    model_plain: TIGT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: Feb 3, 2024
    date_iso: '2024-02-03'
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
    - 0.014
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
  - model: FloydNet
    model_plain: FloydNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_iso: '2026-01-27'
    date_display: Jan 2026
    codebase_url: https://github.com/ocx-lab/FloydNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.016
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
  - model: PST
    model_plain: PST
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2405.02795'
    title: Graph as Point Set
    date: May 5, 2024
    date_iso: '2024-05-05'
    date_display: May 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.018
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
  - model: GSSC
    model_plain: GSSC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.05815'
    title: What Can We Learn from State Space Models for Machine Learning on Graphs?
    date: Jun 9, 2024
    date_iso: '2024-06-09'
    date_display: Jun 2024
    codebase_url: https://github.com/Graph-COM/GSSC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.019
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
  - model: PPGN++(6)
    model_plain: PPGN++(6)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.08450'
    title: 'Subgraphormer: Unifying Subgraph GNNs and Graph Transformers via Graph
      Products'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: https://github.com/BarSGuy/Subgraphormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.02
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
  - model: PPGN++
    model_plain: PPGN++
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.11556'
    title: Equivariant Polynomials for Graph Neural Networks
    date: Feb 22, 2023
    date_iso: '2023-02-22'
    date_display: Feb 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.02
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
  - model: GPM
    model_plain: GPM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2501.18739'
    title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    date: Jan 30, 2025
    date_iso: '2025-01-30'
    date_display: Jan 2025
    codebase_url: https://github.com/Zehong-Wang/GPM
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.021
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
  - model: CS-GNN
    model_plain: CS-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2406.09291'
    title: A Flexible, Equivariant Framework for Subgraph GNNs via Graph Products
      and Graph Coarsening
    date: Jun 13, 2024
    date_iso: '2024-06-13'
    date_display: Jun 2024
    codebase_url: https://github.com/BarSGuy/Efficient-Subgraph-GNNs
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.021
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
  - model: CIN
    model_plain: CIN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.12575'
    title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    date: Jun 23, 2021
    date_iso: '2021-06-23'
    date_display: Jun 2021
    codebase_url: https://github.com/twitter-research/cwn
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.022
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
  - model: GNN-SSWL+
    model_plain: GNN-SSWL+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.387
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.08450'
    title: 'Subgraphormer: Unifying Subgraph GNNs and Graph Transformers via Graph
      Products'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: https://github.com/BarSGuy/Subgraphormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.022
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
  - model: SSWL+
    model_plain: SSWL+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.02795'
    title: Graph as Point Set
    date: May 5, 2024
    date_iso: '2024-05-05'
    date_display: May 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.022
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
  - model: Subgraphormer
    model_plain: Subgraphormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.293
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.08450'
    title: 'Subgraphormer: Unifying Subgraph GNNs and Graph Transformers via Graph
      Products'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: https://github.com/BarSGuy/Subgraphormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.023
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
  - model: GRIT
    model_plain: GRIT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_iso: '2023-10-31'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.023
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
  - model: GRIT 2-QiQRW
    model_plain: GRIT 2-QiQRW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_iso: '2023-10-31'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.023
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
  - model: I^2-GNN
    model_plain: I^2-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.04941'
    title: Distance-Restricted Folklore Weisfeiler-Leman GNNs with Provable Cycle
      Counting Power
    date: Sep 10, 2023
    date_iso: '2023-09-10'
    date_display: Sep 2023
    codebase_url: https://github.com/zml72062/DR-FWL-2
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.023
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
  - model: I^2-GNNs
    model_plain: I^2-GNNs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2210.13978'
    title: Boosting the Cycle Counting Power of Graph Neural Networks with I$^2$-GNNs
    date: Oct 22, 2022
    date_iso: '2022-10-22'
    date_display: Oct 2022
    codebase_url: https://github.com/GraphPKU/I2GNN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.023
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
  - model: UnionGPS
    model_plain: UnionGPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.15747'
    title: Union Subgraph Neural Networks
    date: May 25, 2023
    date_iso: '2023-05-25'
    date_display: May 2023
    codebase_url: https://github.com/AngusMonroe/UnionSNN
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0236
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
    - null
    - null
    - null
  - model: MPNNs
    model_plain: MPNNs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.10767'
    title: 'P-tensors: a General Framework for Higher Order Message Passing in Subgraph
      Neural Networks'
    date: Jun 19, 2023
    date_iso: '2023-06-19'
    date_display: Jun 2023
    codebase_url: https://github.com/arhands/ptensors
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.024
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
  - model: First order P-tensors
    model_plain: First order P-tensors
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.10767'
    title: 'P-tensors: a General Framework for Higher Order Message Passing in Subgraph
      Neural Networks'
    date: Jun 19, 2023
    date_iso: '2023-06-19'
    date_display: Jun 2023
    codebase_url: https://github.com/arhands/ptensors
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.024
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
  - model: Local 2-GNN
    model_plain: Local 2-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_iso: '2026-01-27'
    date_display: Jan 2026
    codebase_url: https://github.com/ocx-lab/FloydNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.024
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
  - model: SignNet
    model_plain: SignNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.11556'
    title: Equivariant Polynomials for Graph Neural Networks
    date: Feb 22, 2023
    date_iso: '2023-02-22'
    date_display: Feb 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.024
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
  - model: Lorentz
    model_plain: Lorentz
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1910.12892'
    title: Hyperbolic Graph Neural Networks
    date: Oct 28, 2019
    date_iso: '2019-10-28'
    date_display: Oct 2019
    codebase_url: https://github.com/facebookresearch/hgnn
    published_conference: NeurIPS 2019
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.024
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
  - model: ET+RRWP
    model_plain: ET+RRWP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2401.10119'
    title: Towards Principled Graph Transformers
    date: Jan 18, 2024
    date_iso: '2024-01-18'
    date_display: Jan 2024
    codebase_url: https://github.com/luis-mueller/towards-principled-gts
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.024
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
  - model: SUN
    model_plain: SUN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.526
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.08450'
    title: 'Subgraphormer: Unifying Subgraph GNNs and Graph Transformers via Graph
      Products'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: https://github.com/BarSGuy/Subgraphormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.024
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
  - model: Graphormer
    model_plain: Graphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_iso: '2026-01-27'
    date_display: Jan 2026
    codebase_url: https://github.com/ocx-lab/FloydNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.025
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
  - model: DRFWL
    model_plain: DRFWL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.02795'
    title: Graph as Point Set
    date: May 5, 2024
    date_iso: '2024-05-05'
    date_display: May 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.025
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
  - model: GRIT 1-CQRW
    model_plain: GRIT 1-CQRW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_iso: '2023-10-31'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.025
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
  - model: Graphormer-GD
    model_plain: Graphormer-GD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_iso: '2023-10-31'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.025
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
  - model: d-DRFWL(2) GNN
    model_plain: d-DRFWL(2) GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.04941'
    title: Distance-Restricted Folklore Weisfeiler-Leman GNNs with Provable Cycle
      Counting Power
    date: Sep 10, 2023
    date_iso: '2023-09-10'
    date_display: Sep 2023
    codebase_url: https://github.com/zml72062/DR-FWL-2
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.025
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
  - model: Unionormer
    model_plain: Unionormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.15747'
    title: Union Subgraph Neural Networks
    date: May 25, 2023
    date_iso: '2023-05-25'
    date_display: May 2023
    codebase_url: https://github.com/AngusMonroe/UnionSNN
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0252
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
  - model: ET
    model_plain: ET
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2401.10119'
    title: Towards Principled Graph Transformers
    date: Jan 18, 2024
    date_iso: '2024-01-18'
    date_display: Jan 2024
    codebase_url: https://github.com/luis-mueller/towards-principled-gts
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.026
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
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.15747'
    title: Union Subgraph Neural Networks
    date: May 25, 2023
    date_iso: '2023-05-25'
    date_display: May 2023
    codebase_url: https://github.com/AngusMonroe/UnionSNN
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0262
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0025
    - null
    - null
    - null
    - null
    - null
  - model: Subgraph GNN
    model_plain: Subgraph GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_iso: '2026-01-27'
    date_display: Jan 2026
    codebase_url: https://github.com/ocx-lab/FloydNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.028
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
  - model: URPE
    model_plain: URPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.492
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.08450'
    title: 'Subgraphormer: Unifying Subgraph GNNs and Graph Transformers via Graph
      Products'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: https://github.com/BarSGuy/Subgraphormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.028
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
  - model: Graphormer-URPE
    model_plain: Graphormer-URPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_iso: '2023-10-31'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.028
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
  - model: NGNN
    model_plain: NGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.08450'
    title: 'Subgraphormer: Unifying Subgraph GNNs and Graph Transformers via Graph
      Products'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: https://github.com/BarSGuy/Subgraphormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.029
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
  - model: DSS-GNN
    model_plain: DSS-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.08450'
    title: 'Subgraphormer: Unifying Subgraph GNNs and Graph Transformers via Graph
      Products'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: https://github.com/BarSGuy/Subgraphormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.029
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
  - model: ESAN
    model_plain: ESAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.02795'
    title: Graph as Point Set
    date: May 5, 2024
    date_iso: '2024-05-05'
    date_display: May 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.029
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
  - model: Nested GIN
    model_plain: Nested GIN*
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.13978'
    title: Boosting the Cycle Counting Power of Graph Neural Networks with I$^2$-GNNs
    date: Oct 22, 2022
    date_iso: '2022-10-22'
    date_display: Oct 2022
    codebase_url: https://github.com/GraphPKU/I2GNN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.029
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
  - model: CNNs
    model_plain: CNNs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.00696'
    title: Graph in Graph Neural Network
    date: Jun 30, 2024
    date_iso: '2024-06-30'
    date_display: Jun 2024
    codebase_url: https://github.com/wangjs96/Graph-in-Graph-Neural-Network
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.029
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
  - model: MPNN
    model_plain: MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_iso: '2026-01-27'
    date_display: Jan 2026
    codebase_url: https://github.com/ocx-lab/FloydNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.03
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
  - model: MAG-GNN
    model_plain: MAG-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.09291'
    title: A Flexible, Equivariant Framework for Subgraph GNNs via Graph Products
      and Graph Coarsening
    date: Jun 13, 2024
    date_iso: '2024-06-13'
    date_display: Jun 2024
    codebase_url: https://github.com/BarSGuy/Efficient-Subgraph-GNNs
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.03
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
  - model: Graphormer
    model_plain: Graphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.15747'
    title: Union Subgraph Neural Networks
    date: May 25, 2023
    date_iso: '2023-05-25'
    date_display: May 2023
    codebase_url: https://github.com/AngusMonroe/UnionSNN
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0309
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
  - model: Poincare
    model_plain: Poincare
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1910.12892'
    title: Hyperbolic Graph Neural Networks
    date: Oct 28, 2019
    date_iso: '2019-10-28'
    date_display: Oct 2019
    codebase_url: https://github.com/facebookresearch/hgnn
    published_conference: NeurIPS 2019
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.031
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0001
    - null
    - null
    - null
    - null
    - null
  - model: GGNN
    model_plain: GGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1910.12892'
    title: Hyperbolic Graph Neural Networks
    date: Oct 28, 2019
    date_iso: '2019-10-28'
    date_display: Oct 2019
    codebase_url: https://github.com/facebookresearch/hgnn
    published_conference: NeurIPS 2019
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.032
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
  - model: Euclidean
    model_plain: Euclidean
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1910.12892'
    title: Hyperbolic Graph Neural Networks
    date: Oct 28, 2019
    date_iso: '2019-10-28'
    date_display: Oct 2019
    codebase_url: https://github.com/facebookresearch/hgnn
    published_conference: NeurIPS 2019
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.033
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
  - model: GNN-AK+
    model_plain: GNN-AK+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2501.18739'
    title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    date: Jan 30, 2025
    date_iso: '2025-01-30'
    date_display: Jan 2025
    codebase_url: https://github.com/Zehong-Wang/GPM
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.034
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
  - model: Graph ViT
    model_plain: Graph ViT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2501.18739'
    title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    date: Jan 30, 2025
    date_iso: '2025-01-30'
    date_display: Jan 2025
    codebase_url: https://github.com/Zehong-Wang/GPM
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.035
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
  - model: CRaWl
    model_plain: CRaWl
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2501.18739'
    title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    date: Jan 30, 2025
    date_iso: '2025-01-30'
    date_display: Jan 2025
    codebase_url: https://github.com/Zehong-Wang/GPM
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.036
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
  - model: SAT
    model_plain: SAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2501.18739'
    title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    date: Jan 30, 2025
    date_iso: '2025-01-30'
    date_display: Jan 2025
    codebase_url: https://github.com/Zehong-Wang/GPM
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.036
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
  row_count: 150
  rows_json: /data/datasets/zinc/full-rows.json
  chart_json: /data/datasets/zinc/full-chart.json
  arch_counts:
    gnn: 83
    hybrid: 25
    graph_transformer: 27
    llm: 0
    walk: 1
    traditional: 7
  metric_counts:
  - 139
  - 3
  - 1
  - 8
  - 3
  - 3
  milestones: &id001
  - value: 1.366
    std: 0.023
    model: SD-VAE
    arxiv_id: '1802.08786'
    title: Syntax-Directed Variational Autoencoder for Structured Data
    date: '2018-02-15'
  - value: 0.022
    std: 0.002
    model: CIN
    arxiv_id: '2106.12575'
    title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    date: '2021-06-23'
  - value: 0.02
    std: 0.001
    model: PPGN++
    arxiv_id: '2302.11556'
    title: Equivariant Polynomials for Graph Neural Networks
    date: '2023-02-22'
  - value: 0.014
    std: 0.001
    model: TIGT
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: '2024-02-03'
  milestones_by_metric:
    MAE: *id001
    QED:
    - value: 0.68
      std: null
      model: DiffLinker
      arxiv_id: '2210.05274'
      title: Equivariant 3D-Conditional Diffusion Models for Molecular Linker Design
      date: '2022-10-11'
    RMSD:
    - value: 0.32
      std: null
      model: DiffLinker
      arxiv_id: '2210.05274'
      title: Equivariant 3D-Conditional Diffusion Models for Molecular Linker Design
      date: '2022-10-11'
    RMSE:
    - value: 0.022
      std: 0.002
      model: CIN
      arxiv_id: '2310.19142'
      title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
      date: '2023-10-29'
    Recovery:
    - value: 0.94
      std: null
      model: 3DLinker (given anchors)
      arxiv_id: '2210.05274'
      title: Equivariant 3D-Conditional Diffusion Models for Molecular Linker Design
      date: '2022-10-11'
    SA:
    - value: 3.01
      std: null
      model: DiffLinker
      arxiv_id: '2210.05274'
      title: Equivariant 3D-Conditional Diffusion Models for Molecular Linker Design
      date: '2022-10-11'
---

