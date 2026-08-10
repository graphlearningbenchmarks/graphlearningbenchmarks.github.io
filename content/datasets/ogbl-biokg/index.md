---
title: ogbl-biokg
slug: ogbl-biokg
benchmark: OGB
task_type: link_prediction
description: Biological knowledge graph link prediction (5 entity types, 51 relations).
primary_metric: MRR
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.OGBLinkPropPredDataset.html
stats:
  num_graphs: 93773
  avg_nodes: 5088434.0
  avg_edges: null
  num_classes: null
result_count: 12
best_model:
  model: PairRE+LRE
  value: 0.836
  metric: MRR
  arxiv_id: '2204.13957'
  paper_title: 'PIE: a Parameter and Inference Efficient Solution for Large Scale
    Knowledge Graph Embedding Reasoning'
papers:
- arxiv_id: '2302.02209'
  title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
    Graphs
  date_iso: '2023-02-04'
  venue: NeurIPS 2023
- arxiv_id: '2209.08271'
  title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
  date_iso: '2022-09-17'
  venue: ''
- arxiv_id: '2204.13957'
  title: 'PIE: a Parameter and Inference Efficient Solution for Large Scale Knowledge
    Graph Embedding Reasoning'
  date_iso: '2022-04-29'
  venue: ''
- arxiv_id: '2106.06935'
  title: 'Neural Bellman-Ford Networks: A General Graph Neural Network Framework for
    Link Prediction'
  date_iso: '2021-06-13'
  venue: NeurIPS 2021
- arxiv_id: '2011.03798'
  title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
  date_iso: '2020-11-07'
  venue: ''
- arxiv_id: '2005.00687'
  title: OGB
  date_iso: '2020-05-02'
  venue: NeurIPS 2020
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: MRR
  default_metric: MRR
  higher_is_better: true
  stats:
    num_graphs: 93773
    avg_nodes: 5088434.0
    avg_edges: null
    num_classes: null
  metrics:
  - MRR
  metric_display_names:
  - MRR
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: PairRE+LRE
    model_plain: PairRE+LRE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 501.0
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2204.13957'
    title: 'PIE: a Parameter and Inference Efficient Solution for Large Scale Knowledge
      Graph Embedding Reasoning'
    date: Apr 29, 2022
    date_iso: '2022-04-29'
    date_display: Apr 2022
    codebase_url: https://github.com/migalkin/NodePiece
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.836
    metric_stds:
    - null
  - model: NBFnet
    model_plain: NBFnet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 3.0
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.06935'
    title: 'Neural Bellman-Ford Networks: A General Graph Neural Network Framework
      for Link Prediction'
    date: Jun 13, 2021
    date_iso: '2021-06-13'
    date_display: Jun 2021
    codebase_url: https://github.com/DeepGraphLearning/NBFNet
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8317
    metric_stds:
    - null
  - model: AutoSF
    model_plain: AutoSF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 93.824
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.06935'
    title: 'Neural Bellman-Ford Networks: A General Graph Neural Network Framework
      for Link Prediction'
    date: Jun 13, 2021
    date_iso: '2021-06-13'
    date_display: Jun 2021
    codebase_url: https://github.com/DeepGraphLearning/NBFNet
    published_conference: NeurIPS 2021
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8309
    metric_stds:
    - null
  - model: TripleREv2
    model_plain: TripleREv2
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 500.0
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2209.08271'
    title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
    date: Sep 17, 2022
    date_iso: '2022-09-17'
    date_display: Sep 2022
    codebase_url: https://github.com/DeepGraphLearning/KnowledgeGraph-
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8272
    metric_stds:
    - 0.0007
  - model: TripleRE
    model_plain: TripleRE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2209.08271'
    title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
    date: Sep 17, 2022
    date_iso: '2022-09-17'
    date_display: Sep 2022
    codebase_url: https://github.com/DeepGraphLearning/KnowledgeGraph-
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8191
    metric_stds:
    - 0.0014
  - model: PairRE
    model_plain: PairRE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2011.03798'
    title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    date: Nov 7, 2020
    date_iso: '2020-11-07'
    date_display: Nov 2020
    codebase_url: https://github.com/alipay/KnowledgeGraphEmbeddingsViaPairedRelationVectors
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8164
    metric_stds:
    - 0.0005
  - model: ComplEx
    model_plain: ComplEx
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2005.00687'
    title: OGB
    date: May 2, 2020
    date_iso: '2020-05-02'
    date_display: May 2020
    codebase_url: https://github.com/snap-stanford/ogb
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8095
    metric_stds:
    - 0.0007
  - model: DistMult
    model_plain: DistMult
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2005.00687'
    title: OGB
    date: May 2, 2020
    date_iso: '2020-05-02'
    date_display: May 2020
    codebase_url: https://github.com/snap-stanford/ogb
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8043
    metric_stds:
    - 0.0003
  - model: RotatE
    model_plain: RotatE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2005.00687'
    title: OGB
    date: May 2, 2020
    date_iso: '2020-05-02'
    date_display: May 2020
    codebase_url: https://github.com/snap-stanford/ogb
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7989
    metric_stds:
    - 0.0004
  - model: C-MPNN
    model_plain: C-MPNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.02209'
    title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
      Graphs
    date: Feb 4, 2023
    date_iso: '2023-02-04'
    date_display: Feb 2023
    codebase_url: https://github.com/HxyScotthuang/CMPNN
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.79
    metric_stds:
    - null
  - model: TransE
    model_plain: TransE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2005.00687'
    title: OGB
    date: May 2, 2020
    date_iso: '2020-05-02'
    date_display: May 2020
    codebase_url: https://github.com/snap-stanford/ogb
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7452
    metric_stds:
    - 0.0004
  - model: RGCN
    model_plain: RGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.02209'
    title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
      Graphs
    date: Feb 4, 2023
    date_iso: '2023-02-04'
    date_display: Feb 2023
    codebase_url: https://github.com/HxyScotthuang/CMPNN
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.636
    metric_stds:
    - null
  row_count: 12
  rows_json: ''
  chart_json: /data/datasets/ogbl-biokg/standard-split-chart.json
  arch_counts:
    gnn: 7
    hybrid: 0
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 5
  metric_counts:
  - 12
  milestones: &id001
  - value: 0.8095
    std: 0.0007
    model: ComplEx
    arxiv_id: '2005.00687'
    title: OGB
    date: '2020-05-02'
  - value: 0.8164
    std: 0.0005
    model: PairRE
    arxiv_id: '2011.03798'
    title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
    date: '2020-11-07'
  - value: 0.8317
    std: null
    model: NBFnet
    arxiv_id: '2106.06935'
    title: 'Neural Bellman-Ford Networks: A General Graph Neural Network Framework
      for Link Prediction'
    date: '2021-06-13'
  - value: 0.836
    std: null
    model: PairRE+LRE
    arxiv_id: '2204.13957'
    title: 'PIE: a Parameter and Inference Efficient Solution for Large Scale Knowledge
      Graph Embedding Reasoning'
    date: '2022-04-29'
  milestones_by_metric:
    MRR: *id001
---

