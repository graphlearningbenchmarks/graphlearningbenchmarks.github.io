---
title: Peptides-func
slug: peptides-func
benchmark: LRGB
task_type: graph_classification
description: Multi-label graph classification on peptide molecules (10 classes).
primary_metric: AP
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.LRGBDataset.html
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 10
result_count: 197
best_model:
  model: LightGBM
  value: 0.746
  metric: AP
  arxiv_id: '2501.17901'
  paper_title: Molecular fingerprints are strong models for peptide function prediction
papers:
- arxiv_id: '2606.00757'
  title: 'RADE: Random Add-Drop Edge as a Regularizer'
  date_iso: '2026-05-30'
  venue: ICML 2026
- arxiv_id: '2605.12358'
  title: From Message-Passing to Linearized Graph Sequence Models
  date_iso: '2026-05-12'
  venue: ''
- arxiv_id: '2604.24293'
  title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
    via Continuous Phase Transitions'
  date_iso: '2026-04-27'
  venue: ''
- arxiv_id: '2601.18917'
  title: 'GraIP: A Benchmarking Framework For Neural Graph Inverse Problems'
  date_iso: '2026-01-26'
  venue: ''
- arxiv_id: '2510.08450'
  title: 'gLSTM: Mitigating Over-Squashing by Increasing Storage Capacity'
  date_iso: '2025-10-09'
  venue: ''
- arxiv_id: '2509.06743'
  title: Long-Range Graph Wavelet Networks
  date_iso: '2025-09-08'
  venue: NeurIPS 2025
- arxiv_id: '2506.01231'
  title: Towards Efficient Few-shot Graph Neural Architecture Search via Partitioning
    Gradient Contribution
  date_iso: '2025-06-02'
  venue: KDD 2025
- arxiv_id: '2502.10818'
  title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
    Recurrent and Graph Learning'
  date_iso: '2025-02-15'
  venue: ''
- arxiv_id: '2501.17901'
  title: Molecular fingerprints are strong models for peptide function prediction
  date_iso: '2025-01-29'
  venue: ''
- arxiv_id: '2412.15589'
  title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
    Graph Information Bottleneck
  date_iso: '2024-12-20'
  venue: AAAI 2024
- arxiv_id: '2411.12732'
  title: Benchmarking Positional Encodings for GNNs and Graph Transformers
  date_iso: '2024-11-19'
  venue: KDD 2024
- arxiv_id: '2408.07654'
  title: 'Graph Triple Attention Network: A Decoupled Perspective'
  date_iso: '2024-08-14'
  venue: ''
- arxiv_id: '2407.12136'
  title: Molecular Topological Profile (MOLTOP) - Simple and Strong Baseline for Molecular
    Graph Classification
  date_iso: '2024-07-16'
  venue: ''
- arxiv_id: '2407.04236'
  title: Graph Pooling via Ricci Flow
  date_iso: '2024-07-05'
  venue: TMLR 2024
- arxiv_id: '2407.01214'
  title: Revisiting Random Walks for Learning on Graphs
  date_iso: '2024-07-01'
  venue: ICLR 2024
- arxiv_id: '2406.12059'
  title: A Scalable and Effective Alternative to Graph Transformers
  date_iso: '2024-06-17'
  venue: AAAI 2024
- arxiv_id: '2406.09291'
  title: A Flexible, Equivariant Framework for Subgraph GNNs via Graph Products and
    Graph Coarsening
  date_iso: '2024-06-13'
  venue: NeurIPS 2024
- arxiv_id: '2405.11951'
  title: 'Distinguished In Uniform: Self Attention Vs. Virtual Nodes'
  date_iso: '2024-05-20'
  venue: ICLR 2024
- arxiv_id: '2404.09774'
  title: 'RandAlign: A Parameter-Free Method for Regularizing Graph Convolutional
    Networks'
  date_iso: '2024-04-15'
  venue: ''
- arxiv_id: '2403.13749'
  title: 'Weisfeiler and Leman Go Loopy: A New Hierarchy for Graph Representational
    Learning'
  date_iso: '2024-03-20'
  venue: NeurIPS 2024
- arxiv_id: '2310.07430'
  title: Non-backtracking Graph Neural Networks
  date_iso: '2023-10-11'
  venue: TMLR 2023
- arxiv_id: '2310.01668'
  title: Locality-Aware Graph Rewiring in GNNs
  date_iso: '2023-10-02'
  venue: ICLR 2023
- arxiv_id: '2309.09384'
  title: Mitigating Over-Smoothing and Over-Squashing using Augmentations of Forman-Ricci
    Curvature
  date_iso: '2023-09-17'
  venue: ''
- arxiv_id: '2306.03561'
  title: 'CIN++: Enhancing Topological Message Passing'
  date_iso: '2023-06-06'
  venue: ''
- arxiv_id: '2302.08647'
  title: Multiresolution Graph Transformers and Wavelet Positional Encoding for Learning
    Hierarchical Structures
  date_iso: '2023-02-17'
  venue: ''
- arxiv_id: '2211.15779'
  title: Revisiting Over-smoothing and Over-squashing using Ollivier's Ricci Curvature
  date_iso: '2022-11-28'
  venue: ICML 2022
- arxiv_id: '2206.08164'
  title: LRGB
  date_iso: '2022-06-16'
  venue: NeurIPS 2022
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: AP
  default_metric: AP
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: 10
  metrics:
  - AP
  - Accuracy
  metric_display_names:
  - AP
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: LightGBM
    model_plain: LightGBM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    arxiv_id: '2501.17901'
    title: Molecular fingerprints are strong models for peptide function prediction
    date: Jan 29, 2025
    date_iso: '2025-01-29'
    date_display: Jan 2025
    codebase_url: https://github.com/MLCIL/peptides_molecular_fingerprints_classification
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.746
    - null
    metric_stds:
    - null
    - null
  - model: ECFP
    model_plain: ECFP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2501.17901'
    title: Molecular fingerprints are strong models for peptide function prediction
    date: Jan 29, 2025
    date_iso: '2025-01-29'
    date_display: Jan 2025
    codebase_url: https://github.com/MLCIL/peptides_molecular_fingerprints_classification
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.746
    - null
    metric_stds:
    - null
    - null
  - model: TT
    model_plain: TT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2501.17901'
    title: Molecular fingerprints are strong models for peptide function prediction
    date: Jan 29, 2025
    date_iso: '2025-01-29'
    date_display: Jan 2025
    codebase_url: https://github.com/MLCIL/peptides_molecular_fingerprints_classification
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7318
    - null
    metric_stds:
    - null
    - null
  - model: RDKit
    model_plain: RDKit
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2501.17901'
    title: Molecular fingerprints are strong models for peptide function prediction
    date: Jan 29, 2025
    date_iso: '2025-01-29'
    date_display: Jan 2025
    codebase_url: https://github.com/MLCIL/peptides_molecular_fingerprints_classification
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7311
    - null
    metric_stds:
    - null
    - null
  - model: S^2GCN
    model_plain: S^2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7311
    - null
    metric_stds:
    - 0.0066
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
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7261
    - null
    metric_stds:
    - 0.0011
    - null
  - model: MPNNs
    model_plain: MPNNs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.08450'
    title: 'gLSTM: Mitigating Over-Squashing by Increasing Storage Capacity'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
    date_display: Oct 2025
    codebase_url: https://github.com/HughBlayney/gLSTM
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.725
    - null
    metric_stds:
    - 0.0023
    - null
  - model: DRAGON
    model_plain: DRAGON
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.24293'
    title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
      via Continuous Phase Transitions'
    date: Apr 27, 2026
    date_iso: '2026-04-27'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.724
    - null
    metric_stds:
    - 0.045
    - null
  - model: LR-GWN
    model_plain: LR-GWN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2509.06743'
    title: Long-Range Graph Wavelet Networks
    date: Sep 8, 2025
    date_iso: '2025-09-08'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7216
    - null
    metric_stds:
    - 0.0041
    - null
  - model: kGCN-SSM
    model_plain: kGCN-SSM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7212
    - null
    metric_stds:
    - 0.0027
    - null
  - model: NBA-GCN+LapPE
    model_plain: NBA-GCN+LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_iso: '2023-10-11'
    date_display: Oct 2023
    codebase_url: https://github.com/seonghyun26/nba-gnn
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7207
    - null
    metric_stds:
    - 0.0028
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
    arxiv_id: '2604.24293'
    title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
      via Continuous Phase Transitions'
    date: Apr 27, 2026
    date_iso: '2026-04-27'
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
    - 0.716
    - null
    metric_stds:
    - 0.005
    - null
  - model: DRew-GCN+LapPE
    model_plain: DRew-GCN+LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_iso: '2023-10-11'
    date_display: Oct 2023
    codebase_url: https://github.com/seonghyun26/nba-gnn
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.715
    - null
    metric_stds:
    - 0.0044
    - null
  - model: DRew
    model_plain: DRew
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.715
    - null
    metric_stds:
    - 0.0044
    - null
  - model: Random Forest
    model_plain: Random Forest
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    arxiv_id: '2501.17901'
    title: Molecular fingerprints are strong models for peptide function prediction
    date: Jan 29, 2025
    date_iso: '2025-01-29'
    date_display: Jan 2025
    codebase_url: https://github.com/MLCIL/peptides_molecular_fingerprints_classification
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7148
    - null
    metric_stds:
    - 0.0013
    - null
  - model: HGODE
    model_plain: HGODE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.24293'
    title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
      via Continuous Phase Transitions'
    date: Apr 27, 2026
    date_iso: '2026-04-27'
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
    - 0.714
    - null
    metric_stds:
    - 0.022
    - null
  - model: DRew-GIN+LapPE
    model_plain: DRew-GIN+LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_iso: '2023-10-11'
    date_display: Oct 2023
    codebase_url: https://github.com/seonghyun26/nba-gnn
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7126
    - null
    metric_stds:
    - 0.0045
    - null
  - model: RWNN-DeBERTa
    model_plain: RWNN-DeBERTa
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_iso: '2024-07-01'
    date_display: Jul 2024
    codebase_url: https://github.com/jw9730/random-walk
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7123
    - null
    metric_stds:
    - 0.0016
    - null
  - model: BuNN
    model_plain: BuNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.24293'
    title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
      via Continuous Phase Transitions'
    date: Apr 27, 2026
    date_iso: '2026-04-27'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: true
    metric_values:
    - 0.712
    - null
    metric_stds:
    - 0.067
    - null
  - model: GREAD-Exp
    model_plain: GREAD-Exp
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.24293'
    title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
      via Continuous Phase Transitions'
    date: Apr 27, 2026
    date_iso: '2026-04-27'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.711
    - null
    metric_stds:
    - 0.04
    - null
  - model: NeuralWalker
    model_plain: NeuralWalker
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7096
    - null
    metric_stds:
    - 0.0078
    - null
  - model: GRED
    model_plain: GRED
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7085
    - null
    metric_stds:
    - 0.0027
    - null
  - model: CRaWl
    model_plain: CRaWl
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_iso: '2024-07-01'
    date_display: Jul 2024
    codebase_url: https://github.com/jw9730/random-walk
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7074
    - null
    metric_stds:
    - null
    - null
  - model: GMN
    model_plain: GMN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7071
    - null
    metric_stds:
    - 0.0083
    - null
  - model: NBA-GIN+LapPE
    model_plain: NBA-GIN+LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_iso: '2023-10-11'
    date_display: Oct 2023
    codebase_url: https://github.com/seonghyun26/nba-gnn
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7071
    - null
    metric_stds:
    - 0.0067
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
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7059
    - null
    metric_stds:
    - 0.0089
    - null
  - model: GRAMA_GatedGCN
    model_plain: GRAMA_GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7049
    - null
    metric_stds:
    - 0.0051
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
    arxiv_id: '2604.24293'
    title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
      via Continuous Phase Transitions'
    date: Apr 27, 2026
    date_iso: '2026-04-27'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.704
    - null
    metric_stds:
    - 0.046
    - null
  - model: DeGTA
    model_plain: DeGTA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    - 0.7023
    - null
    metric_stds:
    - 0.0101
    - null
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7006
    - null
    metric_stds:
    - 0.0033
    - null
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.24293'
    title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
      via Continuous Phase Transitions'
    date: Apr 27, 2026
    date_iso: '2026-04-27'
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
    - 0.699
    - null
    metric_stds:
    - 0.003
    - null
  - model: GRIT
    model_plain: GRIT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.6988
    - null
    metric_stds:
    - 0.0082
    - null
  - model: NBA-GatedGCN+LapPE
    model_plain: NBA-GatedGCN+LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_iso: '2023-10-11'
    date_display: Oct 2023
    codebase_url: https://github.com/seonghyun26/nba-gnn
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6982
    - null
    metric_stds:
    - 0.0014
    - null
  - model: FROND
    model_plain: FROND
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.24293'
    title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
      via Continuous Phase Transitions'
    date: Apr 27, 2026
    date_iso: '2026-04-27'
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
    - 0.698
    - null
    metric_stds:
    - 0.034
    - null
  - model: DRew-GatedGCN+LapPE
    model_plain: DRew-GatedGCN+LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_iso: '2023-10-11'
    date_display: Oct 2023
    codebase_url: https://github.com/seonghyun26/nba-gnn
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6977
    - null
    metric_stds:
    - 0.0026
    - null
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
    - 0.6975
    - null
    metric_stds:
    - 0.0025
    - null
  - model: WaveGC
    model_plain: WaveGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.06743'
    title: Long-Range Graph Wavelet Networks
    date: Sep 8, 2025
    date_iso: '2025-09-08'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6973
    - null
    metric_stds:
    - 0.0043
    - null
  - model: Graph MLP-Mixer/ViT
    model_plain: Graph MLP-Mixer/ViT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_iso: '2023-10-11'
    date_display: Oct 2023
    codebase_url: https://github.com/seonghyun26/nba-gnn
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.697
    - null
    metric_stds:
    - 0.008
    - null
  - model: NBA-GIN
    model_plain: NBA-GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_iso: '2023-10-11'
    date_display: Oct 2023
    codebase_url: https://github.com/seonghyun26/nba-gnn
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6961
    - null
    metric_stds:
    - 0.0045
    - null
  - model: NBA-GCN
    model_plain: NBA-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_iso: '2023-10-11'
    date_display: Oct 2023
    codebase_url: https://github.com/seonghyun26/nba-gnn
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6951
    - null
    metric_stds:
    - 0.0024
    - null
  - model: DRew-GIN
    model_plain: DRew-GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_iso: '2026-05-12'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.694
    - null
    metric_stds:
    - 0.0074
    - null
  - model: S-CGIB
    model_plain: S-CGIB
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2412.15589'
    title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
      Graph Information Bottleneck
    date: Dec 20, 2024
    date_iso: '2024-12-20'
    date_display: Dec 2024
    codebase_url: https://github.com/NSLab-CUK/S-CGIB
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.694
    - null
    metric_stds:
    - 0.002
    - null
  - model: Extremely Randomized Trees
    model_plain: Extremely Randomized Trees
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    arxiv_id: '2501.17901'
    title: Molecular fingerprints are strong models for peptide function prediction
    date: Jan 29, 2025
    date_iso: '2025-01-29'
    date_display: Jan 2025
    codebase_url: https://github.com/MLCIL/peptides_molecular_fingerprints_classification
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6938
    - null
    metric_stds:
    - 0.0006
    - null
  - model: kGCN-SSM
    model_plain: kGCN-SSM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.08450'
    title: 'gLSTM: Mitigating Over-Squashing by Increasing Storage Capacity'
    date: Oct 9, 2025
    date_iso: '2025-10-09'
    date_display: Oct 2025
    codebase_url: https://github.com/HughBlayney/gLSTM
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6902
    - null
    metric_stds:
    - 0.0022
    - null
  - model: Graph ViT
    model_plain: Graph ViT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6876
    - null
    metric_stds:
    - 0.0059
    - null
  - model: GRIT+RRWP
    model_plain: GRIT+RRWP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6865
    - null
    metric_stds:
    - 0.005
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
    arxiv_id: '2405.11951'
    title: 'Distinguished In Uniform: Self Attention Vs. Virtual Nodes'
    date: May 20, 2024
    date_iso: '2024-05-20'
    date_display: May 2024
    codebase_url: https://github.com/toenshoff/VN-vs-GT
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.686
    - null
    metric_stds:
    - 0.005
    - null
  - model: MixHop-GCN+LapPE
    model_plain: MixHop-GCN+LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_iso: '2023-10-11'
    date_display: Oct 2023
    codebase_url: https://github.com/seonghyun26/nba-gnn
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6843
    - null
    metric_stds:
    - 0.0049
    - null
  - model: DIGL+MPNN+LapPE
    model_plain: DIGL+MPNN+LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_iso: '2023-10-11'
    date_display: Oct 2023
    codebase_url: https://github.com/seonghyun26/nba-gnn
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.683
    - null
    metric_stds:
    - 0.0026
    - null
  - model: SIMPLE
    model_plain: SIMPLE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.18917'
    title: 'GraIP: A Benchmarking Framework For Neural Graph Inverse Problems'
    date: Jan 26, 2026
    date_iso: '2026-01-26'
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
    - 0.683
    - null
    metric_stds:
    - 0.009
    - null
  row_count: 197
  rows_json: /data/datasets/peptides-func/standard-split-rows.json
  chart_json: /data/datasets/peptides-func/standard-split-chart.json
  arch_counts:
    gnn: 93
    hybrid: 30
    graph_transformer: 39
    llm: 0
    walk: 1
    traditional: 23
  metric_counts:
  - 181
  - 16
  milestones: &id001
  - value: 0.6439
    std: 0.0075
    model: SAN+RWSE
    arxiv_id: '2206.08164'
    title: LRGB
    date: '2022-06-16'
  - value: 0.6817
    std: 0.0064
    model: MGT+WavePE
    arxiv_id: '2302.08647'
    title: Multiresolution Graph Transformers and Wavelet Positional Encoding for
      Learning Hierarchical Structures
    date: '2023-02-17'
  - value: 0.7207
    std: 0.0028
    model: NBA-GCN+LapPE
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: '2023-10-11'
  - value: 0.7311
    std: 0.0066
    model: S^2GCN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: '2024-11-19'
  milestones_by_metric:
    AP: *id001
    Accuracy:
    - value: 0.69
      std: 0.01
      model: ORC
      arxiv_id: '2407.04236'
      title: Graph Pooling via Ricci Flow
      date: '2024-07-05'
---

