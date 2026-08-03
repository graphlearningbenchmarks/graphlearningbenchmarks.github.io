---
title: House
slug: house
benchmark: Hypergraph Benchmarks
task_type: node_classification
description: US House of Representatives voting hypergraph node classification (2
  classes).
primary_metric: Accuracy
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 1
  avg_nodes: null
  avg_edges: null
  num_classes: 2
result_count: 44
best_model:
  model: HealHGNN
  value: 0.7718
  metric: Accuracy
  arxiv_id: '2603.00599'
  paper_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local
    Exchanger
papers:
- arxiv_id: '2603.00599'
  title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
  date_iso: '2026-02-28'
  venue: ''
- arxiv_id: '2308.10077'
  title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
    Views
  date_iso: '2023-08-19'
  venue: ''
- arxiv_id: '2202.09025'
  title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
  date_iso: '2022-02-18'
  venue: ICLR 2022
- arxiv_id: '2106.13264'
  title: Hypergraph Benchmarks
  date_iso: '2021-06-24'
  venue: ICLR 2021
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
    avg_nodes: null
    avg_edges: null
    num_classes: 2
  metrics:
  - Accuracy
  - Completeness
  - Homogeneity
  - Silhouette
  metric_display_names:
  - Accuracy
  - Completeness
  - Homogeneity
  - Silhouette
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: HealHGNN
    model_plain: HealHGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7718
    - null
    - null
    - null
    metric_stds:
    - 0.0235
    - null
    - null
    - null
  - model: Deep-HGNN
    model_plain: Deep-HGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7526
    - null
    - null
    - null
    metric_stds:
    - 0.0176
    - null
    - null
    - null
  - model: mechanism (shared)
    model_plain: mechanism (shared)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.747
    - null
    - null
    - null
    metric_stds:
    - 0.0756
    - null
    - null
    - null
  - model: KHGNN
    model_plain: KHGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7431
    - null
    - null
    - null
    metric_stds:
    - 0.0287
    - null
    - null
    - null
  - model: SheafHyperGNN
    model_plain: SheafHyperGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7384
    - null
    - null
    - null
    metric_stds:
    - 0.023
    - null
    - null
    - null
  - model: FrameHGNN
    model_plain: FrameHGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7282
    - null
    - null
    - null
    metric_stds:
    - 0.0222
    - null
    - null
    - null
  - model: ED-HNN
    model_plain: ED-HNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
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
    - null
    - null
    metric_stds:
    - 0.0228
    - null
    - null
    - null
  - model: HAN (full batch)
    model_plain: HAN (full batch)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_iso: '2021-06-24'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/AllSet
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7105
    - null
    - null
    - null
    metric_stds:
    - 0.0226
    - null
    - null
    - null
  - model: PhenomNN
    model_plain: PhenomNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7071
    - null
    - null
    - null
    metric_stds:
    - 0.0235
    - null
    - null
    - null
  - model: AllSetTransformer
    model_plain: AllSetTransformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_iso: '2021-06-24'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/AllSet
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6933
    - null
    - null
    - null
    metric_stds:
    - 0.022
    - null
    - null
    - null
  - model: CEGAT
    model_plain: CEGAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_iso: '2021-06-24'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/AllSet
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6909
    - null
    - null
    - null
    metric_stds:
    - 0.03
    - null
    - null
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
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_iso: '2021-06-24'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/AllSet
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6793
    - null
    - null
    - null
    metric_stds:
    - 0.0233
    - null
    - null
    - null
  - model: AllDeepSets
    model_plain: AllDeepSets
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_iso: '2021-06-24'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/AllSet
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6782
    - null
    - null
    - null
    metric_stds:
    - 0.024
    - null
    - null
    - null
  - model: HNHN
    model_plain: HNHN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_iso: '2021-06-24'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/AllSet
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.678
    - null
    - null
    - null
    metric_stds:
    - 0.0259
    - null
    - null
    - null
  - model: UniGCNII
    model_plain: UniGCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_iso: '2021-06-24'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/AllSet
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6725
    - null
    - null
    - null
    metric_stds:
    - 0.0257
    - null
    - null
    - null
  - model: CECGN
    model_plain: CECGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_iso: '2021-06-24'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/AllSet
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.628
    - null
    - null
    - null
    metric_stds:
    - 0.0261
    - null
    - null
    - null
  - model: HGNN
    model_plain: HGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_iso: '2021-06-24'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/AllSet
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6139
    - null
    - null
    - null
    metric_stds:
    - 0.0296
    - null
    - null
    - null
  - model: HCHA
    model_plain: HCHA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_iso: '2021-06-24'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/AllSet
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6136
    - null
    - null
    - null
    metric_stds:
    - 0.0253
    - null
    - null
    - null
  - model: HyperGCN
    model_plain: HyperGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/Mingzhang21/HealHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6013
    - null
    - null
    - null
    metric_stds:
    - 0.0176
    - null
    - null
    - null
  - model: NWR-GAE
    model_plain: NWR-GAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5864
    - null
    - null
    - null
    metric_stds:
    - 0.0561
    - null
    - null
    - null
  - model: MVGRL
    model_plain: MVGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5351
    - null
    - null
    - null
    metric_stds:
    - 0.0326
    - null
    - null
    - null
  - model: VGAE
    model_plain: VGAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4932
    - null
    - null
    - null
    metric_stds:
    - 0.0919
    - null
    - null
    - null
  - model: HyperGCN
    model_plain: HyperGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: Jun 24, 2021
    date_iso: '2021-06-24'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/AllSet
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4831
    - null
    - null
    - null
    metric_stds:
    - 0.0293
    - null
    - null
    - null
  - model: DGI
    model_plain: DGI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4648
    - null
    - null
    - null
    metric_stds:
    - 0.0797
    - null
    - null
    - null
  - model: GraphWave
    model_plain: GraphWave
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4596
    - null
    - null
    - null
    metric_stds:
    - 0.022
    - null
    - null
    - null
  - model: GAE
    model_plain: GAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.454
    - null
    - null
    - null
    metric_stds:
    - 0.0999
    - null
    - null
    - null
  - model: GraphCL
    model_plain: GraphCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4486
    - null
    - null
    - null
    metric_stds:
    - 0.0373
    - null
    - null
    - null
  - model: DeepWalk
    model_plain: DeepWalk
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4121
    - null
    - null
    - null
    metric_stds:
    - 0.034
    - null
    - null
    - null
  - model: ARGVA
    model_plain: ARGVA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4108
    - null
    - null
    - null
    metric_stds:
    - 0.0485
    - null
    - null
    - null
  - model: Node2Vec
    model_plain: Node2Vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4054
    - null
    - null
    - null
    metric_stds:
    - 0.0162
    - null
    - null
    - null
  - model: RolX
    model_plain: RolX
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2567
    - null
    - null
    - null
    metric_stds:
    - 0.1178
    - null
    - null
    - null
  - model: struc2vec
    model_plain: struc2vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: Aug 19, 2023
    date_iso: '2023-08-19'
    date_display: Aug 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2372
    - null
    - null
    - null
    metric_stds:
    - 0.1369
    - null
    - null
    - null
  - model: DeepWalk
    model_plain: DeepWalk
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.01
    - 0.01
    - 0.29
    metric_stds:
    - null
    - null
    - null
    - null
  - model: Node2Vec
    model_plain: Node2Vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.01
    - 0.01
    - 0.33
    metric_stds:
    - null
    - null
    - null
    - null
  - model: RolX
    model_plain: RolX
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 1.0
    - 1.0
    - 0.99
    metric_stds:
    - null
    - null
    - null
    - null
  - model: struc2vec
    model_plain: struc2vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.99
    - 0.99
    - 0.45
    metric_stds:
    - null
    - null
    - null
    - null
  - model: GraphWave
    model_plain: GraphWave
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 1.0
    - 1.0
    - 0.99
    metric_stds:
    - null
    - null
    - null
    - null
  - model: GAE
    model_plain: GAE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 1.0
    - 1.0
    - 0.99
    metric_stds:
    - null
    - null
    - null
    - null
  - model: VGAE
    model_plain: VGAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.27
    - 0.25
    - 0.21
    metric_stds:
    - null
    - null
    - null
    - null
  - model: ARGVA
    model_plain: ARGVA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.28
    - 0.28
    - 0.19
    metric_stds:
    - null
    - null
    - null
    - null
  - model: DGI
    model_plain: DGI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 1.0
    - 1.0
    - 0.99
    metric_stds:
    - null
    - null
    - null
    - null
  - model: GraphCL
    model_plain: GraphCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 1.0
    - 1.0
    - 0.99
    metric_stds:
    - null
    - null
    - null
    - null
  - model: MVGRL
    model_plain: MVGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 1.0
    - 1.0
    - 0.99
    metric_stds:
    - null
    - null
    - null
    - null
  - model: NWR-GAE
    model_plain: NWR-GAE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.09025'
    title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: https://github.com/mtang724/NWR-GAE
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 1.0
    - 1.0
    - 0.99
    metric_stds:
    - null
    - null
    - null
    - null
  row_count: 44
  rows_json: ''
  chart_json: /data/datasets/house/standard-split-chart.json
  arch_counts:
    gnn: 29
    hybrid: 2
    graph_transformer: 1
    llm: 0
    walk: 6
    traditional: 5
  metric_counts:
  - 32
  - 12
  - 12
  - 12
  milestones: &id001
  - value: 0.747
    std: 0.0756
    model: mechanism (shared)
    arxiv_id: '2308.10077'
    title: Contrastive Learning for Non-Local Graphs with Multi-Resolution Structural
      Views
    date: '2023-08-19'
  milestones_by_metric:
    Accuracy: *id001
    Completeness:
    - value: 1.0
      std: null
      model: RolX
      arxiv_id: '2202.09025'
      title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
      date: '2022-02-18'
    Homogeneity:
    - value: 1.0
      std: null
      model: RolX
      arxiv_id: '2202.09025'
      title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
      date: '2022-02-18'
    Silhouette:
    - value: 0.99
      std: null
      model: RolX
      arxiv_id: '2202.09025'
      title: Graph Auto-Encoder Via Neighborhood Wasserstein Reconstruction
      date: '2022-02-18'
---

