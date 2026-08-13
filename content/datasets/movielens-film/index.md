---
title: MovieLens Film
slug: movielens-film
benchmark: Other Graph Benchmarks
task_type: node_classification
short_description: Predict one or more of nine genre labels per film; this is not
  the Actor/Film dataset on a MovieLens/IMDb movie graph.
description: '**9-class node classification** on a MovieLens/IMDb movie graph, predicting
  one or more of nine genre labels per film; this is not the Actor/Film dataset. Evaluated
  by Micro-F1.'
detailed_description:
  task: Movie graph with genre labels from the MovieLens/IMDb film benchmark; distinct
    from the five-class Actor graph sometimes called Film. The primary catalog metric
    is Micro-F1.
  data: Movie graph with genre labels from the MovieLens/IMDb film benchmark; distinct
    from the five-class Actor graph sometimes called Film. The cataloged artifact
    reports 1 graphs, 9 target classes or tasks.
  features: 'Input construction is dataset-specific and follows the cited release:
    program call graphs, 3D point coordinates, text-derived vectors, product attributes,
    or movie metadata. Added edges, neighborhood graphs, and feature normalization
    are preprocessing choices.'
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses Micro-F1 (higher is better). Exact masks or folds must
    come from the cited release.'
  quirks_and_pitfalls: These entries come from unrelated upstream benchmarks and have
    no shared protocol. Report the exact graph construction, split, feature pipeline,
    and label granularity; similarly named Film, Actor, IMDB, or Amazon artifacts
    are not interchangeable.
sources:
- title: MovieLens datasets
  url: https://grouplens.org/datasets/movielens/
  kind: benchmark_or_upstream_source
primary_metric: Micro-F1
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 1
  avg_nodes: 18352.0
  avg_edges: null
  num_classes: 9
result_count: 7
best_model:
  model: CLN-HWN-mini
  value: 0.575
  metric: Micro-F1
  arxiv_id: '1609.04508'
  paper_title: Column Networks for Collective Classification
papers:
- arxiv_id: '1609.04508'
  title: Column Networks for Collective Classification
  date_iso: '2016-09-15'
  venue: AAAI 2016
variants:
- slug: standard-split
  name: Standard split
  notes: MovieLens/IMDb film graph used by Bruna et al. 2016.
  is_standard: true
  primary_metric: Micro-F1
  default_metric: Micro-F1
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 18352.0
    avg_edges: null
    num_classes: 9
  metrics:
  - Micro-F1
  metric_display_names:
  - Micro-F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: CLN-HWN-mini
    model_plain: CLN-HWN-mini
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '1609.04508'
    title: Column Networks for Collective Classification
    date: Sep 15, 2016
    date_iso: '2016-09-15'
    date_display: Sep 2016
    codebase_url: https://github.com/trangptm/Column_networks
    published_conference: AAAI 2016
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2016
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.575
    metric_stds:
    - null
  - model: CLN-HWN-full
    model_plain: CLN-HWN-full
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '1609.04508'
    title: Column Networks for Collective Classification
    date: Sep 15, 2016
    date_iso: '2016-09-15'
    date_display: Sep 2016
    codebase_url: https://github.com/trangptm/Column_networks
    published_conference: AAAI 2016
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2016
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.574
    metric_stds:
    - null
  - model: CLN-FNN
    model_plain: CLN-FNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '1609.04508'
    title: Column Networks for Collective Classification
    date: Sep 15, 2016
    date_iso: '2016-09-15'
    date_display: Sep 2016
    codebase_url: https://github.com/trangptm/Column_networks
    published_conference: AAAI 2016
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2016
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.543
    metric_stds:
    - null
  - model: SL-LR
    model_plain: SL-LR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1609.04508'
    title: Column Networks for Collective Classification
    date: Sep 15, 2016
    date_iso: '2016-09-15'
    date_display: Sep 2016
    codebase_url: https://github.com/trangptm/Column_networks
    published_conference: AAAI 2016
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2016
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.534
    metric_stds:
    - null
  - model: HWN-noRel
    model_plain: HWN-noRel
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1609.04508'
    title: Column Networks for Collective Classification
    date: Sep 15, 2016
    date_iso: '2016-09-15'
    date_display: Sep 2016
    codebase_url: https://github.com/trangptm/Column_networks
    published_conference: AAAI 2016
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2016
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.508
    metric_stds:
    - null
  - model: nbC-IC
    model_plain: nbC-IC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1609.04508'
    title: Column Networks for Collective Classification
    date: Sep 15, 2016
    date_iso: '2016-09-15'
    date_display: Sep 2016
    codebase_url: https://github.com/trangptm/Column_networks
    published_conference: AAAI 2016
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2016
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.466
    metric_stds:
    - null
  - model: nbC-RL
    model_plain: nbC-RL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1609.04508'
    title: Column Networks for Collective Classification
    date: Sep 15, 2016
    date_iso: '2016-09-15'
    date_display: Sep 2016
    codebase_url: https://github.com/trangptm/Column_networks
    published_conference: AAAI 2016
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2016
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.435
    metric_stds:
    - null
  row_count: 7
  rows_json: ''
  chart_json: /data/datasets/movielens-film/standard-split-chart.json
  arch_counts:
    gnn: 1
    hybrid: 3
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 3
  metric_counts:
  - 7
  milestones: &id001
  - value: 0.575
    std: null
    model: CLN-HWN-mini
    arxiv_id: '1609.04508'
    title: Column Networks for Collective Classification
    date: '2016-09-15'
  milestones_by_metric:
    Micro-F1: *id001
---

