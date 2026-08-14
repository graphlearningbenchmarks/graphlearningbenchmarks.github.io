---
title: twitch-gamers
slug: twitch-gamers
benchmark: LINKX Benchmarks
task_type: node_classification
short_description: Twitch streamer network binary node classification (streaming language).
description: '**Binary node classification** Twitch streamer network binary node classification
  (streaming language). Uses the released sparse node features and a low-homophily
  graph. Feature-only baselines are essential because structure can be weakly predictive.
  Evaluated by Accuracy.'
detailed_description:
  task: Twitch streamer network binary node classification (streaming language). The
    primary catalog metric is Accuracy.
  data: Twitch streamer network binary node classification (streaming language). The
    cataloged artifact reports 1 graphs, 2 target classes or tasks.
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
- title: PyTorch Geometric twitch-gamers loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.LINKXDataset.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.LINKXDataset.html
stats:
  num_graphs: 1
  avg_nodes: 168114.0
  avg_edges: 6797557.0
  num_classes: 2
  extra_stats:
    adjusted_homophily: 0.09
    edge_feature_dim: 0
    edge_feature_type: unweighted mutual-follower links
    edge_homophily: 0.545
    feature_type: streaming-language indicator and Twitch user metadata
    heterophily: 0.455
    node_feature_dim: 7
    statistic_notes: LINKX Table 5 and the Twitch Gamers source report 168,114 nodes
      and 6,797,557 edges.
result_count: 62
best_model:
  model: GloGNN
  value: 0.6634
  metric: Accuracy
  arxiv_id: '2405.20724'
  paper_title: on Large Graphs using Intersecting Communities
papers:
- arxiv_id: '2408.07191'
  title: Joint Graph Rewiring and Feature Denoising via Spectral Resonance
  date_iso: '2024-08-13'
  venue: ICLR 2024
- arxiv_id: '2406.01249'
  title: Equivariant Machine Learning on Graphs with Nonlinear Spectral Filters
  date_iso: '2024-06-03'
  venue: NeurIPS 2024
- arxiv_id: '2405.20724'
  title: on Large Graphs using Intersecting Communities
  date_iso: '2024-05-31'
  venue: NeurIPS 2024
- arxiv_id: '2402.15270'
  title: Smoothed Graph Contrastive Learning via Seamless Proximity Integration
  date_iso: '2024-02-23'
  venue: ''
- arxiv_id: '2311.05185'
  title: Mixture of Weak & Strong Experts on Graphs
  date_iso: '2023-11-09'
  venue: ICLR 2023
- arxiv_id: '2302.12432'
  title: Graph Neural Networks with Learnable and Optimal Polynomial Bases
  date_iso: '2023-02-24'
  venue: ICML 2023
- arxiv_id: '2212.02483'
  title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
  date_iso: '2022-12-05'
  venue: ICML 2022
- arxiv_id: '2206.14337'
  title: Deformable Graph Transformer
  date_iso: '2022-06-29'
  venue: ''
- arxiv_id: '2204.04874'
  title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
  date_iso: '2022-04-11'
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
    avg_nodes: 168114.0
    avg_edges: 6797557.0
    num_classes: 2
    extra_stats:
      adjusted_homophily: 0.09
      edge_feature_dim: 0
      edge_feature_type: unweighted mutual-follower links
      edge_homophily: 0.545
      feature_type: streaming-language indicator and Twitch user metadata
      heterophily: 0.455
      node_feature_dim: 7
      statistic_notes: LINKX Table 5 and the Twitch Gamers source report 168,114 nodes
        and 6,797,557 edges.
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GloGNN
    model_plain: GloGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.20724'
    title: on Large Graphs using Intersecting Communities
    date: May 31, 2024
    date_iso: '2024-05-31'
    date_display: May 2024
    codebase_url: https://github.com/benfinkelshtein/ICGNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.6634
    metric_stds:
    - 0.0029
  - model: DGT
    model_plain: DGT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.6609
    metric_stds:
    - 0.0022
  - model: ICG_u-NN
    model_plain: ICG_u-NN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.20724'
    title: on Large Graphs using Intersecting Communities
    date: May 31, 2024
    date_iso: '2024-05-31'
    date_display: May 2024
    codebase_url: https://github.com/benfinkelshtein/ICGNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.6608
    metric_stds:
    - 0.0074
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.6606
    metric_stds:
    - 0.0019
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
    - 0.6603
    metric_stds:
    - 0.0016
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
    - 0.6597
    metric_stds:
    - 0.002
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
    - 0.657
    metric_stds:
    - 0.002
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
    - 0.6564
    metric_stds:
    - 0.0027
  - model: DGT-light
    model_plain: DGT-light
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6559
    metric_stds:
    - 0.0025
  - model: ICG-NN
    model_plain: ICG-NN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.20724'
    title: on Large Graphs using Intersecting Communities
    date: May 31, 2024
    date_iso: '2024-05-31'
    date_display: May 2024
    codebase_url: https://github.com/benfinkelshtein/ICGNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.6527
    metric_stds:
    - 0.0082
  - model: MixHop
    model_plain: MixHop
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.652
    metric_stds:
    - 0.0012
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6517
    metric_stds:
    - 0.0016
  - model: GCN+JDR
    model_plain: GCN+JDR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2408.07191'
    title: Joint Graph Rewiring and Feature Denoising via Spectral Resonance
    date: Aug 13, 2024
    date_iso: '2024-08-13'
    date_display: Aug 2024
    codebase_url: https://github.com/jlinki/JDR
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6514
    metric_stds:
    - 0.0019
  - model: JKNet
    model_plain: JKNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6508
    metric_stds:
    - 0.0007
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
    - 0.6503
    metric_stds:
    - 0.0027
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
    - 0.6491
    metric_stds:
    - 0.0022
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
    - 0.6485
    metric_stds:
    - 0.0021
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6473
    metric_stds:
    - 0.0011
  - model: GCN + FoSR
    model_plain: GCN + FoSR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2408.07191'
    title: Joint Graph Rewiring and Feature Denoising via Spectral Resonance
    date: Aug 13, 2024
    date_iso: '2024-08-13'
    date_display: Aug 2024
    codebase_url: https://github.com/jlinki/JDR
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6465
    metric_stds:
    - 0.0015
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
    - 0.6438
    metric_stds:
    - 0.0014
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6434
    metric_stds:
    - 0.0012
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
    - 0.6432
    metric_stds:
    - 0.0034
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
    - 0.6427
    metric_stds:
    - 0.0031
  - model: FavardGNN
    model_plain: FavardGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.6426
    metric_stds:
    - 0.0012
  - model: GATv2
    model_plain: GATv2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6415
    metric_stds:
    - 0.0009
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
    - 0.6374
    metric_stds:
    - 0.0023
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
    - 0.6342
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
    - 0.6339
    metric_stds:
    - 0.0061
  - model: GT-sparse
    model_plain: GT-sparse
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6309
    metric_stds:
    - 0.0071
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.629
    metric_stds:
    - 0.0022
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
    - 0.6276
    metric_stds:
    - 0.0022
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2204.04874'
    title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
    date: Apr 11, 2022
    date_iso: '2022-04-11'
    date_display: Apr 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6274
    metric_stds:
    - 0.0003
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
    - 0.6259
    metric_stds:
    - 0.0038
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
    - 0.6259
    metric_stds:
    - 0.004
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
    - 0.6231
    metric_stds:
    - 0.0037
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
    - 0.6218
    metric_stds:
    - 0.0026
  - model: AF-GCL
    model_plain: AF-GCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2204.04874'
    title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
    date: Apr 11, 2022
    date_iso: '2022-04-11'
    date_display: Apr 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6204
    metric_stds:
    - 0.0017
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
    - 0.6199
    metric_stds:
    - 0.003
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
    - 0.6189
    metric_stds:
    - 0.0029
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
    - 0.6176
    metric_stds:
    - 0.006
  - model: DeepWalk
    model_plain: DeepWalk
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2204.04874'
    title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
    date: Apr 11, 2022
    date_iso: '2022-04-11'
    date_display: Apr 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6171
    metric_stds:
    - 0.0041
  - model: GCN + DIGL
    model_plain: GCN + DIGL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2408.07191'
    title: Joint Graph Rewiring and Feature Denoising via Spectral Resonance
    date: Aug 13, 2024
    date_iso: '2024-08-13'
    date_display: Aug 2024
    codebase_url: https://github.com/jlinki/JDR
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6164
    metric_stds:
    - 0.0014
  - model: DGI
    model_plain: DGI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2204.04874'
    title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
    date: Apr 11, 2022
    date_iso: '2022-04-11'
    date_display: Apr 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6147
    metric_stds:
    - 0.0056
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_iso: '2022-06-29'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6114
    metric_stds:
    - 0.0006
  - model: Node2cec
    model_plain: Node2cec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2204.04874'
    title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
    date: Apr 11, 2022
    date_iso: '2022-04-11'
    date_display: Apr 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6112
    metric_stds:
    - 0.0029
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
    - 0.6105
    metric_stds:
    - 0.0023
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
    - 0.6102
    metric_stds:
    - 0.0014
  - model: BGRL
    model_plain: BGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2204.04874'
    title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
    date: Apr 11, 2022
    date_iso: '2022-04-11'
    date_display: Apr 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6093
    metric_stds:
    - 0.0032
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
    - 0.6092
    metric_stds:
    - 0.0007
  - model: TIDE-m
    model_plain: TIDE-m
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.02483'
    title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
    date: Dec 5, 2022
    date_iso: '2022-12-05'
    date_display: Dec 2022
    codebase_url: https://github.com/maysambehmanesh/TIDE
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6081
    metric_stds:
    - 0.0004
  row_count: 62
  rows_json: /data/datasets/twitch-gamers/standard-split-rows.json
  chart_json: /data/datasets/twitch-gamers/standard-split-chart.json
  arch_counts:
    gnn: 42
    hybrid: 15
    graph_transformer: 1
    llm: 0
    walk: 2
    traditional: 2
  metric_counts:
  - 62
  milestones: &id001
  - value: 0.6606
    std: 0.0019
    model: LINKX
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: '2022-02-04'
  - value: 0.6609
    std: 0.0022
    model: DGT
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: '2022-06-29'
  - value: 0.6634
    std: 0.0029
    model: GloGNN
    arxiv_id: '2405.20724'
    title: on Large Graphs using Intersecting Communities
    date: '2024-05-31'
  milestones_by_metric:
    Accuracy: *id001
---

