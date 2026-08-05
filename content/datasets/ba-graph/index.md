---
title: BA graph
slug: ba-graph
benchmark: GraphBench
task_type: graph_classification
description: Graph classification on Barabási–Albert random graphs (GraphBench algorithmic
  reasoning).
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://graphbench.github.io/website/datasets.html
stats:
  num_graphs: 21000000
  avg_nodes: 264.0
  avg_edges: 3667.0
  num_classes: null
result_count: 15
best_model:
  model: F4-MPNN
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
- arxiv_id: '2402.16029'
  title: 'GraphWiz: An Instruction-Following Language Model for Graph Computational
    Problems'
  date_iso: '2024-02-25'
  venue: ''
- arxiv_id: '2310.04560'
  title: 'Talk like a Graph: Encoding Graphs for Large Language Models'
  date_iso: '2023-10-06'
  venue: ICLR 2023
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
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: F4-MPNN
    model_plain: F4-MPNN
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
    metric_stds:
    - 0.0068
  - model: F7-MPNN
    model_plain: F7-MPNN
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
    metric_stds:
    - 0.0065
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
    - 0.94
    metric_stds:
    - null
  - model: F3-MPNN
    model_plain: F3-MPNN
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
    metric_stds:
    - 0.0085
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
    metric_stds:
    - 0.0058
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
    metric_stds:
    - 0.0063
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
    - 0.85
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
    metric_stds:
    - 0.0045
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
    metric_stds:
    - 0.0135
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
    - 0.82
    metric_stds:
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
    - 0.78
    metric_stds:
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
    - 0.75
    metric_stds:
    - null
  - model: GraphWiz
    model_plain: GraphWiz
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2402.16029'
    title: 'GraphWiz: An Instruction-Following Language Model for Graph Computational
      Problems'
    date: Feb 25, 2024
    date_iso: '2024-02-25'
    date_display: Feb 2024
    codebase_url: https://github.com/nuochenpku/Graph-Reasoning-LLM
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6812
    metric_stds:
    - null
  - model: Zero-shot
    model_plain: Zero-shot
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2310.04560'
    title: 'Talk like a Graph: Encoding Graphs for Large Language Models'
    date: Oct 6, 2023
    date_iso: '2023-10-06'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.502
    metric_stds:
    - null
  - model: CoT
    model_plain: CoT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2310.04560'
    title: 'Talk like a Graph: Encoding Graphs for Large Language Models'
    date: Oct 6, 2023
    date_iso: '2023-10-06'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4
    metric_stds:
    - null
  row_count: 15
  rows_json: ''
  chart_json: /data/datasets/ba-graph/standard-split-chart.json
  arch_counts:
    gnn: 10
    hybrid: 0
    graph_transformer: 0
    llm: 3
    walk: 2
    traditional: 0
  metric_counts:
  - 15
  milestones: &id001
  - value: 0.502
    std: null
    model: Zero-shot
    arxiv_id: '2310.04560'
    title: 'Talk like a Graph: Encoding Graphs for Large Language Models'
    date: '2023-10-06'
  - value: 0.6812
    std: null
    model: GraphWiz
    arxiv_id: '2402.16029'
    title: 'GraphWiz: An Instruction-Following Language Model for Graph Computational
      Problems'
    date: '2024-02-25'
  - value: 0.9793
    std: 0.0068
    model: F4-MPNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: '2025-05-16'
  milestones_by_metric:
    Accuracy: *id001
---

