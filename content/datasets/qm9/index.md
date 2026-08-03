---
title: QM9
slug: qm9
benchmark: Quantum Chemistry
task_type: graph_regression
description: Multi-target quantum property regression on 130k drug-like organic molecules
  (19 targets).
primary_metric: gap
higher_is_better: false
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.QM9.html
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 19
result_count: 132
best_model:
  model: PF-GNN
  value: 0.017
  metric: gap
  arxiv_id: '2401.17752'
  paper_title: 'PF-GNN: Differentiable particle filtering based approximation of universal
    graph representations'
papers:
- arxiv_id: '2510.13615'
  title: 'Message Passing on the Edge: Towards Scalable and Expressive GNNs'
  date_iso: '2025-10-15'
  venue: ''
- arxiv_id: '2505.23086'
  title: Equivariant Spherical Transformer for Efficient Molecular Modeling
  date_iso: '2025-05-29'
  venue: ''
- arxiv_id: '2406.03145'
  title: E(n) Equivariant Message Passing Cellular Networks
  date_iso: '2024-06-05'
  venue: ''
- arxiv_id: '2401.17752'
  title: 'PF-GNN: Differentiable particle filtering based approximation of universal
    graph representations'
  date_iso: '2024-01-31'
  venue: ICLR 2024
- arxiv_id: '2310.19142'
  title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
  date_iso: '2023-10-29'
  venue: NeurIPS 2023
- arxiv_id: '2310.02970'
  title: Fast, Expressive SE$(n)$ Equivariant Networks through Weight-Sharing in Position-Orientation
    Space
  date_iso: '2023-10-04'
  venue: ICLR 2023
- arxiv_id: '2305.04963'
  title: 'From Relational Pooling to Subgraph GNNs: A Universal Framework for More
    Expressive Graph Neural Networks'
  date_iso: '2023-05-08'
  venue: ICML 2023
- arxiv_id: '2304.04757'
  title: A new perspective on building efficient and expressive 3D equivariant graph
    neural networks
  date_iso: '2023-04-07'
  venue: NeurIPS 2023
- arxiv_id: '2303.10576'
  title: An Efficient Subgraph GNN with Provable Substructure Counting Power
  date_iso: '2023-03-19'
  venue: KDD 2023
- arxiv_id: '2210.16518'
  title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
    interactive message passing for molecules'
  date_iso: '2022-10-29'
  venue: ''
- arxiv_id: '2209.15101'
  title: Improving Molecular Pretraining with Complementary Featurizations
  date_iso: '2022-09-29'
  venue: ''
- arxiv_id: '2208.04529'
  title: Motif-based Graph Representation Learning with Application to Chemical Molecules
  date_iso: '2022-08-09'
  venue: ''
- arxiv_id: '2206.11010'
  title: Agent-based Graph Neural Networks
  date_iso: '2022-06-22'
  venue: ICLR 2022
- arxiv_id: '2205.00354'
  title: Graph Anisotropic Diffusion
  date_iso: '2022-04-30'
  venue: ICLR 2022
- arxiv_id: '2111.06283'
  title: 'DropGNN: Random Dropouts Increase the Expressiveness of Graph Neural Networks'
  date_iso: '2021-11-11'
  venue: NeurIPS 2021
- arxiv_id: '2110.04126'
  title: 3D Infomax improves GNNs for Molecular Property Prediction
  date_iso: '2021-10-08'
  venue: ICML 2021
- arxiv_id: '2110.01191'
  title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
  date_iso: '2021-10-04'
  venue: AAAI 2021
- arxiv_id: '2011.14115'
  title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
    Molecules
  date_iso: '2020-11-28'
  venue: NeurIPS 2020
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: gap
  default_metric: gap
  higher_is_better: false
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: 19
  metrics:
  - gap
  - mu
  - alpha
  - U0
  - H
  - G
  - Cv
  - S
  - HOMO
  - LUMO
  - zpve
  - R2
  - U
  metric_display_names:
  - HOMO-LUMO gap
  - Dipole moment
  - Polarizability
  - Internal energy (U₀)
  - Enthalpy (H)
  - Free energy (G)
  - Heat capacity (Cv)
  - Entropy (S)
  - HOMO
  - LUMO
  - Zero point vibrational energy
  - Electronic spatial extent (R²)
  - Internal energy (U)
  show_all_metrics_desktop: true
  chart_default_log_scale: true
  chart_hidden_models:
  - MLP
  rows:
  - model: PF-GNN
    model_plain: PF-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.017
    - 0.017
    - 0.017
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - 0.001
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DimeNet++
    model_plain: DimeNet++
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.019
    - 0.019
    - 0.019
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - 0.001
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Molformer
    model_plain: Molformer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.025
    - 0.028
    - 0.041
    - 7.52
    - 7.38
    - 8.11
    - 0.025
    - null
    - 0.025
    - 0.026
    - 2.05
    - 0.35
    - 7.52
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
    - null
    - null
    - null
    - null
  - model: FGNN
    model_plain: FGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.027
    - 0.027
    - 0.027
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - 0.001
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: δ-2-LGNN
    model_plain: δ-2-LGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.029
    - 0.029
    - 0.029
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - 0.001
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DimeNet++
    model_plain: DimeNet++
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.032
    - 0.028
    - 0.043
    - 6.32
    - 6.53
    - 7.56
    - 0.023
    - null
    - 0.024
    - 0.019
    - 1.21
    - 0.331
    - 6.28
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
    - null
    - null
    - null
    - null
  - model: SphereNet
    model_plain: SphereNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.032
    - 0.026
    - 0.047
    - 6.26
    - 6.4
    - 8.0
    - 0.021
    - null
    - 0.024
    - 0.019
    - 1.12
    - 0.292
    - 6.26
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
    - null
    - null
    - null
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
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.034
    - 0.034
    - 0.034
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - 0.001
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SE(3)-Transformer
    model_plain: SE(3)-Transformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.035
    - 0.051
    - 0.142
    - null
    - null
    - null
    - null
    - null
    - 0.035
    - 0.033
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
    - null
    - null
    - null
    - null
  - model: LEFTNet
    model_plain: LEFTNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.039
    - 0.011
    - 0.039
    - 0.005
    - 5.0
    - 6.0
    - 5.0
    - 5.0
    - 0.024
    - 0.018
    - 1.19
    - null
    - 0.005
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
    - null
    - null
    - null
    - null
  - model: PaiNN
    model_plain: PaiNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.046
    - 0.012
    - 0.045
    - 5.85
    - 5.98
    - 7.35
    - 0.024
    - null
    - 0.028
    - 0.02
    - 1.28
    - 0.066
    - 5.53
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
    - null
    - null
    - null
    - null
  - model: 3-IGN
    model_plain: 3-IGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.046
    - 0.046
    - 0.046
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - 0.001
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: LieTransformer
    model_plain: LieTransformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.052
    - 0.061
    - 0.104
    - 17.0
    - 16.0
    - 27.0
    - 0.041
    - null
    - 0.033
    - 0.029
    - 3.55
    - 2.29
    - 16.0
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
    - null
    - null
    - null
    - null
  - model: MEGNet_full
    model_plain: MEGNet_full
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.061
    - 0.04
    - 0.083
    - 9.0
    - 10.0
    - 10.0
    - 0.03
    - null
    - 0.038
    - 0.031
    - 1.4
    - 0.265
    - 10.0
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
    - null
    - null
    - null
    - null
  - model: 1-2-3-GNN
    model_plain: 1-2-3-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.062
    - 0.062
    - 0.062
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - 0.001
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SchNet
    model_plain: SchNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.063
    - 0.033
    - 0.235
    - 14.0
    - 14.0
    - 14.0
    - 0.033
    - null
    - 0.041
    - 0.034
    - 1.7
    - 0.073
    - 19.0
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
    - null
    - null
    - null
    - null
  - model: MGCN
    model_plain: MGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.064
    - 0.056
    - 0.03
    - 12.9
    - 14.6
    - 16.2
    - 0.038
    - null
    - 0.042
    - 0.057
    - 1.12
    - 0.11
    - 14.4
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
    - null
    - null
    - null
    - null
  - model: 1-2-GNN
    model_plain: 1-2-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.068
    - 0.068
    - 0.068
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - 0.001
    - 0.001
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
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
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: Oct 4, 2021
    date_iso: '2021-10-04'
    date_display: Oct 2021
    codebase_url: https://github.com/smiles724/Molformer
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.069
    - 0.03
    - 0.092
    - 45.0
    - 39.0
    - 44.0
    - 0.8
    - null
    - 0.043
    - 0.037
    - 1.27
    - 0.15
    - 45.0
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
    - null
    - null
    - null
    - null
  - model: GINE-ε
    model_plain: GINE-ε
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.081
    - 0.081
    - 0.081
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - 0.003
    - 0.003
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: 1-3-GNN
    model_plain: 1-3-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/pfgnn/PF-GNN
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.088
    - 0.088
    - 0.088
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.007
    - 0.007
    - 0.007
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: EST
    model_plain: EST
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.23086'
    title: Equivariant Spherical Transformer for Efficient Molecular Modeling
    date: May 29, 2025
    date_iso: '2025-05-29'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 28.0
    - 0.011
    - null
    - 5.92
    - 7.03
    - 7.03
    - null
    - null
    - null
    - null
    - null
    - null
    - 5.92
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
    - null
    - null
    - null
    - null
  - model: Equiformer v2
    model_plain: Equiformer v2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.23086'
    title: Equivariant Spherical Transformer for Efficient Molecular Modeling
    date: May 29, 2025
    date_iso: '2025-05-29'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 29.0
    - 0.01
    - 0.05
    - 6.49
    - 7.57
    - 7.57
    - 0.023
    - null
    - null
    - null
    - null
    - null
    - 6.49
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
    - null
    - null
    - null
    - null
  - model: Equiformer
    model_plain: Equiformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.23086'
    title: Equivariant Spherical Transformer for Efficient Molecular Modeling
    date: May 29, 2025
    date_iso: '2025-05-29'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 30.0
    - 0.011
    - 0.046
    - 6.74
    - 7.63
    - 7.63
    - 0.023
    - null
    - null
    - null
    - null
    - null
    - 6.74
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
    - null
    - null
    - null
    - null
  - model: PθNITA​ (fiber bundle)
    model_plain: PθNITA​ (fiber bundle)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.02970'
    title: Fast, Expressive SE$(n)$ Equivariant Networks through Weight-Sharing in
      Position-Orientation Space
    date: Oct 4, 2023
    date_iso: '2023-10-04'
    date_display: Oct 2023
    codebase_url: https://github.com/ebekkers/ponita
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 30.4
    - null
    - 0.0375
    - 8.31
    - 8.04
    - 0.00863
    - 0.0242
    - null
    - null
    - null
    - null
    - null
    - 8.67
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
    - null
    - null
    - null
    - null
  - model: PaxNet
    model_plain: PaxNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.16518'
    title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
      interactive message passing for molecules'
    date: Oct 29, 2022
    date_iso: '2022-10-29'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 31.0
    - 10.8
    - 44.7
    - 5.9
    - 6.04
    - 7.14
    - 23.1
    - null
    - 22.8
    - 19.2
    - 1.17
    - null
    - 5.92
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
    - null
    - null
    - null
    - null
  - model: SphereNet
    model_plain: SphereNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.16518'
    title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
      interactive message passing for molecules'
    date: Oct 29, 2022
    date_iso: '2022-10-29'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 31.1
    - 24.5
    - 44.9
    - 6.26
    - 6.33
    - 7.78
    - 22.0
    - null
    - 22.8
    - 18.9
    - 1.12
    - null
    - 6.36
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
    - null
    - null
    - null
    - null
  - model: ViSNet
    model_plain: ViSNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.16518'
    title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
      interactive message passing for molecules'
    date: Oct 29, 2022
    date_iso: '2022-10-29'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 31.7
    - 9.5
    - 41.1
    - 4.23
    - 4.52
    - 5.86
    - 23.0
    - null
    - 17.3
    - 14.8
    - 1.56
    - null
    - 4.25
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
    - null
    - null
    - null
    - null
  - model: EQGAT
    model_plain: EQGAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.23086'
    title: Equivariant Spherical Transformer for Efficient Molecular Modeling
    date: May 29, 2025
    date_iso: '2025-05-29'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 32.0
    - 0.011
    - 0.053
    - 25.0
    - 23.0
    - 23.0
    - 0.024
    - null
    - null
    - null
    - null
    - null
    - 25.0
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
    - null
    - null
    - null
    - null
  - model: SphereNet
    model_plain: SphereNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 32.0
    - 0.026
    - 0.046
    - 0.006
    - 6.0
    - 8.0
    - 7.0
    - null
    - 0.023
    - 0.018
    - 1.12
    - null
    - 0.007
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
    - null
    - null
    - null
    - null
  - model: ComENet
    model_plain: ComENet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.16518'
    title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
      interactive message passing for molecules'
    date: Oct 29, 2022
    date_iso: '2022-10-29'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 32.4
    - 24.5
    - 45.2
    - 6.59
    - 6.86
    - 7.98
    - 24.0
    - null
    - 23.1
    - 19.8
    - 1.2
    - null
    - 6.82
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
    - null
    - null
    - null
    - null
  - model: DimeNet++
    model_plain: DimeNet++
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.16518'
    title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
      interactive message passing for molecules'
    date: Oct 29, 2022
    date_iso: '2022-10-29'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 32.6
    - 29.7
    - 43.5
    - 6.32
    - 6.53
    - 7.56
    - 23.0
    - null
    - 24.6
    - 19.5
    - 1.21
    - null
    - 6.28
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
    - null
    - null
    - null
    - null
  - model: Equiformer
    model_plain: Equiformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 33.0
    - 0.014
    - 0.056
    - 0.01
    - 10.0
    - 10.0
    - 11.0
    - null
    - 0.017
    - 0.016
    - 1.32
    - null
    - 0.011
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
    - null
    - null
    - null
    - null
  - model: DimeNet++
    model_plain: DimeNet++
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 33.0
    - 0.03
    - 0.044
    - 6.0
    - 7.0
    - 8.0
    - 6.0
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
    - null
    - null
    - null
    - null
  - model: DimeNet++
    model_plain: DimeNet++
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02970'
    title: Fast, Expressive SE$(n)$ Equivariant Networks through Weight-Sharing in
      Position-Orientation Space
    date: Oct 4, 2023
    date_iso: '2023-10-04'
    date_display: Oct 2023
    codebase_url: https://github.com/ebekkers/ponita
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 34.8
    - 0.0286
    - 0.0469
    - 8.02
    - 8.11
    - 0.0249
    - 0.0249
    - null
    - 27.8
    - 19.7
    - 1.29
    - null
    - 7.89
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
    - null
    - null
    - null
    - null
  - model: TorchMD-Net
    model_plain: TorchMD-Net
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.23086'
    title: Equivariant Spherical Transformer for Efficient Molecular Modeling
    date: May 29, 2025
    date_iso: '2025-05-29'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 36.0
    - 0.011
    - 0.059
    - 6.38
    - 7.62
    - 7.62
    - 0.026
    - null
    - null
    - null
    - null
    - null
    - 6.38
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
    - null
    - null
    - null
    - null
  - model: ET
    model_plain: ET
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.16518'
    title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
      interactive message passing for molecules'
    date: Oct 29, 2022
    date_iso: '2022-10-29'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 36.1
    - 11.0
    - 59.0
    - 6.15
    - 6.16
    - 7.62
    - 26.0
    - null
    - 20.3
    - 17.5
    - 1.84
    - null
    - 6.38
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
    - null
    - null
    - null
    - null
  - model: SEGNN
    model_plain: SEGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 42.0
    - 0.023
    - 0.06
    - 13.0
    - 15.0
    - 15.0
    - 13.0
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
    - null
    - null
    - null
    - null
  - model: EQGAT
    model_plain: EQGAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 44.0
    - 0.014
    - 0.063
    - 13.0
    - 13.0
    - 12.0
    - 13.0
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
    - null
    - null
    - null
    - null
  - model: PaiNN
    model_plain: PaiNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.16518'
    title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
      interactive message passing for molecules'
    date: Oct 29, 2022
    date_iso: '2022-10-29'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 45.7
    - 12.0
    - 45.0
    - 5.85
    - 5.98
    - 7.35
    - 24.0
    - null
    - 27.6
    - 20.4
    - 1.28
    - null
    - 5.83
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
    - null
    - null
    - null
    - null
  - model: PaiNN
    model_plain: PaiNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 46.0
    - 0.012
    - 0.045
    - 0.006
    - 6.0
    - 7.0
    - 6.0
    - null
    - 0.028
    - 0.02
    - 1.28
    - null
    - 0.006
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
    - null
    - null
    - null
    - null
  - model: EGNN
    model_plain: EGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.16518'
    title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
      interactive message passing for molecules'
    date: Oct 29, 2022
    date_iso: '2022-10-29'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 48.0
    - 29.0
    - 71.0
    - 11.0
    - 12.0
    - 12.0
    - 31.0
    - null
    - 29.0
    - 25.0
    - 1.55
    - null
    - 12.0
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
    - null
    - null
    - null
    - null
  - model: LieConv
    model_plain: LieConv
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 49.0
    - 0.032
    - 0.084
    - 19.0
    - 24.0
    - 22.0
    - 19.0
    - 0.0
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
    - null
    - null
    - null
    - null
  - model: ClofNet
    model_plain: ClofNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 53.0
    - 0.04
    - 0.063
    - 8.0
    - 9.0
    - 9.0
    - 9.0
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
    - null
    - null
    - null
    - null
  - model: SE(3)-Tr.
    model_plain: SE(3)-Tr.
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 53.0
    - 0.051
    - 0.142
    - 0.0
    - null
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
    - null
    - null
    - null
    - null
  - model: TFN
    model_plain: TFN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 58.0
    - 0.064
    - 0.223
    - 0.0
    - null
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
    - null
    - null
    - null
    - null
  - model: Cormorant
    model_plain: Cormorant
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 61.0
    - 0.038
    - 0.085
    - 22.0
    - 21.0
    - 20.0
    - 21.0
    - 0.0
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
    - null
    - null
    - null
    - null
  - model: SchNet
    model_plain: SchNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.16518'
    title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
      interactive message passing for molecules'
    date: Oct 29, 2022
    date_iso: '2022-10-29'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 63.0
    - 33.0
    - 235.0
    - 14.0
    - 14.0
    - 14.0
    - 33.0
    - null
    - 41.0
    - 34.0
    - 1.7
    - null
    - 19.0
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
    - null
    - null
    - null
    - null
  - model: NMP
    model_plain: NMP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.04757'
    title: A new perspective on building efficient and expressive 3D equivariant graph
      neural networks
    date: Apr 7, 2023
    date_iso: '2023-04-07'
    date_display: Apr 2023
    codebase_url: https://github.com/yuanqidu/LeftNet
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 69.0
    - 0.03
    - 0.092
    - 20.0
    - 17.0
    - 19.0
    - 20.0
    - 0.0
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
    - null
    - null
    - null
    - null
  - model: True 3D SMP
    model_plain: True 3D SMP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.04126'
    title: 3D Infomax improves GNNs for Molecular Property Prediction
    date: Oct 8, 2021
    date_iso: '2021-10-08'
    date_display: Oct 2021
    codebase_url: https://github.com/HannesStark/3DInfomax
    published_conference: ICML 2021
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2021
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 85.1
    - 0.0726
    - 0.1542
    - null
    - null
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
    - null
    - null
    - null
    - null
  row_count: 132
  rows_json: /data/datasets/qm9/standard-split-rows.json
  chart_json: /data/datasets/qm9/standard-split-chart.json
  arch_counts:
    gnn: 105
    hybrid: 13
    graph_transformer: 6
    llm: 1
    walk: 0
    traditional: 2
  metric_counts:
  - 68
  - 127
  - 127
  - 100
  - 93
  - 93
  - 94
  - 4
  - 94
  - 94
  - 86
  - 27
  - 91
  milestones: &id001
  - value: 0.025
    std: null
    model: Molformer
    arxiv_id: '2110.01191'
    title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
    date: '2021-10-04'
  - value: 0.017
    std: 0.001
    model: PF-GNN
    arxiv_id: '2401.17752'
    title: 'PF-GNN: Differentiable particle filtering based approximation of universal
      graph representations'
    date: '2024-01-31'
  milestones_by_metric:
    gap: *id001
    mu:
    - value: 0.0253
      std: null
      model: DeepMoleNet
      arxiv_id: '2011.14115'
      title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
        Molecules
      date: '2020-11-28'
    - value: 0.012
      std: null
      model: PaiNN
      arxiv_id: '2110.01191'
      title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
      date: '2021-10-04'
    - value: 0.011
      std: null
      model: LEFTNet
      arxiv_id: '2304.04757'
      title: A new perspective on building efficient and expressive 3D equivariant
        graph neural networks
      date: '2023-04-07'
    - value: 0.01
      std: null
      model: Equiformer v2
      arxiv_id: '2505.23086'
      title: Equivariant Spherical Transformer for Efficient Molecular Modeling
      date: '2025-05-29'
    alpha:
    - value: 0.03
      std: null
      model: MGCN
      arxiv_id: '2011.14115'
      title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
        Molecules
      date: '2020-11-28'
    - value: 0.017
      std: 0.001
      model: PF-GNN
      arxiv_id: '2401.17752'
      title: 'PF-GNN: Differentiable particle filtering based approximation of universal
        graph representations'
      date: '2024-01-31'
    U0:
    - value: 6.32
      std: null
      model: DimeNet++
      arxiv_id: '2011.14115'
      title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
        Molecules
      date: '2020-11-28'
    - value: 5.85
      std: null
      model: PaiNN
      arxiv_id: '2110.01191'
      title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
      date: '2021-10-04'
    - value: 0.022
      std: null
      model: PPGN
      arxiv_id: '2111.06283'
      title: 'DropGNN: Random Dropouts Increase the Expressiveness of Graph Neural
        Networks'
      date: '2021-11-11'
    - value: 0.0
      std: null
      model: TFN
      arxiv_id: '2304.04757'
      title: A new perspective on building efficient and expressive 3D equivariant
        graph neural networks
      date: '2023-04-07'
    H:
    - value: 6.53
      std: null
      model: DimeNet++
      arxiv_id: '2011.14115'
      title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
        Molecules
      date: '2020-11-28'
    - value: 5.98
      std: null
      model: PaiNN
      arxiv_id: '2110.01191'
      title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
      date: '2021-10-04'
    - value: 0.0294
      std: null
      model: PPGN
      arxiv_id: '2111.06283'
      title: 'DropGNN: Random Dropouts Increase the Expressiveness of Graph Neural
        Networks'
      date: '2021-11-11'
    - value: 0.016
      std: null
      model: IDMPNN
      arxiv_id: '2305.04963'
      title: 'From Relational Pooling to Subgraph GNNs: A Universal Framework for
        More Expressive Graph Neural Networks'
      date: '2023-05-08'
    G:
    - value: 7.56
      std: null
      model: DimeNet++
      arxiv_id: '2011.14115'
      title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
        Molecules
      date: '2020-11-28'
    - value: 7.35
      std: null
      model: PaiNN
      arxiv_id: '2110.01191'
      title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
      date: '2021-10-04'
    - value: 0.0469
      std: null
      model: 1-2-3 GNN
      arxiv_id: '2111.06283'
      title: 'DropGNN: Random Dropouts Increase the Expressiveness of Graph Neural
        Networks'
      date: '2021-11-11'
    - value: 0.0159
      std: null
      model: IDMPNN
      arxiv_id: '2305.04963'
      title: 'From Relational Pooling to Subgraph GNNs: A Universal Framework for
        More Expressive Graph Neural Networks'
      date: '2023-05-08'
    - value: 0.00863
      std: null
      model: PθNITA​ (fiber bundle)
      arxiv_id: '2310.02970'
      title: Fast, Expressive SE$(n)$ Equivariant Networks through Weight-Sharing
        in Position-Orientation Space
      date: '2023-10-04'
    Cv:
    - value: 0.023
      std: null
      model: DimeNet++
      arxiv_id: '2011.14115'
      title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
        Molecules
      date: '2020-11-28'
    - value: 0.021
      std: null
      model: SphereNet
      arxiv_id: '2110.01191'
      title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
      date: '2021-10-04'
    - value: 0.0144
      std: null
      model: PPGN
      arxiv_id: '2111.06283'
      title: 'DropGNN: Random Dropouts Increase the Expressiveness of Graph Neural
        Networks'
      date: '2021-11-11'
    S:
    - value: 0.0
      std: null
      model: NMP
      arxiv_id: '2304.04757'
      title: A new perspective on building efficient and expressive 3D equivariant
        graph neural networks
      date: '2023-04-07'
    HOMO:
    - value: 23.9
      std: null
      model: DeepMoleNet
      arxiv_id: '2011.14115'
      title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
        Molecules
      date: '2020-11-28'
    - value: 0.024
      std: null
      model: DimeNet++
      arxiv_id: '2110.01191'
      title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
      date: '2021-10-04'
    - value: 0.00174
      std: null
      model: PPGN
      arxiv_id: '2111.06283'
      title: 'DropGNN: Random Dropouts Increase the Expressiveness of Graph Neural
        Networks'
      date: '2021-11-11'
    LUMO:
    - value: 19.5
      std: null
      model: DimeNet++
      arxiv_id: '2011.14115'
      title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
        Molecules
      date: '2020-11-28'
    - value: 0.019
      std: null
      model: DimeNet++
      arxiv_id: '2110.01191'
      title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
      date: '2021-10-04'
    - value: 0.00177
      std: null
      model: DropMPNN
      arxiv_id: '2111.06283'
      title: 'DropGNN: Random Dropouts Increase the Expressiveness of Graph Neural
        Networks'
      date: '2021-11-11'
    - value: 0.0016
      std: null
      model: AgentNet
      arxiv_id: '2206.11010'
      title: Agent-based Graph Neural Networks
      date: '2022-06-22'
    zpve:
    - value: 1.12
      std: null
      model: MGCN
      arxiv_id: '2011.14115'
      title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
        Molecules
      date: '2020-11-28'
    - value: 0.000112
      std: null
      model: DropMPNN
      arxiv_id: '2111.06283'
      title: 'DropGNN: Random Dropouts Increase the Expressiveness of Graph Neural
        Networks'
      date: '2021-11-11'
    R2:
    - value: 0.066
      std: null
      model: PaiNN
      arxiv_id: '2110.01191'
      title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
      date: '2021-10-04'
    U:
    - value: 6.28
      std: null
      model: DimeNet++
      arxiv_id: '2011.14115'
      title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
        Molecules
      date: '2020-11-28'
    - value: 5.53
      std: null
      model: PaiNN
      arxiv_id: '2110.01191'
      title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular Graphs'
      date: '2021-10-04'
    - value: 0.0409
      std: null
      model: DropMPNN
      arxiv_id: '2111.06283'
      title: 'DropGNN: Random Dropouts Increase the Expressiveness of Graph Neural
        Networks'
      date: '2021-11-11'
    - value: 0.005
      std: null
      model: LEFTNet
      arxiv_id: '2304.04757'
      title: A new perspective on building efficient and expressive 3D equivariant
        graph neural networks
      date: '2023-04-07'
---

