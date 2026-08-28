---
title: Wisconsin
slug: wisconsin
benchmark: Heterophilic Graphs
task_type: node_classification
short_description: WebKB node classification on Wisconsin university webpages (5 classes).
description: '**5-class node classification** WebKB node classification on Wisconsin
  university webpages (5 classes). Uses the Geom-GCN/PyG node features and graph.
  Evaluated by Accuracy.'
detailed_description:
  task: WebKB node classification on Wisconsin university webpages (5 classes). The
    primary catalog metric is Accuracy.
  data: WebKB node classification on Wisconsin university webpages (5 classes).
  features: 'Features and edges follow the Geom-GCN/PyG artifact: WebKB uses webpage
    bag-of-words and hyperlinks, Actor uses film-page keywords and co-occurrence links,
    and WikipediaNetwork uses page features and hyperlinks.'
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses Accuracy (higher is better). Exact masks or folds must
    come from the cited release.'
  quirks_and_pitfalls: These small or repurposed graphs have contested preprocessing
    and split conventions. Results across Geom-GCN, PyG, and corrected heterophily
    artifacts are not automatically comparable; class imbalance and high variance
    require multiple splits.
sources:
- title: Heterophilic Graphs benchmark
  arxiv_id: '2110.14446'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric Wisconsin loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.WebKB.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.WebKB.html
stats:
  num_graphs: 1
  avg_nodes: 251.0
  avg_edges: 499.0
  num_classes: 5
  extra_stats:
    edge_feature_dim: 0
    edge_feature_type: webpage hyperlinks; no edge attributes
    edge_homophily: 0.21
    heterophily: 0.79
    label_imbalance: strong class imbalance; class counts are reported in the heterophily
      benchmark appendix
    node_feature_dim: 1703
    node_feature_type: sparse bag-of-words webpage features
    statistic_notes: Geom-GCN/WebKB preprocessing; exact edge counts can vary across
      cleaned versions
result_count: 319
best_model:
  model: ACM-GCN
  value: 0.958
  metric: Accuracy
  arxiv_id: '2504.19785'
  paper_title: Heterophily-informed Message Passing
papers:
- arxiv_id: '2605.21247'
  title: Graph Navier–Stokes Networks
  date_iso: '2026-05-20'
  venue: ''
- arxiv_id: '2604.19028'
  title: Learning Posterior Predictive Distributions for Node Classification from
    Synthetic Graph Priors
  date_iso: '2026-04-21'
  venue: ICLR 2026
- arxiv_id: '2603.26178'
  title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
    Learning via Ricci Flow'
  date_iso: '2026-03-27'
  venue: ''
- arxiv_id: '2602.15634'
  title: 'Beyond ReLU: Bifurcation, Oversmoothing, and Topological Priors'
  date_iso: '2026-02-17'
  venue: ''
- arxiv_id: '2601.22943'
  title: 'Scalable Topology-Preserving Graph Coarsening: Concepts and Algorithms'
  date_iso: '2026-01-30'
  venue: ''
- arxiv_id: '2601.18917'
  title: 'GraIP: A Benchmarking Framework For Neural Graph Inverse Problems'
  date_iso: '2026-01-26'
  venue: ''
- arxiv_id: '2511.16062'
  title: Gauge-Equivariant Graph Networks via Self-Interference Cancellation
  date_iso: '2025-11-20'
  venue: ''
- arxiv_id: '2506.14291'
  title: 'Equivariance Everywhere All At Once: A Recipe for Graph Foundation Models'
  date_iso: '2025-06-17'
  venue: ''
- arxiv_id: '2506.06582'
  title: 'Demystifying Topological Message-Passing with Relational Structures: A Case
    Study on Oversquashing in Simplicial Message-Passing'
  date_iso: '2025-06-06'
  venue: ICLR 2025
- arxiv_id: '2505.15845'
  title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
    Learning Models'
  date_iso: '2025-05-19'
  venue: ''
- arxiv_id: '2505.11346'
  title: What Can We Learn From MIMO Graph Convolutions?
  date_iso: '2025-05-16'
  venue: IJCAI 2025
- arxiv_id: '2504.19785'
  title: Heterophily-informed Message Passing
  date_iso: '2025-04-28'
  venue: TMLR 2025
- arxiv_id: '2502.08092'
  title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
  date_iso: '2025-02-12'
  venue: KDD 2025
- arxiv_id: '2501.19089'
  title: Resolving Oversmoothing with Opinion Dissensus
  date_iso: '2025-01-31'
  venue: ''
- arxiv_id: '2410.05593'
  title: When Graph Neural Networks Meet Dynamic Mode Decomposition
  date_iso: '2024-10-08'
  venue: ICLR 2024
- arxiv_id: '2408.13471'
  title: Disentangled Generative Graph Representation Learning
  date_iso: '2024-08-24'
  venue: ''
- arxiv_id: '2408.07654'
  title: 'Graph Triple Attention Network: A Decoupled Perspective'
  date_iso: '2024-08-14'
  venue: ''
- arxiv_id: '2407.11907'
  title: 'GraphFM: A generalist graph transformer that learns transferable representations
    across diverse domains'
  date_iso: '2024-07-16'
  venue: TMLR 2024
- arxiv_id: '2406.12539'
  title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering GNNs for
    Heterophilic Graphs'
  date_iso: '2024-06-18'
  venue: KDD 2024
- arxiv_id: '2406.10863'
  title: Global-Local Graph Neural Networks for Node-Classification
  date_iso: '2024-06-01'
  venue: ''
- arxiv_id: '2405.20652'
  title: 'Sign is Not a Remedy: Multiset-to-Multiset Message Passing for Learning
    on Heterophilic Graphs'
  date_iso: '2024-05-31'
  venue: ICML 2024
- arxiv_id: '2405.18581'
  title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation Decomposition
    via Large Language Models'
  date_iso: '2024-05-28'
  venue: ''
- arxiv_id: '2405.13902'
  title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training Framework'
  date_iso: '2024-05-22'
  venue: ''
- arxiv_id: '2404.17099'
  title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
    with FROND
  date_iso: '2024-04-26'
  venue: ICLR 2024
- arxiv_id: '2312.08221'
  title: Curriculum-Enhanced Residual Soft An-Isotropic Normalization for Over-smoothness
    in Deep GNNs
  date_iso: '2023-12-13'
  venue: AAAI 2023
- arxiv_id: '2311.14864'
  title: Effective Structural Encodings via Local Curvature Profiles
  date_iso: '2023-11-24'
  venue: ICLR 2023
- arxiv_id: '2310.16401'
  title: Graph Neural Networks with a Distribution of Parametrized Graphs
  date_iso: '2023-10-25'
  venue: ICML 2023
- arxiv_id: '2310.07430'
  title: Non-backtracking Graph Neural Networks
  date_iso: '2023-10-11'
  venue: TMLR 2023
- arxiv_id: '2310.01089'
  title: 'GraphText: Graph Reasoning in Text Space'
  date_iso: '2023-10-02'
  venue: ''
- arxiv_id: '2309.04082'
  title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
    Learning'
  date_iso: '2023-09-08'
  venue: ''
- arxiv_id: '2306.10466'
  title: 'Graph Ladling: Shockingly Simple Parallel GNN Training without Intermediate
    Communication'
  date_iso: '2023-06-18'
  venue: ICML 2023
- arxiv_id: '2305.16780'
  title: Graph Neural Convection-Diffusion with Heterophily
  date_iso: '2023-05-26'
  venue: IJCAI 2023
- arxiv_id: '2302.12357'
  title: 'Auto-HeG: Automated Graph Neural Network on Heterophilic Graphs'
  date_iso: '2023-02-23'
  venue: WWW 2023
- arxiv_id: '2212.02483'
  title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
  date_iso: '2022-12-05'
  venue: ICML 2022
- arxiv_id: '2211.14065'
  title: 'Beyond Smoothing: Unsupervised Graph Representation Learning with Edge Heterophily
    Discriminating'
  date_iso: '2022-11-25'
  venue: AAAI 2022
- arxiv_id: '2211.11761'
  title: 'From Node Interaction to Hop Interaction: New Effective and Scalable Graph
    Learning Paradigm'
  date_iso: '2022-11-21'
  venue: ''
- arxiv_id: '2210.09789'
  title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
  date_iso: '2022-10-18'
  venue: ICLR 2022
- arxiv_id: '2206.14418'
  title: Optimization-Induced Graph Implicit Nonlinear Diffusion
  date_iso: '2022-06-29'
  venue: ICML 2022
- arxiv_id: '2206.02386'
  title: Restructuring Graphs for Higher Homophily via Adaptive Spectral Clustering
  date_iso: '2022-06-06'
  venue: AAAI 2022
- arxiv_id: '2106.06134'
  title: Is Homophily a Necessity for Graph Neural Networks?
  date_iso: '2021-06-11'
  venue: ICLR 2021
- arxiv_id: '2105.07634'
  title: Improving Graph Neural Networks with Simple Architecture Design
  date_iso: '2021-05-17'
  venue: ''
- arxiv_id: '2103.14187'
  title: 'Beyond Low-Pass Filters: Adaptive Feature Propagation on Graphs'
  date_iso: '2021-03-26'
  venue: ''
- arxiv_id: '2005.14612'
  title: Non-Local Graph Neural Networks
  date_iso: '2020-05-29'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: Geom-GCN 10 fixed splits.
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 251.0
    avg_edges: 499.0
    num_classes: 5
    extra_stats:
      edge_feature_dim: 0
      edge_feature_type: webpage hyperlinks; no edge attributes
      edge_homophily: 0.21
      heterophily: 0.79
      label_imbalance: strong class imbalance; class counts are reported in the heterophily
        benchmark appendix
      node_feature_dim: 1703
      node_feature_type: sparse bag-of-words webpage features
      statistic_notes: Geom-GCN/WebKB preprocessing; exact edge counts can vary across
        cleaned versions
  metrics:
  - Accuracy
  - F1
  - Micro-F1
  metric_display_names:
  - Accuracy
  - F1
  - Micro-F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: ACM-GCN
    model_plain: ACM-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.19785'
    title: Heterophily-informed Message Passing
    date: Apr 28, 2025
    date_iso: '2025-04-28'
    date_display: Apr 2025
    codebase_url: https://github.com/AaltoML/heterophily-imp
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.958
    - null
    - null
    metric_stds:
    - 0.02
    - null
    - null
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.19785'
    title: Heterophily-informed Message Passing
    date: Apr 28, 2025
    date_iso: '2025-04-28'
    date_display: Apr 2025
    codebase_url: https://github.com/AaltoML/heterophily-imp
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.938
    - null
    - null
    metric_stds:
    - 0.024
    - null
    - null
  - model: DMD++
    model_plain: DMD++
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2410.05593'
    title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    date: Oct 8, 2024
    date_iso: '2024-10-08'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.919
    - null
    - null
    metric_stds:
    - 0.026
    - null
    - null
  - model: F-GREAD-BS
    model_plain: F-GREAD-BS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.17099'
    title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
      with FROND
    date: Apr 26, 2024
    date_iso: '2024-04-26'
    date_display: Apr 2024
    codebase_url: https://github.com/zknus/ICLR2024-FROND
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9059
    - null
    - null
    metric_stds:
    - 0.038
    - null
    - null
  - model: GNSN
    model_plain: GNSN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.21247'
    title: Graph Navier–Stokes Networks
    date: May 20, 2026
    date_iso: '2026-05-20'
    date_display: May 2026
    codebase_url: https://github.com/Duckbluee/Graph-Navier-Stokes-Networks
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9002
    - null
    - null
    metric_stds:
    - 0.0194
    - null
    - null
  - model: GLGCNII
    model_plain: GLGCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.10863'
    title: Global-Local Graph Neural Networks for Node-Classification
    date: Jun 1, 2024
    date_iso: '2024-06-01'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8972
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GREAD-BS
    model_plain: GREAD-BS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.17099'
    title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
      with FROND
    date: Apr 26, 2024
    date_iso: '2024-04-26'
    date_display: Apr 2024
    codebase_url: https://github.com/zknus/ICLR2024-FROND
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8941
    - null
    - null
    metric_stds:
    - 0.033
    - null
    - null
  - model: Sheaf
    model_plain: Sheaf
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.17099'
    title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
      with FROND
    date: Apr 26, 2024
    date_iso: '2024-04-26'
    date_display: Apr 2024
    codebase_url: https://github.com/zknus/ICLR2024-FROND
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8941
    - null
    - null
    metric_stds:
    - 0.0474
    - null
    - null
  - model: DMD-ACMP
    model_plain: DMD-ACMP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2410.05593'
    title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    date: Oct 8, 2024
    date_iso: '2024-10-08'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.894
    - null
    - null
    metric_stds:
    - 0.022
    - null
    - null
  - model: M2M-GNN
    model_plain: M2M-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.20652'
    title: 'Sign is Not a Remedy: Multiset-to-Multiset Message Passing for Learning
      on Heterophilic Graphs'
    date: May 31, 2024
    date_iso: '2024-05-31'
    date_display: May 2024
    codebase_url: https://github.com/Jinx-byebye/m2mgnn
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8901
    - null
    - null
    metric_stds:
    - 0.041
    - null
    - null
  - model: Framelets
    model_plain: Framelets
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.05593'
    title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    date: Oct 8, 2024
    date_iso: '2024-10-08'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.889
    - null
    - null
    metric_stds:
    - 0.032
    - null
    - null
  - model: SGOS-Expn
    model_plain: SGOS-Expn
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.15634'
    title: 'Beyond ReLU: Bifurcation, Oversmoothing, and Topological Priors'
    date: Feb 17, 2026
    date_iso: '2026-02-17'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8882
    - null
    - null
    metric_stds:
    - 0.0362
    - null
    - null
  - model: Diag-NSD
    model_plain: Diag-NSD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.16780'
    title: Graph Neural Convection-Diffusion with Heterophily
    date: May 26, 2023
    date_iso: '2023-05-26'
    date_display: May 2023
    codebase_url: https://github.com/zknus/Graph-Diffusion-CDE
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8863
    - null
    - null
    metric_stds:
    - 0.0275
    - null
    - null
  - model: GRAND
    model_plain: GRAND
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.05593'
    title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    date: Oct 8, 2024
    date_iso: '2024-10-08'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.886
    - null
    - null
    metric_stds:
    - 0.021
    - null
    - null
  - model: MM-FGCN
    model_plain: MM-FGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.21247'
    title: Graph Navier–Stokes Networks
    date: May 20, 2026
    date_iso: '2026-05-20'
    date_display: May 2026
    codebase_url: https://github.com/Duckbluee/Graph-Navier-Stokes-Networks
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.885
    - null
    - null
    metric_stds:
    - 0.041
    - null
    - null
  - model: ACM-GCN
    model_plain: ACM-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.11761'
    title: 'From Node Interaction to Hop Interaction: New Effective and Scalable Graph
      Learning Paradigm'
    date: Nov 21, 2022
    date_iso: '2022-11-21'
    date_display: Nov 2022
    codebase_url: https://github.com/JC-202/HopGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8843
    - null
    - null
    metric_stds:
    - 0.0322
    - null
    - null
  - model: FSGNN
    model_plain: FSGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2105.07634'
    title: Improving Graph Neural Networks with Simple Architecture Design
    date: May 17, 2021
    date_iso: '2021-05-17'
    date_display: May 2021
    codebase_url: https://github.com/sunilkmaurya/FSGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8843
    - null
    - null
    metric_stds:
    - 0.0322
    - null
    - null
  - model: MUSE
    model_plain: MUSE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_iso: '2024-08-24'
    date_display: Aug 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8824
    - null
    - null
    metric_stds:
    - 0.032
    - null
    - null
  - model: LRGNN
    model_plain: LRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_iso: '2024-08-24'
    date_display: Aug 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8823
    - null
    - null
    metric_stds:
    - 0.0354
    - null
    - null
  - model: GNRF
    model_plain: GNRF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.26178'
    title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
      Learning via Ricci Flow'
    date: Mar 27, 2026
    date_iso: '2026-03-27'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.882
    - null
    - null
    metric_stds:
    - 0.0384
    - null
    - null
  - model: PPGNN
    model_plain: PPGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02386'
    title: Restructuring Graphs for Higher Homophily via Adaptive Spectral Clustering
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/seanli3/graph_restructure
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.882
    - null
    - null
    metric_stds:
    - 0.033
    - null
    - null
  - model: GIND
    model_plain: GIND
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.14418'
    title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: https://github.com/7qchen/GIND
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8804
    - null
    - null
    metric_stds:
    - 0.0397
    - null
    - null
  - model: Ord. GNN
    model_plain: Ord. GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.20652'
    title: 'Sign is Not a Remedy: Multiset-to-Multiset Message Passing for Learning
      on Heterophilic Graphs'
    date: May 31, 2024
    date_iso: '2024-05-31'
    date_display: May 2024
    codebase_url: https://github.com/Jinx-byebye/m2mgnn
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8804
    - null
    - null
    metric_stds:
    - 0.036
    - null
    - null
  - model: OGNN
    model_plain: OGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_iso: '2024-08-24'
    date_display: Aug 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8804
    - null
    - null
    metric_stds:
    - 0.0363
    - null
    - null
  - model: Auto-HeG
    model_plain: Auto-HeG
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.12357'
    title: 'Auto-HeG: Automated Graph Neural Network on Heterophilic Graphs'
    date: Feb 23, 2023
    date_iso: '2023-02-23'
    date_display: Feb 2023
    codebase_url: ''
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8784
    - null
    - null
    metric_stds:
    - 0.0359
    - null
    - null
  - model: GCON
    model_plain: GCON
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.21247'
    title: Graph Navier–Stokes Networks
    date: May 20, 2026
    date_iso: '2026-05-20'
    date_display: May 2026
    codebase_url: https://github.com/Duckbluee/Graph-Navier-Stokes-Networks
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.878
    - null
    - null
    metric_stds:
    - 0.033
    - null
    - null
  - model: GRAFF
    model_plain: GRAFF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.17099'
    title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
      with FROND
    date: Apr 26, 2024
    date_iso: '2024-04-26'
    date_display: Apr 2024
    codebase_url: https://github.com/zknus/ICLR2024-FROND
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8745
    - null
    - null
    metric_stds:
    - 0.0294
    - null
    - null
  - model: NLMLP
    model_plain: NLMLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2005.14612'
    title: Non-Local Graph Neural Networks
    date: May 29, 2020
    date_iso: '2020-05-29'
    date_display: May 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.873
    - null
    - null
    metric_stds:
    - 0.043
    - null
    - null
  - model: DiGGR
    model_plain: DiGGR
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_iso: '2024-08-24'
    date_display: Aug 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8725
    - null
    - null
    metric_stds:
    - 0.0441
    - null
    - null
  - model: A-DGN(GCN)
    model_plain: A-DGN(GCN)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: Oct 18, 2022
    date_iso: '2022-10-18'
    date_display: Oct 2022
    codebase_url: https://github.com/gravins/Anti-SymmetricDGN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8725
    - null
    - null
    metric_stds:
    - 0.0364
    - null
    - null
  - model: GloGNN
    model_plain: GloGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.16780'
    title: Graph Neural Convection-Diffusion with Heterophily
    date: May 26, 2023
    date_iso: '2023-05-26'
    date_display: May 2023
    codebase_url: https://github.com/zknus/Graph-Diffusion-CDE
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8706
    - null
    - null
    metric_stds:
    - 0.0353
    - null
    - null
  - model: EM-ACM
    model_plain: EM-ACM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.16401'
    title: Graph Neural Networks with a Distribution of Parametrized Graphs
    date: Oct 25, 2023
    date_iso: '2023-10-25'
    date_display: Oct 2023
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8706
    - null
    - null
    metric_stds:
    - 0.0251
    - null
    - null
  - model: WRGAT
    model_plain: WRGAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.11761'
    title: 'From Node Interaction to Hop Interaction: New Effective and Scalable Graph
      Learning Paradigm'
    date: Nov 21, 2022
    date_iso: '2022-11-21'
    date_display: Nov 2022
    codebase_url: https://github.com/JC-202/HopGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8698
    - null
    - null
    metric_stds:
    - 0.0378
    - null
    - null
  - model: GOAL
    model_plain: GOAL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.20652'
    title: 'Sign is Not a Remedy: Multiset-to-Multiset Message Passing for Learning
      on Heterophilic Graphs'
    date: May 31, 2024
    date_iso: '2024-05-31'
    date_display: May 2024
    codebase_url: https://github.com/Jinx-byebye/m2mgnn
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8698
    - null
    - null
    metric_stds:
    - 0.044
    - null
    - null
  - model: de_attn + ada_inte
    model_plain: de_attn + ada_inte
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2408.07654'
    title: 'Graph Triple Attention Network: A Decoupled Perspective'
    date: Aug 14, 2024
    date_iso: '2024-08-14'
    date_display: Aug 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8695
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: EIGNN
    model_plain: EIGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.14418'
    title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: https://github.com/7qchen/GIND
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8686
    - null
    - null
    metric_stds:
    - 0.0554
    - null
    - null
  - model: GGCN
    model_plain: GGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: Oct 18, 2022
    date_iso: '2022-10-18'
    date_display: Oct 2022
    codebase_url: https://github.com/gravins/Anti-SymmetricDGN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8686
    - null
    - null
    metric_stds:
    - 0.0329
    - null
    - null
  - model: H_2GCN
    model_plain: H_2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2005.14612'
    title: Non-Local Graph Neural Networks
    date: May 29, 2020
    date_iso: '2020-05-29'
    date_display: May 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.867
    - null
    - null
    metric_stds:
    - 0.047
    - null
    - null
  - model: H2GCN
    model_plain: H2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02386'
    title: Restructuring Graphs for Higher Homophily via Adaptive Spectral Clustering
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/seanli3/graph_restructure
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.867
    - null
    - null
    metric_stds:
    - 0.047
    - null
    - null
  - model: SANE
    model_plain: SANE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2302.12357'
    title: 'Auto-HeG: Automated Graph Neural Network on Heterophilic Graphs'
    date: Feb 23, 2023
    date_iso: '2023-02-23'
    date_display: Feb 2023
    codebase_url: ''
    published_conference: WWW 2023
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8667
    - null
    - null
    metric_stds:
    - 0.0502
    - null
    - null
  - model: H2GCN-1
    model_plain: H2GCN-1
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2105.07634'
    title: Improving Graph Neural Networks with Simple Architecture Design
    date: May 17, 2021
    date_iso: '2021-05-17'
    date_display: May 2021
    codebase_url: https://github.com/sunilkmaurya/FSGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8667
    - null
    - null
    metric_stds:
    - 0.0469
    - null
    - null
  - model: BIMP
    model_plain: BIMP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2501.19089'
    title: Resolving Oversmoothing with Opinion Dissensus
    date: Jan 31, 2025
    date_iso: '2025-01-31'
    date_display: Jan 2025
    codebase_url: ''
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
    - null
    metric_stds:
    - 0.0433
    - null
    - null
  - model: MLP + GCN
    model_plain: MLP + GCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2106.06134'
    title: Is Homophily a Necessity for Graph Neural Networks?
    date: Jun 11, 2021
    date_iso: '2021-06-11'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/GPRGNN
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8643
    - null
    - null
    metric_stds:
    - 0.04
    - null
    - null
  - model: ACMP
    model_plain: ACMP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.16780'
    title: Graph Neural Convection-Diffusion with Heterophily
    date: May 26, 2023
    date_iso: '2023-05-26'
    date_display: May 2023
    codebase_url: https://github.com/zknus/Graph-Diffusion-CDE
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.861
    - null
    - null
    metric_stds:
    - 0.04
    - null
    - null
  - model: H2GCN-2
    model_plain: H2GCN-2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.06134'
    title: Is Homophily a Necessity for Graph Neural Networks?
    date: Jun 11, 2021
    date_iso: '2021-06-11'
    date_display: Jun 2021
    codebase_url: https://github.com/jianhao2016/GPRGNN
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8588
    - null
    - null
    metric_stds:
    - 0.0422
    - null
    - null
  - model: HopGNN
    model_plain: HopGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.11761'
    title: 'From Node Interaction to Hop Interaction: New Effective and Scalable Graph
      Learning Paradigm'
    date: Nov 21, 2022
    date_iso: '2022-11-21'
    date_display: Nov 2022
    codebase_url: https://github.com/JC-202/HopGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8569
    - null
    - null
    metric_stds:
    - 0.0543
    - null
    - null
  - model: Sine-Poly(A)-sh
    model_plain: Sine-Poly(A)-sh
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.15634'
    title: 'Beyond ReLU: Bifurcation, Oversmoothing, and Topological Priors'
    date: Feb 17, 2026
    date_iso: '2026-02-17'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8562
    - null
    - null
    metric_stds:
    - 0.0
    - null
    - null
  - model: SimP-GCN
    model_plain: SimP-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2005.14612'
    title: Non-Local Graph Neural Networks
    date: May 29, 2020
    date_iso: '2020-05-29'
    date_display: May 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.855
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: PloyGCL
    model_plain: PloyGCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.21247'
    title: Graph Navier–Stokes Networks
    date: May 20, 2026
    date_iso: '2026-05-20'
    date_display: May 2026
    codebase_url: https://github.com/Duckbluee/Graph-Navier-Stokes-Networks
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.855
    - null
    - null
    metric_stds:
    - 0.0188
    - null
    - null
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02386'
    title: Restructuring Graphs for Higher Homophily via Adaptive Spectral Clustering
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/seanli3/graph_restructure
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.855
    - null
    - null
    metric_stds:
    - 0.05
    - null
    - null
  row_count: 319
  rows_json: /data/datasets/wisconsin/standard-split-rows.json
  chart_json: /data/datasets/wisconsin/standard-split-chart.json
  arch_counts:
    gnn: 238
    hybrid: 51
    graph_transformer: 7
    llm: 0
    walk: 2
    traditional: 16
  metric_counts:
  - 296
  - 11
  - 12
  milestones: &id001
  - value: 0.873
    std: 0.043
    model: NLMLP
    arxiv_id: '2005.14612'
    title: Non-Local Graph Neural Networks
    date: '2020-05-29'
  - value: 0.8843
    std: 0.0322
    model: FSGNN
    arxiv_id: '2105.07634'
    title: Improving Graph Neural Networks with Simple Architecture Design
    date: '2021-05-17'
  - value: 0.8863
    std: 0.0275
    model: Diag-NSD
    arxiv_id: '2305.16780'
    title: Graph Neural Convection-Diffusion with Heterophily
    date: '2023-05-26'
  - value: 0.9059
    std: 0.038
    model: F-GREAD-BS
    arxiv_id: '2404.17099'
    title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
      with FROND
    date: '2024-04-26'
  - value: 0.919
    std: 0.026
    model: DMD++
    arxiv_id: '2410.05593'
    title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    date: '2024-10-08'
  - value: 0.958
    std: 0.02
    model: ACM-GCN
    arxiv_id: '2504.19785'
    title: Heterophily-informed Message Passing
    date: '2025-04-28'
  milestones_by_metric:
    Accuracy: *id001
    F1:
    - value: 0.836
      std: 0.0114
      model: FPS-T
      arxiv_id: '2309.04082'
      title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
        Learning'
      date: '2023-09-08'
    Micro-F1:
    - value: 0.869
      std: 0.042
      model: Vanilla ASGAT
      arxiv_id: '2103.14187'
      title: 'Beyond Low-Pass Filters: Adaptive Feature Propagation on Graphs'
      date: '2021-03-26'
---

