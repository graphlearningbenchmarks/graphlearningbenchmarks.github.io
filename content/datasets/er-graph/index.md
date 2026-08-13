---
title: ER graph
slug: er-graph
benchmark: GraphBench
task_type: graph_regression
short_description: Predict optimal objectives or decode feasible MIS, max-cut, and
  coloring solutions on Erdős–Rényi graphs.
description: '**Graph regression** Predict an optimal combinatorial-objective value
  in the supervised protocol, or learn node scores decoded into feasible solutions
  in the unsupervised protocol. Graphs have no supplied node or edge features, so
  topology is the model input. Evaluated by MAE.'
detailed_description:
  task: Predict an optimal combinatorial-objective value in the supervised protocol,
    or learn node scores decoded into feasible solutions in the unsupervised protocol.
    The included problems are maximum independent set, max-cut, and graph coloring.
  data: Synthetic Erdős–Rényi graphs are sampled in small and large regimes by controlling
    node count and independent edge probability. GraphBench reports 50,000 instances
    per dataset.
  features: Graphs have no supplied node or edge features, so topology is the model
    input. Targets and surrogate losses are problem-specific rather than properties
    of the ER generator itself.
  splits_and_evaluation: The supervised benchmark reports MAE on optimum values obtained
    with conventional solvers. The unsupervised benchmark evaluates the objective
    value after a problem-specific decoder enforces feasibility.
  quirks_and_pitfalls: ER graph is a generator family, not a single graph-classification
    dataset. Density strongly controls difficulty, and comparisons are meaningful
    only when problem, scale, generator parameters, split, and learning protocol match.
sources:
- title: GraphBench
  arxiv_id: '2512.04475'
  kind: benchmark_definition
- title: On Random Graphs I
  url: https://doi.org/10.5486/PMD.1959.6.3-4.290
  kind: generator_origin
primary_metric: MAE
higher_is_better: true
pyg_url: https://graphbench.github.io/website/datasets.html
stats:
  num_graphs: 21000000
  avg_nodes: 264.0
  avg_edges: 3667.0
  num_classes: null
result_count: 5
best_model:
  model: Diffusion Wavelets
  value: 0.93
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
    num_graphs: 21000000
    avg_nodes: 264.0
    avg_edges: 3667.0
    num_classes: null
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
    - 0.93
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
    - 0.88
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
    - 0.85
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
    - 0.72
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
    - 0.7
    metric_stds:
    - null
  row_count: 5
  rows_json: ''
  chart_json: /data/datasets/er-graph/standard-split-chart.json
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
  - value: 0.93
    std: null
    model: Diffusion Wavelets
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: '2017-10-27'
  milestones_by_metric:
    Accuracy: *id001
---

