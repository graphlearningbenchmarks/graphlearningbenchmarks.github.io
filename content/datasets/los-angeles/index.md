---
title: Los Angeles
slug: los-angeles
benchmark: City-Networks
task_type: node_classification
short_description: Predict an accessibility class for every intersection on the Los
  Angeles road graph.
description: '**Node classification** on the Los Angeles road graph, predicting an
  accessibility class for every intersection. Street segments are edges and labels
  depend on long-range network structure. Evaluated by Accuracy.'
detailed_description:
  task: Los Angeles road-network node classification from the City-Networks benchmark.
    Labels are derived from long-range accessibility statistics on the city graph.
    The primary catalog metric is Accuracy.
  data: Los Angeles road-network node classification from the City-Networks benchmark.
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
- title: PyTorch Geometric Los Angeles loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.CityNetwork.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.CityNetwork.html
stats:
  num_graphs: 1
  avg_nodes: 241000.0
  avg_edges: 343000.0
  num_classes: null
result_count: 10
best_model:
  model: Exphormer
  value: 0.638
  metric: Accuracy
  arxiv_id: '2503.09008'
  paper_title: City-Networks
papers:
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
    avg_nodes: 241000.0
    avg_edges: 343000.0
    num_classes: null
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.638
    metric_stds:
    - 0.006
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
    - 0.614
    metric_stds:
    - 0.004
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
    - 0.614
    metric_stds:
    - 0.003
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
    - 0.601
    metric_stds:
    - 0.007
  - model: GraphGPS
    model_plain: GraphGPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.598
    metric_stds:
    - 0.005
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
    - 0.595
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
    - 0.583
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
    - 0.56
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
    - 0.555
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
    - 0.241
    metric_stds:
    - 0.005
  row_count: 10
  rows_json: ''
  chart_json: /data/datasets/los-angeles/standard-split-chart.json
  arch_counts:
    gnn: 5
    hybrid: 1
    graph_transformer: 2
    llm: 0
    walk: 0
    traditional: 2
  metric_counts:
  - 10
  milestones: &id001
  - value: 0.638
    std: 0.006
    model: Exphormer
    arxiv_id: '2503.09008'
    title: City-Networks
    date: '2025-03-12'
  milestones_by_metric:
    Accuracy: *id001
---

