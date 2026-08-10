---
title: Non-Dissipative Graph Propagation for Non-Local Community Detection
arxiv_id: '2508.14097'
source_url: ''
authors:
- name: W. Leeney
  orcid: null
  s2_author_id: '2216723257'
  s2_url: null
- name: Alessio Gravina
  orcid: null
  s2_author_id: '2042289369'
  s2_url: null
- name: Davide Bacciu
  orcid: null
  s2_author_id: '2294893543'
  s2_url: null
published_date: Jun 30, 2025
published_date_iso: '2025-06-30'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Community detection in graphs aims to cluster nodes into meaningful groups,
  a task particularly challenging in heterophilic graphs, where nodes sharing similarities
  and membership to the same community are typically distantly connected. This is
  particularly evident when this task is tackled by graph neural networks, since they
  rely on an inherently local message passing scheme to learn the node representations
  that serve to cluster nodes into communities. In this work, we argue that the ability
  to propagate long-range information during message passing is key to effectively
  perform community detection in heterophilic graphs. To this end, we introduce the
  Unsupervised Antisymmetric Graph Neural Network (uAGNN), a novel unsupervised community
  detection approach leveraging non-dissipative dynamical systems to ensure stability
  and to propagate long-range information effectively. By employing antisymmetric
  weight matrices, uAGNN captures both local and global graph structures, overcoming
  the limitations posed by heterophilic scenarios. Extensive experiments across ten
  datasets demonstrate uAGNN’s superior performance in high and medium heterophilic
  settings, where traditional methods fail to exploit long-range dependencies. These
  results highlight uAGNN’s potential as a powerful tool for unsupervised community
  detection in diverse graph environments.
codebase_url: https://github.com/willleeney/ugle
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- uAGNN
mrr: 0.0533
adjusted_mrr: 0.0533
mrr_dataset_count: 4
benchmark_categories:
- Heterophilic Graphs
- Heterogeneous Graph Benchmarks
- Hypergraph Benchmarks
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 2
  total: 6
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 1
  total: 4
- benchmark: Hypergraph Benchmarks
  benchmark_slug: hypergraph-benchmarks
  evaluated: 4
  total: 10
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id004
  dataset: AMAP
  is_multi_metric: true
  rows:
  - model: GANN
    model_key: gann
    model_plain: GANN
    metric_values:
    - 0.9405
    - null
    - null
    metric_stds:
    - 0.0037
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    published_venue: ''
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.9405
    sort_std: 0.0037
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    metric_values:
    - 0.9308
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    published_venue: ''
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.9308
    sort_std: 0.0026
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.9238
    - null
    - null
    metric_stds:
    - 0.0014
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    published_venue: ''
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.9238
    sort_std: 0.0014
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.8115
    - null
    - null
    metric_stds:
    - 0.0105
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.07778'
    title: 'GANN: Graph Alignment Neural Network for Semi-Supervised Learning'
    published_venue: ''
    date: Mar 14, 2023
    date_display: Mar 2023
    date_iso: '2023-03-14'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 14
    is_best: false
    sort_value: 0.8115
    sort_std: 0.0105
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    metric_values:
    - 0.34
    - 0.53
    - 0.92
    metric_stds:
    - 0.02
    - 0.02
    - 0.14
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6987
    sort_std: 0.0054
    true_value: 0.6987
    true_std: 0.0054
    paper_value: 0.34
    paper_std: 0.02
    has_value_gap: true
    has_value_note: false
    value_gap: 0.35869999999999996
    value_gap_source_arxiv: '2307.14613'
    value_gap_source_title: Self-Contrastive Graph Diffusion Network
    value_note: ''
    at_pub_value: 0.6987
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-07-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.35869999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
    global_rank: 27
  - model: DMoN
    model_key: dmon
    model_plain: DMoN
    metric_values:
    - 0.67
    - 0.61
    - 0.6
    metric_stds:
    - 0.1
    - 0.08
    - 0.49
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.67
    sort_std: 0.1
    true_value: 0.67
    true_std: 0.1
    paper_value: 0.67
    paper_std: 0.1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 32
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    metric_values:
    - 0.65
    - 0.6
    - 0.23
    metric_stds:
    - 0.07
    - 0.04
    - 0.18
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.65
    sort_std: 0.07
    true_value: 0.65
    true_std: 0.07
    paper_value: 0.65
    paper_std: 0.07
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: 0.1597
    at_pub_std: 0.0153
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.4903
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: improved
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: false
    is_std_outlier: false
    global_rank: 37
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - 0.25
    - 0.27
    - 0.3
    metric_stds:
    - 0.03
    - 0.08
    - 0.02
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6283
    sort_std: 0.0159
    true_value: 0.6283
    true_std: 0.0159
    paper_value: 0.25
    paper_std: 0.03
    has_value_gap: true
    has_value_note: false
    value_gap: 0.37829999999999997
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_note: ''
    at_pub_value: 0.6283
    at_pub_std: 0.0159
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.37829999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
    global_rank: 40
  - model: VGAER
    model_key: vgaer
    model_plain: VGAER
    metric_values:
    - 0.61
    - 0.55
    - 0.7
    metric_stds:
    - 0.16
    - 0.18
    - 0.18
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.61
    sort_std: 0.16
    true_value: 0.61
    true_std: 0.16
    paper_value: 0.61
    paper_std: 0.16
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 41
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    metric_values:
    - 0.51
    - 0.6
    - 0.87
    metric_stds:
    - 0.09
    - 0.04
    - 0.13
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.51
    sort_std: 0.09
    true_value: 0.51
    true_std: 0.09
    paper_value: 0.51
    paper_std: 0.09
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 49
  - model: uAGNN
    model_key: uagnn
    model_plain: uAGNN
    metric_values:
    - 0.48
    - 0.5
    - 0.87
    metric_stds:
    - 0.09
    - 0.1
    - 0.08
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.48
    sort_std: 0.09
    true_value: 0.48
    true_std: 0.09
    paper_value: 0.48
    paper_std: 0.09
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 51
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    metric_values:
    - 0.48
    - 0.54
    - 0.79
    metric_stds:
    - 0.1
    - 0.02
    - 0.06
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.48
    sort_std: 0.1
    true_value: 0.48
    true_std: 0.1
    paper_value: 0.48
    paper_std: 0.1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 50
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - 0.34
    - 0.24
    - 0.84
    metric_stds:
    - 0.06
    - 0.08
    - 0.26
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.34
    sort_std: 0.06
    true_value: 0.34
    true_std: 0.06
    paper_value: 0.34
    paper_std: 0.06
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 53
  metrics:
  - F1
  - NMI
  - Conductance
  primary_metric: F1
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  - NMI
  - Conductance
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id006
  dataset: BAT
  is_multi_metric: true
  rows:
  - model: GraphLearner
    model_key: graphlearner
    model_plain: GraphLearner
    metric_values:
    - 0.754
    - null
    - null
    metric_stds:
    - 0.0088
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.03559'
    title: 'GraphLearner: Graph Node Clustering with Fully Learnable Augmentation'
    published_venue: ''
    date: Dec 7, 2022
    date_display: Dec 2022
    date_iso: '2022-12-07'
    codebase_url: https://github.com/xihongyang1999/GraphLearner
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.754
    sort_std: 0.0088
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: SCGDN
    model_key: scgdn
    model_plain: SCGDN
    metric_values:
    - 0.7449
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.14613'
    title: Self-Contrastive Graph Diffusion Network
    published_venue: ''
    date: Jul 27, 2023
    date_display: Jul 2023
    date_iso: '2023-07-27'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.7449
    sort_std: 0.0026
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: SCGC
    model_key: scgc
    model_plain: SCGC
    metric_values:
    - 0.7222
    - null
    - null
    metric_stds:
    - 0.0097
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    published_venue: ''
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.7222
    sort_std: 0.0097
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - 0.65
    - 0.31
    - 0.66
    metric_stds:
    - 0.05
    - 0.07
    - 0.13
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7047
    sort_std: 0.037
    true_value: 0.7047
    true_std: 0.037
    paper_value: 0.65
    paper_std: 0.05
    has_value_gap: true
    has_value_note: false
    value_gap: 0.05469999999999997
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_note: ''
    at_pub_value: 0.7047
    at_pub_std: 0.037
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.05469999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    metric_values:
    - 0.46
    - 0.25
    - 1.0
    metric_stds:
    - 0.04
    - 0.04
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6987
    sort_std: 0.0054
    true_value: 0.6987
    true_std: 0.0054
    paper_value: 0.46
    paper_std: 0.04
    has_value_gap: true
    has_value_note: false
    value_gap: 0.23869999999999997
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_note: ''
    at_pub_value: 0.6987
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.23869999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
    global_rank: 8
  - model: uAGNN
    model_key: uagnn
    model_plain: uAGNN
    metric_values:
    - 0.54
    - 0.48
    - 0.75
    metric_stds:
    - 0.1
    - 0.12
    - 0.17
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.54
    sort_std: 0.1
    true_value: 0.54
    true_std: 0.1
    paper_value: 0.54
    paper_std: 0.1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 12
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    metric_values:
    - 0.53
    - 0.34
    - 0.86
    metric_stds:
    - 0.03
    - 0.06
    - 0.24
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.53
    sort_std: 0.03
    true_value: 0.53
    true_std: 0.03
    paper_value: 0.53
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 14
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    metric_values:
    - 0.52
    - 0.23
    - 0.72
    metric_stds:
    - 0.03
    - 0.05
    - 0.15
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.52
    sort_std: 0.03
    true_value: 0.52
    true_std: 0.03
    paper_value: 0.52
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 16
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - 0.44
    - 0.29
    - 0.58
    metric_stds:
    - 0.06
    - 0.05
    - 0.14
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.44
    sort_std: 0.06
    true_value: 0.44
    true_std: 0.06
    paper_value: 0.44
    paper_std: 0.06
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 23
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    metric_values:
    - 0.36
    - 0.27
    - 0.42
    metric_stds:
    - 0.06
    - 0.05
    - 0.13
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.44
    sort_std: 0.0062
    true_value: 0.44
    true_std: 0.0062
    paper_value: 0.36
    paper_std: 0.06
    has_value_gap: true
    has_value_note: false
    value_gap: 0.08000000000000002
    value_gap_source_arxiv: '2212.03559'
    value_gap_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    value_note: ''
    at_pub_value: 0.44
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.08000000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: false
    is_std_outlier: false
    global_rank: 22
  - model: DMoN
    model_key: dmon
    model_plain: DMoN
    metric_values:
    - 0.38
    - 0.15
    - 0.19
    metric_stds:
    - 0.07
    - 0.05
    - 0.38
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.38
    sort_std: 0.07
    true_value: 0.38
    true_std: 0.07
    paper_value: 0.38
    paper_std: 0.07
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 26
  - model: VGAER
    model_key: vgaer
    model_plain: VGAER
    metric_values:
    - 0.36
    - 0.12
    - 0.51
    metric_stds:
    - 0.06
    - 0.06
    - 0.15
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.36
    sort_std: 0.06
    true_value: 0.36
    true_std: 0.06
    paper_value: 0.36
    paper_std: 0.06
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 27
  metrics:
  - F1
  - NMI
  - Conductance
  primary_metric: F1
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  - NMI
  - Conductance
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: Cornell
  is_multi_metric: true
  rows:
  - model: FPS-T
    model_key: fps-t
    model_plain: FPS-T
    metric_values:
    - 0.7216
    - null
    - null
    - null
    metric_stds:
    - 0.0296
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2309.04082'
    title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
      Learning'
    published_venue: ''
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.7216
    sort_std: 0.0296
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: TokenGT
    model_key: tokengt
    model_plain: TokenGT
    metric_values:
    - 0.7162
    - null
    - null
    - null
    metric_stds:
    - 0.0213
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2309.04082'
    title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
      Learning'
    published_venue: ''
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.7162
    sort_std: 0.0213
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - 0.7054
    - null
    - null
    - null
    metric_stds:
    - 0.0201
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.04082'
    title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
      Learning'
    published_venue: ''
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: true
    sort_value: 0.7054
    sort_std: 0.0201
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.5838
    - null
    - null
    - null
    metric_stds:
    - 0.0404
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2309.04082'
    title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
      Learning'
    published_venue: ''
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 5
    is_best: false
    sort_value: 0.5838
    sort_std: 0.0404
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - null
    - 0.34
    - 0.06
    - 0.88
    metric_stds:
    - null
    - 0.06
    - 0.01
    - 0.23
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.34
    sort_std: 0.06
    true_value: 0.34
    true_std: 0.06
    paper_value: 0.34
    paper_std: 0.06
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 12
  - model: DMoN
    model_key: dmon
    model_plain: DMoN
    metric_values:
    - null
    - 0.34
    - 0.22
    - 0.52
    metric_stds:
    - null
    - 0.05
    - 0.07
    - 0.37
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.34
    sort_std: 0.05
    true_value: 0.34
    true_std: 0.05
    paper_value: 0.34
    paper_std: 0.05
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 13
  - model: uAGNN
    model_key: uagnn
    model_plain: uAGNN
    metric_values:
    - null
    - 0.29
    - 0.27
    - 0.44
    metric_stds:
    - null
    - 0.04
    - 0.07
    - 0.15
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.29
    sort_std: 0.04
    true_value: 0.29
    true_std: 0.04
    paper_value: 0.29
    paper_std: 0.04
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 14
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - null
    - 0.27
    - 0.06
    - 0.49
    metric_stds:
    - null
    - 0.05
    - 0.02
    - 0.34
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.27
    sort_std: 0.05
    true_value: 0.27
    true_std: 0.05
    paper_value: 0.27
    paper_std: 0.05
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 15
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    metric_values:
    - null
    - 0.25
    - 0.05
    - 1.0
    metric_stds:
    - null
    - 0.03
    - 0.01
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.25
    sort_std: 0.03
    true_value: 0.25
    true_std: 0.03
    paper_value: 0.25
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 16
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    metric_values:
    - null
    - 0.25
    - 0.05
    - 0.84
    metric_stds:
    - null
    - 0.02
    - 0.01
    - 0.14
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.25
    sort_std: 0.02
    true_value: 0.25
    true_std: 0.02
    paper_value: 0.25
    paper_std: 0.02
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 17
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    metric_values:
    - null
    - 0.24
    - 0.05
    - 0.99
    metric_stds:
    - null
    - 0.03
    - 0.02
    - 0.02
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.24
    sort_std: 0.03
    true_value: 0.24
    true_std: 0.03
    paper_value: 0.24
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 18
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    metric_values:
    - null
    - 0.23
    - 0.03
    - 0.4
    metric_stds:
    - null
    - 0.03
    - 0.01
    - 0.32
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.23
    sort_std: 0.03
    true_value: 0.23
    true_std: 0.03
    paper_value: 0.23
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 19
  - model: VGAER
    model_key: vgaer
    model_plain: VGAER
    metric_values:
    - null
    - 0.22
    - 0.08
    - 0.4
    metric_stds:
    - null
    - 0.02
    - 0.03
    - 0.1
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.22
    sort_std: 0.02
    true_value: 0.22
    true_std: 0.02
    paper_value: 0.22
    paper_std: 0.02
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 20
  metrics:
  - Accuracy
  - F1
  - NMI
  - Conductance
  primary_metric: Accuracy
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - F1
  - NMI
  - Conductance
  metric: F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id003
  dataset: DBLP
  is_multi_metric: true
  rows:
  - model: AUG_bal
    model_key: aug_bal
    model_plain: AUG_bal
    metric_values:
    - 0.9454
    - null
    - null
    - null
    metric_stds:
    - 0.0123
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2302.14061'
    title: Semantic-aware Node Synthesis for Imbalanced Heterogeneous Information
      Networks
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.9454
    sort_std: 0.0123
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: AUG_min
    model_key: aug_min
    model_plain: AUG_min
    metric_values:
    - 0.9375
    - null
    - null
    - null
    metric_stds:
    - 0.0115
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2302.14061'
    title: Semantic-aware Node Synthesis for Imbalanced Heterogeneous Information
      Networks
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.9375
    sort_std: 0.0115
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: AUG_ran
    model_key: aug_ran
    model_plain: AUG_ran
    metric_values:
    - 0.9368
    - null
    - null
    - null
    metric_stds:
    - 0.0108
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2302.14061'
    title: Semantic-aware Node Synthesis for Imbalanced Heterogeneous Information
      Networks
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: true
    sort_value: 0.9368
    sort_std: 0.0108
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    metric_values:
    - null
    - 0.72
    - 0.37
    - 1.0
    metric_stds:
    - null
    - 0.05
    - 0.05
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.862
    sort_std: null
    true_value: 0.862
    true_std: null
    paper_value: 0.72
    paper_std: 0.05
    has_value_gap: true
    has_value_note: false
    value_gap: 0.14200000000000002
    value_gap_source_arxiv: '2403.03670'
    value_gap_source_title: 'CDC: A Simple Framework for Complex Data Clustering'
    value_note: ''
    at_pub_value: 0.862
    at_pub_std: null
    at_pub_source_arxiv: '2403.03670'
    at_pub_source_title: 'CDC: A Simple Framework for Complex Data Clustering'
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-03-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.14200000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'CDC: A Simple Framework for Complex Data Clustering'
    comparison_source_arxiv: '2403.03670'
    is_best: false
    is_std_outlier: false
    global_rank: 23
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - null
    - 0.42
    - 0.35
    - 0.98
    metric_stds:
    - null
    - 0.21
    - 0.18
    - 0.01
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.792
    sort_std: null
    true_value: 0.792
    true_std: null
    paper_value: 0.42
    paper_std: 0.21
    has_value_gap: true
    has_value_note: false
    value_gap: 0.37200000000000005
    value_gap_source_arxiv: '2203.10866'
    value_gap_source_title: Unsupervised Network Embedding Beyond Homophily
    value_note: ''
    at_pub_value: 0.792
    at_pub_std: null
    at_pub_source_arxiv: '2203.10866'
    at_pub_source_title: Unsupervised Network Embedding Beyond Homophily
    at_pub_source_date_iso: '2022-03-21'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2022-03-21'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: 0.37200000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Unsupervised Network Embedding Beyond Homophily
    comparison_source_arxiv: '2203.10866'
    is_best: false
    is_std_outlier: false
    global_rank: 32
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - 0.732
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2203.10866'
    title: Unsupervised Network Embedding Beyond Homophily
    published_venue: ''
    date: Mar 21, 2022
    date_display: Mar 2022
    date_iso: '2022-03-21'
    codebase_url: https://github.com/zhiqiangzhongddu/SELENE
    uses_external_data: false
    is_global_top: true
    global_rank: 39
    is_best: false
    sort_value: 0.732
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: uAGNN
    model_key: uagnn
    model_plain: uAGNN
    metric_values:
    - null
    - 0.71
    - 0.41
    - 0.67
    metric_stds:
    - null
    - 0.14
    - 0.12
    - 0.14
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.71
    sort_std: 0.14
    true_value: 0.71
    true_std: 0.14
    paper_value: 0.71
    paper_std: 0.14
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 41
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    metric_values:
    - null
    - 0.64
    - 0.33
    - 0.95
    metric_stds:
    - null
    - 0.07
    - 0.05
    - 0.03
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.64
    sort_std: 0.07
    true_value: 0.64
    true_std: 0.07
    paper_value: 0.64
    paper_std: 0.07
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 45
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    metric_values:
    - null
    - 0.6
    - 0.31
    - 0.66
    metric_stds:
    - null
    - 0.11
    - 0.02
    - 0.18
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6
    sort_std: 0.11
    true_value: 0.6
    true_std: 0.11
    paper_value: 0.6
    paper_std: 0.11
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 48
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - null
    - 0.55
    - 0.28
    - 0.86
    metric_stds:
    - null
    - 0.07
    - 0.03
    - 0.11
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.55
    sort_std: 0.07
    true_value: 0.55
    true_std: 0.07
    paper_value: 0.55
    paper_std: 0.07
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: 0.2479
    at_pub_std: null
    at_pub_source_arxiv: '2305.10738'
    at_pub_source_title: Deep Temporal Graph Clustering
    at_pub_source_date_iso: '2023-05-18'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.30210000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: improved
    comparison_source_title: Deep Temporal Graph Clustering
    comparison_source_arxiv: '2305.10738'
    is_best: false
    is_std_outlier: false
    global_rank: 50
  - model: DMoN
    model_key: dmon
    model_plain: DMoN
    metric_values:
    - null
    - 0.5
    - 0.22
    - 0.99
    metric_stds:
    - null
    - 0.07
    - 0.09
    - 0.02
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5
    sort_std: 0.07
    true_value: 0.5
    true_std: 0.07
    paper_value: 0.5
    paper_std: 0.07
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 51
  - model: VGAER
    model_key: vgaer
    model_plain: VGAER
    metric_values:
    - null
    - 0.5
    - 0.24
    - 0.42
    metric_stds:
    - null
    - 0.13
    - 0.11
    - 0.08
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5
    sort_std: 0.13
    true_value: 0.5
    true_std: 0.13
    paper_value: 0.5
    paper_std: 0.13
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 52
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    metric_values:
    - null
    - 0.45
    - 0.14
    - 0.88
    metric_stds:
    - null
    - 0.06
    - 0.02
    - 0.02
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.45
    sort_std: 0.06
    true_value: 0.45
    true_std: 0.06
    paper_value: 0.45
    paper_std: 0.06
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 54
  metrics:
  - Micro-F1
  - F1
  - NMI
  - Conductance
  primary_metric: Micro-F1
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - F1
  - NMI
  - Conductance
  metric: F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id007
  dataset: EAT
  is_multi_metric: true
  rows:
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    metric_values:
    - 0.7702
    - null
    - null
    metric_stds:
    - 0.0033
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    published_venue: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    codebase_url: https://github.com/yueliu1999/HSAN
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.7702
    sort_std: 0.0033
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: HSAN
    model_key: hsan
    model_plain: HSAN
    metric_values:
    - 0.7702
    - null
    - null
    metric_stds:
    - 0.0033
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    published_venue: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    codebase_url: https://github.com/yueliu1999/HSAN
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.7702
    sort_std: 0.0033
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    metric_values:
    - 0.7682
    - null
    - null
    metric_stds:
    - 0.0023
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    published_venue: ''
    date: Dec 16, 2022
    date_display: Dec 2022
    date_iso: '2022-12-16'
    codebase_url: https://github.com/yueliu1999/HSAN
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: true
    sort_value: 0.7682
    sort_std: 0.0023
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    metric_values:
    - 0.41
    - 0.13
    - 1.0
    metric_stds:
    - 0.02
    - 0.02
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7596
    sort_std: 0.0023
    true_value: 0.7596
    true_std: 0.0023
    paper_value: 0.41
    paper_std: 0.02
    has_value_gap: true
    has_value_note: false
    value_gap: 0.3496000000000001
    value_gap_source_arxiv: '2212.08665'
    value_gap_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    value_note: ''
    at_pub_value: 0.7596
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-12-16'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.3496000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Hard Sample Aware Network for Contrastive Deep Graph
      Clustering [5]
    comparison_source_arxiv: '2212.08665'
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    metric_values:
    - 0.48
    - 0.31
    - 1.0
    metric_stds:
    - 0.03
    - 0.02
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.48
    sort_std: 0.03
    true_value: 0.48
    true_std: 0.03
    paper_value: 0.48
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 20
  - model: uAGNN
    model_key: uagnn
    model_plain: uAGNN
    metric_values:
    - 0.47
    - 0.32
    - 0.4
    metric_stds:
    - 0.05
    - 0.01
    - 0.37
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.47
    sort_std: 0.05
    true_value: 0.47
    true_std: 0.05
    paper_value: 0.47
    paper_std: 0.05
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 23
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - 0.47
    - 0.22
    - 0.93
    metric_stds:
    - 0.06
    - 0.06
    - 0.16
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.47
    sort_std: 0.06
    true_value: 0.47
    true_std: 0.06
    paper_value: 0.47
    paper_std: 0.06
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: 0.4107
    at_pub_std: 0.0312
    at_pub_source_arxiv: '2212.08665'
    at_pub_source_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering
      [5]
    at_pub_source_date_iso: '2022-12-16'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.059299999999999964
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 22
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - 0.46
    - 0.26
    - 0.73
    metric_stds:
    - 0.05
    - 0.02
    - 0.22
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.46
    sort_std: 0.05
    true_value: 0.46
    true_std: 0.05
    paper_value: 0.46
    paper_std: 0.05
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 25
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    metric_values:
    - 0.42
    - 0.22
    - 0.49
    metric_stds:
    - 0.06
    - 0.02
    - 0.19
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.42
    sort_std: 0.06
    true_value: 0.42
    true_std: 0.06
    paper_value: 0.42
    paper_std: 0.06
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: 0.3231
    at_pub_std: 0.0097
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.09689999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: improved
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: false
    is_std_outlier: false
    global_rank: 27
  - model: DMoN
    model_key: dmon
    model_plain: DMoN
    metric_values:
    - 0.35
    - 0.07
    - 0.59
    metric_stds:
    - 0.04
    - 0.02
    - 0.48
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.35
    sort_std: 0.04
    true_value: 0.35
    true_std: 0.04
    paper_value: 0.35
    paper_std: 0.04
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 28
  - model: VGAER
    model_key: vgaer
    model_plain: VGAER
    metric_values:
    - 0.34
    - 0.11
    - 0.51
    metric_stds:
    - 0.03
    - 0.06
    - 0.2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.34
    sort_std: 0.03
    true_value: 0.34
    true_std: 0.03
    paper_value: 0.34
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 30
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    metric_values:
    - 0.19
    - 0.06
    - 0.93
    metric_stds:
    - 0.02
    - 0.02
    - 0.01
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.19
    sort_std: 0.02
    true_value: 0.19
    true_std: 0.02
    paper_value: 0.19
    paper_std: 0.02
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 32
  metrics:
  - F1
  - NMI
  - Conductance
  primary_metric: F1
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  - NMI
  - Conductance
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: Texas
  is_multi_metric: true
  rows:
  - model: FPS-T
    model_key: fps-t
    model_plain: FPS-T
    metric_values:
    - 0.8919
    - null
    - null
    - null
    metric_stds:
    - 0.0237
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2309.04082'
    title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
      Learning'
    published_venue: ''
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.8919
    sort_std: 0.0237
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: TokenGT
    model_key: tokengt
    model_plain: TokenGT
    metric_values:
    - 0.8865
    - null
    - null
    - null
    metric_stds:
    - 0.0206
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2309.04082'
    title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
      Learning'
    published_venue: ''
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.8865
    sort_std: 0.0206
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: HAT
    model_key: hat
    model_plain: HAT
    metric_values:
    - 0.8216
    - null
    - null
    - null
    metric_stds:
    - 0.0252
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.04082'
    title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
      Learning'
    published_venue: ''
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.8216
    sort_std: 0.0252
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.7054
    - null
    - null
    - null
    metric_stds:
    - 0.03
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2309.04082'
    title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
      Learning'
    published_venue: ''
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 4
    is_best: false
    sort_value: 0.7054
    sort_std: 0.03
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - 0.6838
    - null
    - null
    - null
    metric_stds:
    - 0.0354
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.04082'
    title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
      Learning'
    published_venue: ''
    date: Sep 8, 2023
    date_display: Sep 2023
    date_iso: '2023-09-08'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 5
    is_best: false
    sort_value: 0.6838
    sort_std: 0.0354
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - null
    - 0.31
    - 0.12
    - 0.7
    metric_stds:
    - null
    - 0.03
    - 0.02
    - 0.29
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.541
    sort_std: null
    true_value: 0.541
    true_std: null
    paper_value: 0.31
    paper_std: 0.03
    has_value_gap: true
    has_value_note: false
    value_gap: 0.23100000000000004
    value_gap_source_arxiv: '2203.10866'
    value_gap_source_title: Unsupervised Network Embedding Beyond Homophily
    value_note: ''
    at_pub_value: 0.541
    at_pub_std: null
    at_pub_source_arxiv: '2203.10866'
    at_pub_source_title: Unsupervised Network Embedding Beyond Homophily
    at_pub_source_date_iso: '2022-03-21'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2022-03-21'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: 0.23100000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Unsupervised Network Embedding Beyond Homophily
    comparison_source_arxiv: '2203.10866'
    is_best: false
    is_std_outlier: false
    global_rank: 16
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    metric_values:
    - null
    - 0.35
    - 0.14
    - 0.7
    metric_stds:
    - null
    - 0.05
    - 0.02
    - 0.15
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.35
    sort_std: 0.05
    true_value: 0.35
    true_std: 0.05
    paper_value: 0.35
    paper_std: 0.05
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 24
  - model: uAGNN
    model_key: uagnn
    model_plain: uAGNN
    metric_values:
    - null
    - 0.33
    - 0.22
    - 0.46
    metric_stds:
    - null
    - 0.09
    - 0.07
    - 0.14
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.33
    sort_std: 0.09
    true_value: 0.33
    true_std: 0.09
    paper_value: 0.33
    paper_std: 0.09
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 26
  - model: DMoN
    model_key: dmon
    model_plain: DMoN
    metric_values:
    - null
    - 0.33
    - 0.21
    - 0.8
    metric_stds:
    - null
    - 0.02
    - 0.04
    - 0.21
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.33
    sort_std: 0.02
    true_value: 0.33
    true_std: 0.02
    paper_value: 0.33
    paper_std: 0.02
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 25
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    metric_values:
    - null
    - 0.29
    - 0.15
    - 0.82
    metric_stds:
    - null
    - 0.08
    - 0.0
    - 0.3
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.29
    sort_std: 0.08
    true_value: 0.29
    true_std: 0.08
    paper_value: 0.29
    paper_std: 0.08
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 27
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - null
    - 0.29
    - 0.1
    - 0.77
    metric_stds:
    - null
    - 0.02
    - 0.02
    - 0.24
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.29
    sort_std: 0.02
    true_value: 0.29
    true_std: 0.02
    paper_value: 0.29
    paper_std: 0.02
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 28
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    metric_values:
    - null
    - 0.24
    - 0.06
    - 0.76
    metric_stds:
    - null
    - 0.03
    - 0.03
    - 0.11
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.24
    sort_std: 0.03
    true_value: 0.24
    true_std: 0.03
    paper_value: 0.24
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 29
  - model: VGAER
    model_key: vgaer
    model_plain: VGAER
    metric_values:
    - null
    - 0.24
    - 0.08
    - 0.48
    metric_stds:
    - null
    - 0.03
    - 0.02
    - 0.1
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.24
    sort_std: 0.03
    true_value: 0.24
    true_std: 0.03
    paper_value: 0.24
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 30
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    metric_values:
    - null
    - 0.21
    - 0.03
    - 0.42
    metric_stds:
    - null
    - 0.03
    - 0.01
    - 0.25
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.21
    sort_std: 0.03
    true_value: 0.21
    true_std: 0.03
    paper_value: 0.21
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 31
  metrics:
  - Accuracy
  - F1
  - NMI
  - Conductance
  primary_metric: Accuracy
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - F1
  - NMI
  - Conductance
  metric: F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id005
  dataset: UAT
  is_multi_metric: true
  rows:
  - model: SCAGC
    model_key: scagc
    model_plain: SCAGC
    metric_values:
    - 0.7277
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    published_venue: ''
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.7277
    sort_std: 0.0016
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: SCGC
    model_key: scgc
    model_plain: SCGC
    metric_values:
    - 0.7222
    - null
    - null
    metric_stds:
    - 0.0097
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    published_venue: ''
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.7222
    sort_std: 0.0097
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: AGE
    model_key: age
    model_plain: AGE
    metric_values:
    - 0.7174
    - null
    - null
    metric_stds:
    - 0.0093
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    published_venue: ''
    date: May 11, 2022
    date_display: May 2022
    date_iso: '2022-05-11'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: true
    sort_value: 0.7174
    sort_std: 0.0093
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    metric_values:
    - 0.54
    - 0.16
    - 1.0
    metric_stds:
    - 0.01
    - 0.04
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6987
    sort_std: 0.0054
    true_value: 0.6987
    true_std: 0.0054
    paper_value: 0.54
    paper_std: 0.01
    has_value_gap: true
    has_value_note: false
    value_gap: 0.15869999999999995
    value_gap_source_arxiv: '2205.07865'
    value_gap_source_title: Simple Contrastive Graph Clustering
    value_note: ''
    at_pub_value: 0.6987
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2205.07865'
    at_pub_source_title: Simple Contrastive Graph Clustering
    at_pub_source_date_iso: '2022-05-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.15869999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Simple Contrastive Graph Clustering
    comparison_source_arxiv: '2205.07865'
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: uAGNN
    model_key: uagnn
    model_plain: uAGNN
    metric_values:
    - 0.53
    - 0.29
    - 0.69
    metric_stds:
    - 0.02
    - 0.02
    - 0.23
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.53
    sort_std: 0.02
    true_value: 0.53
    true_std: 0.02
    paper_value: 0.53
    paper_std: 0.02
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 15
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - 0.52
    - 0.24
    - 0.7
    metric_stds:
    - 0.03
    - 0.03
    - 0.15
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.52
    sort_std: 0.03
    true_value: 0.52
    true_std: 0.03
    paper_value: 0.52
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 18
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    metric_values:
    - 0.52
    - 0.27
    - 0.94
    metric_stds:
    - 0.03
    - 0.01
    - 0.19
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.52
    sort_std: 0.03
    true_value: 0.52
    true_std: 0.03
    paper_value: 0.52
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 19
  - model: DMoN
    model_key: dmon
    model_plain: DMoN
    metric_values:
    - 0.49
    - 0.2
    - 0.67
    metric_stds:
    - 0.04
    - 0.04
    - 0.44
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.49
    sort_std: 0.04
    true_value: 0.49
    true_std: 0.04
    paper_value: 0.49
    paper_std: 0.04
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 25
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - 0.49
    - 0.29
    - 0.9
    metric_stds:
    - 0.04
    - 0.02
    - 0.03
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.49
    sort_std: 0.04
    true_value: 0.49
    true_std: 0.04
    paper_value: 0.49
    paper_std: 0.04
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: 0.3944
    at_pub_std: 0.0219
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.09560000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: improved
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: false
    is_std_outlier: false
    global_rank: 24
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    metric_values:
    - 0.48
    - 0.24
    - 0.88
    metric_stds:
    - 0.02
    - 0.0
    - 0.11
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.48
    sort_std: 0.02
    true_value: 0.48
    true_std: 0.02
    paper_value: 0.48
    paper_std: 0.02
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 26
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    metric_values:
    - 0.17
    - 0.2
    - 0.5
    metric_stds:
    - 0.13
    - 0.05
    - 0.2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4619
    sort_std: 0.0087
    true_value: 0.4619
    true_std: 0.0087
    paper_value: 0.17
    paper_std: 0.13
    has_value_gap: true
    has_value_note: false
    value_gap: 0.29189999999999994
    value_gap_source_arxiv: '2212.03559'
    value_gap_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    value_note: ''
    at_pub_value: 0.4619
    at_pub_std: 0.0087
    at_pub_source_arxiv: '2212.03559'
    at_pub_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.29189999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'GraphLearner: Graph Node Clustering with Fully Learnable
      Augmentation'
    comparison_source_arxiv: '2212.03559'
    is_best: false
    is_std_outlier: false
    global_rank: 29
  - model: VGAER
    model_key: vgaer
    model_plain: VGAER
    metric_values:
    - 0.44
    - 0.2
    - 0.75
    metric_stds:
    - 0.03
    - 0.02
    - 0.12
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.44
    sort_std: 0.03
    true_value: 0.44
    true_std: 0.03
    paper_value: 0.44
    paper_std: 0.03
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 30, 2025
    date_display: Jun 2025
    date_iso: '2025-06-30'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 31
  metrics:
  - F1
  - NMI
  - Conductance
  primary_metric: F1
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  - NMI
  - Conductance
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
  - *id002
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id003
- benchmark: Hypergraph Benchmarks
  datasets:
  - *id004
  - *id005
  - *id006
  - *id007
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
  - benchmark: Hypergraph Benchmarks
    benchmark_slug: hypergraph-benchmarks
    datasets:
    - dataset: AMAP
      dataset_slug: amap
    - dataset: UAT
      dataset_slug: uat
    - dataset: BAT
      dataset_slug: bat
    - dataset: EAT
      dataset_slug: eat
single_proposed_model: uAGNN
main_figure: /figures/2508.14097/main_figure.jpegoptim.jpg
---

