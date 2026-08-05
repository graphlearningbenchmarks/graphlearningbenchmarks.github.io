---
title: MalNet-Tiny
slug: malnet-tiny
benchmark: Other Graph Benchmarks
task_type: graph_classification
description: 'Malware detection graph classification on a tiny (balanced 5-class)
  subset of the MalNet-Large dataset. Graphs are function call graphs of Android apps.

  '
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MalNetTiny.html
stats:
  num_graphs: 5000
  avg_nodes: null
  avg_edges: null
  num_classes: 5
result_count: 37
best_model:
  model: GMN
  value: 0.9415
  metric: Accuracy
  arxiv_id: '2402.08678'
  paper_title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
papers:
- arxiv_id: '2510.13615'
  title: 'Message Passing on the Edge: Towards Scalable and Expressive GNNs'
  date_iso: '2025-10-15'
  venue: ''
- arxiv_id: '2509.13735'
  title: State Space Models over Directed Graphs
  date_iso: '2025-09-17'
  venue: ''
- arxiv_id: '2402.08678'
  title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
  date_iso: '2024-02-13'
  venue: KDD 2024
- arxiv_id: '2210.13148'
  title: Transformers over Directed Acyclic Graphs
  date_iso: '2022-10-24'
  venue: NeurIPS 2022
- arxiv_id: '2205.12454'
  title: Recipe for a General, Powerful, Scalable Graph Transformer
  date_iso: '2022-05-25'
  venue: NeurIPS 2022
- arxiv_id: '2011.07682'
  title: A Large-Scale Database for Graph Representation Learning
  date_iso: '2020-11-16'
  venue: NeurIPS 2020
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 5000
    avg_nodes: null
    avg_edges: null
    num_classes: 5
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GMN
    model_plain: GMN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9415
    metric_stds:
    - 0.002
  - model: DirGraphSSM
    model_plain: DirGraphSSM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_iso: '2025-09-17'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9409
    metric_stds:
    - 0.0023
  - model: DAG+SAT-plus
    model_plain: DAG+SAT-plus
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_iso: '2025-09-17'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9407
    metric_stds:
    - 0.002
  - model: Graph-Mamba
    model_plain: Graph-Mamba
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_iso: '2025-09-17'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9406
    metric_stds:
    - 0.0018
  - model: DAG+Transformer-plus
    model_plain: DAG+Transformer-plus
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_iso: '2025-09-17'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9404
    metric_stds:
    - 0.0019
  - model: Exphormer
    model_plain: Exphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9402
    metric_stds:
    - 0.002
  - model: Transformer
    model_plain: Transformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.935
    metric_stds:
    - 0.006
  - model: DAG+GraphGPS
    model_plain: DAG+GraphGPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2210.13148'
    title: Transformers over Directed Acyclic Graphs
    date: Oct 24, 2022
    date_iso: '2022-10-24'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9345
    metric_stds:
    - 0.0041
  - model: EB-GNN
    model_plain: EB-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.13615'
    title: 'Message Passing on the Edge: Towards Scalable and Expressive GNNs'
    date: Oct 15, 2025
    date_iso: '2025-10-15'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.933
    metric_stds:
    - 0.0066
  - model: SignNetⁿbⁿDeepSets
    model_plain: SignNetⁿbⁿDeepSets
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9313
    metric_stds:
    - null
  - model: GPS + Mamba
    model_plain: GPS + Mamba
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9311
    metric_stds:
    - 0.0042
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9298
    metric_stds:
    - 0.0047
  - model: HyMN
    model_plain: HyMN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.13615'
    title: 'Message Passing on the Edge: Towards Scalable and Expressive GNNs'
    date: Oct 15, 2025
    date_iso: '2025-10-15'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9284
    metric_stds:
    - 0.0052
  - model: RWSE
    model_plain: RWSE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9277
    metric_stds:
    - null
  - model: LapPE
    model_plain: LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9274
    metric_stds:
    - null
  - model: GraphGPS
    model_plain: GraphGPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.13148'
    title: Transformers over Directed Acyclic Graphs
    date: Oct 24, 2022
    date_iso: '2022-10-24'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9264
    metric_stds:
    - 0.0078
  - model: Performer
    model_plain: Performer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9264
    metric_stds:
    - null
  - model: None
    model_plain: None
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9264
    metric_stds:
    - null
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9264
    metric_stds:
    - null
  - model: SignNetⁿbⁿMLP
    model_plain: SignNetⁿbⁿMLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9257
    metric_stds:
    - null
  - model: SAT
    model_plain: SAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_iso: '2025-09-17'
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
    - 0.9256
    metric_stds:
    - 0.0031
  - model: NC-GNN
    model_plain: NC-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.13615'
    title: 'Message Passing on the Edge: Towards Scalable and Expressive GNNs'
    date: Oct 15, 2025
    date_iso: '2025-10-15'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.925
    metric_stds:
    - 0.0056
  - model: BigBird
    model_plain: BigBird
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9234
    metric_stds:
    - null
  - model: GINE
    model_plain: GINE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9227
    metric_stds:
    - null
  - model: PEGⁿbⁿLapEig
    model_plain: PEGⁿbⁿLapEig
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9227
    metric_stds:
    - null
  - model: Gated-GCN
    model_plain: Gated-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9223
    metric_stds:
    - 0.0065
  - model: GPS (Perf.)
    model_plain: GPS (Perf.)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.13615'
    title: 'Message Passing on the Edge: Towards Scalable and Expressive GNNs'
    date: Oct 15, 2025
    date_iso: '2025-10-15'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9214
    metric_stds:
    - 0.0024
  - model: PNA
    model_plain: PNA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9167
    metric_stds:
    - null
  - model: MPNN
    model_plain: MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.13615'
    title: 'Message Passing on the Edge: Towards Scalable and Expressive GNNs'
    date: Oct 15, 2025
    date_iso: '2025-10-15'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.911
    metric_stds:
    - 0.0098
  - model: MagNet
    model_plain: MagNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_iso: '2025-09-17'
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
    - 0.9095
    metric_stds:
    - 0.0025
  - model: DiGCN
    model_plain: DiGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_iso: '2025-09-17'
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
    - 0.9081
    metric_stds:
    - 0.0017
  - model: DirGNN
    model_plain: DirGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_iso: '2025-09-17'
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
    - 0.9073
    metric_stds:
    - 0.0015
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8898
    metric_stds:
    - 0.0055
  - model: Feather
    model_plain: Feather
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2011.07682'
    title: A Large-Scale Database for Graph Representation Learning
    date: Nov 16, 2020
    date_iso: '2020-11-16'
    date_display: Nov 2020
    codebase_url: https://github.com/safreita1/malnet-graph
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.86
    metric_stds:
    - null
  - model: LDP
    model_plain: LDP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.07682'
    title: A Large-Scale Database for Graph Representation Learning
    date: Nov 16, 2020
    date_iso: '2020-11-16'
    date_display: Nov 2020
    codebase_url: https://github.com/safreita1/malnet-graph
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.86
    metric_stds:
    - null
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: Sep 17, 2025
    date_iso: '2025-09-17'
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
    - 0.8509
    metric_stds:
    - 0.0025
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.81
    metric_stds:
    - 0.0
  row_count: 37
  rows_json: ''
  chart_json: /data/datasets/malnet-tiny/standard-split-chart.json
  arch_counts:
    gnn: 16
    hybrid: 5
    graph_transformer: 11
    llm: 0
    walk: 1
    traditional: 0
  metric_counts:
  - 37
  milestones: &id001
  - value: 0.9345
    std: 0.0041
    model: DAG+GraphGPS
    arxiv_id: '2210.13148'
    title: Transformers over Directed Acyclic Graphs
    date: '2022-10-24'
  - value: 0.9415
    std: 0.002
    model: GMN
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: '2024-02-13'
  milestones_by_metric:
    Accuracy: *id001
---

