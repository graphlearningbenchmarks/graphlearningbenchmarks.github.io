---
title: Algorithmic Reasoning
slug: algorithmic-reasoning
benchmark: GraphBench
task_type: graph_classification
short_description: Predict task-specific node, edge, or graph outputs for seven classical
  graph algorithms.
description: '**Mixed node/edge/graph prediction suite** covering topological sorting,
  maximum flow, MST, bridges, Steiner tree, maximum clique, and matching with task-specific
  node, edge, or graph targets. Evaluated by Accuracy.'
detailed_description:
  task: 'Simulate seven graph algorithms through node regression, node classification,
    or edge classification: topological sorting, maximum flow, minimum spanning tree,
    bridge finding, Steiner tree, maximum clique, and maximum matching.'
  data: Each algorithm has easy, medium, and hard synthetic datasets whose train and
    test graphs differ in generator distribution. Training graphs have 16 nodes while
    held-out graphs include 128 nodes, with additional size-generalization tests up
    to 512 nodes in the published experiments.
  features: Inputs encode the graph, algorithm-specific weights or designated vertices,
    and task-relevant node or edge attributes. Unlike CLRS-style processor supervision,
    these datasets focus on final outputs rather than providing a full sequence of
    algorithmic hints.
  splits_and_evaluation: Fixed 98%/1%/1% splits contain about one million graphs per
    difficulty for each algorithm. Classification tasks use accuracy and F1; flow
    and topological-order targets use MAE.
  quirks_and_pitfalls: Difficulty changes both generator distribution and graph size,
    so failures cannot be attributed to only one axis. Edge tasks are transformed
    for some node-token baselines. The old YAML's 21-million count is the approximate
    total across seven tasks, not the size of every individual task.
sources:
- title: GraphBench
  arxiv_id: '2512.04475'
  kind: benchmark_definition
- title: The CLRS Algorithmic Reasoning Benchmark
  arxiv_id: '2205.15659'
  kind: related_protocol
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://graphbench.github.io/website/datasets.html
stats: null
result_count: 8
best_model:
  model: Naive multi-task
  value: 0.9971
  metric: Accuracy
  arxiv_id: '2601.22384'
  paper_title: Graph is a Substrate Across Data Modalities
papers:
- arxiv_id: '2601.22384'
  title: Graph is a Substrate Across Data Modalities
  date_iso: '2026-01-29'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: Naive multi-task
    model_plain: Naive multi-task
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2601.22384'
    title: Graph is a Substrate Across Data Modalities
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: https://github.com/zmli6/G-Substrate
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9971
    metric_stds:
    - null
  - model: Naive single-task
    model_plain: Naive single-task
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2601.22384'
    title: Graph is a Substrate Across Data Modalities
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: https://github.com/zmli6/G-Substrate
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9944
    metric_stds:
    - null
  - model: G-Substrate
    model_plain: G-Substrate
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.22384'
    title: Graph is a Substrate Across Data Modalities
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: https://github.com/zmli6/G-Substrate
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9841
    metric_stds:
    - null
  - model: Naive multi-task + interleave
    model_plain: Naive multi-task + interleave
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2601.22384'
    title: Graph is a Substrate Across Data Modalities
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: https://github.com/zmli6/G-Substrate
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9827
    metric_stds:
    - null
  - model: GITA
    model_plain: GITA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.22384'
    title: Graph is a Substrate Across Data Modalities
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: https://github.com/zmli6/G-Substrate
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: null
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9817
    metric_stds:
    - null
  - model: Unified multi-task
    model_plain: Unified multi-task
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2601.22384'
    title: Graph is a Substrate Across Data Modalities
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: https://github.com/zmli6/G-Substrate
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9809
    metric_stds:
    - null
  - model: Unified single-task
    model_plain: Unified single-task
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2601.22384'
    title: Graph is a Substrate Across Data Modalities
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: https://github.com/zmli6/G-Substrate
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.978
    metric_stds:
    - null
  - model: G-Wiz
    model_plain: G-Wiz
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.22384'
    title: Graph is a Substrate Across Data Modalities
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: https://github.com/zmli6/G-Substrate
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: null
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9774
    metric_stds:
    - null
  row_count: 8
  rows_json: ''
  chart_json: /data/datasets/algorithmic-reasoning/standard-split-chart.json
  arch_counts:
    gnn: 2
    hybrid: 1
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 8
  milestones: &id001
  - value: 0.9971
    std: null
    model: Naive multi-task
    arxiv_id: '2601.22384'
    title: Graph is a Substrate Across Data Modalities
    date: '2026-01-29'
  milestones_by_metric:
    Accuracy: *id001
---

