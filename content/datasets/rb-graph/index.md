---
title: RB graph
slug: rb-graph
benchmark: GraphBench
task_type: graph_regression
short_description: Predict optimal objectives or decode feasible MIS, max-cut, and
  coloring solutions on RB-model graphs.
description: '**Graph regression** Predict the optimal objective value for maximum
  independent set in the supervised setting, or train node scores with differentiable
  surrogates and feasibility-preserving decoders for maximum independent set, max-cut,
  and graph coloring. Evaluated by MAE.'
detailed_description:
  task: Predict the optimal objective value for maximum independent set in the supervised
    setting, or train node scores with differentiable surrogates and feasibility-preserving
    decoders for maximum independent set, max-cut, and graph coloring.
  data: RB-model instances contain n groups of k vertices and use a constraint-tightness
    parameter p; GraphBench rejection-samples to keep graph sizes in configured ranges
    and provides small and large variants with 50,000 instances per dataset.
  features: The graphs contain no node or edge attributes. Topology encodes the optimization
    instance and solver outputs supply supervised optimum-value labels where available.
  splits_and_evaluation: Supervised objective prediction is evaluated by MAE. In unsupervised
    runs, the decoded feasible solution is scored by its achieved objective rather
    than classification accuracy.
  quirks_and_pitfalls: RB means the RB random constraint graph model, not random bipartite
    graph. Its planted group structure and tuned hardness parameters differ materially
    from ER and BA; report the problem, size regime, and learning protocol.
sources:
- title: GraphBench
  arxiv_id: '2512.04475'
  kind: benchmark_definition
- title: Many Hard Examples in Exact Phase Transitions with Application to Generating
    Hard Satisfiable Instances
  url: https://doi.org/10.1016/S0004-3702(01)00125-3
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
  value: 0.85
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
    - 0.85
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
    - 0.81
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
    - 0.78
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
    - 0.62
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
    - 0.6
    metric_stds:
    - null
  row_count: 5
  rows_json: ''
  chart_json: /data/datasets/rb-graph/standard-split-chart.json
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
  - value: 0.85
    std: null
    model: Diffusion Wavelets
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: '2017-10-27'
  milestones_by_metric:
    Accuracy: *id001
---

