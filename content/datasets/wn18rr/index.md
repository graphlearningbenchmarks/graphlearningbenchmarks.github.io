---
title: WN18RR
slug: wn18rr
benchmark: Knowledge Graphs
task_type: link_prediction
description: Knowledge graph link prediction on WordNet (40,943 entities, 11 relations).
primary_metric: MRR
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.WordNet18RR.html
stats:
  num_graphs: 1
  avg_nodes: 40943.0
  avg_edges: 93003.0
  num_classes: 11
result_count: 237
best_model:
  model: PNA, Msg_r^2, f(t)=t
  value: 0.947
  metric: MRR
  arxiv_id: '2302.02209'
  paper_title: A Theory of Link Prediction via Relational Weisfeiler-Leman on Knowledge
    Graphs
papers:
- arxiv_id: '2605.12197'
  title: A Unified Graph Language Model for Multi-Domain Multi-Task Graph Alignment
    Instruction Tuning
  date_iso: '2026-05-12'
  venue: ''
- arxiv_id: '2605.06576'
  title: On the Safety of Graph Representation Learning
  date_iso: '2026-05-07'
  venue: ''
- arxiv_id: '2602.09258'
  title: Generalizing GNNs with Tokenized Mixture of Experts
  date_iso: '2026-02-09'
  venue: KDD 2026
- arxiv_id: '2601.21369'
  title: 'Rethinking Federated Graph Foundation Models: A Graph-Language Alignment-based
    Approach'
  date_iso: '2026-01-29'
  venue: ''
- arxiv_id: '2510.07755'
  title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
    and Inter-domain Knowledge Modeling'
  date_iso: '2025-10-09'
  venue: ''
- arxiv_id: '2507.19526'
  title: Quantizing Text-attributed Graphs for Semantic-Structural Integration
  date_iso: '2025-07-20'
  venue: KDD 2025
- arxiv_id: '2505.12684'
  title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
    Entanglement
  date_iso: '2025-05-19'
  venue: NeurIPS 2025
- arxiv_id: '2505.12027'
  title: Relation-Aware Graph Foundation Model
  date_iso: '2025-05-17'
  venue: ''
- arxiv_id: '2502.00806'
  title: 'UniGraph2: Learning a Unified Embedding Space to Bind Multimodal Graphs'
  date_iso: '2025-02-02'
  venue: WWW 2025
- arxiv_id: '2412.16441'
  title: 'Towards Graph Foundation Models: Learning Generalities Across Graphs via
    Task-Trees'
  date_iso: '2024-12-21'
  venue: ICML 2024
- arxiv_id: '2411.06070'
  title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
  date_iso: '2024-11-09'
  venue: NeurIPS 2024
- arxiv_id: '2410.12609'
  title: 'Towards Graph Foundation Models: Training on Knowledge Graphs Enables Transferability
    to General Graphs'
  date_iso: '2024-10-16'
  venue: NeurIPS 2024
- arxiv_id: '2410.12288'
  title: A Prompt-Based Knowledge Graph Foundation Model for Universal In-Context
    Reasoning
  date_iso: '2024-10-16'
  venue: NeurIPS 2024
- arxiv_id: '2409.12865'
  title: 'KnowFormer: Revisiting Transformers for Knowledge Graph Reasoning'
  date_iso: '2024-09-19'
  venue: ICML 2024
- arxiv_id: '2402.13630'
  title: 'UniGraph: Learning a Unified Cross-Domain Foundation Model for Text-Attributed
    Graphs'
  date_iso: '2024-02-21'
  venue: KDD 2024
- arxiv_id: '2310.04562'
  title: Towards Foundation Models for Knowledge Graph Reasoning
  date_iso: '2023-10-06'
  venue: ICLR 2023
- arxiv_id: '2310.00149'
  title: 'One for All: Towards Training One Graph Model for All Classification Tasks'
  date_iso: '2023-09-29'
  venue: ICLR 2023
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
- arxiv_id: '2206.04798'
  title: 'A*Net: A Scalable Path-based Reasoning Approach for Knowledge Graphs'
  date_iso: '2022-06-07'
  venue: NeurIPS 2022
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
- arxiv_id: '2009.14332'
  title: Multi-hop Attention Graph Neural Networks
  date_iso: '2020-09-29'
  venue: IJCAI 2020
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
  notes: ''
  is_standard: true
  primary_metric: MRR
  default_metric: MRR
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 40943.0
    avg_edges: 93003.0
    num_classes: 11
  metrics:
  - MRR
  - ACC
  - Accuracy
  - F1
  metric_display_names:
  - MRR
  - ACC
  - Accuracy
  - F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: PNA, Msg_r^2, f(t)=t
    model_plain: PNA, Msg_r^2, f(t)=t
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.947
    - null
    - null
    - null
    metric_stds:
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.947
    - null
    - null
    - null
    metric_stds:
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
    - 0.946
    - null
    - null
    - null
    metric_stds:
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
    - 0.946
    - null
    - null
    - null
    metric_stds:
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
    - 0.944
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: sum, Msg_r^3, f(t)=0
    model_plain: sum, Msg_r^3, f(t)=0
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
    - 0.943
    - null
    - null
    - null
    metric_stds:
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
    - 0.943
    - null
    - null
    - null
    metric_stds:
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
    - 0.941
    - null
    - null
    - null
    metric_stds:
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
    - 0.941
    - null
    - null
    - null
    metric_stds:
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
    - 0.939
    - null
    - null
    - null
    metric_stds:
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
    - 0.937
    - null
    - null
    - null
    metric_stds:
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
    - 0.934
    - null
    - null
    - null
    metric_stds:
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
    - 0.934
    - null
    - null
    - null
    metric_stds:
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
    - 0.932
    - null
    - null
    - null
    metric_stds:
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
    - 0.932
    - null
    - null
    - null
    metric_stds:
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
    - 0.932
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: GFT
    model_plain: GFT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06070'
    title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    date: Nov 9, 2024
    date_iso: '2024-11-09'
    date_display: Nov 2024
    codebase_url: https://github.com/Zehong-Wang/GFT
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9191
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: UniGraph2
    model_plain: UniGraph2
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2502.00806'
    title: 'UniGraph2: Learning a Unified Embedding Space to Bind Multimodal Graphs'
    date: Feb 2, 2025
    date_iso: '2025-02-02'
    date_display: Feb 2025
    codebase_url: https://github.com/yf-he/UniGraph2
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8786
    - null
    - null
    - null
    metric_stds:
    - 0.0006
    - null
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
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8552
    - null
    - null
    - null
    metric_stds:
    - 0.0012
    - null
    - null
    - null
  - model: GIANT
    model_plain: GIANT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06070'
    title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    date: Nov 9, 2024
    date_iso: '2024-11-09'
    date_display: Nov 2024
    codebase_url: https://github.com/Zehong-Wang/GFT
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8436
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: Linear
    model_plain: Linear
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8433
    - null
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
    - null
  - model: FedSage
    model_plain: FedSage
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
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
    - 0.8426
    - null
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
    - null
  - model: UniGraph
    model_plain: UniGraph
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2502.00806'
    title: 'UniGraph2: Learning a Unified Embedding Space to Bind Multimodal Graphs'
    date: Feb 2, 2025
    date_iso: '2025-02-02'
    date_display: Feb 2025
    codebase_url: https://github.com/yf-he/UniGraph2
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8406
    - null
    - null
    - null
    metric_stds:
    - 0.0024
    - null
    - null
    - null
  - model: FED-PUB
    model_plain: FED-PUB
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8379
    - null
    - null
    - null
    metric_stds:
    - 0.0025
    - null
    - null
    - null
  - model: MOON
    model_plain: MOON
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8364
    - null
    - null
    - null
    metric_stds:
    - 0.0045
    - null
    - null
    - null
  - model: FedAvg
    model_plain: FedAvg
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8355
    - null
    - null
    - null
    metric_stds:
    - 0.002
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
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8298
    - null
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
    - null
  - model: FedSage
    model_plain: FedSage
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8295
    - null
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
    - null
  - model: FedAvg
    model_plain: FedAvg
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
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
    - 0.8252
    - null
    - null
    - null
    metric_stds:
    - 0.0023
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
    - 0.825
    - null
    - null
    - null
    metric_stds:
    - null
    - null
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
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
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
    - 0.8244
    - null
    - null
    - null
    metric_stds:
    - 0.0037
    - null
    - null
    - null
  - model: MOON
    model_plain: MOON
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
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
    - 0.8231
    - null
    - null
    - null
    metric_stds:
    - 0.0025
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
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8227
    - null
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
    - null
  - model: Linear
    model_plain: Linear
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
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
    - 0.8225
    - null
    - null
    - null
    metric_stds:
    - 0.0023
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
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
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
    - 0.8171
    - null
    - null
    - null
    metric_stds:
    - 0.003
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
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
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
    - 0.8152
    - null
    - null
    - null
    metric_stds:
    - 0.0024
    - null
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
    arxiv_id: '2601.21369'
    title: 'Rethinking Federated Graph Foundation Models: A Graph-Language Alignment-based
      Approach'
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8135
    - null
    - null
    - null
    metric_stds:
    - 0.0031
    - null
    - null
    - null
  - model: FedSage
    model_plain: FedSage
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.21369'
    title: 'Rethinking Federated Graph Foundation Models: A Graph-Language Alignment-based
      Approach'
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8126
    - null
    - null
    - null
    metric_stds:
    - 0.0026
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
    arxiv_id: '2510.07755'
    title: 'FedBook: A Unified Federated Graph Foundation Codebook with Intra-domain
      and Inter-domain Knowledge Modeling'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
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
    - 0.8124
    - null
    - null
    - null
    metric_stds:
    - 0.0055
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
    - 0.809
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: FED-PUB
    model_plain: FED-PUB
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.21369'
    title: 'Rethinking Federated Graph Foundation Models: A Graph-Language Alignment-based
      Approach'
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8065
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
    - null
  - model: MOON
    model_plain: MOON
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.21369'
    title: 'Rethinking Federated Graph Foundation Models: A Graph-Language Alignment-based
      Approach'
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8062
    - null
    - null
    - null
    metric_stds:
    - 0.0042
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
    arxiv_id: '2601.21369'
    title: 'Rethinking Federated Graph Foundation Models: A Graph-Language Alignment-based
      Approach'
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8033
    - null
    - null
    - null
    metric_stds:
    - 0.0006
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
    arxiv_id: '2505.12684'
    title: Towards Effective Federated Graph Foundation Model via Mitigating Knowledge
      Entanglement
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8025
    - null
    - null
    - null
    metric_stds:
    - 0.0028
    - null
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
    arxiv_id: '2411.06070'
    title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    date: Nov 9, 2024
    date_iso: '2024-11-09'
    date_display: Nov 2024
    codebase_url: https://github.com/Zehong-Wang/GFT
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8016
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: FedAvg
    model_plain: FedAvg
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.21369'
    title: 'Rethinking Federated Graph Foundation Models: A Graph-Language Alignment-based
      Approach'
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8007
    - null
    - null
    - null
    metric_stds:
    - 0.0012
    - null
    - null
    - null
  - model: OFA
    model_plain: OFA*
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.21369'
    title: 'Rethinking Federated Graph Foundation Models: A Graph-Language Alignment-based
      Approach'
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: Linear
    model_plain: Linear
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2601.21369'
    title: 'Rethinking Federated Graph Foundation Models: A Graph-Language Alignment-based
      Approach'
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7983
    - null
    - null
    - null
    metric_stds:
    - 0.003
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
    arxiv_id: '2601.21369'
    title: 'Rethinking Federated Graph Foundation Models: A Graph-Language Alignment-based
      Approach'
    date: Jan 29, 2026
    date_iso: '2026-01-29'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7974
    - null
    - null
    - null
    metric_stds:
    - 0.0014
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
    arxiv_id: '2411.06070'
    title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    date: Nov 9, 2024
    date_iso: '2024-11-09'
    date_display: Nov 2024
    codebase_url: https://github.com/Zehong-Wang/GFT
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7899
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  row_count: 237
  rows_json: /data/datasets/wn18rr/standard-split-rows.json
  chart_json: /data/datasets/wn18rr/standard-split-chart.json
  arch_counts:
    gnn: 126
    hybrid: 43
    graph_transformer: 3
    llm: 15
    walk: 4
    traditional: 42
  metric_counts:
  - 190
  - 5
  - 42
  - 5
  milestones: &id001
  - value: 0.477
    std: 0.001
    model: RotatE
    arxiv_id: '1902.10197'
    title: 'RotatE: Knowledge Graph Embedding by Relational Rotation in Complex Space'
    date: '2018-09-27'
  - value: 0.479
    std: null
    model: CompGCN
    arxiv_id: '1911.03082'
    title: Composition-based Multi-Relational Graph Convolutional Networks
    date: '2019-11-08'
  - value: 0.502
    std: null
    model: MAGNA + DistMult
    arxiv_id: '2009.14332'
    title: Multi-hop Attention Graph Neural Networks
    date: '2020-09-29'
  - value: 0.533
    std: null
    model: RED-GNN
    arxiv_id: '2212.05767'
    title: 'A Survey of Knowledge Graph Reasoning on Graph Types: Static, Dynamic,
      and Multi-Modal'
    date: '2022-12-12'
  - value: 0.553
    std: null
    model: KGCF
    arxiv_id: '2302.13083'
    title: Knowledge Graph Completion with Counterfactual Augmentation
    date: '2023-02-25'
  - value: 0.9191
    std: null
    model: GFT
    arxiv_id: '2411.06070'
    title: 'GFT: Graph Foundation Model with Transferable Tree Vocabulary'
    date: '2024-11-09'
  milestones_by_metric:
    MRR: *id001
    ACC:
    - value: 0.9352
      std: null
      model: LLMs
      arxiv_id: '2605.12197'
      title: A Unified Graph Language Model for Multi-Domain Multi-Task Graph Alignment
        Instruction Tuning
      date: '2026-05-12'
    Accuracy:
    - value: 0.9814
      std: 0.0025
      model: OFA-llama2-13b
      arxiv_id: '2310.00149'
      title: 'One for All: Towards Training One Graph Model for All Classification
        Tasks'
      date: '2023-09-29'
    F1:
    - value: 0.753
      std: null
      model: LLMs
      arxiv_id: '2605.12197'
      title: A Unified Graph Language Model for Multi-Domain Multi-Task Graph Alignment
        Instruction Tuning
      date: '2026-05-12'
---

