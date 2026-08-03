---
title: Film
slug: film
benchmark: Heterophilic Graphs
task_type: node_classification
description: Film (Actor) co-occurrence node classification (5 classes). Same graph
  as Actor; referred to as "Film" in some papers.
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.Actor.html
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 5
result_count: 92
best_model:
  model: DoG
  value: 0.432
  metric: Accuracy
  arxiv_id: '2503.12563'
  paper_title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
papers:
- arxiv_id: '2605.21247'
  title: Graph Navier–Stokes Networks
  date_iso: '2026-05-20'
  venue: ''
- arxiv_id: '2603.09195'
  title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
  date_iso: '2026-03-10'
  venue: ''
- arxiv_id: '2511.13937'
  title: 'Complex-Weighted Convolutional Networks: Provable Expressiveness via Complex
    Diffusion'
  date_iso: '2025-11-17'
  venue: LoG 2025
- arxiv_id: '2505.11346'
  title: What Can We Learn From MIMO Graph Convolutions?
  date_iso: '2025-05-16'
  venue: IJCAI 2025
- arxiv_id: '2504.13426'
  title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
  date_iso: '2025-04-18'
  venue: ''
- arxiv_id: '2503.12563'
  title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
  date_iso: '2025-03-16'
  venue: TMLR 2025
- arxiv_id: '2406.10871'
  title: Graph Neural Reaction Diffusion Models Submitted to the editors June 2023.
    Accepted in March 2024.
  date_iso: '2024-06-16'
  venue: ''
- arxiv_id: '2404.17099'
  title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
    with FROND
  date_iso: '2024-04-26'
  venue: ICLR 2024
- arxiv_id: '2403.20221'
  title: Graph Neural Aggregation-diffusion with Metastability
  date_iso: '2024-03-29'
  venue: ''
- arxiv_id: '2402.15326'
  title: Understanding Oversmoothing in Diffusion-Based GNNs From the Perspective
    of Operator Semigroup Theory
  date_iso: '2024-02-23'
  venue: KDD 2024
- arxiv_id: '2402.14393'
  title: Graph Parsing Networks
  date_iso: '2024-02-22'
  venue: ICLR 2024
- arxiv_id: '2307.16092'
  title: Feature Transportation Improves Graph Neural Networks
  date_iso: '2023-07-29'
  venue: AAAI 2023
- arxiv_id: '2211.14208'
  title: 'GREAD: Graph Neural Reaction-Diffusion Networks'
  date_iso: '2022-11-25'
  venue: ICML 2022
- arxiv_id: '2210.00513'
  title: Gradient Gating for Deep Multi-Rate Learning on Graphs
  date_iso: '2022-10-02'
  venue: ICLR 2022
- arxiv_id: '2206.10991'
  title: Understanding convolution on graphs via energies
  date_iso: '2022-06-22'
  venue: TMLR 2022
- arxiv_id: '2205.07308'
  title: Finding Global Homophily in Graph Neural Networks When Meeting Heterophily
  date_iso: '2022-05-15'
  venue: ICML 2022
- arxiv_id: '1609.04508'
  title: Column Networks for Collective Classification
  date_iso: '2016-09-15'
  venue: AAAI 2016
variants:
- slug: standard-split
  name: Standard split
  notes: Geom-GCN 10 fixed splits.
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: 5
  metrics:
  - Accuracy
  - Micro-F1
  metric_display_names:
  - Accuracy
  - Micro-F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: DoG
    model_plain: DoG
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_iso: '2025-03-16'
    date_display: Mar 2025
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.432
    - null
    metric_stds:
    - 0.012
    - null
  - model: P^2GNN
    model_plain: P^2GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_iso: '2026-03-10'
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
    - 0.4305
    - null
    metric_stds:
    - 0.0134
    - null
  - model: VR-GNN
    model_plain: VR-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_iso: '2026-03-10'
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
    - 0.4216
    - null
    metric_stds:
    - 0.0042
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
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_iso: '2026-03-10'
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
    - 0.4179
    - null
    metric_stds:
    - 0.0101
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
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_iso: '2025-03-16'
    date_display: Mar 2025
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.416
    - null
    metric_stds:
    - 0.011
    - null
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_iso: '2026-03-10'
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
    - 0.4082
    - null
    metric_stds:
    - 0.0179
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
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_iso: '2026-03-10'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.393
    - null
    metric_stds:
    - 0.0027
    - null
  - model: ADR-GNN_S
    model_plain: ADR-GNN_S
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.16092'
    title: Feature Transportation Improves Graph Neural Networks
    date: Jul 29, 2023
    date_iso: '2023-07-29'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3916
    - null
    metric_stds:
    - 0.0113
    - null
  - model: GNSN
    model_plain: GNSN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.21247'
    title: Graph Navier–Stokes Networks
    date: May 20, 2026
    date_iso: '2026-05-20'
    date_display: May 2026
    codebase_url: https://github.com/Duckbluee/Graph-Navier-Stokes-Networks
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3888
    - null
    metric_stds:
    - 0.0082
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
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_iso: '2026-03-10'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3885
    - null
    metric_stds:
    - 0.0117
    - null
  - model: GloGNN
    model_plain: GloGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_iso: '2026-03-10'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.388
    - null
    metric_stds:
    - 0.013
    - null
  - model: RDGNN-I
    model_plain: RDGNN-I
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.10871'
    title: Graph Neural Reaction Diffusion Models Submitted to the editors June 2023.
      Accepted in March 2024.
    date: Jun 16, 2024
    date_iso: '2024-06-16'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3869
    - null
    metric_stds:
    - 0.0141
    - null
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_iso: '2026-03-10'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3858
    - null
    metric_stds:
    - 0.0025
    - null
  - model: RDGNN-S
    model_plain: RDGNN-S
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.10871'
    title: Graph Neural Reaction Diffusion Models Submitted to the editors June 2023.
      Accepted in March 2024.
    date: Jun 16, 2024
    date_iso: '2024-06-16'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3855
    - null
    metric_stds:
    - 0.0134
    - null
  - model: F-GREAD-BS
    model_plain: F-GREAD-BS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.17099'
    title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
      with FROND
    date: Apr 26, 2024
    date_iso: '2024-04-26'
    date_display: Apr 2024
    codebase_url: https://github.com/zknus/ICLR2024-FROND
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3828
    - null
    metric_stds:
    - 0.0074
    - null
  - model: GPN
    model_plain: GPN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.14393'
    title: Graph Parsing Networks
    date: Feb 22, 2024
    date_iso: '2024-02-22'
    date_display: Feb 2024
    codebase_url: https://github.com/LUMIA-Group/GraphParsingNetworks
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3811
    - null
    metric_stds:
    - 0.0123
    - null
  - model: GREAD-BS
    model_plain: GREAD-BS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.14208'
    title: 'GREAD: Graph Neural Reaction-Diffusion Networks'
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/jeongwhanchoi/GREAD
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.379
    - null
    metric_stds:
    - 0.0117
    - null
  - model: Sheaf(max)
    model_plain: Sheaf(max)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.10991'
    title: Understanding convolution on graphs via energies
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/JRowbottomGit/graff
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3781
    - null
    metric_stds:
    - 0.0115
    - null
  - model: Sheaf
    model_plain: Sheaf
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.14208'
    title: 'GREAD: Graph Neural Reaction-Diffusion Networks'
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/jeongwhanchoi/GREAD
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3781
    - null
    metric_stds:
    - 0.0115
    - null
  - model: SCN
    model_plain: SCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2511.13937'
    title: 'Complex-Weighted Convolutional Networks: Provable Expressiveness via Complex
      Diffusion'
    date: Nov 17, 2025
    date_iso: '2025-11-17'
    date_display: Nov 2025
    codebase_url: https://github.com/clopezamado/complex-weighted-convolutional-networks.git
    published_conference: LoG 2025
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3781
    - null
    metric_stds:
    - 0.0115
    - null
  - model: NSD
    model_plain: NSD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.16092'
    title: Feature Transportation Improves Graph Neural Networks
    date: Jul 29, 2023
    date_iso: '2023-07-29'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3779
    - null
    metric_stds:
    - 0.0115
    - null
  - model: Ours-Expn
    model_plain: Ours-Expn
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.15326'
    title: Understanding Oversmoothing in Diffusion-Based GNNs From the Perspective
      of Operator Semigroup Theory
    date: Feb 23, 2024
    date_iso: '2024-02-23'
    date_display: Feb 2024
    codebase_url: https://github.com/LOGO-CUHKSZ/SGOS
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3779
    - null
    metric_stds:
    - 0.0086
    - null
  - model: GREAD-FB
    model_plain: GREAD-FB*
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.14208'
    title: 'GREAD: Graph Neural Reaction-Diffusion Networks'
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/jeongwhanchoi/GREAD
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.377
    - null
    metric_stds:
    - 0.0051
    - null
  - model: GREAD-ST
    model_plain: GREAD-ST
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.14208'
    title: 'GREAD: Graph Neural Reaction-Diffusion Networks'
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/jeongwhanchoi/GREAD
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3766
    - null
    metric_stds:
    - 0.009
    - null
  - model: GREAD
    model_plain: GREAD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.15326'
    title: Understanding Oversmoothing in Diffusion-Based GNNs From the Perspective
      of Operator Semigroup Theory
    date: Feb 23, 2024
    date_iso: '2024-02-23'
    date_display: Feb 2024
    codebase_url: https://github.com/LOGO-CUHKSZ/SGOS
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3759
    - null
    metric_stds:
    - 0.0106
    - null
  - model: Ours-Log
    model_plain: Ours-Log
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.15326'
    title: Understanding Oversmoothing in Diffusion-Based GNNs From the Perspective
      of Operator Semigroup Theory
    date: Feb 23, 2024
    date_iso: '2024-02-23'
    date_display: Feb 2024
    codebase_url: https://github.com/LOGO-CUHKSZ/SGOS
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3755
    - null
    metric_stds:
    - 0.008
    - null
  - model: GGCN
    model_plain: GGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.10991'
    title: Understanding convolution on graphs via energies
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/JRowbottomGit/graff
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3754
    - null
    metric_stds:
    - 0.0156
    - null
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.10991'
    title: Understanding convolution on graphs via energies
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/JRowbottomGit/graff
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3744
    - null
    metric_stds:
    - 0.013
    - null
  - model: Ours-Exp
    model_plain: Ours-Exp
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.15326'
    title: Understanding Oversmoothing in Diffusion-Based GNNs From the Perspective
      of Operator Semigroup Theory
    date: Feb 23, 2024
    date_iso: '2024-02-23'
    date_display: Feb 2024
    codebase_url: https://github.com/LOGO-CUHKSZ/SGOS
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3737
    - null
    metric_stds:
    - 0.0117
    - null
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
    - 0.3735
    - null
    metric_stds:
    - null
    - null
  - model: G^2
    model_plain: G^2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.16092'
    title: Feature Transportation Improves Graph Neural Networks
    date: Jul 29, 2023
    date_iso: '2023-07-29'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.373
    - null
    metric_stds:
    - 0.0101
    - null
  - model: G2
    model_plain: G2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.10871'
    title: Graph Neural Reaction Diffusion Models Submitted to the editors June 2023.
      Accepted in March 2024.
    date: Jun 16, 2024
    date_iso: '2024-06-16'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.373
    - null
    metric_stds:
    - 0.0101
    - null
  - model: G^2-GAT
    model_plain: G^2-GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.373
    - null
    metric_stds:
    - 0.0087
    - null
  - model: GREAD-AC
    model_plain: GREAD-AC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.14208'
    title: 'GREAD: Graph Neural Reaction-Diffusion Networks'
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/jeongwhanchoi/GREAD
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3721
    - null
    metric_stds:
    - 0.011
    - null
  - model: G^2-GraphSAGE
    model_plain: G^2-GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3714
    - null
    metric_stds:
    - 0.0101
    - null
  - model: GRAFF
    model_plain: GRAFF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.10991'
    title: Understanding convolution on graphs via energies
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/JRowbottomGit/graff
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3711
    - null
    metric_stds:
    - 0.0108
    - null
  - model: ACMII-GCN
    model_plain: ACMII-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.16092'
    title: Feature Transportation Improves Graph Neural Networks
    date: Jul 29, 2023
    date_iso: '2023-07-29'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3709
    - null
    metric_stds:
    - 0.0132
    - null
  - model: G^2-GCN
    model_plain: G^2-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3709
    - null
    metric_stds:
    - 0.0116
    - null
  - model: GREAD-Z
    model_plain: GREAD-Z
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.14208'
    title: 'GREAD: Graph Neural Reaction-Diffusion Networks'
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/jeongwhanchoi/GREAD
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3701
    - null
    metric_stds:
    - 0.0111
    - null
  - model: GRADE-GAT
    model_plain: GRADE-GAT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.20221'
    title: Graph Neural Aggregation-diffusion with Metastability
    date: Mar 29, 2024
    date_iso: '2024-03-29'
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
    - 0.368
    - null
    metric_stds:
    - 0.011
    - null
  - model: GREAD-F
    model_plain: GREAD-F
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.14208'
    title: 'GREAD: Graph Neural Reaction-Diffusion Networks'
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/jeongwhanchoi/GREAD
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3672
    - null
    metric_stds:
    - 0.0066
    - null
  - model: F^2GAT
    model_plain: F^2GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3665
    - null
    metric_stds:
    - 0.0113
    - null
  - model: WRGAT
    model_plain: WRGAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.16092'
    title: Feature Transportation Improves Graph Neural Networks
    date: Jul 29, 2023
    date_iso: '2023-07-29'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3653
    - null
    metric_stds:
    - 0.0077
    - null
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.10991'
    title: Understanding convolution on graphs via energies
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/JRowbottomGit/graff
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3653
    - null
    metric_stds:
    - 0.007
    - null
  - model: CWCN
    model_plain: CWCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2511.13937'
    title: 'Complex-Weighted Convolutional Networks: Provable Expressiveness via Complex
      Diffusion'
    date: Nov 17, 2025
    date_iso: '2025-11-17'
    date_display: Nov 2025
    codebase_url: https://github.com/clopezamado/complex-weighted-convolutional-networks.git
    published_conference: LoG 2025
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3651
    - null
    metric_stds:
    - 0.0126
    - null
  - model: LMGC
    model_plain: LMGC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11346'
    title: What Can We Learn From MIMO Graph Convolutions?
    date: May 16, 2025
    date_iso: '2025-05-16'
    date_display: May 2025
    codebase_url: https://github.com/roth-andreas/mimo-graph-convolutions
    published_conference: IJCAI 2025
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.363
    - null
    metric_stds:
    - 0.004
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
    arxiv_id: '2211.14208'
    title: 'GREAD: Graph Neural Reaction-Diffusion Networks'
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/jeongwhanchoi/GREAD
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3628
    - null
    metric_stds:
    - 0.0109
    - null
  - model: RF-GCN
    model_plain: RF-GCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_iso: '2025-04-18'
    date_display: Apr 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3618
    - null
    metric_stds:
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
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.361
    - null
    metric_stds:
    - 0.0155
    - null
  - model: LINX
    model_plain: LINX
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.21247'
    title: Graph Navier–Stokes Networks
    date: May 20, 2026
    date_iso: '2026-05-20'
    date_display: May 2026
    codebase_url: https://github.com/Duckbluee/Graph-Navier-Stokes-Networks
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.361
    - null
    metric_stds:
    - 0.0155
    - null
  row_count: 92
  rows_json: /data/datasets/film/standard-split-rows.json
  chart_json: /data/datasets/film/standard-split-chart.json
  arch_counts:
    gnn: 66
    hybrid: 19
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 5
  metric_counts:
  - 85
  - 7
  milestones: &id001
  - value: 0.3781
    std: 0.0115
    model: Sheaf(max)
    arxiv_id: '2206.10991'
    title: Understanding convolution on graphs via energies
    date: '2022-06-22'
  - value: 0.379
    std: 0.0117
    model: GREAD-BS
    arxiv_id: '2211.14208'
    title: 'GREAD: Graph Neural Reaction-Diffusion Networks'
    date: '2022-11-25'
  - value: 0.3916
    std: 0.0113
    model: ADR-GNN_S
    arxiv_id: '2307.16092'
    title: Feature Transportation Improves Graph Neural Networks
    date: '2023-07-29'
  - value: 0.432
    std: 0.012
    model: DoG
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: '2025-03-16'
  milestones_by_metric:
    Accuracy: *id001
    Micro-F1:
    - value: 0.575
      std: null
      model: CLN-HWN-mini
      arxiv_id: '1609.04508'
      title: Column Networks for Collective Classification
      date: '2016-09-15'
---

