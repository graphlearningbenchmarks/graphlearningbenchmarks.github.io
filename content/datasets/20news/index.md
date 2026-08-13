---
title: 20News
slug: 20news
benchmark: Other Graph Benchmarks
task_type: graph_classification
short_description: Predict one of 20 newsgroup topics on text-derived document graphs.
description: '**20-class graph classification** on text-derived document graphs, predicting
  one of 20 newsgroup topics. Evaluated by Accuracy.'
detailed_description:
  task: 20 Newsgroups text classification represented as a graph (nodes = documents,
    edges = TF-IDF similarity). 20 classes. The primary catalog metric is Accuracy.
  data: 20 Newsgroups text classification represented as a graph (nodes = documents,
    edges = TF-IDF similarity). 20 classes. The cataloged artifact reports 20 target
    classes or tasks.
  features: 'Input construction is dataset-specific and follows the cited release:
    program call graphs, 3D point coordinates, text-derived vectors, product attributes,
    or movie metadata. Added edges, neighborhood graphs, and feature normalization
    are preprocessing choices.'
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses Accuracy (higher is better). Exact masks or folds must
    come from the cited release.'
  quirks_and_pitfalls: These entries come from unrelated upstream benchmarks and have
    no shared protocol. Report the exact graph construction, split, feature pipeline,
    and label granularity; similarly named Film, Actor, IMDB, or Amazon artifacts
    are not interchangeable.
sources:
- title: 20 Newsgroups corpus documentation
  url: https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_20newsgroups.html
  kind: benchmark_or_upstream_source
primary_metric: Accuracy
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 20
result_count: 21
best_model:
  model: ARMA
  value: 0.7002
  metric: Accuracy
  arxiv_id: '1901.01343'
  paper_title: Graph Neural Networks With Convolutional ARMA Filters
papers:
- arxiv_id: '2102.05034'
  title: 'SLAPS: Self-Supervision Improves Structure Learning for Graph Neural Networks'
  date_iso: '2021-02-09'
  venue: NeurIPS 2021
- arxiv_id: '1903.11960'
  title: Learning Discrete Structures for Graph Neural Networks
  date_iso: '2019-03-28'
  venue: ICML 2019
- arxiv_id: '1901.01343'
  title: Graph Neural Networks With Convolutional ARMA Filters
  date_iso: '2019-01-05'
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
    num_classes: 20
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: ARMA
    model_plain: ARMA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1901.01343'
    title: Graph Neural Networks With Convolutional ARMA Filters
    date: Jan 5, 2019
    date_iso: '2019-01-05'
    date_display: Jan 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7002
    metric_stds:
    - 0.001
  - model: CayleyNet
    model_plain: CayleyNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1901.01343'
    title: Graph Neural Networks With Convolutional ARMA Filters
    date: Jan 5, 2019
    date_iso: '2019-01-05'
    date_display: Jan 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6884
    metric_stds:
    - 0.003
  - model: Chebyshev
    model_plain: Chebyshev
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1901.01343'
    title: Graph Neural Networks With Convolutional ARMA Filters
    date: Jan 5, 2019
    date_iso: '2019-01-05'
    date_display: Jan 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6824
    metric_stds:
    - 0.002
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1901.01343'
    title: Graph Neural Networks With Convolutional ARMA Filters
    date: Jan 5, 2019
    date_iso: '2019-01-05'
    date_display: Jan 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6545
    metric_stds:
    - 0.002
  - model: SLAPS (MLP)
    model_plain: SLAPS (MLP)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2102.05034'
    title: 'SLAPS: Self-Supervision Improves Structure Learning for Graph Neural Networks'
    date: Feb 9, 2021
    date_iso: '2021-02-09'
    date_display: Feb 2021
    codebase_url: https://github.com/BorealisAI/SLAPS-GNN
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.504
    metric_stds:
    - 0.007
  - model: IDGL
    model_plain: IDGL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2102.05034'
    title: 'SLAPS: Self-Supervision Improves Structure Learning for Graph Neural Networks'
    date: Feb 9, 2021
    date_iso: '2021-02-09'
    date_display: Feb 2021
    codebase_url: https://github.com/BorealisAI/SLAPS-GNN
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.485
    metric_stds:
    - 0.006
  - model: SemiEmb
    model_plain: SemiEmb
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.469
    metric_stds:
    - 0.001
  - model: ManiReg
    model_plain: ManiReg
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.466
    metric_stds:
    - 0.015
  - model: LDS
    model_plain: LDS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.464
    metric_stds:
    - 0.016
  - model: kNN-GCN
    model_plain: kNN-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2102.05034'
    title: 'SLAPS: Self-Supervision Improves Structure Learning for Graph Neural Networks'
    date: Feb 9, 2021
    date_iso: '2021-02-09'
    date_display: Feb 2021
    codebase_url: https://github.com/BorealisAI/SLAPS-GNN
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.463
    metric_stds:
    - 0.003
  - model: LogReg
    model_plain: LogReg
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.427
    metric_stds:
    - 0.017
  - model: kNN-GCN
    model_plain: kNN-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.413
    metric_stds:
    - 0.006
  - model: RBF SVM
    model_plain: RBF SVM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.41
    metric_stds:
    - 0.011
  - model: Linear SVM
    model_plain: Linear SVM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.403
    metric_stds:
    - 0.014
  - model: Dense-GCN
    model_plain: Dense-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.401
    metric_stds:
    - 0.015
  - model: rf
    model_plain: rf
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4
    metric_stds:
    - 0.011
  - model: RBF-GCN
    model_plain: RBF-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.393
    metric_stds:
    - 0.014
  - model: FFNN
    model_plain: FFNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.386
    metric_stds:
    - 0.014
  - model: LP
    model_plain: LP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.353
    metric_stds:
    - 0.009
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2102.05034'
    title: 'SLAPS: Self-Supervision Improves Structure Learning for Graph Neural Networks'
    date: Feb 9, 2021
    date_iso: '2021-02-09'
    date_display: Feb 2021
    codebase_url: https://github.com/BorealisAI/SLAPS-GNN
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.304
    metric_stds:
    - 0.001
  - model: Sparse-GCN
    model_plain: Sparse-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1903.11960'
    title: Learning Discrete Structures for Graph Neural Networks
    date: Mar 28, 2019
    date_iso: '2019-03-28'
    date_display: Mar 2019
    codebase_url: https://github.com/lucfra/LDS-GNN
    published_conference: ICML 2019
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.247
    metric_stds:
    - 0.012
  row_count: 21
  rows_json: ''
  chart_json: /data/datasets/20news/standard-split-chart.json
  arch_counts:
    gnn: 12
    hybrid: 1
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 8
  metric_counts:
  - 21
  milestones: &id001
  - value: 0.7002
    std: 0.001
    model: ARMA
    arxiv_id: '1901.01343'
    title: Graph Neural Networks With Convolutional ARMA Filters
    date: '2019-01-05'
  milestones_by_metric:
    Accuracy: *id001
---

