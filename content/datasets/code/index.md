---
title: Code
slug: code
benchmark: OGB
task_type: graph_classification
description: Code AST-level method name prediction (ogbg-code2). 143k Python snippets.
primary_metric: F1
higher_is_better: true
pyg_url: https://ogb.stanford.edu/docs/leader_graphprop/#ogbg-code2
stats:
  num_graphs: 452741
  avg_nodes: 125.2
  avg_edges: 124.2
  num_classes: 1
result_count: 17
best_model:
  model: K-Subtree SAT
  value: 0.1937
  metric: F1
  arxiv_id: '2406.12059'
  paper_title: A Scalable and Effective Alternative to Graph Transformers
papers:
- arxiv_id: '2406.12059'
  title: A Scalable and Effective Alternative to Graph Transformers
  date_iso: '2024-06-17'
  venue: AAAI 2024
- arxiv_id: '2311.07966'
  title: Higher-Order Expander Graph Propagation
  date_iso: '2023-11-14'
  venue: ''
- arxiv_id: '2206.02886'
  title: Graph Rationalization with Environment-based Augmentations
  date_iso: '2022-06-06'
  venue: KDD 2022
variants:
- slug: standard-split
  name: Standard split
  notes: OGB project split.
  is_standard: true
  primary_metric: F1
  default_metric: F1
  higher_is_better: true
  stats:
    num_graphs: 452741
    avg_nodes: 125.2
    avg_edges: 124.2
    num_classes: 1
  metrics:
  - F1
  - ROC-AUC
  metric_display_names:
  - F1
  - ROC-AUC
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: K-Subtree SAT
    model_plain: K-Subtree SAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.12059'
    title: A Scalable and Effective Alternative to Graph Transformers
    date: Jun 17, 2024
    date_iso: '2024-06-17'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.1937
    - null
    metric_stds:
    - 0.0028
    - null
  - model: GECO
    model_plain: GECO
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.12059'
    title: A Scalable and Effective Alternative to Graph Transformers
    date: Jun 17, 2024
    date_iso: '2024-06-17'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.1915
    - null
    metric_stds:
    - 0.002
    - null
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.12059'
    title: A Scalable and Effective Alternative to Graph Transformers
    date: Jun 17, 2024
    date_iso: '2024-06-17'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.1894
    - null
    metric_stds:
    - 0.0024
    - null
  - model: GraphTrans (GCN-Virtual)
    model_plain: GraphTrans (GCN-Virtual)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.12059'
    title: A Scalable and Effective Alternative to Graph Transformers
    date: Jun 17, 2024
    date_iso: '2024-06-17'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.183
    - null
    metric_stds:
    - 0.0024
    - null
  - model: higher-order expander graph propagation
    model_plain: higher-order expander graph propagation
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2311.07966'
    title: Higher-Order Expander Graph Propagation
    date: Nov 14, 2023
    date_iso: '2023-11-14'
    date_display: Nov 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1519
    - null
    metric_stds:
    - 0.002
    - null
  - model: EGP
    model_plain: EGP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.07966'
    title: Higher-Order Expander Graph Propagation
    date: Nov 14, 2023
    date_iso: '2023-11-14'
    date_display: Nov 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1497
    - null
    metric_stds:
    - 0.0015
    - null
  - model: Plain GIN
    model_plain: Plain GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.07966'
    title: Higher-Order Expander Graph Propagation
    date: Nov 14, 2023
    date_iso: '2023-11-14'
    date_display: Nov 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1495
    - null
    metric_stds:
    - 0.0023
    - null
  - model: GIN + 3-Regular Bipartite Expander + Summation
    model_plain: GIN + 3-Regular Bipartite Expander + Summation
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.07966'
    title: Higher-Order Expander Graph Propagation
    date: Nov 14, 2023
    date_iso: '2023-11-14'
    date_display: Nov 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1254
    - null
    metric_stds:
    - 0.0029
    - null
  - model: U-NetsPool
    model_plain: U-NetsPool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.7757
    metric_stds:
    - null
    - 0.0173
  - model: SelfAttnPool
    model_plain: SelfAttnPool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.7383
    metric_stds:
    - null
    - 0.0541
  - model: StableGNN
    model_plain: StableGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.6607
    metric_stds:
    - null
    - 0.05
  - model: OOD-GNN
    model_plain: OOD-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.8096
    metric_stds:
    - null
    - 0.0132
  - model: IRM
    model_plain: IRM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.7947
    metric_stds:
    - null
    - 0.0186
  - model: DIR
    model_plain: DIR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.6751
    metric_stds:
    - null
    - 0.0323
  - model: DIR+RepAug
    model_plain: DIR+RepAug
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.7677
    metric_stds:
    - null
    - 0.0226
  - model: GREA-RepAug
    model_plain: GREA-RepAug
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.7655
    metric_stds:
    - null
    - 0.0529
  - model: two augmentation methods based on environment subgraphs
    model_plain: two augmentation methods based on environment subgraphs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.8191
    metric_stds:
    - null
    - 0.024
  row_count: 17
  rows_json: ''
  chart_json: /data/datasets/code/standard-split-chart.json
  arch_counts:
    gnn: 8
    hybrid: 6
    graph_transformer: 2
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 8
  - 9
  milestones: &id001
  - value: 0.1519
    std: 0.002
    model: higher-order expander graph propagation
    arxiv_id: '2311.07966'
    title: Higher-Order Expander Graph Propagation
    date: '2023-11-14'
  - value: 0.1937
    std: 0.0028
    model: K-Subtree SAT
    arxiv_id: '2406.12059'
    title: A Scalable and Effective Alternative to Graph Transformers
    date: '2024-06-17'
  milestones_by_metric:
    F1: *id001
    ROC-AUC:
    - value: 0.8191
      std: 0.024
      model: two augmentation methods based on environment subgraphs
      arxiv_id: '2206.02886'
      title: Graph Rationalization with Environment-based Augmentations
      date: '2022-06-06'
---

