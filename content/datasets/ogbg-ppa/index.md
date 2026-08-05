---
title: ogbg-ppa
slug: ogbg-ppa
benchmark: OGB
task_type: graph_classification
description: Protein-protein association subgraph classification (37 taxonomic groups).
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://ogb.stanford.edu/docs/graphprop/#ogbg-ppa
stats:
  num_graphs: 158100
  avg_nodes: 243.4
  avg_edges: 2266.1
  num_classes: 37
result_count: 53
best_model:
  model: A-NLSF
  value: 0.8149
  metric: Accuracy
  arxiv_id: '2509.24886'
  paper_title: Adaptive Canonicalization with Application to Invariant Anisotropic
    Geometric Networks
papers:
- arxiv_id: '2510.05583'
  title: 'When does global attention help: a unified empirical study on atomistic
    graph learning'
  date_iso: '2025-10-07'
  venue: ''
- arxiv_id: '2509.24886'
  title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
    Networks
  date_iso: '2025-09-29'
  venue: ''
- arxiv_id: '2502.16233'
  title: Graph Self-Supervised Learning with Learnable Structural and Positional Encodings
  date_iso: '2025-02-22'
  venue: WWW 2025
- arxiv_id: '2407.02758'
  title: Differential Encoding for Improved Representation Learning Over Graphs
  date_iso: '2024-07-03'
  venue: ''
- arxiv_id: '2407.00696'
  title: Graph in Graph Neural Network
  date_iso: '2024-06-30'
  venue: ''
- arxiv_id: '2406.12059'
  title: A Scalable and Effective Alternative to Graph Transformers
  date_iso: '2024-06-17'
  venue: AAAI 2024
- arxiv_id: '2305.06102'
  title: Towards Better Graph Representation Learning with Parameterized Decomposition
    & Filtering
  date_iso: '2023-05-10'
  venue: ICML 2023
- arxiv_id: '2301.11956'
  title: On the Connection Between MPNN and Graph Transformer
  date_iso: '2023-01-27'
  venue: ICML 2023
- arxiv_id: '2211.14568'
  title: 'BeGin: Extensive Benchmark Scenarios and An Easy-to-use Framework for Graph
    Continual Learning'
  date_iso: '2022-11-26'
  venue: ''
- arxiv_id: '2211.06605'
  title: Comprehensive Analysis of Over-smoothing in Graph Neural Networks from Markov
    Chains Perspective
  date_iso: '2022-11-12'
  venue: ''
- arxiv_id: '2210.02997'
  title: Expander Graph Propagation
  date_iso: '2022-10-06'
  venue: LoG 2022
- arxiv_id: '2206.11010'
  title: Agent-based Graph Neural Networks
  date_iso: '2022-06-22'
  venue: ICLR 2022
- arxiv_id: '2206.02059'
  title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
  date_iso: '2022-06-04'
  venue: TMLR 2022
- arxiv_id: '2202.03036'
  title: Structure-Aware Transformer for Graph Representation Learning
  date_iso: '2022-02-07'
  venue: ICML 2022
- arxiv_id: '2103.16584'
  title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
  date_iso: '2021-03-30'
  venue: ''
- arxiv_id: '2103.01488'
  title: 'Multi-Level Attention Pooling for Graph Neural Networks: Unifying Graph
    Representations with Multiple Localities'
  date_iso: '2021-03-02'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: OGB species split.
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 158100
    avg_nodes: 243.4
    avg_edges: 2266.1
    num_classes: 37
  metrics:
  - Accuracy
  - FWT
  metric_display_names:
  - Accuracy
  - FWT
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: A-NLSF
    model_plain: A-NLSF
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: Sep 29, 2025
    date_iso: '2025-09-29'
    date_display: Sep 2025
    codebase_url: https://github.com/ywelld/_ac
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8149
    - null
    metric_stds:
    - 0.0067
    - null
  - model: differential encoding
    model_plain: differential encoding
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.02758'
    title: Differential Encoding for Improved Representation Learning Over Graphs
    date: Jul 3, 2024
    date_iso: '2024-07-03'
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
    - 0.8096
    - null
    metric_stds:
    - 0.0029
    - null
  - model: MPNN + VN + NoPE
    model_plain: MPNN + VN + NoPE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_iso: '2023-01-27'
    date_display: Jan 2023
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8055
    - null
    metric_stds:
    - 0.0038
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
    - 0.8017
    - null
    metric_stds:
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
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_iso: '2023-01-27'
    date_display: Jan 2023
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8015
    - null
    metric_stds:
    - 0.0033
    - null
  - model: GSO
    model_plain: GSO
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.06102'
    title: Towards Better Graph Representation Learning with Parameterized Decomposition
      & Filtering
    date: May 10, 2023
    date_iso: '2023-05-10'
    date_display: May 2023
    codebase_url: https://github.com/qslim/PDF
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.801
    - null
    metric_stds:
    - 0.0052
    - null
  - model: GECO
    model_plain: GECO
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.12059'
    title: A Scalable and Effective Alternative to Graph Transformers
    date: Jun 17, 2024
    date_iso: '2024-06-17'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7982
    - null
    metric_stds:
    - 0.0042
    - null
  - model: ExpC
    model_plain: ExpC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7976
    - null
    metric_stds:
    - 0.0072
    - null
  - model: regularization term
    model_plain: regularization term
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06605'
    title: Comprehensive Analysis of Over-smoothing in Graph Neural Networks from
      Markov Chains Perspective
    date: Nov 12, 2022
    date_iso: '2022-11-12'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.78
    - null
    metric_stds:
    - 0.0037
    - null
  - model: DeeperGCN+FLAG
    model_plain: DeeperGCN+FLAG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.531
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7752
    - null
    metric_stds:
    - 0.0069
    - null
  - model: OAP+GatedGCN
    model_plain: OAP+GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: Sep 29, 2025
    date_iso: '2025-09-29'
    date_display: Sep 2025
    codebase_url: https://github.com/ywelld/_ac
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7745
    - null
    metric_stds:
    - 0.0098
    - null
  - model: GEN
    model_plain: GEN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06605'
    title: Comprehensive Analysis of Over-smoothing in Graph Neural Networks from
      Markov Chains Perspective
    date: Nov 12, 2022
    date_iso: '2022-11-12'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7712
    - null
    metric_stds:
    - 0.0071
    - null
  - model: DeeperGCN
    model_plain: DeeperGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.532
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7712
    - null
    metric_stds:
    - 0.0071
    - null
  - model: DeeperG
    model_plain: DeeperG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 5.6
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.06102'
    title: Towards Better Graph Representation Learning with Parameterized Decomposition
      & Filtering
    date: May 10, 2023
    date_iso: '2023-05-10'
    date_display: May 2023
    codebase_url: https://github.com/qslim/PDF
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7712
    - null
    metric_stds:
    - 0.0071
    - null
  - model: PHC-GNN
    model_plain: PHC-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7561
    - null
    metric_stds:
    - null
    - null
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: Sep 29, 2025
    date_iso: '2025-09-29'
    date_display: Sep 2025
    codebase_url: https://github.com/ywelld/_ac
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7531
    - null
    metric_stds:
    - 0.0083
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
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: Sep 29, 2025
    date_iso: '2025-09-29'
    date_display: Sep 2025
    codebase_url: https://github.com/ywelld/_ac
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7522
    - null
    metric_stds:
    - 0.0056
    - null
  - model: KS-SAT
    model_plain: KS-SAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2305.06102'
    title: Towards Better Graph Representation Learning with Parameterized Decomposition
      & Filtering
    date: May 10, 2023
    date_iso: '2023-05-10'
    date_display: May 2023
    codebase_url: https://github.com/qslim/PDF
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7522
    - null
    metric_stds:
    - 0.0056
    - null
  - model: K-Subtree SAT
    model_plain: K-Subtree SAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7522
    - null
    metric_stds:
    - 0.0056
    - null
  - model: k-subtree SAT-PNA
    model_plain: k-subtree SAT-PNA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7522
    - null
    metric_stds:
    - 0.0056
    - null
  - model: k-subtree SAT-GCN
    model_plain: k-subtree SAT-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7483
    - null
    metric_stds:
    - 0.0048
    - null
  - model: k-subtree SAT-GIN
    model_plain: k-subtree SAT-GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7306
    - null
    metric_stds:
    - 0.0076
    - null
  - model: GIN+VN+Flag
    model_plain: GIN+VN+Flag
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 3.29
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7245
    - null
    metric_stds:
    - 0.0114
    - null
  - model: AgentNet
    model_plain: AgentNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.11010'
    title: Agent-based Graph Neural Networks
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/KarolisMart/AgentNet
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7233
    - null
    metric_stds:
    - 0.0062
    - null
  - model: JK
    model_plain: JK
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.01488'
    title: 'Multi-Level Attention Pooling for Graph Neural Networks: Unifying Graph
      Representations with Multiple Localities'
    date: Mar 2, 2021
    date_iso: '2021-03-02'
    date_display: Mar 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7198
    - null
    metric_stds:
    - 0.0013
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7194
    - null
    metric_stds:
    - 0.0043
    - null
  - model: naive
    model_plain: naive
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.01488'
    title: 'Multi-Level Attention Pooling for Graph Neural Networks: Unifying Graph
      Representations with Multiple Localities'
    date: Mar 2, 2021
    date_iso: '2021-03-02'
    date_display: Mar 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7184
    - null
    metric_stds:
    - 0.0011
    - null
  - model: MLAP
    model_plain: MLAP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2103.01488'
    title: 'Multi-Level Attention Pooling for Graph Neural Networks: Unifying Graph
      Representations with Multiple Localities'
    date: Mar 2, 2021
    date_iso: '2021-03-02'
    date_display: Mar 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7183
    - null
    metric_stds:
    - 0.0012
    - null
  - model: StructPosGSSL-FA
    model_plain: StructPosGSSL-FA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2502.16233'
    title: Graph Self-Supervised Learning with Learnable Structural and Positional
      Encodings
    date: Feb 22, 2025
    date_iso: '2025-02-22'
    date_display: Feb 2025
    codebase_url: https://github.com/wokas36/StructPosGSSL
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.709
    - null
    metric_stds:
    - 0.0186
    - null
  - model: StructPosGSSL-SA
    model_plain: StructPosGSSL-SA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2502.16233'
    title: Graph Self-Supervised Learning with Learnable Structural and Positional
      Encodings
    date: Feb 22, 2025
    date_iso: '2025-02-22'
    date_display: Feb 2025
    codebase_url: https://github.com/wokas36/StructPosGSSL
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7081
    - null
    metric_stds:
    - 0.0145
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7066
    - null
    metric_stds:
    - 0.0165
    - null
  - model: GIN + 3-cycle count feature
    model_plain: GIN + 3-cycle count feature
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7058
    - null
    metric_stds:
    - 0.0064
    - null
  - model: GIN+VN
    model_plain: GIN+VN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 3.29
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7037
    - null
    metric_stds:
    - 0.0107
    - null
  - model: GIN+virtual node
    model_plain: GIN+virtual node
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.11010'
    title: Agent-based Graph Neural Networks
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/KarolisMart/AgentNet
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7037
    - null
    metric_stds:
    - 0.0107
    - null
  - model: GIN-Virtual Node
    model_plain: GIN-Virtual Node
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7037
    - null
    metric_stds:
    - 0.0107
    - null
  - model: GIN + EGP
    model_plain: GIN + EGP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.02997'
    title: Expander Graph Propagation
    date: Oct 6, 2022
    date_iso: '2022-10-06'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: LoG 2022
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7027
    - null
    metric_stds:
    - 0.0159
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
    arxiv_id: '2206.11010'
    title: Agent-based Graph Neural Networks
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/KarolisMart/AgentNet
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7025
    - null
    metric_stds:
    - 0.0052
    - null
  - model: GIN + Master Node
    model_plain: GIN + Master Node
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.02997'
    title: Expander Graph Propagation
    date: Oct 6, 2022
    date_iso: '2022-10-06'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: LoG 2022
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6916
    - null
    metric_stds:
    - 0.0154
    - null
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 3.336
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6892
    - null
    metric_stds:
    - 0.01
    - null
  - model: GCN+virtual node
    model_plain: GCN+virtual node
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_iso: '2023-01-27'
    date_display: Jan 2023
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6857
    - null
    metric_stds:
    - 0.0061
    - null
  - model: GCN-Virtual Node
    model_plain: GCN-Virtual Node
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6857
    - null
    metric_stds:
    - 0.0061
    - null
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.537
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6839
    - null
    metric_stds:
    - 0.0084
    - null
  - model: S4
    model_plain: S4
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.05583'
    title: 'When does global attention help: a unified empirical study on atomistic
      graph learning'
    date: Oct 7, 2025
    date_iso: '2025-10-07'
    date_display: Oct 2025
    codebase_url: https://github.com/ORNL/HydraGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6701
    - null
    metric_stds:
    - null
    - null
  - model: S1
    model_plain: S1
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.05583'
    title: 'When does global attention help: a unified empirical study on atomistic
      graph learning'
    date: Oct 7, 2025
    date_iso: '2025-10-07'
    date_display: Oct 2025
    codebase_url: https://github.com/ORNL/HydraGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6524
    - null
    metric_stds:
    - null
    - null
  - model: Transformer
    model_plain: Transformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6454
    - null
    metric_stds:
    - 0.0033
    - null
  - model: S2
    model_plain: S2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.05583'
    title: 'When does global attention help: a unified empirical study on atomistic
      graph learning'
    date: Oct 7, 2025
    date_iso: '2025-10-07'
    date_display: Oct 2025
    codebase_url: https://github.com/ORNL/HydraGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6375
    - null
    metric_stds:
    - null
    - null
  - model: S3
    model_plain: S3
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.05583'
    title: 'When does global attention help: a unified empirical study on atomistic
      graph learning'
    date: Oct 7, 2025
    date_iso: '2025-10-07'
    date_display: Oct 2025
    codebase_url: https://github.com/ORNL/HydraGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5324
    - null
    metric_stds:
    - null
    - null
  - model: Bare
    model_plain: Bare
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.14568'
    title: 'BeGin: Extensive Benchmark Scenarios and An Easy-to-use Framework for
      Graph Continual Learning'
    date: Nov 26, 2022
    date_iso: '2022-11-26'
    date_display: Nov 2022
    codebase_url: https://github.com/ShinhwanKang/BeGin
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 15.7
    metric_stds:
    - null
    - 1.3
  - model: LwF
    model_plain: LwF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2211.14568'
    title: 'BeGin: Extensive Benchmark Scenarios and An Easy-to-use Framework for
      Graph Continual Learning'
    date: Nov 26, 2022
    date_iso: '2022-11-26'
    date_display: Nov 2022
    codebase_url: https://github.com/ShinhwanKang/BeGin
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 19.7
    metric_stds:
    - null
    - 1.5
  - model: EWC
    model_plain: EWC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.14568'
    title: 'BeGin: Extensive Benchmark Scenarios and An Easy-to-use Framework for
      Graph Continual Learning'
    date: Nov 26, 2022
    date_iso: '2022-11-26'
    date_display: Nov 2022
    codebase_url: https://github.com/ShinhwanKang/BeGin
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 11.5
    metric_stds:
    - null
    - 1.7
  row_count: 53
  rows_json: /data/datasets/ogbg-ppa/standard-split-rows.json
  chart_json: /data/datasets/ogbg-ppa/standard-split-chart.json
  arch_counts:
    gnn: 32
    hybrid: 10
    graph_transformer: 4
    llm: 0
    walk: 0
    traditional: 5
  metric_counts:
  - 47
  - 6
  milestones: &id001
  - value: 0.7198
    std: 0.0013
    model: JK
    arxiv_id: '2103.01488'
    title: 'Multi-Level Attention Pooling for Graph Neural Networks: Unifying Graph
      Representations with Multiple Localities'
    date: '2021-03-02'
  - value: 0.7752
    std: 0.0069
    model: DeeperGCN+FLAG
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: '2021-03-30'
  - value: 0.7976
    std: 0.0072
    model: ExpC
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: '2022-02-07'
  - value: 0.8055
    std: 0.0038
    model: MPNN + VN + NoPE
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: '2023-01-27'
  - value: 0.8096
    std: 0.0029
    model: differential encoding
    arxiv_id: '2407.02758'
    title: Differential Encoding for Improved Representation Learning Over Graphs
    date: '2024-07-03'
  - value: 0.8149
    std: 0.0067
    model: A-NLSF
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: '2025-09-29'
  milestones_by_metric:
    Accuracy: *id001
    FWT:
    - value: 19.7
      std: 1.5
      model: LwF
      arxiv_id: '2211.14568'
      title: 'BeGin: Extensive Benchmark Scenarios and An Easy-to-use Framework for
        Graph Continual Learning'
      date: '2022-11-26'
---

