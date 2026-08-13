---
title: UAT
slug: uat
benchmark: Hypergraph Benchmarks
task_type: node_classification
short_description: US Airport Transactions hypergraph node classification (4 region
  classes, 1190 nodes).
description: '**4-class node classification** US Airport Transactions hypergraph node
  classification (4 region classes, 1190 nodes). Uses node-hyperedge incidence and
  the released node features. Clique expansion changes the input by discarding hyperedge
  identity. Evaluated by F1.'
detailed_description:
  task: US Airport Transactions hypergraph node classification (4 region classes,
    1190 nodes). The primary catalog metric is F1.
  data: US Airport Transactions hypergraph node classification (4 region classes,
    1190 nodes). The cataloged artifact reports 1 graphs, 4 target classes or tasks.
  features: The release represents higher-order membership with a node-hyperedge incidence
    relation and supplies node features where available. Some source datasets have
    no measured features and use documented synthetic features; clique expansion is
    an alternative representation that discards hyperedge identity.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses F1 (higher is better). Exact masks or folds must come from
    the cited release.'
  quirks_and_pitfalls: Do not silently replace incidence propagation with clique expansion
    or merge distinct releases sharing a short name. Random synthetic features, split
    seeds, hyperedge multiplicity, and isolated-node handling can dominate results
    and must be reported.
sources:
- title: Hypergraph Benchmarks benchmark
  arxiv_id: '2106.13264'
  kind: benchmark_or_upstream_source
primary_metric: F1
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 1
  avg_nodes: 1190.0
  avg_edges: null
  num_classes: 4
result_count: 79
best_model:
  model: SCAGC
  value: 0.7277
  metric: F1
  arxiv_id: '2205.07865'
  paper_title: Simple Contrastive Graph Clustering
papers:
- arxiv_id: '2509.15024'
  title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
  date_iso: '2025-09-18'
  venue: ''
- arxiv_id: '2507.20127'
  title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph Message-passing'
  date_iso: '2025-07-27'
  venue: ''
- arxiv_id: '2508.14097'
  title: Non-Dissipative Graph Propagation for Non-Local Community Detection
  date_iso: '2025-06-30'
  venue: ''
- arxiv_id: '2406.15797'
  title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
    Clustering'
  date_iso: '2024-06-22'
  venue: ''
- arxiv_id: '2403.03666'
  title: Provable Filter for Real-world Graph Clustering
  date_iso: '2024-03-06'
  venue: ''
- arxiv_id: '2212.03559'
  title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
  date_iso: '2022-12-07'
  venue: ''
- arxiv_id: '2205.07865'
  title: Simple Contrastive Graph Clustering
  date_iso: '2022-05-11'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: F1
  default_metric: F1
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 1190.0
    avg_edges: null
    num_classes: 4
  metrics:
  - F1
  - ACC
  - Conductance
  - NMI
  metric_display_names:
  - F1
  - ACC
  - Conductance
  - NMI
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: SCAGC
    model_plain: SCAGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7277
    - null
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
    - null
  - model: SCGC
    model_plain: SCGC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7222
    - null
    - null
    - null
    metric_stds:
    - 0.0097
    - null
    - null
    - null
  - model: AGE
    model_plain: AGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7174
    - null
    - null
    - null
    metric_stds:
    - 0.0093
    - null
    - null
    - null
  - model: DAEGC
    model_plain: DAEGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6987
    - null
    - null
    - null
    metric_stds:
    - 0.0054
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
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6808
    - null
    - null
    - null
    metric_stds:
    - 0.0176
    - null
    - null
    - null
  - model: DFCN
    model_plain: DFCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6718
    - null
    - null
    - null
    metric_stds:
    - 0.0013
    - null
    - null
    - null
  - model: ARGA
    model_plain: ARGA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.643
    - null
    - null
    - null
    metric_stds:
    - 0.0195
    - null
    - null
    - null
  - model: SynC KMeans
    model_plain: SynC KMeans
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_iso: '2024-06-22'
    date_display: Jun 2024
    codebase_url: https://github.com/Marigoldwu/SynC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5891
    - null
    - null
    - null
    metric_stds:
    - 0.0102
    - null
    - null
    - null
  - model: SynC SSL
    model_plain: SynC SSL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_iso: '2024-06-22'
    date_display: Jun 2024
    codebase_url: https://github.com/Marigoldwu/SynC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5734
    - null
    - null
    - null
    metric_stds:
    - 0.0023
    - null
    - null
    - null
  - model: SCGC
    model_plain: SCGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_iso: '2024-06-22'
    date_display: Jun 2024
    codebase_url: https://github.com/Marigoldwu/SynC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5552
    - null
    - null
    - null
    metric_stds:
    - 0.0087
    - null
    - null
    - null
  - model: NeuCGC
    model_plain: NeuCGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_iso: '2024-06-22'
    date_display: Jun 2024
    codebase_url: https://github.com/Marigoldwu/SynC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5535
    - null
    - null
    - null
    metric_stds:
    - 0.0126
    - null
    - null
    - null
  - model: HomoCAGC
    model_plain: HomoCAGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_iso: '2024-06-22'
    date_display: Jun 2024
    codebase_url: https://github.com/Marigoldwu/SynC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5531
    - null
    - null
    - null
    metric_stds:
    - 0.0087
    - null
    - null
    - null
  - model: CCGC
    model_plain: CCGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_iso: '2024-06-22'
    date_display: Jun 2024
    codebase_url: https://github.com/Marigoldwu/SynC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5524
    - null
    - null
    - null
    metric_stds:
    - 0.0169
    - null
    - null
    - null
  - model: Vanilla GAE
    model_plain: Vanilla GAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_iso: '2024-06-22'
    date_display: Jun 2024
    codebase_url: https://github.com/Marigoldwu/SynC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5439
    - null
    - null
    - null
    metric_stds:
    - 0.0089
    - null
    - null
    - null
  - model: HSAN
    model_plain: HSAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_iso: '2024-06-22'
    date_display: Jun 2024
    codebase_url: https://github.com/Marigoldwu/SynC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.542
    - null
    - null
    - null
    metric_stds:
    - 0.0184
    - null
    - null
    - null
  - model: DAEGC
    model_plain: DAEGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.14097'
    title: Non-Dissipative Graph Propagation for Non-Local Community Detection
    date: Jun 30, 2025
    date_iso: '2025-06-30'
    date_display: Jun 2025
    codebase_url: https://github.com/willleeney/ugle
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.54
    - null
    - 1.0
    - 0.16
    metric_stds:
    - 0.01
    - null
    - 0.0
    - 0.04
  - model: uAGNN
    model_plain: uAGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.14097'
    title: Non-Dissipative Graph Propagation for Non-Local Community Detection
    date: Jun 30, 2025
    date_iso: '2025-06-30'
    date_display: Jun 2025
    codebase_url: https://github.com/willleeney/ugle
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.53
    - null
    - 0.69
    - 0.29
    metric_stds:
    - 0.02
    - null
    - 0.23
    - 0.02
  - model: SSGC
    model_plain: SSGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5279
    - null
    - null
    - null
    metric_stds:
    - 0.0001
    - null
    - null
    - null
  - model: GraphLearner
    model_plain: GraphLearner
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5277
    - null
    - null
    - null
    metric_stds:
    - 0.0261
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
    arxiv_id: '2508.14097'
    title: Non-Dissipative Graph Propagation for Non-Local Community Detection
    date: Jun 30, 2025
    date_iso: '2025-06-30'
    date_display: Jun 2025
    codebase_url: https://github.com/willleeney/ugle
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.52
    - null
    - 0.7
    - 0.24
    metric_stds:
    - 0.03
    - null
    - 0.15
    - 0.03
  - model: GRACE
    model_plain: GRACE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.14097'
    title: Non-Dissipative Graph Propagation for Non-Local Community Detection
    date: Jun 30, 2025
    date_iso: '2025-06-30'
    date_display: Jun 2025
    codebase_url: https://github.com/willleeney/ugle
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.52
    - null
    - 0.94
    - 0.27
    metric_stds:
    - 0.03
    - null
    - 0.19
    - 0.01
  - model: AGC-DRR
    model_plain: AGC-DRR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_iso: '2024-06-22'
    date_display: Jun 2024
    codebase_url: https://github.com/Marigoldwu/SynC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5197
    - null
    - null
    - null
    metric_stds:
    - 0.021
    - null
    - null
    - null
  - model: NS4GC
    model_plain: NS4GC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_iso: '2024-06-22'
    date_display: Jun 2024
    codebase_url: https://github.com/Marigoldwu/SynC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5176
    - null
    - null
    - null
    metric_stds:
    - 0.0052
    - null
    - null
    - null
  - model: SDCN
    model_plain: SDCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5066
    - null
    - null
    - null
    metric_stds:
    - 0.0149
    - null
    - null
    - null
  - model: DEAGC
    model_plain: DEAGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5033
    - null
    - null
    - null
    metric_stds:
    - 0.0064
    - null
    - null
    - null
  - model: DMoN
    model_plain: DMoN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.14097'
    title: Non-Dissipative Graph Propagation for Non-Local Community Detection
    date: Jun 30, 2025
    date_iso: '2025-06-30'
    date_display: Jun 2025
    codebase_url: https://github.com/willleeney/ugle
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.49
    - null
    - 0.67
    - 0.2
    metric_stds:
    - 0.04
    - null
    - 0.44
    - 0.04
  - model: MVGRL
    model_plain: MVGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.14097'
    title: Non-Dissipative Graph Propagation for Non-Local Community Detection
    date: Jun 30, 2025
    date_iso: '2025-06-30'
    date_display: Jun 2025
    codebase_url: https://github.com/willleeney/ugle
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.49
    - null
    - 0.9
    - 0.29
    metric_stds:
    - 0.04
    - null
    - 0.03
    - 0.02
  - model: BGRL
    model_plain: BGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.14097'
    title: Non-Dissipative Graph Propagation for Non-Local Community Detection
    date: Jun 30, 2025
    date_iso: '2025-06-30'
    date_display: Jun 2025
    codebase_url: https://github.com/willleeney/ugle
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.48
    - null
    - 0.88
    - 0.24
    metric_stds:
    - 0.02
    - null
    - 0.11
    - 0.0
  - model: AE
    model_plain: AE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4787
    - null
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
    - null
  - model: DEC
    model_plain: DEC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4671
    - null
    - null
    - null
    metric_stds:
    - 0.0012
    - null
    - null
    - null
  - model: SUBLIME
    model_plain: SUBLIME
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4619
    - null
    - null
    - null
    metric_stds:
    - 0.0087
    - null
    - null
    - null
  - model: SDCN
    model_plain: SDCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4559
    - null
    - null
    - null
    metric_stds:
    - 0.0354
    - null
    - null
    - null
  - model: DCRN
    model_plain: DCRN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4481
    - null
    - null
    - null
    metric_stds:
    - 0.0087
    - null
    - null
    - null
  - model: VGAER
    model_plain: VGAER
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.14097'
    title: Non-Dissipative Graph Propagation for Non-Local Community Detection
    date: Jun 30, 2025
    date_iso: '2025-06-30'
    date_display: Jun 2025
    codebase_url: https://github.com/willleeney/ugle
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.44
    - null
    - 0.75
    - 0.2
    metric_stds:
    - 0.03
    - null
    - 0.12
    - 0.02
  - model: AFGRL
    model_plain: AFGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3652
    - null
    - null
    - null
    metric_stds:
    - 0.0089
    - null
    - null
    - null
  - model: GCA
    model_plain: GCA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3572
    - null
    - null
    - null
    metric_stds:
    - 0.0028
    - null
    - null
    - null
  - model: AGC-DRR
    model_plain: AGC-DRR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3518
    - null
    - null
    - null
    metric_stds:
    - 0.0032
    - null
    - null
    - null
  - model: AutoSSL
    model_plain: AutoSSL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: Dec 7, 2022
    date_iso: '2022-12-07'
    date_display: Dec 2022
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3494
    - null
    - null
    - null
    metric_stds:
    - 0.0087
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
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3288
    - null
    - null
    - null
    metric_stds:
    - 0.055
    - null
    - null
    - null
  - model: DFCN
    model_plain: DFCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_iso: '2024-06-22'
    date_display: Jun 2024
    codebase_url: https://github.com/Marigoldwu/SynC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2579
    - null
    - null
    - null
    metric_stds:
    - 0.0029
    - null
    - null
    - null
  - model: K-means
    model_plain: K-means
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: May 11, 2022
    date_iso: '2022-05-11'
    date_display: May 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2396
    - null
    - null
    - null
    metric_stds:
    - 0.0051
    - null
    - null
    - null
  - model: SUBLIME
    model_plain: SUBLIME
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.14097'
    title: Non-Dissipative Graph Propagation for Non-Local Community Detection
    date: Jun 30, 2025
    date_iso: '2025-06-30'
    date_display: Jun 2025
    codebase_url: https://github.com/willleeney/ugle
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: true
    metric_values:
    - 0.17
    - null
    - 0.5
    - 0.2
    metric_stds:
    - 0.13
    - null
    - 0.2
    - 0.05
  - model: DFCN
    model_plain: DFCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.15024'
    title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
    date: Sep 18, 2025
    date_iso: '2025-09-18'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.3361
    - null
    - 0.2649
    metric_stds:
    - null
    - null
    - null
    - null
  - model: SSGC
    model_plain: SSGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.15024'
    title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
    date: Sep 18, 2025
    date_iso: '2025-09-18'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.3674
    - null
    - 0.0804
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
    arxiv_id: '2509.15024'
    title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
    date: Sep 18, 2025
    date_iso: '2025-09-18'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.4416
    - null
    - 0.2153
    metric_stds:
    - null
    - null
    - null
    - null
  - model: SDCN
    model_plain: SDCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.15024'
    title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
    date: Sep 18, 2025
    date_iso: '2025-09-18'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5225
    - null
    - 0.2161
    metric_stds:
    - null
    - null
    - null
    - null
  - model: MCGC
    model_plain: MCGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.15024'
    title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
    date: Sep 18, 2025
    date_iso: '2025-09-18'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.4193
    - null
    - 0.1664
    metric_stds:
    - null
    - null
    - null
    - null
  - model: FGC
    model_plain: FGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.15024'
    title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
    date: Sep 18, 2025
    date_iso: '2025-09-18'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5303
    - null
    - 0.2706
    metric_stds:
    - null
    - null
    - null
    - null
  - model: SCGC
    model_plain: SCGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2509.15024'
    title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
    date: Sep 18, 2025
    date_iso: '2025-09-18'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5658
    - null
    - 0.2807
    metric_stds:
    - null
    - null
    - null
    - null
  - model: CCGC
    model_plain: CCGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.15024'
    title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
    date: Sep 18, 2025
    date_iso: '2025-09-18'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.5634
    - null
    - 0.2815
    metric_stds:
    - null
    - null
    - null
    - null
  row_count: 79
  rows_json: /data/datasets/uat/standard-split-rows.json
  chart_json: /data/datasets/uat/standard-split-chart.json
  arch_counts:
    gnn: 65
    hybrid: 5
    graph_transformer: 0
    llm: 0
    walk: 1
    traditional: 7
  metric_counts:
  - 42
  - 37
  - 9
  - 46
  milestones: &id001
  - value: 0.7277
    std: 0.0016
    model: SCAGC
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: '2022-05-11'
  milestones_by_metric:
    F1: *id001
    ACC:
    - value: 0.5681
      std: 0.0034
      model: two unsupervised strategies
      arxiv_id: '2403.03666'
      title: Provable Filter for Real-world Graph Clustering
      date: '2024-03-06'
    - value: 0.584
      std: null
      model: the idea
      arxiv_id: '2507.20127'
      title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph Message-passing'
      date: '2025-07-27'
    - value: 0.6084
      std: null
      model: AGCN
      arxiv_id: '2509.15024'
      title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
      date: '2025-09-18'
    Conductance:
    - value: 0.5
      std: 0.2
      model: SUBLIME
      arxiv_id: '2508.14097'
      title: Non-Dissipative Graph Propagation for Non-Local Community Detection
      date: '2025-06-30'
    NMI:
    - value: 0.2933
      std: 0.0042
      model: two unsupervised strategies
      arxiv_id: '2403.03666'
      title: Provable Filter for Real-world Graph Clustering
      date: '2024-03-06'
    - value: 0.3074
      std: null
      model: AGCN
      arxiv_id: '2509.15024'
      title: 'Attention Beyond Neighborhoods: Reviving Transformer for Graph Clustering'
      date: '2025-09-18'
---

