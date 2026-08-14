---
title: ogbg-code2
slug: ogbg-code2
benchmark: OGB
task_type: graph_classification
short_description: Predict the subtokens in a Python method's name from the method
  body represented as an abstract syntax tree.
description: '**Set-valued graph prediction** Predict the subtokens in a Python method''s
  name from the method body represented as an abstract syntax tree. Evaluated by F1.'
detailed_description:
  task: Predict the subtokens in a Python method's name from the method body represented
    as an abstract syntax tree. The graph-level output is a sequence, but the official
    F1 score compares sets of predicted and reference subtokens and therefore does
    not reward the correct subtoken order.
  data: The 452,741 methods originate from CodeSearchNet and were extracted from 13,587
    popular GitHub repositories. OGB parses each method into an abstract syntax tree
    and augments the tree with next-token edges; inverse edges are normally added
    for bidirectional message passing.
  features: AST nodes encode a node type drawn from 97 types, an attribute such as
    a variable name, depth, and preorder traversal position. The target method name
    on the root function-definition node, including recursive occurrences, is replaced
    with a special mask token to prevent direct target leakage. Edge features distinguish
    AST, next-token, and inverse-edge direction information.
  splits_and_evaluation: The official project split assigns whole repositories to
    only one of training, validation, or test, testing transfer to unseen codebases.
    Targets are truncated to five subtokens for the published baseline setup, using
    a 5,000-subtoken vocabulary plus an unknown token. Performance is the F1 score
    over predicted and reference subtokens.
  quirks_and_pitfalls: The predecessor ogbg-code dataset is deprecated because method
    names leaked through the input AST; results from it are not comparable to ogbg-code2.
    A random method-level split is substantially easier and permits project-specific
    naming conventions to cross split boundaries. The usual F1 metric is order-insensitive,
    so it does not fully measure method-name generation quality.
sources:
- title: Open Graph Benchmark
  arxiv_id: '2005.00687'
  kind: benchmark_definition
- title: OGB graph property prediction documentation
  url: https://ogb.stanford.edu/docs/graphprop/#ogbg-code2
  kind: official_documentation
- title: CodeSearchNet Challenge
  arxiv_id: '1909.09436'
  kind: upstream_data_source
primary_metric: F1
higher_is_better: true
pyg_url: https://ogb.stanford.edu/docs/leader_graphprop/#ogbg-code2
stats:
  num_graphs: 452741
  avg_nodes: 125.2
  avg_edges: 124.2
  num_classes: 1
  extra_stats:
    avg_degree: 1.984
    degree_convention: derived as 2 × avg_edges / avg_nodes for the augmented graph
      treated as undirected
    edge_feature_type: AST, next-token, and inverse-edge relation metadata
    label_imbalance: not applicable; the target is a variable-length set of method-name
      subtokens
    node_feature_type: AST node type, attribute, depth, and preorder metadata
    statistic_notes: no fixed numeric feature dimension is exposed because AST attributes
      are heterogeneous; clustering coefficient and diameter are not reported
result_count: 43
best_model:
  model: GMN
  value: 0.206
  metric: F1
  arxiv_id: '2509.13735'
  paper_title: State Space Models over Directed Graphs
papers:
- arxiv_id: '2511.08028'
  title: Generalizable Insights for Graph Transformers in Theory and Practice
  date_iso: '2025-11-11'
  venue: NeurIPS 2025
- arxiv_id: '2509.13735'
  title: State Space Models over Directed Graphs
  date_iso: '2025-09-17'
  venue: ''
- arxiv_id: '2406.12059'
  title: A Scalable and Effective Alternative to Graph Transformers
  date_iso: '2024-06-17'
  venue: AAAI 2024
- arxiv_id: '2311.07966'
  title: Higher-Order Expander Graph Propagation
  date_iso: '2023-11-14'
  venue: ''
- arxiv_id: '2301.11956'
  title: On the Connection Between MPNN and Graph Transformer
  date_iso: '2023-01-27'
  venue: ICML 2023
- arxiv_id: '2210.13148'
  title: Transformers over Directed Acyclic Graphs
  date_iso: '2022-10-24'
  venue: Neural Information Processing Systems
- arxiv_id: '2202.03036'
  title: Structure-Aware Transformer for Graph Representation Learning
  date_iso: '2022-02-07'
  venue: International Conference on Machine Learning
- arxiv_id: '2201.08821'
  title: Representing Long-Range Context for Graph Neural Networks with Global Attention
  date_iso: '2022-01-21'
  venue: Neural Information Processing Systems
- arxiv_id: '2106.08279'
  title: First Place Solution of KDD Cup 2021 & OGB Large-Scale Challenge Graph Prediction
    Track
  date_iso: '2021-06-15'
  venue: ''
- arxiv_id: '2102.09844'
  title: E(n) Equivariant Graph Neural Networks
  date_iso: '2021-02-19'
  venue: International Conference on Machine Learning
- arxiv_id: '2101.07965'
  title: Directed Acyclic Graph Neural Networks
  date_iso: '2021-01-20'
  venue: International Conference on Learning Representations
- arxiv_id: '1810.00826'
  title: How Powerful are Graph Neural Networks?
  date_iso: '2018-10-01'
  venue: International Conference on Learning Representations
- arxiv_id: '1806.08804'
  title: Hierarchical Graph Representation Learning with Differentiable Pooling
  date_iso: '2018-06-22'
  venue: Neural Information Processing Systems
- arxiv_id: '1710.10903'
  title: Graph Attention Networks
  date_iso: '2017-10-30'
  venue: International Conference on Learning Representations
- arxiv_id: '1706.02216'
  title: Inductive Representation Learning on Large Graphs
  date_iso: '2017-06-07'
  venue: Neural Information Processing Systems
- arxiv_id: '1704.07912'
  title: Neural Message Passing for Quantum Chemistry
  date_iso: '2017-04-25'
  venue: 'arXiv: Numerical Analysis'
- arxiv_id: '1609.02907'
  title: Semi-Supervised Classification with Graph Convolutional Networks
  date_iso: '2016-09-09'
  venue: International Conference on Learning Representations
variants:
- slug: standard-split
  name: Standard split
  notes: OGB project split.
  is_standard: true
  primary_metric: F1
  default_metric: F1
  higher_is_better: true
  stats:
    num_graphs: 452741
    avg_nodes: 125.2
    avg_edges: 124.2
    num_classes: 1
    extra_stats:
      avg_degree: 1.984
      degree_convention: derived as 2 × avg_edges / avg_nodes for the augmented graph
        treated as undirected
      edge_feature_type: AST, next-token, and inverse-edge relation metadata
      label_imbalance: not applicable; the target is a variable-length set of method-name
        subtokens
      node_feature_type: AST node type, attribute, depth, and preorder metadata
      statistic_notes: no fixed numeric feature dimension is exposed because AST attributes
        are heterogeneous; clustering coefficient and diameter are not reported
  metrics:
  - F1
  metric_display_names:
  - F1
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
    - 0.206
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
    - 0.205
    metric_stds:
    - 0.0023
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
    - 0.203
    metric_stds:
    - 0.0023
  - model: DAG+SAT
    model_plain: DAG+SAT
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
    - 0.202
    metric_stds:
    - 0.002
  - model: Exphormer
    model_plain: Exphormer
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
    - 0.199
    metric_stds:
    - 0.002
  - model: LPE
    model_plain: LPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1948
    metric_stds:
    - 0.0021
  - model: RRWP
    model_plain: RRWP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1942
    metric_stds:
    - 0.001
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
    - 0.194
    metric_stds:
    - 0.003
  - model: RWSE
    model_plain: RWSE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1939
    metric_stds:
    - 0.0047
  - model: K-Subtree SAT
    model_plain: K-Subtree SAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_iso: '2023-01-27'
    date_display: Jan 2023
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1937
    metric_stds:
    - 0.0028
  - model: k-subtree SAT-PNA
    model_plain: k-subtree SAT-PNA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1937
    metric_stds:
    - 0.0028
  - model: SPE
    model_plain: SPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1935
    metric_stds:
    - 0.0021
  - model: k-subtree SAT-GCN
    model_plain: k-subtree SAT-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1934
    metric_stds:
    - 0.002
  - model: NoPE
    model_plain: NoPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1927
    metric_stds:
    - 0.002
  - model: GECO
    model_plain: GECO
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.12059'
    title: A Scalable and Effective Alternative to Graph Transformers
    date: Jun 17, 2024
    date_iso: '2024-06-17'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1915
    metric_stds:
    - 0.002
  - model: k-subtree SAT-GIN
    model_plain: k-subtree SAT-GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.191
    metric_stds:
    - 0.0023
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_iso: '2023-01-27'
    date_display: Jan 2023
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1894
    metric_stds:
    - 0.0024
  - model: GraphGPS
    model_plain: GraphGPS
    is_baseline: true
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.189
    metric_stds:
    - 0.002
  - model: DAG+Transformer
    model_plain: DAG+Transformer
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
    - 0.188
    metric_stds:
    - 0.002
  - model: GraphTrans (GCN-Virtual)
    model_plain: GraphTrans (GCN-Virtual)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_iso: '2023-01-27'
    date_display: Jan 2023
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.183
    metric_stds:
    - 0.0024
  - model: GraphTrans
    model_plain: GraphTrans
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 9.1
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2201.08821'
    title: Representing Long-Range Context for Graph Neural Networks with Global Attention
    date: Jan 21, 2022
    date_iso: '2022-01-21'
    date_display: Jan 2022
    codebase_url: https://github.com/ucbrise/graphtrans
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.183
    metric_stds:
    - 0.0024
  - model: PACE
    model_plain: PACE
    is_baseline: true
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.178
    metric_stds:
    - 0.002
  - model: DAGNN (SOTA)
    model_plain: DAGNN (SOTA)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2201.08821'
    title: Representing Long-Range Context for Graph Neural Networks with Global Attention
    date: Jan 21, 2022
    date_iso: '2022-01-21'
    date_display: Jan 2022
    codebase_url: https://github.com/ucbrise/graphtrans
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1751
    metric_stds:
    - 0.0049
  - model: DAGNN
    model_plain: DAGNN
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
    - 0.175
    metric_stds:
    - 0.005
  - model: MPNN + VN + NoPE
    model_plain: MPNN + VN + NoPE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_iso: '2023-01-27'
    date_display: Jan 2023
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1727
    metric_stds:
    - 0.0017
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
    - 0.169
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
    arxiv_id: '2201.08821'
    title: Representing Long-Range Context for Graph Neural Networks with Global Attention
    date: Jan 21, 2022
    date_iso: '2022-01-21'
    date_display: Jan 2022
    codebase_url: https://github.com/ucbrise/graphtrans
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.167
    metric_stds:
    - 0.0015
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
    - 0.167
    metric_stds:
    - 0.002
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
    - 0.166
    metric_stds:
    - 0.002
  - model: GCN-virtual
    model_plain: GCN-virtual
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2201.08821'
    title: Representing Long-Range Context for Graph Neural Networks with Global Attention
    date: Jan 21, 2022
    date_iso: '2022-01-21'
    date_display: Jan 2022
    codebase_url: https://github.com/ucbrise/graphtrans
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1595
    metric_stds:
    - 0.0018
  - model: GCN+virtual node
    model_plain: GCN+virtual node
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_iso: '2023-01-27'
    date_display: Jan 2023
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1595
    metric_stds:
    - 0.0018
  - model: GIN-virtual
    model_plain: GIN-virtual
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2201.08821'
    title: Representing Long-Range Context for Graph Neural Networks with Global Attention
    date: Jan 21, 2022
    date_iso: '2022-01-21'
    date_display: Jan 2022
    codebase_url: https://github.com/ucbrise/graphtrans
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1581
    metric_stds:
    - 0.002
  - model: GIN+virtual node
    model_plain: GIN+virtual node
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_iso: '2023-01-27'
    date_display: Jan 2023
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1581
    metric_stds:
    - 0.0026
  - model: GCN-Virtual Node
    model_plain: GCN-Virtual Node
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1581
    metric_stds:
    - 0.0026
  - model: GIN-Virtual Node
    model_plain: GIN-Virtual Node
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1581
    metric_stds:
    - 0.0026
  - model: PNA
    model_plain: PNA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2201.08821'
    title: Representing Long-Range Context for Graph Neural Networks with Global Attention
    date: Jan 21, 2022
    date_iso: '2022-01-21'
    date_display: Jan 2022
    codebase_url: https://github.com/ucbrise/graphtrans
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.157
    metric_stds:
    - 0.0032
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
    - 0.157
    metric_stds:
    - 0.002
  - model: higher-order expander graph propagation
    model_plain: higher-order expander graph propagation
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2311.07966'
    title: Higher-Order Expander Graph Propagation
    date: Nov 14, 2023
    date_iso: '2023-11-14'
    date_display: Nov 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1519
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
    arxiv_id: '2201.08821'
    title: Representing Long-Range Context for Graph Neural Networks with Global Attention
    date: Jan 21, 2022
    date_iso: '2022-01-21'
    date_display: Jan 2022
    codebase_url: https://github.com/ucbrise/graphtrans
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1507
    metric_stds:
    - 0.0018
  - model: EGP
    model_plain: EGP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.07966'
    title: Higher-Order Expander Graph Propagation
    date: Nov 14, 2023
    date_iso: '2023-11-14'
    date_display: Nov 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1497
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
    arxiv_id: '2201.08821'
    title: Representing Long-Range Context for Graph Neural Networks with Global Attention
    date: Jan 21, 2022
    date_iso: '2022-01-21'
    date_display: Jan 2022
    codebase_url: https://github.com/ucbrise/graphtrans
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1495
    metric_stds:
    - 0.0023
  - model: Plain GIN
    model_plain: Plain GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.07966'
    title: Higher-Order Expander Graph Propagation
    date: Nov 14, 2023
    date_iso: '2023-11-14'
    date_display: Nov 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1495
    metric_stds:
    - 0.0023
  - model: GIN + 3-Regular Bipartite Expander + Summation
    model_plain: GIN + 3-Regular Bipartite Expander + Summation
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.07966'
    title: Higher-Order Expander Graph Propagation
    date: Nov 14, 2023
    date_iso: '2023-11-14'
    date_display: Nov 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.1254
    metric_stds:
    - 0.0029
  row_count: 43
  rows_json: ''
  chart_json: /data/datasets/ogbg-code2/standard-split-chart.json
  arch_counts:
    gnn: 17
    hybrid: 12
    graph_transformer: 13
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 43
  milestones: &id001
  - value: 0.183
    std: 0.0024
    model: GraphTrans
    arxiv_id: '2201.08821'
    title: Representing Long-Range Context for Graph Neural Networks with Global Attention
    date: '2022-01-21'
  - value: 0.1937
    std: 0.0028
    model: k-subtree SAT-PNA
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: '2022-02-07'
  - value: 0.206
    std: 0.002
    model: GMN
    arxiv_id: '2509.13735'
    title: State Space Models over Directed Graphs
    date: '2025-09-17'
  milestones_by_metric:
    F1: *id001
---

