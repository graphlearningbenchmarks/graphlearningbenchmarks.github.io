---
title: EAT
slug: eat
benchmark: Hypergraph Benchmarks
task_type: node_classification
description: European Airport Transactions hypergraph node classification (4 region
  classes, 399 nodes).
primary_metric: F1
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 1
  avg_nodes: 399.0
  avg_edges: null
  num_classes: 4
result_count: 51
best_model:
  model: ProGCL
  value: 0.7702
  metric: F1
  arxiv_id: '2212.08665'
  paper_title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
papers:
- arxiv_id: '2508.14097'
  title: Non-Dissipative Graph Propagation for Non-Local Community Detection
  date_iso: '2025-06-30'
  venue: ''
- arxiv_id: '2307.14613'
  title: Self-Contrastive Graph Diffusion Network
  date_iso: '2023-07-27'
  venue: ''
- arxiv_id: '2212.08665'
  title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
  date_iso: '2022-12-16'
  venue: AAAI 2022
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
    avg_nodes: 399.0
    avg_edges: null
    num_classes: 4
  metrics:
  - F1
  - Conductance
  - NMI
  metric_display_names:
  - F1
  - Conductance
  - NMI
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: ProGCL
    model_plain: ProGCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7702
    - null
    - null
    metric_stds:
    - 0.0033
    - null
    - null
  - model: HSAN
    model_plain: HSAN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7702
    - null
    - null
    metric_stds:
    - 0.0033
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
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7682
    - null
    - null
    metric_stds:
    - 0.0023
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
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7681
    - null
    - null
    metric_stds:
    - 0.0145
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
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7598
    - null
    - null
    metric_stds:
    - 0.0068
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
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7596
    - null
    - null
    metric_stds:
    - 0.0023
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
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7551
    - null
    - null
    metric_stds:
    - 0.0077
    - null
    - null
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7277
    - null
    - null
    metric_stds:
    - 0.0016
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
    metric_stds:
    - 0.0097
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
    - 0.7174
    - null
    - null
    metric_stds:
    - 0.0093
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
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7157
    - null
    - null
    metric_stds:
    - 0.0248
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
    - 0.7125
    - null
    - null
    metric_stds:
    - 0.0031
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
    metric_stds:
    - 0.0054
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
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6928
    - null
    - null
    metric_stds:
    - 0.023
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
    metric_stds:
    - 0.0176
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
    metric_stds:
    - 0.0195
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5763
    - null
    - null
    metric_stds:
    - 0.001
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
    - 0.5753
    - null
    - null
    metric_stds:
    - 0.0067
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
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5455
    - null
    - null
    metric_stds:
    - 0.0097
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
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5344
    - null
    - null
    metric_stds:
    - 0.0081
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
    metric_stds:
    - 0.0001
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
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5153
    - null
    - null
    metric_stds:
    - 0.0038
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
    metric_stds:
    - 0.0149
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
    - 0.4822
    - null
    - null
    metric_stds:
    - 0.0033
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
    - 0.48
    - 1.0
    - 0.31
    metric_stds:
    - 0.03
    - 0.0
    - 0.02
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
    metric_stds:
    - 0.002
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
    - 0.4706
    - null
    - null
    metric_stds:
    - 0.0066
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
    - 0.47
    - 0.93
    - 0.22
    metric_stds:
    - 0.06
    - 0.16
    - 0.06
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
    - 0.47
    - 0.4
    - 0.32
    metric_stds:
    - 0.05
    - 0.37
    - 0.01
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
    metric_stds:
    - 0.0012
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
    - 0.46
    - 0.73
    - 0.26
    metric_stds:
    - 0.05
    - 0.22
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
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: Dec 16, 2022
    date_iso: '2022-12-16'
    date_display: Dec 2022
    codebase_url: https://github.com/yueliu1999/HSAN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4375
    - null
    - null
    metric_stds:
    - 0.0078
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
    - 0.4308
    - null
    - null
    metric_stds:
    - 0.0326
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
    - 0.4295
    - null
    - null
    metric_stds:
    - 0.0004
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
    - 0.4254
    - null
    - null
    metric_stds:
    - 0.0045
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
    is_std_outlier: false
    metric_values:
    - 0.42
    - 0.49
    - 0.22
    metric_stds:
    - 0.06
    - 0.19
    - 0.02
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
    - 0.41
    - 1.0
    - 0.13
    metric_stds:
    - 0.02
    - 0.0
    - 0.02
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
    - 0.352
    - null
    - null
    metric_stds:
    - 0.0017
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
    - 0.35
    - 0.59
    - 0.07
    metric_stds:
    - 0.04
    - 0.48
    - 0.02
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
    - 0.3472
    - null
    - null
    metric_stds:
    - 0.0016
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
    - 0.3472
    - null
    - null
    metric_stds:
    - 0.0016
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
    - 0.34
    - 0.51
    - 0.11
    metric_stds:
    - 0.03
    - 0.2
    - 0.06
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
    - 0.3342
    - null
    - null
    metric_stds:
    - 0.031
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
    metric_stds:
    - 0.055
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
    - 0.3231
    - null
    - null
    metric_stds:
    - 0.0097
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
    - 0.3053
    - null
    - null
    metric_stds:
    - 0.0147
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
    - 0.2535
    - null
    - null
    metric_stds:
    - 0.0075
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
    - 0.2502
    - null
    - null
    metric_stds:
    - 0.0021
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
    metric_stds:
    - 0.0051
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
    - 0.2182
    - null
    - null
    metric_stds:
    - 0.0098
    - null
    - null
  row_count: 51
  rows_json: /data/datasets/eat/standard-split-rows.json
  chart_json: /data/datasets/eat/standard-split-chart.json
  arch_counts:
    gnn: 46
    hybrid: 2
    graph_transformer: 0
    llm: 0
    walk: 1
    traditional: 2
  metric_counts:
  - 51
  - 9
  - 9
  milestones: &id001
  - value: 0.7277
    std: 0.0016
    model: SCAGC
    arxiv_id: '2205.07865'
    title: Simple Contrastive Graph Clustering
    date: '2022-05-11'
  - value: 0.7702
    std: 0.0033
    model: ProGCL
    arxiv_id: '2212.08665'
    title: Hard Sample Aware Network for Contrastive Deep Graph Clustering [5]
    date: '2022-12-16'
  milestones_by_metric:
    F1: *id001
    Conductance:
    - value: 0.4
      std: 0.37
      model: uAGNN
      arxiv_id: '2508.14097'
      title: Non-Dissipative Graph Propagation for Non-Local Community Detection
      date: '2025-06-30'
    NMI:
    - value: 0.32
      std: 0.01
      model: uAGNN
      arxiv_id: '2508.14097'
      title: Non-Dissipative Graph Propagation for Non-Local Community Detection
      date: '2025-06-30'
---

