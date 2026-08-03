---
title: ER graph
slug: er-graph
benchmark: GraphBench
task_type: graph_classification
description: Graph classification on Erdos-Renyi random graphs (GraphBench algorithmic
  reasoning).
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://graphbench.github.io/website/datasets.html
stats:
  num_graphs: 21000000
  avg_nodes: 264.0
  avg_edges: 3667.0
  num_classes: null
result_count: 25
best_model:
  model: FloydNet
  value: 1.0
  metric: Accuracy
  arxiv_id: '2601.19094'
  paper_title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
papers:
- arxiv_id: '2601.19094'
  title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
  date_iso: '2026-01-27'
  venue: ''
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
  - model: FloydNet
    model_plain: FloydNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_iso: '2026-01-27'
    date_display: Jan 2026
    codebase_url: https://github.com/ocx-lab/FloydNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.0
    metric_stds:
    - null
  - model: PGN
    model_plain: PGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_iso: '2026-01-27'
    date_display: Jan 2026
    codebase_url: https://github.com/ocx-lab/FloydNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.995
    metric_stds:
    - null
  - model: RecGNN
    model_plain: RecGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_iso: '2026-01-27'
    date_display: Jan 2026
    codebase_url: https://github.com/ocx-lab/FloydNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.995
    metric_stds:
    - null
  - model: GIN(E)
    model_plain: GIN(E)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_iso: '2026-01-27'
    date_display: Jan 2026
    codebase_url: https://github.com/ocx-lab/FloydNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.993
    metric_stds:
    - null
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9793
    metric_stds:
    - 0.0068
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.966
    metric_stds:
    - 0.0065
  - model: GraphWiz (LLaMA 2-13B)
    model_plain: GraphWiz (LLaMA 2-13B)
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
    - 0.9475
    metric_stds:
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
    - 0.93
    metric_stds:
    - null
  - model: GraphWiz-DPO (LLaMA 2-7B)
    model_plain: GraphWiz-DPO (LLaMA 2-7B)
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
    - 0.89
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
    - 0.88
    metric_stds:
    - null
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.875
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
    - 0.875
    metric_stds:
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
    - 0.84
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
    - 0.72
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
    - 0.7
    metric_stds:
    - null
  - model: GPT-4 (2-shot)
    model_plain: GPT-4 (2-shot)
    is_baseline: true
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
    - 0.525
    metric_stds:
    - null
  - model: GPT-3.5 (2-shot)
    model_plain: GPT-3.5 (2-shot)
    is_baseline: true
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
    - 0.5125
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
    - 0.451
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
    - 0.412
    metric_stds:
    - null
  row_count: 25
  rows_json: ''
  chart_json: /data/datasets/er-graph/standard-split-chart.json
  arch_counts:
    gnn: 16
    hybrid: 1
    graph_transformer: 0
    llm: 6
    walk: 2
    traditional: 0
  metric_counts:
  - 25
  milestones: &id001
  - value: 0.451
    std: null
    model: Zero-shot
    arxiv_id: '2310.04560'
    title: 'Talk like a Graph: Encoding Graphs for Large Language Models'
    date: '2023-10-06'
  - value: 0.9475
    std: null
    model: GraphWiz (LLaMA 2-13B)
    arxiv_id: '2402.16029'
    title: 'GraphWiz: An Instruction-Following Language Model for Graph Computational
      Problems'
    date: '2024-02-25'
  - value: 0.9793
    std: 0.0068
    model: F_4-MPNN
    arxiv_id: '2505.11298'
    title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
    date: '2025-05-16'
  milestones_by_metric:
    Accuracy: *id001
---

