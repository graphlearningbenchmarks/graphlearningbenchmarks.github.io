---
title: BA graph
slug: ba-graph
benchmark: GraphBench
task_type: graph_regression
short_description: Predict optimal objectives or decode feasible MIS, max-cut, and
  coloring solutions on Barabási–Albert graphs.
description: '**Graph regression** Predict an optimal combinatorial-objective value
  in the supervised protocol, or learn node scores that a problem-specific decoder
  turns into a feasible solution in the unsupervised protocol. Evaluated by MAE.'
detailed_description:
  task: Predict an optimal combinatorial-objective value in the supervised protocol,
    or learn node scores that a problem-specific decoder turns into a feasible solution
    in the unsupervised protocol. GraphBench covers maximum independent set, max-cut,
    and graph coloring.
  data: Synthetic Barabási–Albert preferential-attachment graphs are generated in
    small and large regimes. The generator controls graph size and the number of edges
    attached by each newly added node; GraphBench reports 50,000 instances per dataset.
  features: The released problem graphs contain no node or edge features. Their topology
    is the input; labels or training losses depend on the selected optimization problem
    and protocol.
  splits_and_evaluation: Supervised experiments predict the solver-derived optimum
    and report MAE. Unsupervised experiments minimize a differentiable surrogate,
    decode node scores to a feasible solution, and evaluate that solution's objective
    value.
  quirks_and_pitfalls: BA graph names a graph generator, not one classification target.
    Results must identify the optimization problem, small or large regime, and supervised
    or unsupervised protocol. Solver-derived labels become expensive and potentially
    status-dependent for hard instances.
sources:
- title: GraphBench
  arxiv_id: '2512.04475'
  kind: benchmark_definition
- title: Emergence of Scaling in Random Networks
  url: https://doi.org/10.1126/science.286.5439.509
  kind: generator_origin
primary_metric: MAE
higher_is_better: true
pyg_url: https://graphbench.github.io/website/datasets.html
stats:
  num_graphs: 100000
  avg_nodes: 500.0
  avg_edges: 1992.0
  num_classes: null
  extra_stats:
    avg_degree: 7.97
    edge_feature_dim: 0
    feature_type: no intrinsic node features; topology is the optimization input
    label_imbalance: objective and decoded-solution targets vary by MIS, max-cut,
      or coloring protocol
    node_feature_dim: 0
    size_regimes: 'small: 50,000 graphs, 249.9 nodes, 991.6 edges; large: 50,000 graphs,
      750.1 nodes, 2,992.4 edges'
    statistic_notes: GraphBench Table 2 reports separate small and large BA graph
      populations.
result_count: 5
best_model:
  model: Diffusion Wavelets
  value: 0.94
  metric: Accuracy
  arxiv_id: '1710.10321'
  paper_title: Learning Structural Node Embeddings via Diffusion Wavelets
papers:
- arxiv_id: '1710.10321'
  title: Learning Structural Node Embeddings via Diffusion Wavelets
  date_iso: '2017-10-27'
  venue: KDD 2017
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 100000
    avg_nodes: 500.0
    avg_edges: 1992.0
    num_classes: null
    extra_stats:
      avg_degree: 7.97
      edge_feature_dim: 0
      feature_type: no intrinsic node features; topology is the optimization input
      label_imbalance: objective and decoded-solution targets vary by MIS, max-cut,
        or coloring protocol
      node_feature_dim: 0
      size_regimes: 'small: 50,000 graphs, 249.9 nodes, 991.6 edges; large: 50,000
        graphs, 750.1 nodes, 2,992.4 edges'
      statistic_notes: GraphBench Table 2 reports separate small and large BA graph
        populations.
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: Diffusion Wavelets
    model_plain: Diffusion Wavelets
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_iso: '2017-10-27'
    date_display: Oct 2017
    codebase_url: ''
    published_conference: KDD 2017
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2017
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.94
    metric_stds:
    - null
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_iso: '2017-10-27'
    date_display: Oct 2017
    codebase_url: ''
    published_conference: KDD 2017
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.85
    metric_stds:
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
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_iso: '2017-10-27'
    date_display: Oct 2017
    codebase_url: ''
    published_conference: KDD 2017
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.82
    metric_stds:
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
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_iso: '2017-10-27'
    date_display: Oct 2017
    codebase_url: ''
    published_conference: KDD 2017
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.78
    metric_stds:
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
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_iso: '2017-10-27'
    date_display: Oct 2017
    codebase_url: ''
    published_conference: KDD 2017
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.75
    metric_stds:
    - null
  row_count: 5
  rows_json: ''
  chart_json: /data/datasets/ba-graph/standard-split-chart.json
  arch_counts:
    gnn: 3
    hybrid: 0
    graph_transformer: 0
    llm: 0
    walk: 2
    traditional: 0
  metric_counts:
  - 5
  milestones: &id001
  - value: 0.94
    std: null
    model: Diffusion Wavelets
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: '2017-10-27'
  milestones_by_metric:
    Accuracy: *id001
---

