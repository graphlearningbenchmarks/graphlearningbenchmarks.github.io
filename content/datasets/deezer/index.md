---
title: Deezer
slug: deezer
benchmark: Heterophilic Graphs
task_type: node_classification
description: Deezer Europe user friendship graph binary node classification (like/dislike)
  from the heterophilic benchmark.
primary_metric: ROC-AUC
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.HeterophilousGraphDataset.html
stats:
  num_graphs: 1
  avg_nodes: 28281.0
  avg_edges: 1650703.0
  num_classes: 2
result_count: 19
best_model:
  model: CLP
  value: 0.6569
  metric: Accuracy
  arxiv_id: '2205.09389'
  paper_title: Simplifying Node Classification on Heterophilous Graphs with Compatible
    Label Propagation
papers:
- arxiv_id: '2604.19028'
  title: Learning Posterior Predictive Distributions for Node Classification from
    Synthetic Graph Priors
  date_iso: '2026-04-21'
  venue: ICLR 2026
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
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 28281.0
    avg_edges: 1650703.0
    num_classes: 2
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.6569
    metric_stds:
    - 0.0032
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.6504
    metric_stds:
    - 0.0045
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
    - 0.6495
    metric_stds:
    - 0.0039
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
    - 0.6416
    metric_stds:
    - 0.0085
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
    - 0.6392
    metric_stds:
    - 0.0071
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
    - 0.6377
    metric_stds:
    - 0.003
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
    - 0.6282
    metric_stds:
    - 0.0068
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
    - 0.6274
    metric_stds:
    - 0.0039
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
    - 0.6233
    metric_stds:
    - 0.0081
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
    - 0.5994
    metric_stds:
    - 0.0055
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
    - 0.5707
    metric_stds:
    - 0.0064
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
    - 0.5599
    metric_stds:
    - 0.0378
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
    - 0.5595
    metric_stds:
    - 0.0034
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
    - 0.5544
    metric_stds:
    - 0.0046
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
    - 0.5424
    metric_stds:
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
    - 0.5369
    metric_stds:
    - 0.0229
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
    - 0.5345
    metric_stds:
    - 0.0065
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
    - 0.5213
    metric_stds:
    - 0.0302
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
    - 0.2434
    metric_stds:
    - 0.0121
  row_count: 19
  rows_json: ''
  chart_json: /data/datasets/deezer/standard-split-chart.json
  arch_counts:
    gnn: 13
    hybrid: 3
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 3
  metric_counts:
  - 19
  milestones: &id001
  - value: 0.6569
    std: 0.0032
    model: CLP
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: '2022-05-19'
  milestones_by_metric:
    Accuracy: *id001
---

