---
title: Pokec
slug: pokec
benchmark: LINKX Benchmarks
task_type: node_classification
short_description: Slovak social network Pokec node classification (binary gender,
  1.6M nodes).
description: '**Binary node classification** Slovak social network Pokec node classification
  (binary gender, 1.6M nodes). Uses the released sparse node features and a low-homophily
  graph. Feature-only baselines are essential because structure can be weakly predictive.
  Evaluated by Accuracy.'
detailed_description:
  task: Slovak social network Pokec node classification (binary gender, 1.6M nodes).
    The primary catalog metric is Accuracy.
  data: Slovak social network Pokec node classification (binary gender, 1.6M nodes).
    The cataloged artifact reports 1 graphs, 2 target classes or tasks.
  features: Each release supplies a sparse node-feature matrix, graph edges, and node
    labels. Feature meaning varies by source; structure and features are deliberately
    evaluated without assuming neighboring labels agree.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses Accuracy (higher is better). Exact masks or folds must
    come from the cited release.'
  quirks_and_pitfalls: These are transductive single-graph tasks with fixed random
    splits. Label homophily is low and class balance varies; feature-only and structure-only
    baselines are essential, and similarly named OGB/source datasets may use different
    labels or splits.
sources:
- title: LINKX Benchmarks benchmark
  arxiv_id: '2110.14446'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric Pokec loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.LINKXDataset.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.LINKXDataset.html
stats:
  num_graphs: 1
  avg_nodes: 662143.0
  avg_edges: 13806079.0
  num_classes: 2
result_count: 67
best_model:
  model: MoE-H2GCN
  value: 0.8302
  metric: Accuracy
  arxiv_id: '2311.05185'
  paper_title: Mixture of Weak & Strong Experts on Graphs
papers:
- arxiv_id: '2604.27387'
  title: 'Robust Learning on Heterogeneous Graphs with Heterophily: A Graph Structure
    Learning Approach'
  date_iso: '2026-04-30'
  venue: ''
- arxiv_id: '2504.13266'
  title: 'Graph Learning at Scale: Characterizing and Optimizing Pre-Propagation GNNs'
  date_iso: '2025-04-17'
  venue: ''
- arxiv_id: '2406.01249'
  title: Equivariant Machine Learning on Graphs with Nonlinear Spectral Filters
  date_iso: '2024-06-03'
  venue: NeurIPS 2024
- arxiv_id: '2311.05185'
  title: Mixture of Weak & Strong Experts on Graphs
  date_iso: '2023-11-09'
  venue: ICLR 2023
- arxiv_id: '2302.12432'
  title: Graph Neural Networks with Learnable and Optimal Polynomial Bases
  date_iso: '2023-02-24'
  venue: ICML 2023
- arxiv_id: '2301.09474'
  title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
  date_iso: '2023-01-23'
  venue: ICLR 2023
- arxiv_id: '2211.14383'
  title: Interpreting Unfairness in Graph Neural Networks via Training Node Attribution
  date_iso: '2022-11-25'
  venue: AAAI 2022
- arxiv_id: '2202.04187'
  title: 'FMP: Toward Fair Graph Message Passing against Topology Bias'
  date_iso: '2022-02-08'
  venue: ''
- arxiv_id: '2202.03580'
  title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
  date_iso: '2022-02-04'
  venue: NeurIPS 2022
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
    avg_nodes: 662143.0
    avg_edges: 13806079.0
    num_classes: 2
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: MoE-H2GCN
    model_plain: MoE-H2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8302
    metric_stds:
    - 0.003
  - model: att-Node-level NLSFs
    model_plain: att-Node-level NLSFs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.01249'
    title: Equivariant Machine Learning on Graphs with Nonlinear Spectral Filters
    date: Jun 3, 2024
    date_iso: '2024-06-03'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8296
    metric_stds:
    - 0.001
  - model: OptBasisGNN
    model_plain: OptBasisGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.12432'
    title: Graph Neural Networks with Learnable and Optimal Polynomial Bases
    date: Feb 24, 2023
    date_iso: '2023-02-24'
    date_display: Feb 2023
    codebase_url: https://github.com/yuziGuo/FarOptBasis
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8283
    metric_stds:
    - 0.0004
  - model: ChebNetII
    model_plain: ChebNetII
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8233
    metric_stds:
    - 0.0028
  - model: LINKX
    model_plain: LINKX
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8204
    metric_stds:
    - 0.0007
  - model: HOGA
    model_plain: HOGA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.13266'
    title: 'Graph Learning at Scale: Characterizing and Optimizing Pre-Propagation
      GNNs'
    date: Apr 17, 2025
    date_iso: '2025-04-17'
    date_display: Apr 2025
    codebase_url: https://github.com/cornell-zhang/preprop-gnn
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
    - null
  - model: BernNet
    model_plain: BernNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.0921
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8167
    metric_stds:
    - 0.0017
  - model: MixHop
    model_plain: MixHop
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.12432'
    title: Graph Neural Networks with Learnable and Optimal Polynomial Bases
    date: Feb 24, 2023
    date_iso: '2023-02-24'
    date_display: Feb 2023
    codebase_url: https://github.com/yuziGuo/FarOptBasis
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8107
    metric_stds:
    - 0.0016
  - model: SIGN
    model_plain: SIGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.13266'
    title: 'Graph Learning at Scale: Characterizing and Optimizing Pre-Propagation
      GNNs'
    date: Apr 17, 2025
    date_iso: '2025-04-17'
    date_display: Apr 2025
    codebase_url: https://github.com/cornell-zhang/preprop-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8101
    metric_stds:
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
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8089
    metric_stds:
    - 0.0016
  - model: GPR-GNN
    model_plain: GPR-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.0921
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8074
    metric_stds:
    - 0.0022
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.01249'
    title: Equivariant Machine Learning on Graphs with Nonlinear Spectral Filters
    date: Jun 3, 2024
    date_iso: '2024-06-03'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8074
    metric_stds:
    - 0.002
  - model: LINK
    model_plain: LINK
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8054
    metric_stds:
    - 0.0003
  - model: MoE-GIN-skip
    model_plain: MoE-GIN-skip
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.797
    metric_stds:
    - 0.0023
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7894
    metric_stds:
    - 0.0011
  - model: GPR-GNN
    model_plain: GPR-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7883
    metric_stds:
    - 0.0005
  - model: MoE-SAGE
    model_plain: MoE-SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7784
    metric_stds:
    - 0.0004
  - model: MoE-GCN
    model_plain: MoE-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7728
    metric_stds:
    - 0.0008
  - model: GraphMoE-GCN
    model_plain: GraphMoE-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7699
    metric_stds:
    - 0.001
  - model: GraphMoE-SAGE
    model_plain: GraphMoE-SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7667
    metric_stds:
    - 0.0008
  - model: GIN-skip
    model_plain: GIN-skip
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7629
    metric_stds:
    - 0.0051
  - model: MoE-GIN
    model_plain: MoE-GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7611
    metric_stds:
    - 0.0039
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7576
    metric_stds:
    - 0.0004
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.0921
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7545
    metric_stds:
    - 0.0017
  - model: GCN-skip
    model_plain: GCN-skip
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7346
    metric_stds:
    - 0.0004
  - model: ChebNet
    model_plain: ChebNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7271
    metric_stds:
    - 0.0066
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04187'
    title: 'FMP: Toward Fair Graph Message Passing against Topology Bias'
    date: Feb 8, 2022
    date_iso: '2022-02-08'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7178
    metric_stds:
    - 0.0037
  - model: SGC
    model_plain: SGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04187'
    title: 'FMP: Toward Fair Graph Message Passing against Topology Bias'
    date: Feb 8, 2022
    date_iso: '2022-02-08'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7124
    metric_stds:
    - 0.0046
  - model: FMP
    model_plain: FMP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04187'
    title: 'FMP: Toward Fair Graph Message Passing against Topology Bias'
    date: Feb 8, 2022
    date_iso: '2022-02-08'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.705
    metric_stds:
    - 0.005
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2202.04187'
    title: 'FMP: Toward Fair Graph Message Passing against Topology Bias'
    date: Feb 8, 2022
    date_iso: '2022-02-08'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7048
    metric_stds:
    - 0.0077
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04187'
    title: 'FMP: Toward Fair Graph Message Passing against Topology Bias'
    date: Feb 8, 2022
    date_iso: '2022-02-08'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6976
    metric_stds:
    - 0.013
  - model: DIFFormer-s
    model_plain: DIFFormer-s
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2301.09474'
    title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    date: Jan 23, 2023
    date_iso: '2023-01-23'
    date_display: Jan 2023
    codebase_url: https://github.com/qitianwu/DIFFormer
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6924
    metric_stds:
    - 0.0076
  - model: NodeFormer
    model_plain: NodeFormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2301.09474'
    title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    date: Jan 23, 2023
    date_iso: '2023-01-23'
    date_display: Jan 2023
    codebase_url: https://github.com/qitianwu/DIFFormer
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6832
    metric_stds:
    - 0.0045
  - model: APPNP
    model_plain: APPNP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.04187'
    title: 'FMP: Toward Fair Graph Message Passing against Topology Bias'
    date: Feb 8, 2022
    date_iso: '2022-02-08'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6691
    metric_stds:
    - 0.0146
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2301.09474'
    title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    date: Jan 23, 2023
    date_iso: '2023-01-23'
    date_display: Jan 2023
    codebase_url: https://github.com/qitianwu/DIFFormer
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6557
    metric_stds:
    - 0.0034
  - model: NIFTY
    model_plain: NIFTY
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.14383'
    title: Interpreting Unfairness in Graph Neural Networks via Training Node Attribution
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/yushundong/BIND
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.653
    metric_stds:
    - 0.002
  - model: FairGNN
    model_plain: FairGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.14383'
    title: Interpreting Unfairness in Graph Neural Networks via Training Node Attribution
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/yushundong/BIND
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.64
    metric_stds:
    - 0.007
  - model: BIND 1%
    model_plain: BIND 1%
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.14383'
    title: Interpreting Unfairness in Graph Neural Networks via Training Node Attribution
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/yushundong/BIND
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.635
    metric_stds:
    - 0.004
  - model: Van. GCN
    model_plain: Van. GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.14383'
    title: Interpreting Unfairness in Graph Neural Networks via Training Node Attribution
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/yushundong/BIND
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.632
    metric_stds:
    - 0.007
  - model: BIND 10%
    model_plain: BIND 10%
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.14383'
    title: Interpreting Unfairness in Graph Neural Networks via Training Node Attribution
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/yushundong/BIND
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.629
    metric_stds:
    - 0.004
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6237
    metric_stds:
    - 0.0002
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2301.09474'
    title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    date: Jan 23, 2023
    date_iso: '2023-01-23'
    date_display: Jan 2023
    codebase_url: https://github.com/qitianwu/DIFFormer
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6231
    metric_stds:
    - 0.0113
  - model: EDITS
    model_plain: EDITS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.14383'
    title: Interpreting Unfairness in Graph Neural Networks via Training Node Attribution
    date: Nov 25, 2022
    date_iso: '2022-11-25'
    date_display: Nov 2022
    codebase_url: https://github.com/yushundong/BIND
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.616
    metric_stds:
    - 0.009
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2301.09474'
    title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    date: Jan 23, 2023
    date_iso: '2023-01-23'
    date_display: Jan 2023
    codebase_url: https://github.com/qitianwu/DIFFormer
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6015
    metric_stds:
    - 0.0003
  - model: AdaGCN
    model_plain: AdaGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5592
    metric_stds:
    - 0.0035
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_iso: '2023-11-09'
    date_display: Nov 2023
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5337
    metric_stds:
    - 0.0215
  - model: LP
    model_plain: LP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2301.09474'
    title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    date: Jan 23, 2023
    date_iso: '2023-01-23'
    date_display: Jan 2023
    codebase_url: https://github.com/qitianwu/DIFFormer
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5273
    metric_stds:
    - null
  - model: SGC
    model_plain: SGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2301.09474'
    title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
    date: Jan 23, 2023
    date_iso: '2023-01-23'
    date_display: Jan 2023
    codebase_url: https://github.com/qitianwu/DIFFormer
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5203
    metric_stds:
    - 0.0084
  - model: HGUL
    model_plain: HGUL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.27387'
    title: 'Robust Learning on Heterogeneous Graphs with Heterophily: A Graph Structure
      Learning Approach'
    date: Apr 30, 2026
    date_iso: '2026-04-30'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3305
    metric_stds:
    - 0.0057
  - model: Simple-HGN
    model_plain: Simple-HGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.27387'
    title: 'Robust Learning on Heterogeneous Graphs with Heterophily: A Graph Structure
      Learning Approach'
    date: Apr 30, 2026
    date_iso: '2026-04-30'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3166
    metric_stds:
    - 0.0086
  row_count: 67
  rows_json: /data/datasets/pokec/standard-split-rows.json
  chart_json: /data/datasets/pokec/standard-split-chart.json
  arch_counts:
    gnn: 46
    hybrid: 13
    graph_transformer: 4
    llm: 0
    walk: 0
    traditional: 4
  metric_counts:
  - 67
  milestones: &id001
  - value: 0.8233
    std: 0.0028
    model: ChebNetII
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: '2022-02-04'
  - value: 0.8283
    std: 0.0004
    model: OptBasisGNN
    arxiv_id: '2302.12432'
    title: Graph Neural Networks with Learnable and Optimal Polynomial Bases
    date: '2023-02-24'
  - value: 0.8302
    std: 0.003
    model: MoE-H2GCN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: '2023-11-09'
  milestones_by_metric:
    Accuracy: *id001
---

