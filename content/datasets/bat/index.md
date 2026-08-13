---
title: BAT
slug: bat
benchmark: Hypergraph Benchmarks
task_type: node_classification
short_description: Brazilian Airport Transactions hypergraph node classification (4
  region classes, 131 nodes).
description: '**4-class node classification** Brazilian Airport Transactions hypergraph
  node classification (4 region classes, 131 nodes). Uses node-hyperedge incidence
  and the released node features. Clique expansion changes the input by discarding
  hyperedge identity. Evaluated by F1.'
detailed_description:
  task: Brazilian Airport Transactions hypergraph node classification (4 region classes,
    131 nodes). The primary catalog metric is F1.
  data: Brazilian Airport Transactions hypergraph node classification (4 region classes,
    131 nodes). The cataloged artifact reports 1 graphs, 4 target classes or tasks.
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
  avg_nodes: 131.0
  avg_edges: null
  num_classes: 4
result_count: 55
best_model:
  model: GraphLearner
  value: 0.754
  metric: F1
  arxiv_id: '2212.03559'
  paper_title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
papers:
- arxiv_id: '2508.14097'
  title: Non-Dissipative Graph Propagation for Non-Local Community Detection
  date_iso: '2025-06-30'
  venue: ''
- arxiv_id: '2308.06827'
  title: Reinforcement Graph Clustering with Unknown Cluster Number
  date_iso: '2023-08-13'
  venue: ''
- arxiv_id: '2307.14613'
  title: Self-Contrastive Graph Diffusion Network
  date_iso: '2023-07-27'
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
    avg_nodes: 131.0
    avg_edges: null
    num_classes: 4
  metrics:
  - F1
  - ARI
  - Conductance
  - NMI
  metric_display_names:
  - F1
  - ARI
  - Conductance
  - NMI
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.754
    - null
    - null
    - null
    metric_stds:
    - 0.0088
    - null
    - null
    - null
  - model: SCGDN
    model_plain: SCGDN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.14613'
    title: Self-Contrastive Graph Diffusion Network
    date: Jul 27, 2023
    date_iso: '2023-07-27'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7449
    - null
    - null
    - null
    metric_stds:
    - 0.0026
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
    is_best: false
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
    - 0.7174
    - null
    - null
    - null
    metric_stds:
    - 0.0093
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7125
    - null
    - null
    - null
    metric_stds:
    - 0.0031
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
    - 0.7125
    - null
    - null
    - null
    metric_stds:
    - 0.0031
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
    - 0.7047
    - null
    - null
    - null
    metric_stds:
    - 0.037
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
    - 0.674
    - null
    - null
    - null
    metric_stds:
    - 0.0035
    - null
    - null
    - null
  - model: ProGCL
    model_plain: ProGCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.14613'
    title: Self-Contrastive Graph Diffusion Network
    date: Jul 27, 2023
    date_iso: '2023-07-27'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5608
    - null
    - null
    - null
    metric_stds:
    - 0.0089
    - null
    - null
    - null
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
    is_std_outlier: true
    metric_values:
    - 0.54
    - null
    - 0.75
    - 0.48
    metric_stds:
    - 0.1
    - null
    - 0.17
    - 0.12
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
    - 0.5371
    - null
    - null
    - null
    metric_stds:
    - 0.0034
    - null
    - null
    - null
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
    - 0.53
    - null
    - 0.86
    - 0.34
    metric_stds:
    - 0.03
    - null
    - 0.24
    - 0.06
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
    - 0.5223
    - null
    - null
    - null
    metric_stds:
    - 0.0003
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
    arxiv_id: '2307.14613'
    title: Self-Contrastive Graph Diffusion Network
    date: Jul 27, 2023
    date_iso: '2023-07-27'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5223
    - null
    - null
    - null
    metric_stds:
    - 0.0003
    - null
    - null
    - null
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
    - 0.52
    - null
    - 0.72
    - 0.23
    metric_stds:
    - 0.03
    - null
    - 0.15
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
    arxiv_id: '2307.14613'
    title: Self-Contrastive Graph Diffusion Network
    date: Jul 27, 2023
    date_iso: '2023-07-27'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.509
    - null
    - null
    - null
    metric_stds:
    - 0.0012
    - null
    - null
    - null
  - model: MGAE
    model_plain: MGAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.14613'
    title: Self-Contrastive Graph Diffusion Network
    date: Jul 27, 2023
    date_iso: '2023-07-27'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5083
    - null
    - null
    - null
    metric_stds:
    - 0.0323
    - null
    - null
    - null
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
    - 0.4653
    - null
    - null
    - null
    metric_stds:
    - 0.0057
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
    - 0.4645
    - null
    - null
    - null
    metric_stds:
    - 0.059
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
    - 0.46
    - null
    - 1.0
    - 0.25
    metric_stds:
    - 0.04
    - null
    - 0.0
    - 0.04
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
    is_std_outlier: true
    metric_values:
    - 0.44
    - null
    - 0.58
    - 0.29
    metric_stds:
    - 0.06
    - null
    - 0.14
    - 0.05
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
    - 0.44
    - null
    - null
    - null
    metric_stds:
    - 0.0062
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
    - 0.4233
    - null
    - null
    - null
    metric_stds:
    - 0.0051
    - null
    - null
    - null
  - model: GDCL
    model_plain: GDCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.14613'
    title: Self-Contrastive Graph Diffusion Network
    date: Jul 27, 2023
    date_iso: '2023-07-27'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3994
    - null
    - null
    - null
    metric_stds:
    - 0.0057
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
    is_std_outlier: true
    metric_values:
    - 0.38
    - null
    - 0.19
    - 0.15
    metric_stds:
    - 0.07
    - null
    - 0.38
    - 0.05
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
    - 0.36
    - null
    - 0.42
    - 0.27
    metric_stds:
    - 0.06
    - null
    - 0.13
    - 0.05
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
    is_std_outlier: true
    metric_values:
    - 0.36
    - null
    - 0.51
    - 0.12
    metric_stds:
    - 0.06
    - null
    - 0.15
    - 0.06
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
    - 0.3484
    - null
    - null
    - null
    metric_stds:
    - 0.0015
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
    - 0.2964
    - null
    - null
    - null
    metric_stds:
    - 0.0049
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
  - model: DEC
    model_plain: DEC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.0799
    - null
    - 0.141
    metric_stds:
    - null
    - 0.0121
    - null
    - 0.0199
  - model: DCN
    model_plain: DCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.1375
    - null
    - 0.1803
    metric_stds:
    - null
    - 0.0605
    - null
    - 0.0773
  - model: IDEC
    model_plain: IDEC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.0785
    - null
    - 0.128
    metric_stds:
    - null
    - 0.0131
    - null
    - 0.0174
  - model: AdaGAE
    model_plain: AdaGAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.078
    - null
    - 0.1584
    metric_stds:
    - null
    - 0.0041
    - null
    - 0.0078
  - model: MGAE
    model_plain: MGAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.2415
    - null
    - 0.3059
    metric_stds:
    - null
    - 0.017
    - null
    - 0.0206
  - model: DAEGC
    model_plain: DAEGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.1818
    - null
    - 0.2143
    metric_stds:
    - null
    - 0.0029
    - null
    - 0.0035
  - model: ARGA
    model_plain: ARGA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.4202
    - null
    - 0.4909
    metric_stds:
    - null
    - 0.0121
    - null
    - 0.0054
  - model: SDCN
    model_plain: SDCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.2104
    - null
    - 0.2574
    metric_stds:
    - null
    - 0.0497
    - null
    - 0.0571
  - model: AGE
    model_plain: AGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.2659
    - null
    - 0.3604
    metric_stds:
    - null
    - 0.0183
    - null
    - 0.0154
  - model: MVGRL
    model_plain: MVGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.1345
    - null
    - 0.2933
    metric_stds:
    - null
    - 0.0003
    - null
    - 0.007
  - model: DFCN
    model_plain: DFCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.3776
    - null
    - 0.4877
    metric_stds:
    - null
    - 0.0023
    - null
    - 0.0051
  - model: GDCL
    model_plain: GDCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.1933
    - null
    - 0.317
    metric_stds:
    - null
    - 0.0057
    - null
    - 0.0042
  - model: GCA
    model_plain: GCA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.2669
    - null
    - 0.3888
    metric_stds:
    - null
    - 0.0285
    - null
    - 0.0023
  - model: MCGC
    model_plain: MCGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.0841
    - null
    - 0.2311
    metric_stds:
    - null
    - 0.0032
    - null
    - 0.0056
  - model: AutoSSL
    model_plain: AutoSSL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.1311
    - null
    - 0.1784
    metric_stds:
    - null
    - 0.0081
    - null
    - 0.0098
  - model: AGC-DRR
    model_plain: AGC-DRR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.06827'
    title: Reinforcement Graph Clustering with Unknown Cluster Number
    date: Aug 13, 2023
    date_iso: '2023-08-13'
    date_display: Aug 2023
    codebase_url: https://github.com/yueliu1999/RGC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.1459
    - null
    - 0.1991
    metric_stds:
    - null
    - 0.0013
    - null
    - 0.0024
  row_count: 55
  rows_json: /data/datasets/bat/standard-split-rows.json
  chart_json: /data/datasets/bat/standard-split-chart.json
  arch_counts:
    gnn: 48
    hybrid: 3
    graph_transformer: 0
    llm: 0
    walk: 1
    traditional: 3
  metric_counts:
  - 34
  - 21
  - 8
  - 29
  milestones: &id001
  - value: 0.7222
    std: 0.0097
    model: SCGC
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: '2022-05-11'
  - value: 0.754
    std: 0.0088
    model: GraphLearner
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    date: '2022-12-07'
  milestones_by_metric:
    F1: *id001
    ARI:
    - value: 0.4716
      std: 0.0135
      model: RGC
      arxiv_id: '2308.06827'
      title: Reinforcement Graph Clustering with Unknown Cluster Number
      date: '2023-08-13'
    Conductance:
    - value: 0.19
      std: 0.38
      model: DMoN
      arxiv_id: '2508.14097'
      title: Non-Dissipative Graph Propagation for Non-Local Community Detection
      date: '2025-06-30'
    NMI:
    - value: 0.5158
      std: 0.0083
      model: RGC
      arxiv_id: '2308.06827'
      title: Reinforcement Graph Clustering with Unknown Cluster Number
      date: '2023-08-13'
---

