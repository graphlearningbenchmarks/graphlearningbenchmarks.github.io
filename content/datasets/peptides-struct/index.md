---
title: Peptides-struct
slug: peptides-struct
benchmark: LRGB
task_type: graph_regression
description: Multi-task graph regression on peptide structural properties (11 targets).
primary_metric: MAE
higher_is_better: false
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.LRGBDataset.html
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 11
result_count: 222
best_model:
  model: Energy GNN + attention
  value: 0.036000000000000004
  metric: MAE
  arxiv_id: '2407.00494'
  paper_title: Graph Neural Networks Gone Hogwild
papers:
- arxiv_id: '2605.12358'
  title: From Message-Passing to Linearized Graph Sequence Models
  date_iso: '2026-05-12'
  venue: ''
- arxiv_id: '2605.04834'
  title: Bridging Input Feature Spaces Towards Graph Foundation Models
  date_iso: '2026-05-06'
  venue: ICLR 2026
- arxiv_id: '2604.17324'
  title: 'SigGate-GT: Taming Over-Smoothing in Graph Transformers via Sigmoid-Gated
    Attention'
  date_iso: '2026-04-19'
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
- arxiv_id: '2507.00647'
  title: Cooperative Sheaf Neural Networks
  date_iso: '2025-07-01'
  venue: ICLR 2025
- arxiv_id: '2502.10818'
  title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
    Recurrent and Graph Learning'
  date_iso: '2025-02-15'
  venue: ''
- arxiv_id: '2502.09263'
  title: Can Classic GNNs Be Strong Baselines for Graph-level Tasks? Simple Architectures
    Meet Excellence
  date_iso: '2025-02-13'
  venue: ICML 2025
- arxiv_id: '2502.09570'
  title: Enhancing the Utility of Higher-Order Information in Relational Learning
  date_iso: '2025-02-13'
  venue: ''
- arxiv_id: '2502.01122'
  title: Learning Efficient Positional Encodings with Graph Neural Networks
  date_iso: '2025-02-03'
  venue: ICLR 2025
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
- arxiv_id: '2410.23686'
  title: Towards Dynamic Message Passing on Graphs
  date_iso: '2024-10-31'
  venue: NeurIPS 2024
- arxiv_id: '2409.19414'
  title: Sequential Signal Mixing Aggregation for Message Passing Graph Neural Networks
  date_iso: '2024-09-28'
  venue: NeurIPS 2024
- arxiv_id: '2408.07654'
  title: 'Graph Triple Attention Network: A Decoupled Perspective'
  date_iso: '2024-08-14'
  venue: ''
- arxiv_id: '2407.12419'
  title: Dirac-Bianconi Graph Neural Networks - Enabling Non-Diffusive Long-Range
    Graph Predictions
  date_iso: '2024-07-17'
  venue: ICML 2024
- arxiv_id: '2407.00494'
  title: Graph Neural Networks Gone Hogwild
  date_iso: '2024-06-29'
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
- arxiv_id: '2405.17311'
  title: Probabilistic Graph Rewiring via Virtual Nodes
  date_iso: '2024-05-27'
  venue: NeurIPS 2024
- arxiv_id: '2405.13526'
  title: 'Understanding Virtual Nodes: Oversquashing and Node Heterogeneity'
  date_iso: '2024-05-22'
  venue: ICLR 2024
- arxiv_id: '2405.11951'
  title: 'Distinguished In Uniform: Self Attention Vs. Virtual Nodes'
  date_iso: '2024-05-20'
  venue: ICLR 2024
- arxiv_id: '2310.07430'
  title: Non-backtracking Graph Neural Networks
  date_iso: '2023-10-11'
  venue: TMLR 2023
- arxiv_id: '2310.01704'
  title: Transformers are efficient hierarchical chemical graph learners
  date_iso: '2023-10-02'
  venue: ''
- arxiv_id: '2310.01668'
  title: Locality-Aware Graph Rewiring in GNNs
  date_iso: '2023-10-02'
  venue: ICLR 2023
- arxiv_id: '2306.03561'
  title: 'CIN++: Enhancing Topological Message Passing'
  date_iso: '2023-06-06'
  venue: ''
- arxiv_id: '2302.08647'
  title: Multiresolution Graph Transformers and Wavelet Positional Encoding for Learning
    Hierarchical Structures
  date_iso: '2023-02-17'
  venue: ''
- arxiv_id: '2212.13350'
  title: A Generalization of ViT/MLP-Mixer to Graphs
  date_iso: '2022-12-27'
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
  primary_metric: MAE
  default_metric: MAE
  higher_is_better: false
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: 11
  metrics:
  - MAE
  metric_display_names:
  - MAE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: Energy GNN + attention
    model_plain: Energy GNN + attention
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.00494'
    title: Graph Neural Networks Gone Hogwild
    date: Jun 29, 2024
    date_iso: '2024-06-29'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: true
    metric_values:
    - 0.036000000000000004
    metric_stds:
    - 0.038
  - model: Energy GNN edge-wise
    model_plain: Energy GNN edge-wise
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.00494'
    title: Graph Neural Networks Gone Hogwild
    date: Jun 29, 2024
    date_iso: '2024-06-29'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: true
    metric_values:
    - 0.04
    metric_stds:
    - 0.036000000000000004
  - model: Energy GNN node-wise
    model_plain: Energy GNN node-wise
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.00494'
    title: Graph Neural Networks Gone Hogwild
    date: Jun 29, 2024
    date_iso: '2024-06-29'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: true
    metric_values:
    - 0.195
    metric_stds:
    - 0.017
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.09263'
    title: Can Classic GNNs Be Strong Baselines for Graph-level Tasks? Simple Architectures
      Meet Excellence
    date: Feb 13, 2025
    date_iso: '2025-02-13'
    date_display: Feb 2025
    codebase_url: https://github.com/LUOyk1999/GNNPlus
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2421
    metric_stds:
    - 0.0016
  - model: IPR-MPNN
    model_plain: IPR-MPNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.17311'
    title: Probabilistic Graph Rewiring via Virtual Nodes
    date: May 27, 2024
    date_iso: '2024-05-27'
    date_display: May 2024
    codebase_url: https://github.com/chendiqian/IPR-MPNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2422
    metric_stds:
    - 0.0007
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
    - 0.2424
    metric_stds:
    - 0.001
  - model: SigGate + DropEdge
    model_plain: SigGate + DropEdge
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.17324'
    title: 'SigGate-GT: Taming Over-Smoothing in Graph Transformers via Sigmoid-Gated
      Attention'
    date: Apr 19, 2026
    date_iso: '2026-04-19'
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
    - 0.2428
    metric_stds:
    - 0.001
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.09263'
    title: Can Classic GNNs Be Strong Baselines for Graph-level Tasks? Simple Architectures
      Meet Excellence
    date: Feb 13, 2025
    date_iso: '2025-02-13'
    date_display: Feb 2025
    codebase_url: https://github.com/LUOyk1999/GNNPlus
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2429
    metric_stds:
    - 0.0019
  - model: SigGate
    model_plain: SigGate
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2604.17324'
    title: 'SigGate-GT: Taming Over-Smoothing in Graph Transformers via Sigmoid-Gated
      Attention'
    date: Apr 19, 2026
    date_iso: '2026-04-19'
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
    - 0.2431
    metric_stds:
    - 0.0012
  - model: AMP
    model_plain: AMP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.17311'
    title: Probabilistic Graph Rewiring via Virtual Nodes
    date: May 27, 2024
    date_iso: '2024-05-27'
    date_display: May 2024
    codebase_url: https://github.com/chendiqian/IPR-MPNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2431
    metric_stds:
    - 0.0004
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.09263'
    title: Can Classic GNNs Be Strong Baselines for Graph-level Tasks? Simple Architectures
      Meet Excellence
    date: Feb 13, 2025
    date_iso: '2025-02-13'
    date_display: Feb 2025
    codebase_url: https://github.com/LUOyk1999/GNNPlus
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2431
    metric_stds:
    - 0.002
  - model: ECFP + LightGBM
    model_plain: ECFP + LightGBM
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
    - 0.2432
    metric_stds:
    - null
  - model: CSNN
    model_plain: CSNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2507.00647'
    title: Cooperative Sheaf Neural Networks
    date: Jul 1, 2025
    date_iso: '2025-07-01'
    date_display: Jul 2025
    codebase_url: ''
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2432
    metric_stds:
    - 0.0004
  - model: ECFP + Extremely Randomized Trees
    model_plain: ECFP + Extremely Randomized Trees
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
    - 0.2433
    metric_stds:
    - 0.0001
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
    - 0.2437
    metric_stds:
    - 0.0014
  - model: TT + LightGBM
    model_plain: TT + LightGBM
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
    - 0.2438
    metric_stds:
    - null
  - model: RDKit + Extremely Randomized Trees
    model_plain: RDKit + Extremely Randomized Trees
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
    - 0.244
    metric_stds:
    - 0.0001
  - model: ECFP + Random Forest
    model_plain: ECFP + Random Forest
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
    - 0.2442
    metric_stds:
    - 0.0002
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
    - 0.2447
    metric_stds:
    - 0.0032
  - model: S2GCN+PE
    model_plain: S2GCN+PE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.17311'
    title: Probabilistic Graph Rewiring via Virtual Nodes
    date: May 27, 2024
    date_iso: '2024-05-27'
    date_display: May 2024
    codebase_url: https://github.com/chendiqian/IPR-MPNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2447
    metric_stds:
    - 0.0007
  - model: G-ViT
    model_plain: G-ViT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2507.00647'
    title: Cooperative Sheaf Neural Networks
    date: Jul 1, 2025
    date_iso: '2025-07-01'
    date_display: Jul 2025
    codebase_url: ''
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.24489999999999998
    metric_stds:
    - 0.0016
  - model: GINE-ViT
    model_plain: GINE-ViT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.13350'
    title: A Generalization of ViT/MLP-Mixer to Graphs
    date: Dec 27, 2022
    date_iso: '2022-12-27'
    date_display: Dec 2022
    codebase_url: https://github.com/XiaoxinHe/Graph-ViT-MLPMixer
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2449
    metric_stds:
    - 0.0016
  - model: Graph ViT
    model_plain: Graph ViT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2405.17311'
    title: Probabilistic Graph Rewiring via Virtual Nodes
    date: May 27, 2024
    date_iso: '2024-05-27'
    date_display: May 2024
    codebase_url: https://github.com/chendiqian/IPR-MPNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2449
    metric_stds:
    - 0.0016
  - model: All-In
    model_plain: All-In
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.04834'
    title: Bridging Input Feature Spaces Towards Graph Foundation Models
    date: May 6, 2026
    date_iso: '2026-05-06'
    date_display: May 2026
    codebase_url: https://github.com/MosheEliasof/ALLIN
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2449
    metric_stds:
    - 0.0012
  - model: Graph ViT/MLP-Mixer
    model_plain: Graph ViT/MLP-Mixer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2502.09263'
    title: Can Classic GNNs Be Strong Baselines for Graph-level Tasks? Simple Architectures
      Meet Excellence
    date: Feb 13, 2025
    date_iso: '2025-02-13'
    date_display: Feb 2025
    codebase_url: https://github.com/LUOyk1999/GNNPlus
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2449
    metric_stds:
    - 0.0016
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
    - 0.2449
    metric_stds:
    - 0.0016
  - model: MGT
    model_plain: MGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2502.09263'
    title: Can Classic GNNs Be Strong Baselines for Graph-level Tasks? Simple Architectures
      Meet Excellence
    date: Feb 13, 2025
    date_iso: '2025-02-13'
    date_display: Feb 2025
    codebase_url: https://github.com/LUOyk1999/GNNPlus
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2453
    metric_stds:
    - 0.0025
  - model: MGT+WavePE
    model_plain: MGT+WavePE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.499
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2302.08647'
    title: Multiresolution Graph Transformers and Wavelet Positional Encoding for
      Learning Hierarchical Structures
    date: Feb 17, 2023
    date_iso: '2023-02-17'
    date_display: Feb 2023
    codebase_url: https://github.com/HySonLab/Multires-Graph-Transformer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2453
    metric_stds:
    - 0.0025
  - model: GPNN
    model_plain: GPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2502.09263'
    title: Can Classic GNNs Be Strong Baselines for Graph-level Tasks? Simple Architectures
      Meet Excellence
    date: Feb 13, 2025
    date_iso: '2025-02-13'
    date_display: Feb 2025
    codebase_url: https://github.com/LUOyk1999/GNNPlus
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2454
    metric_stds:
    - 0.0003
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
    - 0.2454
    metric_stds:
    - 0.001
  - model: GraphTrans-ViT
    model_plain: GraphTrans-ViT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.13350'
    title: A Generalization of ViT/MLP-Mixer to Graphs
    date: Dec 27, 2022
    date_iso: '2022-12-27'
    date_display: Dec 2022
    codebase_url: https://github.com/XiaoxinHe/Graph-ViT-MLPMixer
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2455
    metric_stds:
    - 0.0027
  - model: GRED
    model_plain: GRED
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.09263'
    title: Can Classic GNNs Be Strong Baselines for Graph-level Tasks? Simple Architectures
      Meet Excellence
    date: Feb 13, 2025
    date_iso: '2025-02-13'
    date_display: Feb 2025
    codebase_url: https://github.com/LUOyk1999/GNNPlus
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2455
    metric_stds:
    - 0.0013
  - model: GatedGCN+PE+VN_G
    model_plain: GatedGCN+PE+VN_G
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13526'
    title: 'Understanding Virtual Nodes: Oversquashing and Node Heterogeneity'
    date: May 22, 2024
    date_iso: '2024-05-22'
    date_display: May 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2458
    metric_stds:
    - 0.0006
  - model: RDKit + LightGBM
    model_plain: RDKit + LightGBM
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
    - 0.2459
    metric_stds:
    - null
  - model: RDKit + Random Forest
    model_plain: RDKit + Random Forest
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
    - 0.2459
    metric_stds:
    - 0.0002
  - model: GSSC
    model_plain: GSSC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2502.09263'
    title: Can Classic GNNs Be Strong Baselines for Graph-level Tasks? Simple Architectures
      Meet Excellence
    date: Feb 13, 2025
    date_iso: '2025-02-13'
    date_display: Feb 2025
    codebase_url: https://github.com/LUOyk1999/GNNPlus
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2459
    metric_stds:
    - 0.002
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
    - 0.2459
    metric_stds:
    - 0.002
  - model: GRIT
    model_plain: GRIT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13526'
    title: 'Understanding Virtual Nodes: Oversquashing and Node Heterogeneity'
    date: May 22, 2024
    date_iso: '2024-05-22'
    date_display: May 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.246
    metric_stds:
    - 0.0012
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
    - 0.246
    metric_stds:
    - 0.0007
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
    - 0.2462
    metric_stds:
    - 0.0006
  - model: BuNN
    model_plain: BuNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2507.00647'
    title: Cooperative Sheaf Neural Networks
    date: Jul 1, 2025
    date_iso: '2025-07-01'
    date_display: Jul 2025
    codebase_url: ''
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2463
    metric_stds:
    - 0.0012
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
    - 0.2463
    metric_stds:
    - 0.0005
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
    - 0.2464
    metric_stds:
    - 0.0009
  - model: GatedGCN+PE-ViT
    model_plain: GatedGCN+PE-ViT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.13526'
    title: 'Understanding Virtual Nodes: Oversquashing and Node Heterogeneity'
    date: May 22, 2024
    date_iso: '2024-05-22'
    date_display: May 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2465
    metric_stds:
    - 0.0015
  - model: GatedGCN-ViT
    model_plain: GatedGCN-ViT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.13350'
    title: A Generalization of ViT/MLP-Mixer to Graphs
    date: Dec 27, 2022
    date_iso: '2022-12-27'
    date_display: Dec 2022
    codebase_url: https://github.com/XiaoxinHe/Graph-ViT-MLPMixer
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2465
    metric_stds:
    - 0.0015
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
    - 0.2466
    metric_stds:
    - 0.0012
  - model: TT + Extremely Randomized Trees
    model_plain: TT + Extremely Randomized Trees
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
    - 0.2467
    metric_stds:
    - 0.0003
  - model: S2GCN
    model_plain: S2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.17311'
    title: Probabilistic Graph Rewiring via Virtual Nodes
    date: May 27, 2024
    date_iso: '2024-05-27'
    date_display: May 2024
    codebase_url: https://github.com/chendiqian/IPR-MPNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2467
    metric_stds:
    - 0.0019
  - model: GCN-ViT
    model_plain: GCN-ViT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.13350'
    title: A Generalization of ViT/MLP-Mixer to Graphs
    date: Dec 27, 2022
    date_iso: '2022-12-27'
    date_display: Dec 2022
    codebase_url: https://github.com/XiaoxinHe/Graph-ViT-MLPMixer
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2468
    metric_stds:
    - 0.0015
  - model: R-method
    model_plain: R-method
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2502.01122'
    title: Learning Efficient Positional Encodings with Graph Neural Networks
    date: Feb 3, 2025
    date_iso: '2025-02-03'
    date_display: Feb 2025
    codebase_url: https://github.com/ehejin/Pearl-PE
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.247
    metric_stds:
    - 0.001
  row_count: 222
  rows_json: /data/datasets/peptides-struct/standard-split-rows.json
  chart_json: /data/datasets/peptides-struct/standard-split-chart.json
  arch_counts:
    gnn: 100
    hybrid: 49
    graph_transformer: 44
    llm: 0
    walk: 1
    traditional: 19
  metric_counts:
  - 222
  milestones: &id001
  - value: 0.2529
    std: 0.0016
    model: Transformer+LapPE
    arxiv_id: '2206.08164'
    title: LRGB
    date: '2022-06-16'
  - value: 0.2453
    std: 0.0025
    model: MGT+WavePE
    arxiv_id: '2302.08647'
    title: Multiresolution Graph Transformers and Wavelet Positional Encoding for
      Learning Hierarchical Structures
    date: '2023-02-17'
  - value: 0.2424
    std: 0.001
    model: NBA-GIN+LapPE
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: '2023-10-11'
  - value: 0.2421
    std: 0.0016
    model: GCN
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: '2026-05-12'
  milestones_by_metric:
    MAE: *id001
---

