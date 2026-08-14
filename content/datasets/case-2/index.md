---
title: Case 2
slug: case-2
benchmark: Power Flow Benchmarks
task_type: graph_regression
short_description: Jointly predict bus active/reactive power and voltage magnitude
  plus directional branch active/reactive flows on a real provincial grid.
description: '**Joint node-and-edge regression** Jointly predict bus active/reactive
  power and voltage magnitude plus directional branch active/reactive flows on a real
  provincial grid. Evaluated by Accuracy.'
detailed_description:
  task: Jointly predict bus active/reactive power and voltage magnitude plus directional
    branch active/reactive flows on a real provincial grid. Accuracy requires every
    voltage and branch-error threshold to be met for a sample.
  data: Case II uses 366 days of operational data from an unnamed Chinese provincial
    grid. The first 300 days generate 500,000 training and 100,000 test samples; the
    remaining 66 days yield about 150,000 generalization samples with 300--690 buses.
  features: Nodes represent buses with electrical quantities and edges represent transmission
    elements with network parameters. Inputs, targets, units, slack-bus treatment,
    and feasibility status follow the benchmark case generator.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses Accuracy (higher is better). Exact masks or folds must
    come from the cited release.'
  quirks_and_pitfalls: Only converged, feasible operating points should be compared
    under the documented policy. Per-unit conventions, topology changes, solver tolerances,
    and bus-type handling can silently alter labels; these cases do not establish
    transfer to real grids.
sources:
- title: Power Flow Benchmarks benchmark
  arxiv_id: '2601.01387'
  kind: benchmark_or_upstream_source
primary_metric: Accuracy
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 750000
  avg_nodes: null
  avg_edges: null
  num_classes: null
  extra_stats:
    edge_feature_dim: 3
    edge_feature_type: branch admittance, tap-ratio, and topology-derived branch attributes
    feature_type: active/reactive power, voltage magnitude, reactive bounds, self-admittance,
      and bus-type encoding
    node_count_range: 300--690 buses across operational/generalization samples
    node_feature_dim: 7
    sample_semantics: operating-point samples/subgraphs, not independent graph topologies
    statistic_notes: Case II uses 500,000 training samples, 100,000 test samples,
      and about 150,000 generalization samples from 366 days of provincial-grid data.
result_count: 4
best_model:
  model: RMGL
  value: 0.9928
  metric: Accuracy
  arxiv_id: '2601.01387'
  paper_title: Power Flow Benchmarks
papers:
- arxiv_id: '2601.01387'
  title: Power Flow Benchmarks
  date_iso: '2026-01-04'
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
    num_graphs: 750000
    avg_nodes: null
    avg_edges: null
    num_classes: null
    extra_stats:
      edge_feature_dim: 3
      edge_feature_type: branch admittance, tap-ratio, and topology-derived branch
        attributes
      feature_type: active/reactive power, voltage magnitude, reactive bounds, self-admittance,
        and bus-type encoding
      node_count_range: 300--690 buses across operational/generalization samples
      node_feature_dim: 7
      sample_semantics: operating-point samples/subgraphs, not independent graph topologies
      statistic_notes: Case II uses 500,000 training samples, 100,000 test samples,
        and about 150,000 generalization samples from 366 days of provincial-grid
        data.
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: RMGL
    model_plain: RMGL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9928
    metric_stds:
    - null
  - model: MGL
    model_plain: MGL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9607
    metric_stds:
    - null
  - model: GLP
    model_plain: GLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5072
    metric_stds:
    - null
  - model: GLR
    model_plain: GLR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4709
    metric_stds:
    - null
  row_count: 4
  rows_json: ''
  chart_json: /data/datasets/case-2/standard-split-chart.json
  arch_counts:
    gnn: 3
    hybrid: 1
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 4
  milestones: &id001
  - value: 0.9928
    std: null
    model: RMGL
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: '2026-01-04'
  milestones_by_metric:
    Accuracy: *id001
---

