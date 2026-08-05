---
title: Deezer
slug: deezer
benchmark: LINKX Benchmarks
task_type: node_classification
description: Deezer Europe user friendship graph binary node classification (like/dislike),
  used in LINKX-style non-homophily evaluations.
primary_metric: ROC-AUC
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.HeterophilousGraphDataset.html
stats:
  num_graphs: 1
  avg_nodes: 28281.0
  avg_edges: 1650703.0
  num_classes: 2
result_count: 34
best_model:
  model: GPM
  value: 0.6726
  metric: ROC-AUC
  arxiv_id: '2501.18739'
  paper_title: 'Beyond Message Passing: Neural Graph Pattern Machine'
papers:
- arxiv_id: '2604.19028'
  title: Learning Posterior Predictive Distributions for Node Classification from
    Synthetic Graph Priors
  date_iso: '2026-04-21'
  venue: ICLR 2026
- arxiv_id: '2501.18739'
  title: 'Beyond Message Passing: Neural Graph Pattern Machine'
  date_iso: '2025-01-30'
  venue: ICML 2025
- arxiv_id: '2205.09389'
  title: Simplifying Node Classification on Heterophilous Graphs with Compatible Label
    Propagation
  date_iso: '2022-05-19'
  venue: TMLR 2022
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: ROC-AUC
  default_metric: ROC-AUC
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 28281.0
    avg_edges: 1650703.0
    num_classes: 2
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.6726
    - null
    metric_stds:
    - 0.0022
    - null
  - model: NodeFormer
    model_plain: NodeFormer
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.664
    - null
    metric_stds:
    - 0.007
    - null
  - model: OrderedGNN
    model_plain: OrderedGNN
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
    - 0.6612
    - null
    metric_stds:
    - 0.0075
    - null
  - model: APPNP
    model_plain: APPNP
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
    - 0.661
    - null
    metric_stds:
    - 0.006
    - null
  - model: NAGphormer
    model_plain: NAGphormer
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
    - 0.6554
    - null
    metric_stds:
    - 0.0057
    - null
  - model: GOAT
    model_plain: GOAT
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
    - 0.6531
    - null
    metric_stds:
    - 0.0024
    - null
  - model: VCR-Graphormer
    model_plain: VCR-Graphormer
    is_baseline: true
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
    - 0.6528
    - null
    metric_stds:
    - 0.0051
    - null
  - model: GCFormer
    model_plain: GCFormer
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
    - 0.6516
    - null
    metric_stds:
    - 0.0033
    - null
  - model: RAW-GNN
    model_plain: RAW-GNN
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
    - 0.6511
    - null
    metric_stds:
    - 0.0064
    - null
  - model: SAN
    model_plain: SAN
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
    - 0.6429
    - null
    metric_stds:
    - 0.0035
    - null
  - model: RUM
    model_plain: RUM
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
    - 0.6425
    - null
    metric_stds:
    - 0.0062
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
    - 0.632
    - null
    metric_stds:
    - 0.0084
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
    - 0.627
    - null
    metric_stds:
    - 0.007
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
    - 0.617
    - null
    metric_stds:
    - 0.008
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
    - 0.6056
    - null
    metric_stds:
    - 0.0062
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
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.6377
    metric_stds:
    - null
    - 0.003
  - model: LINK
    model_plain: LINK
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5595
    metric_stds:
    - null
    - 0.0034
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5994
    metric_stds:
    - null
    - 0.0055
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.2434
    metric_stds:
    - null
    - 0.0121
  - model: GCN2
    model_plain: GCN2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.6233
    metric_stds:
    - null
    - 0.0081
  - model: MixHop
    model_plain: MixHop
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.6416
    metric_stds:
    - null
    - 0.0085
  - model: SuperGAT
    model_plain: SuperGAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5707
    metric_stds:
    - null
    - 0.0064
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.6274
    metric_stds:
    - null
    - 0.0039
  - model: FAGCN
    model_plain: FAGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.6504
    metric_stds:
    - null
    - 0.0045
  - model: H2GCN
    model_plain: H2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.6282
    metric_stds:
    - null
    - 0.0068
  - model: CPGNN
    model_plain: CPGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.6495
    metric_stds:
    - null
    - 0.0039
  - model: LP
    model_plain: LP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5544
    metric_stds:
    - null
    - 0.0046
  - model: C&S
    model_plain: C&S
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.6392
    metric_stds:
    - null
    - 0.0071
  - model: CLP
    model_plain: CLP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.6569
    metric_stds:
    - null
    - 0.0032
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2604.19028'
    title: Learning Posterior Predictive Distributions for Node Classification from
      Synthetic Graph Priors
    date: Apr 21, 2026
    date_iso: '2026-04-21'
    date_display: Apr 2026
    codebase_url: https://github.com/jeongwhanchoi/NodePFN
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5424
    metric_stds:
    - null
    - 0.0215
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.19028'
    title: Learning Posterior Predictive Distributions for Node Classification from
      Synthetic Graph Priors
    date: Apr 21, 2026
    date_iso: '2026-04-21'
    date_display: Apr 2026
    codebase_url: https://github.com/jeongwhanchoi/NodePFN
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5369
    metric_stds:
    - null
    - 0.0229
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.19028'
    title: Learning Posterior Predictive Distributions for Node Classification from
      Synthetic Graph Priors
    date: Apr 21, 2026
    date_iso: '2026-04-21'
    date_display: Apr 2026
    codebase_url: https://github.com/jeongwhanchoi/NodePFN
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5599
    metric_stds:
    - null
    - 0.0378
  - model: GraphAny(Wisconsin)
    model_plain: GraphAny(Wisconsin)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.19028'
    title: Learning Posterior Predictive Distributions for Node Classification from
      Synthetic Graph Priors
    date: Apr 21, 2026
    date_iso: '2026-04-21'
    date_display: Apr 2026
    codebase_url: https://github.com/jeongwhanchoi/NodePFN
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5213
    metric_stds:
    - null
    - 0.0302
  - model: NodePFN
    model_plain: NodePFN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.19028'
    title: Learning Posterior Predictive Distributions for Node Classification from
      Synthetic Graph Priors
    date: Apr 21, 2026
    date_iso: '2026-04-21'
    date_display: Apr 2026
    codebase_url: https://github.com/jeongwhanchoi/NodePFN
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5345
    metric_stds:
    - null
    - 0.0065
  row_count: 34
  rows_json: ''
  chart_json: /data/datasets/deezer/standard-split-chart.json
  arch_counts:
    gnn: 20
    hybrid: 6
    graph_transformer: 5
    llm: 0
    walk: 0
    traditional: 3
  metric_counts:
  - 15
  - 19
  milestones: &id001
  - value: 0.6726
    std: 0.0022
    model: GPM
    arxiv_id: '2501.18739'
    title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    date: '2025-01-30'
  milestones_by_metric:
    ROC-AUC: *id001
    Accuracy:
    - value: 0.6569
      std: 0.0032
      model: CLP
      arxiv_id: '2205.09389'
      title: Simplifying Node Classification on Heterophilous Graphs with Compatible
        Label Propagation
      date: '2022-05-19'
---

