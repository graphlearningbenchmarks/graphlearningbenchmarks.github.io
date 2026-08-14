---
title: London
slug: london
benchmark: City-Networks
task_type: node_classification
short_description: Predict an accessibility class for every intersection on the London
  road graph.
description: '**Node classification** on the London road graph, predicting an accessibility
  class for every intersection. Street segments are edges and labels depend on long-range
  network structure. Evaluated by Accuracy.'
detailed_description:
  task: London road-network node classification from the City-Networks benchmark.
    Labels are derived from long-range accessibility statistics on the city graph.
    The primary catalog metric is Accuracy.
  data: London road-network node classification from the City-Networks benchmark.
    Labels are derived from long-range accessibility statistics on the city graph.
    The cataloged artifact reports 1 graphs.
  features: Road-network intersections are nodes and street segments are edges. The
    release derives node inputs and accessibility-based labels from the embedded city
    network; adding coordinates, centralities, or external map attributes changes
    the feature set.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses Accuracy (higher is better). Exact masks or folds must
    come from the cited release.'
  quirks_and_pitfalls: The four cities differ in topology, sampling, and label distribution,
    so they are separate datasets rather than interchangeable folds. Labels are derived
    from the same graph, creating a risk of target leakage through engineered centrality
    or accessibility features.
sources:
- title: City-Networks benchmark
  arxiv_id: '2503.09008'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric London loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.CityNetwork.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.CityNetwork.html
stats:
  num_graphs: 1
  avg_nodes: 569000.0
  avg_edges: 759000.0
  num_classes: null
  extra_stats:
    avg_degree: 2.7
    clustering_coefficient: 0.04
    diameter: 404
    edge_feature_dim: 25
    edge_feature_type: road length, speed limit, one-way, reversed, lanes, and road
      type; 25 dimensions after one-hot encoding
    edge_homophily: 0.76
    feature_type: OpenStreetMap junction features plus averaged incident-road features;
      37 dimensions after one-hot encoding and aggregation
    node_feature_dim: 37
    statistic_notes: 'City-Networks Table 1: largest connected component of the undirected
      London road graph; counts and topology statistics are rounded.'
    transitivity: 0.05
result_count: 15
best_model:
  model: GatedGCN
  value: 0.6147
  metric: Accuracy
  arxiv_id: '2604.03815'
  paper_title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
    Power of GraphGPS
papers:
- arxiv_id: '2604.03815'
  title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
    Power of GraphGPS
  date_iso: '2026-04-04'
  venue: ICLR 2026
- arxiv_id: '2503.09008'
  title: City-Networks
  date_iso: '2025-03-12'
  venue: ICLR 2025
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 569000.0
    avg_edges: 759000.0
    num_classes: null
    extra_stats:
      avg_degree: 2.7
      clustering_coefficient: 0.04
      diameter: 404
      edge_feature_dim: 25
      edge_feature_type: road length, speed limit, one-way, reversed, lanes, and road
        type; 25 dimensions after one-hot encoding
      edge_homophily: 0.76
      feature_type: OpenStreetMap junction features plus averaged incident-road features;
        37 dimensions after one-hot encoding and aggregation
      node_feature_dim: 37
      statistic_notes: 'City-Networks Table 1: largest connected component of the
        undirected London road graph; counts and topology statistics are rounded.'
      transitivity: 0.05
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.6147
    metric_stds:
    - 0.0014
  - model: GINE
    model_plain: GINE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.576
    metric_stds:
    - 0.002
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5719
    metric_stds:
    - 0.0109
  - model: GPS + k-MIP
    model_plain: GPS + k-MIP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5605
    metric_stds:
    - null
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_iso: '2025-03-12'
    date_display: Mar 2025
    codebase_url: https://github.com/LeonResearch/City-Networks
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.554
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
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5525
    metric_stds:
    - 0.0006
  - model: ChebNet
    model_plain: ChebNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_iso: '2025-03-12'
    date_display: Mar 2025
    codebase_url: https://github.com/LeonResearch/City-Networks
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.547
    metric_stds:
    - 0.002
  - model: GPS + Performer
    model_plain: GPS + Performer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.532
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
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_iso: '2025-03-12'
    date_display: Mar 2025
    codebase_url: https://github.com/LeonResearch/City-Networks
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.52
    metric_stds:
    - 0.003
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_iso: '2025-03-12'
    date_display: Mar 2025
    codebase_url: https://github.com/LeonResearch/City-Networks
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.501
    metric_stds:
    - 0.007
  - model: Exphormer
    model_plain: Exphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_iso: '2025-03-12'
    date_display: Mar 2025
    codebase_url: https://github.com/LeonResearch/City-Networks
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.495
    metric_stds:
    - 0.004
  - model: SGFormer
    model_plain: SGFormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_iso: '2025-03-12'
    date_display: Mar 2025
    codebase_url: https://github.com/LeonResearch/City-Networks
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.483
    metric_stds:
    - 0.003
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_iso: '2025-03-12'
    date_display: Mar 2025
    codebase_url: https://github.com/LeonResearch/City-Networks
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.482
    metric_stds:
    - 0.003
  - model: DropEdge
    model_plain: DropEdge
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_iso: '2025-03-12'
    date_display: Mar 2025
    codebase_url: https://github.com/LeonResearch/City-Networks
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.45
    metric_stds:
    - 0.003
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_iso: '2025-03-12'
    date_display: Mar 2025
    codebase_url: https://github.com/LeonResearch/City-Networks
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.279
    metric_stds:
    - 0.001
  row_count: 15
  rows_json: ''
  chart_json: /data/datasets/london/standard-split-chart.json
  arch_counts:
    gnn: 9
    hybrid: 2
    graph_transformer: 2
    llm: 0
    walk: 0
    traditional: 2
  metric_counts:
  - 15
  milestones: &id001
  - value: 0.554
    std: 0.002
    model: GraphSAGE
    arxiv_id: '2503.09008'
    title: City-Networks
    date: '2025-03-12'
  - value: 0.6147
    std: 0.0014
    model: GatedGCN
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: '2026-04-04'
  milestones_by_metric:
    Accuracy: *id001
---

