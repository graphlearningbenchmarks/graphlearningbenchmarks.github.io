---
title: FB15k-237
slug: fb15k-237
benchmark: Knowledge Graphs
task_type: link_prediction
description: Knowledge graph link prediction on Freebase (14,541 entities, 237 relations).
primary_metric: MRR
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.FB15k_237.html
stats:
  num_graphs: 1
  avg_nodes: 14541.0
  avg_edges: 272115.0
  num_classes: 237
result_count: 164
best_model:
  model: sum, Msg_r^3, f(t)=0
  value: 0.85
  metric: MRR
  arxiv_id: '2302.02209'
  paper_title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
    Graphs
papers:
- arxiv_id: '2605.09099'
  title: 'GraphNetz: Statistical Benchmarking of Graph Neural Networks with Paired
    Tests and Rank Aggregation'
  date_iso: '2026-05-09'
  venue: ''
- arxiv_id: '2603.00618'
  title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
  date_iso: '2026-02-28'
  venue: ICLR 2026
- arxiv_id: '2410.12288'
  title: A Prompt-Based Knowledge Graph Foundation Model for Universal In-Context
    Reasoning
  date_iso: '2024-10-16'
  venue: NeurIPS 2024
- arxiv_id: '2409.12865'
  title: 'KnowFormer: Revisiting Transformers for Knowledge Graph Reasoning'
  date_iso: '2024-09-19'
  venue: ICML 2024
- arxiv_id: '2302.13083'
  title: Knowledge Graph Completion with Counterfactual Augmentation
  date_iso: '2023-02-25'
  venue: WWW 2023
- arxiv_id: '2302.02209'
  title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
    Graphs
  date_iso: '2023-02-04'
  venue: NeurIPS 2023
- arxiv_id: '2212.05767'
  title: 'A Survey of Knowledge Graph Reasoning on Graph Types: Static, Dynamic, and
    Multi-Modal'
  date_iso: '2022-12-12'
  venue: ''
- arxiv_id: '2211.10738'
  title: Knowledge Graph Contrastive Learning based on Relation-Symmetrical Structure
  date_iso: '2022-11-19'
  venue: ''
- arxiv_id: '2209.08271'
  title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
  date_iso: '2022-09-17'
  venue: ''
- arxiv_id: '2206.04798'
  title: 'A*Net: A Scalable Path-based Reasoning Approach for Knowledge Graphs'
  date_iso: '2022-06-07'
  venue: NeurIPS 2022
- arxiv_id: '2205.14209'
  title: 'StarGraph: Knowledge Representation Learning based on Incomplete Two-hop
    Subgraph'
  date_iso: '2022-05-27'
  venue: ICLR 2022
- arxiv_id: '2112.01064'
  title: 'AutoGEL: An Automated Graph Neural Network with Explicit Link Information'
  date_iso: '2021-12-02'
  venue: NeurIPS 2021
- arxiv_id: '2108.06040'
  title: Knowledge Graph Reasoning with Relational Digraph
  date_iso: '2021-08-13'
  venue: WWW 2021
- arxiv_id: '2106.06935'
  title: 'Neural Bellman-Ford Networks: A General Graph Neural Network Framework for
    Link Prediction'
  date_iso: '2021-06-13'
  venue: NeurIPS 2021
- arxiv_id: '2011.03798'
  title: 'PairRE: Knowledge Graph Embeddings via Paired Relation Vectors'
  date_iso: '2020-11-07'
  venue: ''
- arxiv_id: '2009.14332'
  title: Multi-hop Attention Graph Neural Networks
  date_iso: '2020-09-29'
  venue: IJCAI 2020
- arxiv_id: '1911.06962'
  title: Inductive Relation Prediction by Subgraph Reasoning
  date_iso: '2019-11-16'
  venue: ICML 2019
- arxiv_id: '1911.03082'
  title: Composition-based Multi-Relational Graph Convolutional Networks
  date_iso: '2019-11-08'
  venue: ICLR 2019
- arxiv_id: '1902.10197'
  title: 'RotatE: Knowledge Graph Embedding by Relational Rotation in Complex Space'
  date_iso: '2018-09-27'
  venue: ICLR 2018
- arxiv_id: '1707.01476'
  title: Knowledge Graphs
  date_iso: '2017-07-05'
  venue: AAAI 2017
variants:
- slug: standard-split
  name: Standard split
  notes: Toutanova & Chen 2015 split. Also reports Hits@1, Hits@3, Hits@10.
  is_standard: true
  primary_metric: MRR
  default_metric: MRR
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 14541.0
    avg_edges: 272115.0
    num_classes: 237
  metrics:
  - MRR
  - AUC
  - AUC-PR
  - H@10
  - Hit@1
  - Hit@10
  - Hit@3
  - Hits@10
  - MR
  metric_display_names:
  - MRR
  - AUC
  - AUC-PR
  - H@10
  - Hit@1
  - Hit@10
  - Hit@3
  - Hits@10
  - MR
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: sum, Msg_r^3, f(t)=0
    model_plain: sum, Msg_r^3, f(t)=0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.85
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: sum, Msg_r^3, f(t)=t
    model_plain: sum, Msg_r^3, f(t)=t
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.844
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: relation-specific
    model_plain: relation-specific
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.835
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: LLMs
    model_plain: LLMs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.815
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.023
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PNA, Msg_r^1, f(t)=t
    model_plain: PNA, Msg_r^1, f(t)=t
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.804
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: no readout
    model_plain: no readout
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.804
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PNA, Msg_r^1, f(t)=0
    model_plain: PNA, Msg_r^1, f(t)=0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.801
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: global readout
    model_plain: global readout
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.799
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PNA, Msg_r^3, f(t)=t
    model_plain: PNA, Msg_r^3, f(t)=t
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.795
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: sum, Msg_r^1, f(t)=t
    model_plain: sum, Msg_r^1, f(t)=t
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.794
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
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
    - 0.794
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GCOPE
    model_plain: GCOPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.793
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.022
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GFT
    model_plain: GFT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.791
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.016
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PNA, Msg_r^3, f(t)=0
    model_plain: PNA, Msg_r^3, f(t)=0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.788
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: sum, Msg_r^1, f(t)=0
    model_plain: sum, Msg_r^1, f(t)=0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.784
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SAMGPT
    model_plain: SAMGPT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.776
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.027
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: MDGFM
    model_plain: MDGFM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.776
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.02
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GraphMAE
    model_plain: GraphMAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.772
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.01
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GCC
    model_plain: GCC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.736
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.012
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: sum, Msg_r^2, f(t)=0
    model_plain: sum, Msg_r^2, f(t)=0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.734
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: sum, Msg_r^2, f(t)=t
    model_plain: sum, Msg_r^2, f(t)=t
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.728
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PRODIGY
    model_plain: PRODIGY
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.721
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.069
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PNA, Msg_r^2, f(t)=0
    model_plain: PNA, Msg_r^2, f(t)=0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.715
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PNA, Msg_r^2, f(t)=t
    model_plain: PNA, Msg_r^2, f(t)=t
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.709
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.683
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.014
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: RAGraph
    model_plain: RAGraph
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.645
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.025
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GraIL
    model_plain: GraIL
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
    - 0.642
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.637
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.017
    - null
    - null
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.589
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.015
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: NeuralLP
    model_plain: NeuralLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    - 0.529
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DRUM
    model_plain: DRUM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    - 0.529
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: Feb 28, 2026
    date_iso: '2026-02-28'
    date_display: Feb 2026
    codebase_url: https://github.com/RiemannGraph/GraphGlue
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5243
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.018
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: RGHAT
    model_plain: RGHAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.05767'
    title: 'A Survey of Knowledge Graph Reasoning on Graph Types: Static, Dynamic,
      and Multi-Modal'
    date: Dec 12, 2022
    date_iso: '2022-12-12'
    date_display: Dec 2022
    codebase_url: https://github.com/LIANGKE23/Awesome-Knowledge-Graph-Reasoning
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.522
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: RuleN
    model_plain: RuleN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    - 0.498
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: KnowFormer
    model_plain: KnowFormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2409.12865'
    title: 'KnowFormer: Revisiting Transformers for Knowledge Graph Reasoning'
    date: Sep 19, 2024
    date_iso: '2024-09-19'
    date_display: Sep 2024
    codebase_url: https://github.com/jnanliu/KnowFormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.43
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: KGCF
    model_plain: KGCF
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2302.13083'
    title: Knowledge Graph Completion with Counterfactual Augmentation
    date: Feb 25, 2023
    date_iso: '2023-02-25'
    date_display: Feb 2023
    codebase_url: ''
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.421
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: AdaProp
    model_plain: AdaProp
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2409.12865'
    title: 'KnowFormer: Revisiting Transformers for Knowledge Graph Reasoning'
    date: Sep 19, 2024
    date_iso: '2024-09-19'
    date_display: Sep 2024
    codebase_url: https://github.com/jnanliu/KnowFormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.417
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
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
    - 0.415
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: A*Net
    model_plain: A*Net
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2409.12865'
    title: 'KnowFormer: Revisiting Transformers for Knowledge Graph Reasoning'
    date: Sep 19, 2024
    date_iso: '2024-09-19'
    date_display: Sep 2024
    codebase_url: https://github.com/jnanliu/KnowFormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.411
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Multi-Hop
    model_plain: Multi-Hop
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2206.04798'
    title: 'A*Net: A Scalable Path-based Reasoning Approach for Knowledge Graphs'
    date: Jun 7, 2022
    date_iso: '2022-06-07'
    date_display: Jun 2022
    codebase_url: https://github.com/DeepGraphLearning/AStarNet
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.393
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ComplEx+RP
    model_plain: ComplEx+RP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.04798'
    title: 'A*Net: A Scalable Path-based Reasoning Approach for Knowledge Graphs'
    date: Jun 7, 2022
    date_iso: '2022-06-07'
    date_display: Jun 2022
    codebase_url: https://github.com/DeepGraphLearning/AStarNet
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.388
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: RED-GNN
    model_plain: RED-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2108.06040'
    title: Knowledge Graph Reasoning with Relational Digraph
    date: Aug 13, 2021
    date_iso: '2021-08-13'
    date_display: Aug 2021
    codebase_url: https://github.com/LARS-research/RED-GNN
    published_conference: WWW 2021
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.374
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: HittER
    model_plain: HittER
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2409.12865'
    title: 'KnowFormer: Revisiting Transformers for Knowledge Graph Reasoning'
    date: Sep 19, 2024
    date_iso: '2024-09-19'
    date_display: Sep 2024
    codebase_url: https://github.com/jnanliu/KnowFormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.373
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ComplEX-DURA-SymCL
    model_plain: ComplEX-DURA-SymCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.10738'
    title: Knowledge Graph Contrastive Learning based on Relation-Symmetrical Structure
    date: Nov 19, 2022
    date_iso: '2022-11-19'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.371
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ComplEX-DURA
    model_plain: ComplEX-DURA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2211.10738'
    title: Knowledge Graph Contrastive Learning based on Relation-Symmetrical Structure
    date: Nov 19, 2022
    date_iso: '2022-11-19'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.37
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: MAGNA + DistMult
    model_plain: MAGNA + DistMult
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2009.14332'
    title: Multi-hop Attention Graph Neural Networks
    date: Sep 29, 2020
    date_iso: '2020-09-29'
    date_display: Sep 2020
    codebase_url: https://github.com/xjtuwgt/GNN-MAGNA
    published_conference: IJCAI 2020
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.369
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DPMPN
    model_plain: DPMPN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2108.06040'
    title: Knowledge Graph Reasoning with Relational Digraph
    date: Aug 13, 2021
    date_iso: '2021-08-13'
    date_display: Aug 2021
    codebase_url: https://github.com/LARS-research/RED-GNN
    published_conference: WWW 2021
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.369
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ULTRA
    model_plain: ULTRA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2409.12865'
    title: 'KnowFormer: Revisiting Transformers for Knowledge Graph Reasoning'
    date: Sep 19, 2024
    date_iso: '2024-09-19'
    date_display: Sep 2024
    codebase_url: https://github.com/jnanliu/KnowFormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.368
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ConEx
    model_plain: ConEx
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2212.05767'
    title: 'A Survey of Knowledge Graph Reasoning on Graph Types: Static, Dynamic,
      and Multi-Modal'
    date: Dec 12, 2022
    date_iso: '2022-12-12'
    date_display: Dec 2022
    codebase_url: https://github.com/LIANGKE23/Awesome-Knowledge-Graph-Reasoning
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.366
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: QuatE
    model_plain: QuatE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.14332'
    title: Multi-hop Attention Graph Neural Networks
    date: Sep 29, 2020
    date_iso: '2020-09-29'
    date_display: Sep 2020
    codebase_url: https://github.com/xjtuwgt/GNN-MAGNA
    published_conference: IJCAI 2020
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.366
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  row_count: 164
  rows_json: /data/datasets/fb15k-237/standard-split-rows.json
  chart_json: /data/datasets/fb15k-237/standard-split-chart.json
  arch_counts:
    gnn: 57
    hybrid: 22
    graph_transformer: 2
    llm: 8
    walk: 4
    traditional: 44
  metric_counts:
  - 143
  - 4
  - 4
  - 5
  - 1
  - 1
  - 1
  - 13
  - 1
  milestones: &id001
  - value: 0.338
    std: null
    model: RotatE
    arxiv_id: '1902.10197'
    title: 'RotatE: Knowledge Graph Embedding by Relational Rotation in Complex Space'
    date: '2018-09-27'
  - value: 0.355
    std: null
    model: CompGCN
    arxiv_id: '1911.03082'
    title: Composition-based Multi-Relational Graph Convolutional Networks
    date: '2019-11-08'
  - value: 0.369
    std: null
    model: MAGNA + DistMult
    arxiv_id: '2009.14332'
    title: Multi-hop Attention Graph Neural Networks
    date: '2020-09-29'
  - value: 0.522
    std: null
    model: RGHAT
    arxiv_id: '2212.05767'
    title: 'A Survey of Knowledge Graph Reasoning on Graph Types: Static, Dynamic,
      and Multi-Modal'
    date: '2022-12-12'
  - value: 0.815
    std: 0.023
    model: LLMs
    arxiv_id: '2603.00618'
    title: Multi-domain Riemannian Graph Gluing for Building Graph Foundation Models
    date: '2026-02-28'
  milestones_by_metric:
    MRR: *id001
    AUC: []
    AUC-PR: []
    H@10:
    - value: 0.433
      std: null
      model: KG-ICL pre-train
      arxiv_id: '2410.12288'
      title: A Prompt-Based Knowledge Graph Foundation Model for Universal In-Context
        Reasoning
      date: '2024-10-16'
    Hit@1:
    - value: 0.267
      std: null
      model: GC-OTE
      arxiv_id: '2209.08271'
      title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
      date: '2022-09-17'
    Hit@10:
    - value: 0.552
      std: null
      model: TripleRE
      arxiv_id: '2209.08271'
      title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
      date: '2022-09-17'
    Hit@3:
    - value: 0.396
      std: null
      model: GC-OTE
      arxiv_id: '2209.08271'
      title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
      date: '2022-09-17'
    Hits@10:
    - value: 0.593
      std: null
      model: IMF
      arxiv_id: '2212.05767'
      title: 'A Survey of Knowledge Graph Reasoning on Graph Types: Static, Dynamic,
        and Multi-Modal'
      date: '2022-12-12'
    MR:
    - value: 142.0
      std: null
      model: TripleRE
      arxiv_id: '2209.08271'
      title: 'TripleRE: Knowledge Graph Embeddings via Tripled Relation Vectors'
      date: '2022-09-17'
---

