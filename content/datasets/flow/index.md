---
title: Flow
slug: flow
benchmark: GraphBench
task_type: graph_regression
short_description: 'Predict one scalar per graph: the maximum feasible flow between
  designated source and sink vertices under the supplied edge capacities.'
description: '**Graph regression** Predict one scalar per graph: the maximum feasible
  flow between designated source and sink vertices under the supplied edge capacities.
  Evaluated by MAE.'
detailed_description:
  task: 'Predict one scalar per graph: the maximum feasible flow between designated
    source and sink vertices under the supplied edge capacities.'
  data: Unique synthetic graphs are drawn from ER, stochastic-block, power-law-cluster,
    Newman-Watts-Strogatz, BA, and dual-BA generators. Generator mixtures define easy,
    medium, and hard distribution shifts.
  features: Edge attributes encode capacities or weights needed by the flow problem,
    while node information identifies source and sink. The target is the NetworkX
    reference maximum-flow value.
  splits_and_evaluation: Each difficulty provides one million 16-node training graphs
    plus 10,000 validation and 10,000 128-node test graphs. Graph-level MAE is the
    metric under the fixed 98/1/1 split.
  quirks_and_pitfalls: GraphBench omits flow from its 128-to-512-node size study because
    target magnitude, and therefore raw MAE, scales with network size. Capacity distribution
    and generator shift must be held fixed when comparing errors.
sources:
- title: GraphBench
  arxiv_id: '2512.04475'
  kind: benchmark_definition
- title: A New Approach to the Maximum-Flow Problem
  url: https://doi.org/10.1145/12130.12144
  kind: algorithm_source
primary_metric: MAE
higher_is_better: false
pyg_url: https://graphbench.github.io/website/datasets.html
stats:
  num_graphs: 1020000
  avg_nodes: 17.1
  avg_edges: 48.27
  num_classes: null
  extra_stats:
    avg_degree: 5.64
    edge_feature_dim: 1
    edge_feature_type: capacity
    feature_type: source/sink indicators
    node_feature_dim: 1
    statistic_notes: GraphBench Table 2 reports 16-node training/validation and 64-node
      test regimes for Flow.
result_count: 5
best_model:
  model: RRWP
  value: 1.45
  metric: MAE
  arxiv_id: '2511.08028'
  paper_title: Generalizable Insights for Graph Transformers in Theory and Practice
papers:
- arxiv_id: '2511.08028'
  title: Generalizable Insights for Graph Transformers in Theory and Practice
  date_iso: '2025-11-11'
  venue: NeurIPS 2025
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: MAE
  default_metric: MAE
  higher_is_better: false
  stats:
    num_graphs: 1020000
    avg_nodes: 17.1
    avg_edges: 48.27
    num_classes: null
    extra_stats:
      avg_degree: 5.64
      edge_feature_dim: 1
      edge_feature_type: capacity
      feature_type: source/sink indicators
      node_feature_dim: 1
      statistic_notes: GraphBench Table 2 reports 16-node training/validation and
        64-node test regimes for Flow.
  metrics:
  - MAE
  metric_display_names:
  - MAE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: RRWP
    model_plain: RRWP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.45
    metric_stds:
    - 0.06
  - model: RWSE
    model_plain: RWSE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.49
    metric_stds:
    - 0.02
  - model: NoPE
    model_plain: NoPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.73
    metric_stds:
    - 0.09
  - model: LPE
    model_plain: LPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.75
    metric_stds:
    - 0.12
  - model: SPE
    model_plain: SPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.98
    metric_stds:
    - 0.14
  row_count: 5
  rows_json: ''
  chart_json: /data/datasets/flow/standard-split-chart.json
  arch_counts:
    gnn: 0
    hybrid: 0
    graph_transformer: 5
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 5
  milestones: &id001
  - value: 1.45
    std: 0.06
    model: RRWP
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: '2025-11-11'
  milestones_by_metric:
    MAE: *id001
---

