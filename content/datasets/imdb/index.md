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
result_count: 230
best_model:
  model: ELLA
  value: 0.793
  metric: Micro-F1
  arxiv_id: '2511.17923'
  paper_title: Towards Efficient LLM-aware Heterogeneous Graph Learning
papers:
- arxiv_id: '2511.17923'
  title: Towards Efficient LLM-aware Heterogeneous Graph Learning
  date_iso: '2025-11-22'
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
    is_best: true
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
  - model: HAN
    model_plain: HAN
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
    - 0.6769
    - null
    - null
    - null
    metric_stds:
    - 0.0064
    - null
    - null
    - null
  - model: PMMM
    model_plain: PMMM
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
    - 0.6758
    - null
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
    - null
  - model: DisenHAN
    model_plain: DisenHAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.01927'
    title: 'SlotGAT: Slot-based Message Passing for Heterogeneous Graphs'
    date: May 3, 2024
    date_iso: '2024-05-03'
    date_display: May 2024
    codebase_url: https://github.com/scottjiao/SlotGAT_ICML23
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6748
    - null
    - null
    - null
    metric_stds:
    - 0.0045
    - null
    - null
    - null
  - model: HGB
    model_plain: HGB
    is_baseline: true
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
    - 0.6736
    - null
    - null
    - null
    metric_stds:
    - 0.0057
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
    - 0.6736
    - null
    - null
    - null
    metric_stds:
    - 0.0057
    - null
    - null
    - null
  - model: Simple-HGN
    model_plain: Simple-HGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2112.14936'
    title: Heterogeneous Graph Benchmarks
    date: Aug 14, 2021
    date_iso: '2021-08-14'
    date_display: Aug 2021
    codebase_url: https://github.com/THUDM/HGB
    published_conference: KDD 2021
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6736
    - null
    - null
    - null
    metric_stds:
    - 0.0057
    - null
    - null
    - null
  - model: GraphAdapter
    model_plain: GraphAdapter
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
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
    - 0.673
    - null
    - null
    - null
    metric_stds:
    - 0.005
    - null
    - null
    - null
  - model: HGT
    model_plain: HGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2112.14936'
    title: Heterogeneous Graph Benchmarks
    date: Aug 14, 2021
    date_iso: '2021-08-14'
    date_display: Aug 2021
    codebase_url: https://github.com/THUDM/HGB
    published_conference: KDD 2021
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.672
    - null
    - null
    - null
    metric_stds:
    - 0.0057
    - null
    - null
    - null
  - model: GHGRL
    model_plain: GHGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
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
    - 0.667
    - null
    - null
    - null
    metric_stds:
    - 0.011
    - null
    - null
    - null
  - model: Variant#2
    model_plain: Variant#2
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
    - 0.6668
    - null
    - null
    - null
    metric_stds:
    - 0.0052
    - null
    - null
    - null
  - model: Variant#4
    model_plain: Variant#4
    is_baseline: true
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
    - 0.6665
    - null
    - null
    - null
    metric_stds:
    - 0.005
    - null
    - null
    - null
  - model: Variant#1
    model_plain: Variant#1
    is_baseline: true
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
    - 0.6658
    - null
    - null
    - null
    metric_stds:
    - 0.0042
    - null
    - null
    - null
  - model: RGCN
    model_plain: RGCN
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
    - 0.6651
    - null
    - null
    - null
    metric_stds:
    - 0.0028
    - null
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
    - 0.6629
    - null
    - null
    - null
    metric_stds:
    - 0.0069
    - null
    - null
    - null
  - model: NARS
    model_plain: NARS
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
    - 0.6618
    - null
    - null
    - null
    metric_stds:
    - 0.007
    - null
    - null
    - null
  - model: HDMI
    model_plain: HDMI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2208.10493'
    title: Relational Self-Supervised Learning on Graphs
    date: Aug 21, 2022
    date_iso: '2022-08-21'
    date_display: Aug 2022
    codebase_url: https://github.com/Namkyeong/RGRL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.658
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: RGRL
    model_plain: RGRL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2208.10493'
    title: Relational Self-Supervised Learning on Graphs
    date: Aug 21, 2022
    date_iso: '2022-08-21'
    date_display: Aug 2022
    codebase_url: https://github.com/Namkyeong/RGRL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.658
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: IGNN
    model_plain: IGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.06211'
    title: Implicit Graph Neural Networks
    date: Sep 14, 2020
    date_iso: '2020-09-14'
    date_display: Sep 2020
    codebase_url: https://github.com/SwiftieH/IGNN
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.655
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: GCL
    model_plain: GCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.12547'
    title: Geometry Contrastive Learning on Heterogeneous Graphs
    date: Jun 25, 2022
    date_iso: '2022-06-25'
    date_display: Jun 2022
    codebase_url: https://github.com/hete-graph/CMHG
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6514
    - null
    - null
    - null
    metric_stds:
    - 0.0047
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
    arxiv_id: '2112.14936'
    title: Heterogeneous Graph Benchmarks
    date: Aug 14, 2021
    date_iso: '2021-08-14'
    date_display: Aug 2021
    codebase_url: https://github.com/THUDM/HGB
    published_conference: KDD 2021
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6514
    - null
    - null
    - null
    metric_stds:
    - 0.0045
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
    arxiv_id: '2112.14936'
    title: Heterogeneous Graph Benchmarks
    date: Aug 14, 2021
    date_iso: '2021-08-14'
    date_display: Aug 2021
    codebase_url: https://github.com/THUDM/HGB
    published_conference: KDD 2021
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6486
    - null
    - null
    - null
    metric_stds:
    - 0.0043
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
    arxiv_id: '2112.14936'
    title: Heterogeneous Graph Benchmarks
    date: Aug 14, 2021
    date_iso: '2021-08-14'
    date_display: Aug 2021
    codebase_url: https://github.com/THUDM/HGB
    published_conference: KDD 2021
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6482
    - null
    - null
    - null
    metric_stds:
    - 0.0064
    - null
    - null
    - null
  - model: DMGI
    model_plain: DMGI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.06211'
    title: Implicit Graph Neural Networks
    date: Sep 14, 2020
    date_iso: '2020-09-14'
    date_display: Sep 2020
    codebase_url: https://github.com/SwiftieH/IGNN
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.648
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: EM-GCN[PT]
    model_plain: EM-GCN[PT]
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.16401'
    title: Graph Neural Networks with a Distribution of Parametrized Graphs
    date: Oct 25, 2023
    date_iso: '2023-10-25'
    date_display: Oct 2023
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6478
    - null
    - null
    - null
    metric_stds:
    - 0.0124
    - null
    - null
    - null
  - model: MAGNN
    model_plain: MAGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.14936'
    title: Heterogeneous Graph Benchmarks
    date: Aug 14, 2021
    date_iso: '2021-08-14'
    date_display: Aug 2021
    codebase_url: https://github.com/THUDM/HGB
    published_conference: KDD 2021
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6467
    - null
    - null
    - null
    metric_stds:
    - 0.0167
    - null
    - null
    - null
  - model: HAN
    model_plain: HAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.14936'
    title: Heterogeneous Graph Benchmarks
    date: Aug 14, 2021
    date_iso: '2021-08-14'
    date_display: Aug 2021
    codebase_url: https://github.com/THUDM/HGB
    published_conference: KDD 2021
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6463
    - null
    - null
    - null
    metric_stds:
    - 0.0058
    - null
    - null
    - null
  - model: R-HGNN
    model_plain: R-HGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2105.11122'
    title: Heterogeneous Graph Representation Learning with Relation Awareness
    date: May 24, 2021
    date_iso: '2021-05-24'
    date_display: May 2021
    codebase_url: https://github.com/yule-BUAA/R-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6417
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: GRACE
    model_plain: GRACE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.12547'
    title: Geometry Contrastive Learning on Heterogeneous Graphs
    date: Jun 25, 2022
    date_iso: '2022-06-25'
    date_display: Jun 2022
    codebase_url: https://github.com/hete-graph/CMHG
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6407
    - null
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
    - null
  - model: AM-GCN
    model_plain: AM-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.64
    - null
    - null
    - null
    metric_stds:
    - 0.0013
    - null
    - null
    - null
  - model: space4HGNN
    model_plain: space4HGNN
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
    - 0.6396
    - null
    - null
    - null
    metric_stds:
    - 0.0043
    - null
    - null
    - null
  row_count: 230
  rows_json: /data/datasets/imdb/standard-split-rows.json
  chart_json: /data/datasets/imdb/standard-split-chart.json
  arch_counts:
    gnn: 139
    hybrid: 33
    graph_transformer: 9
    llm: 3
    walk: 8
    traditional: 15
  metric_counts:
  - 166
  - 31
  - 33
  - 10
  milestones: &id001
  - value: 0.655
    std: null
    model: IGNN
    arxiv_id: '2009.06211'
    title: Implicit Graph Neural Networks
    date: '2020-09-14'
  - value: 0.6736
    std: 0.0057
    model: Simple-HGN
    arxiv_id: '2112.14936'
    title: Heterogeneous Graph Benchmarks
    date: '2021-08-14'
  - value: 0.6917
    std: 0.0043
    model: SeHGNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: '2022-07-06'
  - value: 0.782
    std: 0.0138
    model: MHGCN
    arxiv_id: '2208.06129'
    title: Multiplex Heterogeneous Graph Convolutional Network
    date: '2022-08-12'
  - value: 0.793
    std: 0.001
    model: ELLA
    arxiv_id: '2511.17923'
    title: Towards Efficient LLM-aware Heterogeneous Graph Learning
    date: '2025-11-22'
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

