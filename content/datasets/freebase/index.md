---
title: Freebase
slug: freebase
benchmark: Heterogeneous Graph Benchmarks
task_type: node_classification
short_description: Heterogeneous Freebase knowledge graph node classification (8 entity
  types).
description: '**Node classification** Heterogeneous Freebase knowledge graph node
  classification (8 entity types). Uses typed nodes, typed relations, and available
  type-specific features. Evaluated by Macro-F1.'
detailed_description:
  task: Heterogeneous Freebase knowledge graph node classification (8 entity types).
    The primary catalog metric is Macro-F1.
  data: Heterogeneous Freebase knowledge graph node classification (8 entity types).
  features: Inputs are typed graphs with relation-specific edges and type-specific
    feature matrices where available. Some node types lack native features, so learned
    embeddings or propagated features are modeling choices rather than measured attributes.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses Macro-F1 (higher is better). Exact masks or folds must
    come from the cited release.'
  quirks_and_pitfalls: Schema, reverse-edge creation, feature propagation, and negative
    sampling materially affect results. Report the exact release and target type;
    random edge splits may leak future or reciprocal information.
sources:
- title: Heterogeneous Graph Benchmarks benchmark
  arxiv_id: '2112.14936'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric Freebase loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.HGBDataset.html
  kind: implementation_documentation
primary_metric: Macro-F1
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.HGBDataset.html
stats:
  num_graphs: 1
  avg_nodes: 180098.0
  avg_edges: 1057688.0
  num_classes: 7
  extra_stats:
    edge_feature_dim: 0
    feature_type: no native features retained for the target task; one-hot/learned
      type embeddings are preprocessing choices
    node_feature_dim: 0
    num_edge_types: 36
    num_node_types: 8
    statistic_notes: HGB release samples eight Freebase entity genres; Table 1 of
      Lv et al. (2021).
    target_node_type: book
result_count: 83
best_model:
  model: ConCH
  value: 0.6475
  metric: Macro-F1
  arxiv_id: '2012.10024'
  paper_title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
    Networks
papers:
- arxiv_id: '2602.13075'
  title: Unified Multi-Domain Graph Pre-training for Homogeneous and Heterogeneous
    Graphs via Domain-Specific Expert Encoding
  date_iso: '2026-02-13'
  venue: ''
- arxiv_id: '2405.01927'
  title: 'SlotGAT: Slot-based Message Passing for Heterogeneous Graphs'
  date_iso: '2024-05-03'
  venue: ICML 2024
- arxiv_id: '2404.02810'
  title: Generative-Contrastive Heterogeneous Graph Neural Network
  date_iso: '2024-04-03'
  venue: ''
- arxiv_id: '2403.04780'
  title: Graph-oriented Instruction Tuning of Large Language Models for Generic Graph
    Mining
  date_iso: '2024-03-02'
  venue: ''
- arxiv_id: '2310.14481'
  title: Efficient Heterogeneous Graph Learning via Random Projection
  date_iso: '2023-10-23'
  venue: ''
- arxiv_id: '2307.08430'
  title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
  date_iso: '2023-07-17'
  venue: NeurIPS 2023
- arxiv_id: '2210.00248'
  title: Heterogeneous Graph Contrastive Multi-view Learning
  date_iso: '2022-10-01'
  venue: ''
- arxiv_id: '2207.02547'
  title: Simple and Efficient Heterogeneous Graph Neural Network
  date_iso: '2022-07-06'
  venue: AAAI 2022
- arxiv_id: '2112.14936'
  title: Heterogeneous Graph Benchmarks
  date_iso: '2021-08-14'
  venue: KDD 2021
- arxiv_id: '2012.10024'
  title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
    Networks
  date_iso: '2020-12-18'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Macro-F1
  default_metric: Macro-F1
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 180098.0
    avg_edges: 1057688.0
    num_classes: 7
    extra_stats:
      edge_feature_dim: 0
      feature_type: no native features retained for the target task; one-hot/learned
        type embeddings are preprocessing choices
      node_feature_dim: 0
      num_edge_types: 36
      num_node_types: 8
      statistic_notes: HGB release samples eight Freebase entity genres; Table 1 of
        Lv et al. (2021).
      target_node_type: book
  metrics:
  - Macro-F1
  - Micro-F1
  metric_display_names:
  - Macro-F1
  - Micro-F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: ConCH
    model_plain: ConCH
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.6475
    - null
    metric_stds:
    - null
    - null
  - model: HetGNN
    model_plain: HetGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6292
    - null
    metric_stds:
    - null
    - null
  - model: GC-HGNN
    model_plain: GC-HGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_iso: '2024-04-03'
    date_display: Apr 2024
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6247
    - null
    metric_stds:
    - 0.0042
    - null
  - model: MAGNN
    model_plain: MAGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6223
    - null
    metric_stds:
    - null
    - null
  - model: HGT
    model_plain: HGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6176
    - null
    metric_stds:
    - null
    - null
  - model: HDGI
    model_plain: HDGI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6139
    - null
    metric_stds:
    - null
    - null
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.609
    - null
    metric_stds:
    - null
    - null
  - model: HGMAE
    model_plain: HGMAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_iso: '2024-04-03'
    date_display: Apr 2024
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6082
    - null
    metric_stds:
    - 0.0051
    - null
  - model: HGCN
    model_plain: HGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6035
    - null
    metric_stds:
    - null
    - null
  - model: HAN
    model_plain: HAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6011
    - null
    metric_stds:
    - null
    - null
  - model: HeCo
    model_plain: HeCo
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_iso: '2024-04-03'
    date_display: Apr 2024
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5987
    - null
    metric_stds:
    - 0.0033
    - null
  - model: MuseGraph (LLaMA3-8B)
    model_plain: MuseGraph (LLaMA3-8B)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 13.631488
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2403.04780'
    title: Graph-oriented Instruction Tuning of Large Language Models for Generic
      Graph Mining
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/Melinda315/MuseGraph
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5962
    - null
    metric_stds:
    - null
    - null
  - model: HERec
    model_plain: HERec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_iso: '2024-04-03'
    date_display: Apr 2024
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5946
    - null
    metric_stds:
    - 0.0116
    - null
  - model: DeepWalk
    model_plain: DeepWalk
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_iso: '2024-04-03'
    date_display: Apr 2024
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.592
    - null
    metric_stds:
    - 0.005
    - null
  - model: HGCML
    model_plain: HGCML
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_iso: '2024-04-03'
    date_display: Apr 2024
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5892
    - null
    metric_stds:
    - 0.0257
    - null
  - model: HAN
    model_plain: HAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_iso: '2024-04-03'
    date_display: Apr 2024
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.585
    - null
    metric_stds:
    - 0.0093
    - null
  - model: HGT
    model_plain: HGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_iso: '2024-04-03'
    date_display: Apr 2024
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.583
    - null
    metric_stds:
    - 0.0072
    - null
  - model: Mp2vec
    model_plain: Mp2vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.575
    - null
    metric_stds:
    - null
    - null
  - model: Node2Vec
    model_plain: Node2Vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5735
    - null
    metric_stds:
    - null
    - null
  - model: MHGCN
    model_plain: MHGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_iso: '2024-04-03'
    date_display: Apr 2024
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5712
    - null
    metric_stds:
    - 0.0032
    - null
  - model: DMGI
    model_plain: DMGI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_iso: '2024-04-03'
    date_display: Apr 2024
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5599
    - null
    metric_stds:
    - 0.0059
    - null
  - model: Mp2vec
    model_plain: Mp2vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_iso: '2024-04-03'
    date_display: Apr 2024
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.555
    - null
    metric_stds:
    - 0.0049
    - null
  - model: RpHGNN
    model_plain: RpHGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.14481'
    title: Efficient Heterogeneous Graph Learning via Random Projection
    date: Oct 23, 2023
    date_iso: '2023-10-23'
    date_display: Oct 2023
    codebase_url: https://github.com/CrawlScript/RpHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5402
    - null
    metric_stds:
    - 0.0088
    - null
  - model: LMSPS
    model_plain: LMSPS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5326
    - null
    metric_stds:
    - 0.0047
    - null
  - model: HINormer
    model_plain: HINormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5218
    - null
    metric_stds:
    - 0.0039
    - null
  - model: SeHGNN
    model_plain: SeHGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5187
    - null
    metric_stds:
    - 0.0086
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
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5115
    - null
    metric_stds:
    - null
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
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: Dec 18, 2020
    date_iso: '2020-12-18'
    date_display: Dec 2020
    codebase_url: https://github.com/dingdanhao110/Conch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5109
    - null
    metric_stds:
    - null
    - null
  - model: Variant#3
    model_plain: Variant#3
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5071
    - null
    metric_stds:
    - 0.0044
    - null
  - model: Variant#4
    model_plain: Variant#4
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.503
    - null
    metric_stds:
    - 0.0023
    - null
  - model: NARS
    model_plain: NARS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4998
    - null
    metric_stds:
    - 0.0177
    - null
  - model: SlotGAT
    model_plain: SlotGAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4968
    - null
    metric_stds:
    - 0.0197
    - null
  - model: HINormer
    model_plain: HINormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2403.04780'
    title: Graph-oriented Instruction Tuning of Large Language Models for Generic
      Graph Mining
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/Melinda315/MuseGraph
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4887
    - null
    metric_stds:
    - null
    - null
  - model: HGB
    model_plain: HGB
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4772
    - null
    metric_stds:
    - 0.0148
    - null
  - model: Simple-HGN
    model_plain: Simple-HGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2112.14936'
    title: Heterogeneous Graph Benchmarks
    date: Aug 14, 2021
    date_iso: '2021-08-14'
    date_display: Aug 2021
    codebase_url: https://github.com/THUDM/HGB
    published_conference: KDD 2021
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4772
    - null
    metric_stds:
    - 0.0148
    - null
  - model: simpleHGN
    model_plain: simpleHGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.01927'
    title: 'SlotGAT: Slot-based Message Passing for Heterogeneous Graphs'
    date: May 3, 2024
    date_iso: '2024-05-03'
    date_display: May 2024
    codebase_url: https://github.com/scottjiao/SlotGAT_ICML23
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4772
    - null
    metric_stds:
    - 0.0148
    - null
  - model: R-GCN
    model_plain: R-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.04780'
    title: Graph-oriented Instruction Tuning of Large Language Models for Generic
      Graph Mining
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/Melinda315/MuseGraph
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4703
    - null
    metric_stds:
    - null
    - null
  - model: Variant#2
    model_plain: Variant#2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4682
    - null
    metric_stds:
    - 0.0112
    - null
  - model: RGCN
    model_plain: RGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.14936'
    title: Heterogeneous Graph Benchmarks
    date: Aug 14, 2021
    date_iso: '2021-08-14'
    date_display: Aug 2021
    codebase_url: https://github.com/THUDM/HGB
    published_conference: KDD 2021
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4678
    - null
    metric_stds:
    - 0.0077
    - null
  - model: GPH^2
    model_plain: GPH^2
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.13075'
    title: Unified Multi-Domain Graph Pre-training for Homogeneous and Heterogeneous
      Graphs via Domain-Specific Expert Encoding
    date: Feb 13, 2026
    date_iso: '2026-02-13'
    date_display: Feb 2026
    codebase_url: https://github.com/hedongxiao-tju/GPH-2
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4478
    - null
    metric_stds:
    - 0.0547
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
    arxiv_id: '2310.14481'
    title: Efficient Heterogeneous Graph Learning via Random Projection
    date: Oct 23, 2023
    date_iso: '2023-10-23'
    date_display: Oct 2023
    codebase_url: https://github.com/CrawlScript/RpHGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4417
    - null
    metric_stds:
    - 0.0114
    - null
  - model: space4HGNN
    model_plain: space4HGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_iso: '2023-07-17'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4137
    - null
    metric_stds:
    - 0.0449
    - null
  - model: HGPrompt
    model_plain: HGPrompt
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.13075'
    title: Unified Multi-Domain Graph Pre-training for Homogeneous and Heterogeneous
      Graphs via Domain-Specific Expert Encoding
    date: Feb 13, 2026
    date_iso: '2026-02-13'
    date_display: Feb 2026
    codebase_url: https://github.com/hedongxiao-tju/GPH-2
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4078
    - null
    metric_stds:
    - 0.0323
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
    arxiv_id: '2112.14936'
    title: Heterogeneous Graph Benchmarks
    date: Aug 14, 2021
    date_iso: '2021-08-14'
    date_display: Aug 2021
    codebase_url: https://github.com/THUDM/HGB
    published_conference: KDD 2021
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4074
    - null
    metric_stds:
    - 0.0258
    - null
  - model: HeCo
    model_plain: HeCo
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.13075'
    title: Unified Multi-Domain Graph Pre-training for Homogeneous and Heterogeneous
      Graphs via Domain-Specific Expert Encoding
    date: Feb 13, 2026
    date_iso: '2026-02-13'
    date_display: Feb 2026
    codebase_url: https://github.com/hedongxiao-tju/GPH-2
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3799
    - null
    metric_stds:
    - 0.0312
    - null
  - model: HGMAE
    model_plain: HGMAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.13075'
    title: Unified Multi-Domain Graph Pre-training for Homogeneous and Heterogeneous
      Graphs via Domain-Specific Expert Encoding
    date: Feb 13, 2026
    date_iso: '2026-02-13'
    date_display: Feb 2026
    codebase_url: https://github.com/hedongxiao-tju/GPH-2
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3515
    - null
    metric_stds:
    - 0.0362
    - null
  - model: OFA
    model_plain: OFA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2403.04780'
    title: Graph-oriented Instruction Tuning of Large Language Models for Generic
      Graph Mining
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/Melinda315/MuseGraph
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3475
    - null
    metric_stds:
    - null
    - null
  - model: DMGI
    model_plain: DMGI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.13075'
    title: Unified Multi-Domain Graph Pre-training for Homogeneous and Heterogeneous
      Graphs via Domain-Specific Expert Encoding
    date: Feb 13, 2026
    date_iso: '2026-02-13'
    date_display: Feb 2026
    codebase_url: https://github.com/hedongxiao-tju/GPH-2
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3337
    - null
    metric_stds:
    - 0.0232
    - null
  - model: Variant#1
    model_plain: Variant#1
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_iso: '2022-07-06'
    date_display: Jul 2022
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3323
    - null
    metric_stds:
    - 0.0139
    - null
  - model: HERO
    model_plain: HERO
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.13075'
    title: Unified Multi-Domain Graph Pre-training for Homogeneous and Heterogeneous
      Graphs via Domain-Specific Expert Encoding
    date: Feb 13, 2026
    date_iso: '2026-02-13'
    date_display: Feb 2026
    codebase_url: https://github.com/hedongxiao-tju/GPH-2
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3139
    - null
    metric_stds:
    - 0.078
    - null
  row_count: 83
  rows_json: /data/datasets/freebase/standard-split-rows.json
  chart_json: /data/datasets/freebase/standard-split-chart.json
  arch_counts:
    gnn: 38
    hybrid: 22
    graph_transformer: 3
    llm: 10
    walk: 9
    traditional: 1
  metric_counts:
  - 69
  - 14
  milestones: &id001
  - value: 0.6475
    std: null
    model: ConCH
    arxiv_id: '2012.10024'
    title: Leveraging Meta-path Contexts for Classification in Heterogeneous Information
      Networks
    date: '2020-12-18'
  milestones_by_metric:
    Macro-F1: *id001
    Micro-F1:
    - value: 0.7153
      std: 0.0014
      model: HGCML-P
      arxiv_id: '2210.00248'
      title: Heterogeneous Graph Contrastive Multi-view Learning
      date: '2022-10-01'
---

