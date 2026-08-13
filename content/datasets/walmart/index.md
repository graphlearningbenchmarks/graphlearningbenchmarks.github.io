---
title: Walmart
slug: walmart
benchmark: Hypergraph Benchmarks
task_type: node_classification
short_description: Walmart co-purchase trip hypergraph node classification (product
  category, 11 classes).
description: '**11-class node classification** Walmart co-purchase trip hypergraph
  node classification (product category, 11 classes). Uses node-hyperedge incidence
  and the released node features. Clique expansion changes the input by discarding
  hyperedge identity. Evaluated by Accuracy.'
detailed_description:
  task: Walmart co-purchase trip hypergraph node classification (product category,
    11 classes). The primary catalog metric is Accuracy.
  data: Walmart co-purchase trip hypergraph node classification (product category,
    11 classes). The cataloged artifact reports 1 graphs, 11 target classes or tasks.
  features: The release represents higher-order membership with a node-hyperedge incidence
    relation and supplies node features where available. Some source datasets have
    no measured features and use documented synthetic features; clique expansion is
    an alternative representation that discards hyperedge identity.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses Accuracy (higher is better). Exact masks or folds must
    come from the cited release.'
  quirks_and_pitfalls: Do not silently replace incidence propagation with clique expansion
    or merge distinct releases sharing a short name. Random synthetic features, split
    seeds, hyperedge multiplicity, and isolated-node handling can dominate results
    and must be reported.
sources:
- title: Hypergraph Benchmarks benchmark
  arxiv_id: '2106.13264'
  kind: benchmark_or_upstream_source
primary_metric: Accuracy
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 1
  avg_nodes: null
  avg_edges: null
  num_classes: 11
result_count: 17
best_model:
  model: HealHGNN
  value: 0.6822
  metric: Accuracy
  arxiv_id: '2603.00599'
  paper_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local
    Exchanger
papers:
- arxiv_id: '2603.00599'
  title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
  date_iso: '2026-02-28'
  venue: ''
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
    num_classes: 11
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
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
    - 0.6822
    metric_stds:
    - 0.0056
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
    - 0.6679
    metric_stds:
    - 0.0041
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
    - 0.6546
    metric_stds:
    - 0.0025
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6517
    metric_stds:
    - 0.0079
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
    - 0.6455
    metric_stds:
    - 0.0033
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
    - 0.6343
    metric_stds:
    - 0.0043
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
    - 0.6245
    metric_stds:
    - 0.0026
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
    - 0.62
    metric_stds:
    - 0.0024
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5864
    metric_stds:
    - 0.0074
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
    - 0.5445
    metric_stds:
    - 0.0037
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
    - 0.5444
    metric_stds:
    - 0.0024
  - model: HNHN
    model_plain: HNHN
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
    - 0.5118
    metric_stds:
    - 0.0035
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
    - 0.5114
    metric_stds:
    - 0.0056
  - model: HAN (mini batch)
    model_plain: HAN (mini batch)
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
    - 0.4857
    metric_stds:
    - 0.0104
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
    - 0.4718
    metric_stds:
    - 0.0035
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
    - 0.4551
    metric_stds:
    - 0.0024
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
    - 0.4474
    metric_stds:
    - 0.0281
  row_count: 17
  rows_json: ''
  chart_json: /data/datasets/walmart/standard-split-chart.json
  arch_counts:
    gnn: 15
    hybrid: 0
    graph_transformer: 1
    llm: 0
    walk: 0
    traditional: 1
  metric_counts:
  - 17
  milestones: &id001
  - value: 0.6546
    std: 0.0025
    model: AllSetTransformer
    arxiv_id: '2106.13264'
    title: Hypergraph Benchmarks
    date: '2021-06-24'
  - value: 0.6822
    std: 0.0056
    model: HealHGNN
    arxiv_id: '2603.00599'
    title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian Local Exchanger
    date: '2026-02-28'
  milestones_by_metric:
    Accuracy: *id001
---

