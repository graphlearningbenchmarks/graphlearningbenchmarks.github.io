---
title: IMDB
slug: imdb
benchmark: Heterogeneous Graph Benchmarks
task_type: node_classification
description: Heterogeneous IMDB graph — classify movie nodes (3 genres).
primary_metric: Micro-F1
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.IMDB.html
stats:
  num_graphs: 1
  avg_nodes: null
  avg_edges: null
  num_classes: 3
result_count: 287
best_model:
  model: GAT BGNN(m)-SC
  value: 0.8133
  metric: Micro-F1
  arxiv_id: '2210.05920'
  paper_title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
papers:
- arxiv_id: '2511.17923'
  title: Towards Efficient LLM-aware Heterogeneous Graph Learning
  date_iso: '2025-11-22'
  venue: ''
- arxiv_id: '2510.05750'
  title: Are Heterogeneous Graph Neural Networks Truly Effective? A Causal Perspective
  date_iso: '2025-10-07'
  venue: ''
- arxiv_id: '2410.10241'
  title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
  date_iso: '2024-10-14'
  venue: KDD 2024
- arxiv_id: '2408.17198'
  title: Towards Symbolic XAI -- Explanation Through Human Understandable Logical
    Relationships Between Features
  date_iso: '2024-08-30'
  venue: ''
- arxiv_id: '2405.18581'
  title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation Decomposition
    via Large Language Models'
  date_iso: '2024-05-28'
  venue: ''
- arxiv_id: '2405.01927'
  title: 'SlotGAT: Slot-based Message Passing for Heterogeneous Graphs'
  date_iso: '2024-05-03'
  venue: ICML 2024
- arxiv_id: '2403.04780'
  title: Graph-oriented Instruction Tuning of Large Language Models for Generic Graph
    Mining
  date_iso: '2024-03-02'
  venue: ''
- arxiv_id: '2312.05757'
  title: 'Towards Human-like Perception: Learning Structural Causal Model in Heterogeneous
    Graph'
  date_iso: '2023-12-10'
  venue: ''
- arxiv_id: '2310.16401'
  title: Graph Neural Networks with a Distribution of Parametrized Graphs
  date_iso: '2023-10-25'
  venue: ICML 2023
- arxiv_id: '2310.14481'
  title: Efficient Heterogeneous Graph Learning via Random Projection
  date_iso: '2023-10-23'
  venue: ''
- arxiv_id: '2310.15318'
  title: 'HetGPT: Harnessing the Power of Prompt Tuning in Pre-Trained Heterogeneous
    Graph Neural Networks'
  date_iso: '2023-10-23'
  venue: WWW 2023
- arxiv_id: '2307.08430'
  title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
  date_iso: '2023-07-17'
  venue: NeurIPS 2023
- arxiv_id: '2305.19872'
  title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
  date_iso: '2023-05-31'
  venue: WWW 2023
- arxiv_id: '2302.14061'
  title: Semantic-aware Node Synthesis for Imbalanced Heterogeneous Information Networks
  date_iso: '2023-02-27'
  venue: ''
- arxiv_id: '2302.11329'
  title: 'HINormer: Representation Learning On Heterogeneous Information Networks
    with Graph Transformer'
  date_iso: '2023-02-22'
  venue: WWW 2023
- arxiv_id: '2302.06299'
  title: Homophily-oriented Heterogeneous Graph Rewiring
  date_iso: '2023-02-13'
  venue: WWW 2023
- arxiv_id: '2210.05920'
  title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
  date_iso: '2022-10-12'
  venue: AAAI 2022
- arxiv_id: '2210.00248'
  title: Heterogeneous Graph Contrastive Multi-view Learning
  date_iso: '2022-10-01'
  venue: ''
- arxiv_id: '2208.10493'
  title: Relational Self-Supervised Learning on Graphs
  date_iso: '2022-08-21'
  venue: ''
- arxiv_id: '2208.06129'
  title: Multiplex Heterogeneous Graph Convolutional Network
  date_iso: '2022-08-12'
  venue: KDD 2022
- arxiv_id: '2207.02547'
  title: Simple and Efficient Heterogeneous Graph Neural Network
  date_iso: '2022-07-06'
  venue: AAAI 2022
- arxiv_id: '2206.12547'
  title: Geometry Contrastive Learning on Heterogeneous Graphs
  date_iso: '2022-06-25'
  venue: ''
- arxiv_id: '2202.11245'
  title: Exploring Edge Disentanglement for Node Classification
  date_iso: '2022-02-23'
  venue: WWW 2022
- arxiv_id: '2110.11842'
  title: Multi-view Contrastive Graph Clustering
  date_iso: '2021-10-22'
  venue: NeurIPS 2021
- arxiv_id: '2112.14936'
  title: Heterogeneous Graph Benchmarks
  date_iso: '2021-08-14'
  venue: KDD 2021
- arxiv_id: '2105.11122'
  title: Heterogeneous Graph Representation Learning with Relation Awareness
  date_iso: '2021-05-24'
  venue: ''
- arxiv_id: '2009.06211'
  title: Implicit Graph Neural Networks
  date_iso: '2020-09-14'
  venue: NeurIPS 2020
- arxiv_id: '2007.08294'
  title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous Graphs
  date_iso: '2020-07-16'
  venue: NeurIPS 2020
- arxiv_id: '1912.10832'
  title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
  date_iso: '2019-12-19'
  venue: AAAI 2019
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Micro-F1
  default_metric: Micro-F1
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: null
    avg_edges: null
    num_classes: 3
  metrics:
  - Micro-F1
  - Accuracy
  - F1
  - Macro F1
  metric_display_names:
  - Micro-F1
  - Accuracy
  - F1
  - Macro F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GAT BGNN(m)-SC
    model_plain: GAT BGNN(m)-SC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8133
    - null
    - null
    - null
    metric_stds:
    - 0.0179
    - null
    - null
    - null
  - model: SAGE BAN
    model_plain: SAGE BAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8073
    - null
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
    - null
  - model: GAT BGNN(m)-CS
    model_plain: GAT BGNN(m)-CS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8033
    - null
    - null
    - null
    metric_stds:
    - 0.0094
    - null
    - null
    - null
  - model: SAGE BGNN
    model_plain: SAGE BGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7967
    - null
    - null
    - null
    metric_stds:
    - 0.0047
    - null
    - null
    - null
  - model: GCN BGNN(m)-ST
    model_plain: GCN BGNN(m)-ST
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7967
    - null
    - null
    - null
    metric_stds:
    - 0.0027
    - null
    - null
    - null
  - model: SAGE BGNN(m)-TC
    model_plain: SAGE BGNN(m)-TC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7967
    - null
    - null
    - null
    metric_stds:
    - 0.0049
    - null
    - null
    - null
  - model: GAT BAN
    model_plain: GAT BAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.795
    - null
    - null
    - null
    metric_stds:
    - 0.005
    - null
    - null
    - null
  - model: GCN BGNN
    model_plain: GCN BGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7933
    - null
    - null
    - null
    metric_stds:
    - 0.0047
    - null
    - null
    - null
  - model: GAT BGNN
    model_plain: GAT BGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7933
    - null
    - null
    - null
    metric_stds:
    - 0.0094
    - null
    - null
    - null
  - model: SAGE BGNN(m)-CT
    model_plain: SAGE BGNN(m)-CT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7933
    - null
    - null
    - null
    metric_stds:
    - 0.0079
    - null
    - null
    - null
  - model: ELLA
    model_plain: ELLA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 13000.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2511.17923'
    title: Towards Efficient LLM-aware Heterogeneous Graph Learning
    date: Nov 22, 2025
    date_iso: '2025-11-22'
    date_display: Nov 2025
    codebase_url: https://github.com/l-wd/ELLA
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.793
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    - null
  - model: GCN BGNN(m)-TS
    model_plain: GCN BGNN(m)-TS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.79
    - null
    - null
    - null
    metric_stds:
    - 0.0
    - null
    - null
    - null
  - model: Ensemble
    model_plain: Ensemble
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7867
    - null
    - null
    - null
    metric_stds:
    - 0.0094
    - null
    - null
    - null
  - model: GCN BAN
    model_plain: GCN BAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.785
    - null
    - null
    - null
    metric_stds:
    - 0.01
    - null
    - null
    - null
  - model: GAT MulDE
    model_plain: GAT MulDE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.785
    - null
    - null
    - null
    metric_stds:
    - 0.0043
    - null
    - null
    - null
  - model: SAGE LSP
    model_plain: SAGE LSP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7823
    - null
    - null
    - null
    metric_stds:
    - 0.0091
    - null
    - null
    - null
  - model: MHGCN
    model_plain: MHGCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2208.06129'
    title: Multiplex Heterogeneous Graph Convolutional Network
    date: Aug 12, 2022
    date_iso: '2022-08-12'
    date_display: Aug 2022
    codebase_url: https://github.com/BUPT-GAMMA/OpenHGNN
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.782
    - null
    - null
    - null
    metric_stds:
    - 0.0138
    - null
    - null
    - null
  - model: GAT LSP
    model_plain: GAT LSP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.78
    - null
    - null
    - null
    metric_stds:
    - 0.0093
    - null
    - null
    - null
  - model: GCN LSP
    model_plain: GCN LSP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7799
    - null
    - null
    - null
    metric_stds:
    - 0.0121
    - null
    - null
    - null
  - model: SAGE KD
    model_plain: SAGE KD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.779
    - null
    - null
    - null
    metric_stds:
    - 0.0114
    - null
    - null
    - null
  - model: GAT KD
    model_plain: GAT KD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.778
    - null
    - null
    - null
    metric_stds:
    - 0.0125
    - null
    - null
    - null
  - model: GCN KD
    model_plain: GCN KD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.776
    - null
    - null
    - null
    metric_stds:
    - 0.0077
    - null
    - null
    - null
  - model: SAGE NoKD
    model_plain: SAGE NoKD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.776
    - null
    - null
    - null
    metric_stds:
    - 0.0102
    - null
    - null
    - null
  - model: SAGE MulDE
    model_plain: SAGE MulDE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.776
    - null
    - null
    - null
    metric_stds:
    - 0.015
    - null
    - null
    - null
  - model: GCN MulDE
    model_plain: GCN MulDE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.775
    - null
    - null
    - null
    metric_stds:
    - 0.012
    - null
    - null
    - null
  - model: GCN NoKD
    model_plain: GCN NoKD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.772
    - null
    - null
    - null
    metric_stds:
    - 0.004
    - null
    - null
    - null
  - model: MuseGraph (LLaMA3-8B)
    model_plain: MuseGraph (LLaMA3-8B)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 13.631488
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2403.04780'
    title: Graph-oriented Instruction Tuning of Large Language Models for Generic
      Graph Mining
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/Melinda315/MuseGraph
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7657
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: GAT NoKD
    model_plain: GAT NoKD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_iso: '2022-10-12'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.762
    - null
    - null
    - null
    metric_stds:
    - 0.0133
    - null
    - null
    - null
  - model: PSHGCN
    model_plain: PSHGCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/ivam-he/PSHGCN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7446
    - null
    - null
    - null
    metric_stds:
    - 0.0032
    - null
    - null
    - null
  - model: HetSANN.M.R.V
    model_plain: HetSANN.M.R.V
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_iso: '2019-12-19'
    date_display: Dec 2019
    codebase_url: https://github.com/didi/hetsann
    published_conference: AAAI 2019
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7386
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: HALO
    model_plain: HALO
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/ivam-he/PSHGCN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7381
    - null
    - null
    - null
    metric_stds:
    - 0.0072
    - null
    - null
    - null
  - model: SeHGNN
    model_plain: SeHGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/ivam-he/PSHGCN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7342
    - null
    - null
    - null
    metric_stds:
    - 0.0047
    - null
    - null
    - null
  - model: HetSANN.M.R
    model_plain: HetSANN.M.R
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_iso: '2019-12-19'
    date_display: Dec 2019
    codebase_url: https://github.com/didi/hetsann
    published_conference: AAAI 2019
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.732
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: HetSANN
    model_plain: HetSANN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_iso: '2019-12-19'
    date_display: Dec 2019
    codebase_url: https://github.com/didi/hetsann
    published_conference: AAAI 2019
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7311
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: model
    model_plain: model*
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2510.05750'
    title: Are Heterogeneous Graph Neural Networks Truly Effective? A Causal Perspective
    date: Oct 7, 2025
    date_iso: '2025-10-07'
    date_display: Oct 2025
    codebase_url: https://github.com/YXNTU/CausalHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.72
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: simpleHGN
    model_plain: simpleHGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/ivam-he/PSHGCN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7083
    - null
    - null
    - null
    metric_stds:
    - 0.0107
    - null
    - null
    - null
  - model: MHGCN
    model_plain: MHGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/ivam-he/PSHGCN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7028
    - null
    - null
    - null
    metric_stds:
    - 0.0071
    - null
    - null
    - null
  - model: RpHGNN
    model_plain: RpHGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.14481'
    title: Efficient Heterogeneous Graph Learning via Random Projection
    date: Oct 23, 2023
    date_iso: '2023-10-23'
    date_display: Oct 2023
    codebase_url: https://github.com/CrawlScript/RpHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6977
    - null
    - null
    - null
    metric_stds:
    - 0.0066
    - null
    - null
    - null
  - model: SeHGNN
    model_plain: SeHGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6917
    - null
    - null
    - null
    metric_stds:
    - 0.0043
    - null
    - null
    - null
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/ivam-he/PSHGCN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6883
    - null
    - null
    - null
    metric_stds:
    - 0.0095
    - null
    - null
    - null
  - model: EMRGNN
    model_plain: EMRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/ivam-he/PSHGCN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6876
    - null
    - null
    - null
    metric_stds:
    - 0.0078
    - null
    - null
    - null
  - model: LMSPS
    model_plain: LMSPS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.687
    - null
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
    - null
  - model: SlotGAT
    model_plain: SlotGAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6864
    - null
    - null
    - null
    metric_stds:
    - 0.0033
    - null
    - null
    - null
  - model: ChebNetII
    model_plain: ChebNetII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/ivam-he/PSHGCN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6833
    - null
    - null
    - null
    metric_stds:
    - 0.0092
    - null
    - null
    - null
  - model: GTN
    model_plain: GTN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/ivam-he/PSHGCN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6827
    - null
    - null
    - null
    metric_stds:
    - 0.0065
    - null
    - null
    - null
  - model: Variant#3
    model_plain: Variant#3
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6821
    - null
    - null
    - null
    metric_stds:
    - 0.0032
    - null
    - null
    - null
  - model: SeHGNN
    model_plain: SeHGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6821
    - null
    - null
    - null
    metric_stds:
    - 0.0032
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
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/ivam-he/PSHGCN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6813
    - null
    - null
    - null
    metric_stds:
    - 0.0083
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
    arxiv_id: '2305.19872'
    title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative Polynomials
    date: May 31, 2023
    date_iso: '2023-05-31'
    date_display: May 2023
    codebase_url: https://github.com/ivam-he/PSHGCN
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6808
    - null
    - null
    - null
    metric_stds:
    - 0.0049
    - null
    - null
    - null
  - model: HINormer
    model_plain: HINormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2302.11329'
    title: 'HINormer: Representation Learning On Heterogeneous Information Networks
      with Graph Transformer'
    date: Feb 22, 2023
    date_iso: '2023-02-22'
    date_display: Feb 2023
    codebase_url: ''
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6783
    - null
    - null
    - null
    metric_stds:
    - 0.0034
    - null
    - null
    - null
  row_count: 287
  rows_json: /data/datasets/imdb/standard-split-rows.json
  chart_json: /data/datasets/imdb/standard-split-chart.json
  arch_counts:
    gnn: 175
    hybrid: 38
    graph_transformer: 10
    llm: 13
    walk: 11
    traditional: 16
  metric_counts:
  - 223
  - 31
  - 33
  - 10
  milestones: &id001
  - value: 0.7386
    std: null
    model: HetSANN.M.R.V
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: '2019-12-19'
  - value: 0.782
    std: 0.0138
    model: MHGCN
    arxiv_id: '2208.06129'
    title: Multiplex Heterogeneous Graph Convolutional Network
    date: '2022-08-12'
  - value: 0.8133
    std: 0.0179
    model: GAT BGNN(m)-SC
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: '2022-10-12'
  milestones_by_metric:
    Micro-F1: *id001
    Accuracy:
    - value: 0.6736
      std: 0.0057
      model: simpleHGN
      arxiv_id: '2312.05757'
      title: 'Towards Human-like Perception: Learning Structural Causal Model in Heterogeneous
        Graph'
      date: '2023-12-10'
    - value: 0.7157
      std: 0.0042
      model: TAGs (70b)
      arxiv_id: '2405.18581'
      title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
        Decomposition via Large Language Models'
      date: '2024-05-28'
    - value: 0.919
      std: null
      model: BERT-Base, Uncased
      arxiv_id: '2408.17198'
      title: Towards Symbolic XAI -- Explanation Through Human Understandable Logical
        Relationships Between Features
      date: '2024-08-30'
    F1:
    - value: 0.6192
      std: null
      model: SGC
      arxiv_id: '2007.08294'
      title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
        Graphs
      date: '2020-07-16'
    Macro F1:
    - value: 0.6534
      std: 0.0033
      model: HG-SCM
      arxiv_id: '2312.05757'
      title: 'Towards Human-like Perception: Learning Structural Causal Model in Heterogeneous
        Graph'
      date: '2023-12-10'
---

