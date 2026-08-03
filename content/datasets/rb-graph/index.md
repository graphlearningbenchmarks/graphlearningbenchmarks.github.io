---
title: RB graph
slug: rb-graph
benchmark: GraphBench
task_type: graph_classification
description: Node classification on Random Bipartite graphs (GraphBench algorithmic
  reasoning).
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://graphbench.github.io/website/datasets.html
stats:
  num_graphs: 21000000
  avg_nodes: 264.0
  avg_edges: 3667.0
  num_classes: null
result_count: 19
best_model:
  model: F_4-MPNN
  value: 0.9793
  metric: Accuracy
  arxiv_id: '2505.11298'
  paper_title: 'Graph Representational Learning: When Does More Expressivity Hurt
    Generalization?'
papers:
- arxiv_id: '2505.11298'
  title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
  date_iso: '2025-05-16'
  venue: ''
- arxiv_id: '2502.02415'
  title: Fast Graph Generation via Autoregressive Noisy Filtration Modeling
  date_iso: '2025-02-04'
  venue: TMLR 2025
- arxiv_id: '1710.10321'
  title: Learning Structural Node Embeddings via Diffusion Wavelets
  date_iso: '2017-10-27'
  venue: KDD 2017
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 21000000
    avg_nodes: 264.0
    avg_edges: 3667.0
    num_classes: null
  metrics:
  - Accuracy
  - VUN
  metric_display_names:
  - Accuracy
  - VUN
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: F_4-MPNN
    model_plain: F_4-MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_iso: '2025-05-16'
    date_display: May 2025
    codebase_url: https://github.com/RPaolino/GenVsExp
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9793
    - null
    metric_stds:
    - 0.0068
    - null
  - model: F_7-MPNN
    model_plain: F_7-MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_iso: '2025-05-16'
    date_display: May 2025
    codebase_url: https://github.com/RPaolino/GenVsExp
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.966
    - null
    metric_stds:
    - 0.0065
    - null
  - model: F_3-MPNN
    model_plain: F_3-MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_iso: '2025-05-16'
    date_display: May 2025
    codebase_url: https://github.com/RPaolino/GenVsExp
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8657
    - null
    metric_stds:
    - 0.0085
    - null
  - model: Sub-G
    model_plain: Sub-G
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_iso: '2025-05-16'
    date_display: May 2025
    codebase_url: https://github.com/RPaolino/GenVsExp
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8623
    - null
    metric_stds:
    - 0.0058
    - null
  - model: L-G
    model_plain: L-G
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_iso: '2025-05-16'
    date_display: May 2025
    codebase_url: https://github.com/RPaolino/GenVsExp
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8543
    - null
    metric_stds:
    - 0.0063
    - null
  - model: Diffusion Wavelets
    model_plain: Diffusion Wavelets
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_iso: '2017-10-27'
    date_display: Oct 2017
    codebase_url: ''
    published_conference: KDD 2017
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.85
    - null
    metric_stds:
    - null
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
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_iso: '2025-05-16'
    date_display: May 2025
    codebase_url: https://github.com/RPaolino/GenVsExp
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.849
    - null
    metric_stds:
    - 0.0045
    - null
  - model: LF-G
    model_plain: LF-G
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: May 16, 2025
    date_iso: '2025-05-16'
    date_display: May 2025
    codebase_url: https://github.com/RPaolino/GenVsExp
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.845
    - null
    metric_stds:
    - 0.0135
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
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_iso: '2017-10-27'
    date_display: Oct 2017
    codebase_url: ''
    published_conference: KDD 2017
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.81
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
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_iso: '2017-10-27'
    date_display: Oct 2017
    codebase_url: ''
    published_conference: KDD 2017
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.78
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
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_iso: '2017-10-27'
    date_display: Oct 2017
    codebase_url: ''
    published_conference: KDD 2017
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.62
    - null
    metric_stds:
    - null
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
    arxiv_id: '1710.10321'
    title: Learning Structural Node Embeddings via Diffusion Wavelets
    date: Oct 27, 2017
    date_iso: '2017-10-27'
    date_display: Oct 2017
    codebase_url: ''
    published_conference: KDD 2017
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2017
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6
    - null
    metric_stds:
    - null
    - null
  - model: GraphRNN
    model_plain: GraphRNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.02415'
    title: Fast Graph Generation via Autoregressive Noisy Filtration Modeling
    date: Feb 4, 2025
    date_iso: '2025-02-04'
    date_display: Feb 2025
    codebase_url: https://github.com/BorgwardtLab/anfm
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 5.0
    metric_stds:
    - null
    - null
  - model: GRAN
    model_plain: GRAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.02415'
    title: Fast Graph Generation via Autoregressive Noisy Filtration Modeling
    date: Feb 4, 2025
    date_iso: '2025-02-04'
    date_display: Feb 2025
    codebase_url: https://github.com/BorgwardtLab/anfm
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 25.0
    metric_stds:
    - null
    - null
  - model: SPECTRE
    model_plain: SPECTRE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.02415'
    title: Fast Graph Generation via Autoregressive Noisy Filtration Modeling
    date: Feb 4, 2025
    date_iso: '2025-02-04'
    date_display: Feb 2025
    codebase_url: https://github.com/BorgwardtLab/anfm
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 52.5
    metric_stds:
    - null
    - null
  - model: DiGress
    model_plain: DiGress
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.02415'
    title: Fast Graph Generation via Autoregressive Noisy Filtration Modeling
    date: Feb 4, 2025
    date_iso: '2025-02-04'
    date_display: Feb 2025
    codebase_url: https://github.com/BorgwardtLab/anfm
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 60.0
    metric_stds:
    - null
    - null
  - model: Edge
    model_plain: Edge
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.02415'
    title: Fast Graph Generation via Autoregressive Noisy Filtration Modeling
    date: Feb 4, 2025
    date_iso: '2025-02-04'
    date_display: Feb 2025
    codebase_url: https://github.com/BorgwardtLab/anfm
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.0
    metric_stds:
    - null
    - null
  - model: ESGG
    model_plain: ESGG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.02415'
    title: Fast Graph Generation via Autoregressive Noisy Filtration Modeling
    date: Feb 4, 2025
    date_iso: '2025-02-04'
    date_display: Feb 2025
    codebase_url: https://github.com/BorgwardtLab/anfm
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 45.0
    metric_stds:
    - null
    - null
  - model: ANFM (DFS)
    model_plain: ANFM (DFS)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2502.02415'
    title: Fast Graph Generation via Autoregressive Noisy Filtration Modeling
    date: Feb 4, 2025
    date_iso: '2025-02-04'
    date_display: Feb 2025
    codebase_url: https://github.com/BorgwardtLab/anfm
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 65.0
    metric_stds:
    - null
    - null
  row_count: 19
  rows_json: ''
  chart_json: /data/datasets/rb-graph/standard-split-chart.json
  arch_counts:
    gnn: 16
    hybrid: 1
    graph_transformer: 0
    llm: 0
    walk: 2
    traditional: 0
  metric_counts:
  - 12
  - 7
  milestones: &id001
  - value: 0.9793
    std: 0.0068
    model: F_4-MPNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: '2025-05-16'
  milestones_by_metric:
    Accuracy: *id001
    VUN:
    - value: 65.0
      std: null
      model: ANFM (DFS)
      arxiv_id: '2502.02415'
      title: Fast Graph Generation via Autoregressive Noisy Filtration Modeling
      date: '2025-02-04'
---

