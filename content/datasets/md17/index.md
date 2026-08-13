---
title: MD17
slug: md17
benchmark: Quantum Chemistry
task_type: graph_regression
short_description: Ab-initio molecular dynamics — predict energy and forces for small
  organic molecules.
description: '**Energy-and-force regression** Ab-initio molecular dynamics — predict
  energy and forces for small organic molecules. Inputs are atomic species and molecular
  geometries. Evaluated by MAE.'
detailed_description:
  task: Ab-initio molecular dynamics — predict energy and forces for small organic
    molecules. The primary catalog metric is MAE.
  data: Ab-initio molecular dynamics — predict energy and forces for small organic
    molecules.
  features: Atoms, nuclear species, and molecular geometries are the core inputs.
    Graph edges or neighbor lists are model preprocessing choices; energy units, force
    signs, target normalization, and coordinate conventions must match the release.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses MAE (lower is better). Exact masks or folds must come from
    the cited release.'
  quirks_and_pitfalls: Near-duplicate conformations and molecule-wise versus conformation-wise
    splits can cause leakage. Units and reference-energy conventions differ across
    implementations, and MD trajectories are strongly autocorrelated.
sources:
- title: Machine Learning of Accurate Energy-Conserving Molecular Force Fields
  arxiv_id: '1611.04678'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric MD17 loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MD17.html
  kind: implementation_documentation
primary_metric: MAE
higher_is_better: false
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MD17.html
stats: null
result_count: 275
best_model:
  model: QHNet
  value: 1.036e-05
  metric: MAE
  arxiv_id: '2506.09398'
  paper_title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via
    SO(2) Local Frames
papers:
- arxiv_id: '2510.22123'
  title: Learning 3D Anisotropic Noise Distributions Improves Molecular Force Field
    Modeling
  date_iso: '2025-10-25'
  venue: ''
- arxiv_id: '2510.16780'
  title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective Re-mask Decoding'
  date_iso: '2025-10-19'
  venue: ''
- arxiv_id: '2510.04233'
  title: 'PAINET: A Principled Efficient Transformer for 3D Dynamics Modeling'
  date_iso: '2025-10-05'
  venue: ICLR 2025
- arxiv_id: '2506.13174'
  title: 'GeoRecon: Graph-Level Representation Learning for 3D Molecules via Reconstruction-Based
    Pretraining'
  date_iso: '2025-06-16'
  venue: ''
- arxiv_id: '2506.09398'
  title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
    Local Frames
  date_iso: '2025-06-11'
  venue: ''
- arxiv_id: '2503.01431'
  title: How simple can you go? An off-the-shelf transformer approach to molecular
    dynamics
  date_iso: '2025-03-03'
  venue: ''
- arxiv_id: '2502.16284'
  title: 'MolSpectra: Pre-training 3D Molecular Representation with Multi-modal Energy
    Spectra'
  date_iso: '2025-02-22'
  venue: ICLR 2025
- arxiv_id: '2502.08209'
  title: Equivariant Masked position prediction for efficient molecular representation
  date_iso: '2025-02-12'
  venue: ICLR 2025
- arxiv_id: '2502.01171'
  title: Efficient and Scalable Density Functional Theory Hamiltonian Prediction through
    Adaptive Sparsity
  date_iso: '2025-02-03'
  venue: ICML 2025
- arxiv_id: '2410.17878'
  title: Relaxed Equivariance via Multitask Learning
  date_iso: '2024-10-23'
  venue: ''
- arxiv_id: '2410.11443'
  title: Are High-Degree Representations Really Unnecessary in Equivariant Graph Neural
    Networks?
  date_iso: '2024-10-15'
  venue: NeurIPS 2024
- arxiv_id: '2407.11086'
  title: Pre-training with fractional denoising to enhance molecular property prediction
  date_iso: '2024-07-14'
  venue: ''
- arxiv_id: '2407.02263'
  title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform for Machine Learning
    Force Fields'
  date_iso: '2024-07-02'
  venue: ICLR 2024
- arxiv_id: '2406.13265'
  title: Molecule Graph Networks with Many-body Equivariant Interactions
  date_iso: '2024-06-19'
  venue: ''
- arxiv_id: '2406.03794'
  title: Infusing Self-Consistency into Density Functional Theory Hamiltonian Prediction
    via Deep Equilibrium Models
  date_iso: '2024-06-06'
  venue: NeurIPS 2024
- arxiv_id: '2405.16511'
  title: 'SE3Set: Harnessing equivariant hypergraph neural networks for molecular
    representation learning'
  date_iso: '2024-05-26'
  venue: TMLR 2024
- arxiv_id: '2405.10343'
  title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view Molecular
    Representation Learning'
  date_iso: '2024-05-15'
  venue: ICML 2024
- arxiv_id: '2405.05665'
  title: 'SubGDiff: A Subgraph Diffusion Model to Improve Molecular Representation
    Learning'
  date_iso: '2024-05-09'
  venue: NeurIPS 2024
- arxiv_id: '2402.10011'
  title: Clifford Group Equivariant Simplicial Message Passing Networks
  date_iso: '2024-02-15'
  venue: ICLR 2024
- arxiv_id: '2402.07472'
  title: Cartesian atomic cluster expansion for machine learning interatomic potentials
  date_iso: '2024-02-12'
  venue: ''
- arxiv_id: '2402.04836'
  title: On the Completeness of Invariant Geometric Deep Learning Models
  date_iso: '2024-02-07'
  venue: ICLR 2024
- arxiv_id: '2312.03475'
  title: 'Molecule Joint Auto-Encoding: Trajectory Pretraining with 2D and 3D Diffusion'
  date_iso: '2023-12-06'
  venue: NeurIPS 2023
- arxiv_id: '2311.02124'
  title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training Method'
  date_iso: '2023-11-03'
  venue: ICLR 2023
- arxiv_id: '2310.16802'
  title: 'From Molecules to Materials: Pre-training Large Generalizable Models for
    Atomic Property Prediction'
  date_iso: '2023-10-25'
  venue: ICLR 2023
- arxiv_id: '2310.02970'
  title: Fast, Expressive SE$(n)$ Equivariant Networks through Weight-Sharing in Position-Orientation
    Space
  date_iso: '2023-10-04'
  venue: ICLR 2023
- arxiv_id: '2309.15718'
  title: Geometry-enhanced pretraining on interatomic potentials
  date_iso: '2023-09-27'
  venue: ''
- arxiv_id: '2306.09549'
  title: 'QH9: A Quantum Hamiltonian Prediction Benchmark for QM9 Molecules'
  date_iso: '2023-06-15'
  venue: NeurIPS 2023
- arxiv_id: '2306.09375'
  title: Symmetry-Informed Geometric Representation for Molecules, Proteins, and Crystalline
    Materials
  date_iso: '2023-06-15'
  venue: NeurIPS 2023
- arxiv_id: '2306.06482'
  title: 'TensorNet: Cartesian Tensor Representations for Efficient Learning of Molecular
    Potentials'
  date_iso: '2023-06-10'
  venue: NeurIPS 2023
- arxiv_id: '2305.18407'
  title: A Group Symmetric Stochastic Differential Equation Model for Molecule Multi-modal
    Pretraining
  date_iso: '2023-05-28'
  venue: ICML 2023
- arxiv_id: '2304.04757'
  title: A new perspective on building efficient and expressive 3D equivariant graph
    neural networks
  date_iso: '2023-04-07'
  venue: NeurIPS 2023
- arxiv_id: '2302.05743'
  title: Is Distance Matrix Enough for Geometric Deep Learning?
  date_iso: '2023-02-11'
  venue: NeurIPS 2023
- arxiv_id: '2301.08893'
  title: Spatial Attention Kinetic Network with E(n)-Equivariance
  date_iso: '2023-01-21'
  venue: ICLR 2023
- arxiv_id: '2210.16518'
  title: 'ViSNet: an equivariant geometry-enhanced graph neural network with vector-scalar
    interactive message passing for molecules'
  date_iso: '2022-10-29'
  venue: ''
- arxiv_id: '2210.07237'
  title: 'Forces are not Enough: Benchmark and Critical Evaluation for Machine Learning
    Force Fields with Molecular Simulations'
  date_iso: '2022-10-13'
  venue: TMLR 2022
- arxiv_id: '2207.08824'
  title: Energy-Motivated Equivariant Pretraining for 3D Molecular Graphs
  date_iso: '2022-07-18'
  venue: AAAI 2022
- arxiv_id: '2206.13602'
  title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising Distance Matching
  date_iso: '2022-06-27'
  venue: ICLR 2022
- arxiv_id: '2206.07697'
  title: 'MACE: Higher Order Equivariant Message Passing Neural Networks for Fast
    and Accurate Force Fields'
  date_iso: '2022-06-15'
  venue: NeurIPS 2022
- arxiv_id: '2205.14276'
  title: 'So3krates: Equivariant attention for interactions on arbitrary length-scales
    in molecular systems'
  date_iso: '2022-05-28'
  venue: NeurIPS 2022
- arxiv_id: '2205.06643'
  title: The design space of E(3)-equivariant atom-centred interatomic potentials
  date_iso: '2022-05-13'
  venue: ''
- arxiv_id: '2202.02541'
  title: 'TorchMD-NET: Equivariant Transformers for Neural Network based Molecular
    Potentials'
  date_iso: '2022-01-01'
  venue: ''
- arxiv_id: '2108.02913'
  title: 'NewtonNet: A Newtonian message passing network for deep learning of interatomic
    potentials and forces'
  date_iso: '2021-08-06'
  venue: ''
- arxiv_id: '2106.09575'
  title: Rotation Invariant Graph Neural Networks using Spin Convolutions
  date_iso: '2021-06-17'
  venue: ''
- arxiv_id: '2105.00304'
  title: 'SpookyNet: Learning force fields with electronic degrees of freedom and
    nonlocal effects'
  date_iso: '2021-05-01'
  venue: ''
- arxiv_id: '2102.05013'
  title: Spherical Message Passing for 3D Molecular Graphs
  date_iso: '2021-02-09'
  venue: ICLR 2021
- arxiv_id: '2101.03164'
  title: E(3)-Equivariant Graph Neural Networks for Data-Efficient and Accurate Interatomic
    Potentials
  date_iso: '2021-01-08'
  venue: ''
- arxiv_id: '2003.03123'
  title: Directional Message Passing for Molecular Graphs
  date_iso: '2020-03-06'
  venue: ICLR 2020
- arxiv_id: '1902.08408'
  title: 'PhysNet: A Neural Network for Predicting Energies, Forces, Dipole Moments
    and Partial Charges'
  date_iso: '2019-02-22'
  venue: ''
- arxiv_id: '1712.06113'
  title: SchNet -- a deep learning architecture for molecules and materials
  date_iso: '2017-12-17'
  venue: ''
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
    num_classes: null
  metrics:
  - MAE
  - ADE
  - E
  - Energy
  - F
  - FDE
  - Force
  - H
  - RMSD
  - epsilon
  - psi
  metric_display_names:
  - MAE
  - ADE
  - E
  - Energy MAE (kcal mol⁻¹)
  - F
  - FDE
  - Force MAE (kcal mol⁻¹ Å⁻¹)
  - H
  - RMSD
  - epsilon
  - psi
  show_all_metrics_desktop: false
  chart_default_log_scale: true
  chart_hidden_models: []
  rows:
  - model: QHNet
    model_plain: QHNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    date: Jun 11, 2025
    date_iso: '2025-06-11'
    date_display: Jun 2025
    codebase_url: https://github.com/divelab/AIRS
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 1.036e-05
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
  - model: QHNetV2
    model_plain: QHNetV2
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    date: Jun 11, 2025
    date_iso: '2025-06-11'
    date_display: Jun 2025
    codebase_url: https://github.com/divelab/AIRS
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.038e-05
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
  - model: PhiSNet
    model_plain: PhiSNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    date: Jun 11, 2025
    date_iso: '2025-06-11'
    date_display: Jun 2025
    codebase_url: https://github.com/divelab/AIRS
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.759e-05
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
  - model: SPHNet
    model_plain: SPHNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    date: Jun 11, 2025
    date_iso: '2025-06-11'
    date_display: Jun 2025
    codebase_url: https://github.com/divelab/AIRS
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.936e-05
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
  - model: QHNet
    model_plain: QHNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2306.09549'
    title: 'QH9: A Quantum Hamiltonian Prediction Benchmark for QM9 Molecules'
    date: Jun 15, 2023
    date_iso: '2023-06-15'
    date_display: Jun 2023
    codebase_url: https://github.com/divelab/AIRS
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 8.312e-05
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
  - model: ViSNet
    model_plain: ViSNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.02263'
    title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform for Machine
      Learning Force Fields'
    date: Jul 2, 2024
    date_iso: '2024-07-02'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0007
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
  - model: BOTNet
    model_plain: BOTNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.02263'
    title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform for Machine
      Learning Force Fields'
    date: Jul 2, 2024
    date_iso: '2024-07-02'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0007
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
  - model: NequIP
    model_plain: NequIP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.02263'
    title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform for Machine
      Learning Force Fields'
    date: Jul 2, 2024
    date_iso: '2024-07-02'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0009
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
  - model: GeoNGNN
    model_plain: GeoNGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.04836'
    title: On the Completeness of Invariant Geometric Deep Learning Models
    date: Feb 7, 2024
    date_iso: '2024-02-07'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0014
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
  - model: UNiTE
    model_plain: UNiTE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.02263'
    title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform for Machine
      Learning Force Fields'
    date: Jul 2, 2024
    date_iso: '2024-07-02'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.002
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
  - model: PAINET
    model_plain: PAINET
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.04233'
    title: 'PAINET: A Principled Efficient Transformer for 3D Dynamics Modeling'
    date: Oct 5, 2025
    date_iso: '2025-10-05'
    date_display: Oct 2025
    codebase_url: https://github.com/Icarus1411/PAINET
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.00324
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - 0.00183
    - null
    - null
    metric_stds:
    - 0.000119
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - 8.0e-06
    - null
    - null
  - model: EGNO
    model_plain: EGNO
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.17878'
    title: Relaxed Equivariance via Multitask Learning
    date: Oct 23, 2024
    date_iso: '2024-10-23'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0037
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
    - 0.0001
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
  - model: HEGNN
    model_plain: HEGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.17878'
    title: Relaxed Equivariance via Multitask Learning
    date: Oct 23, 2024
    date_iso: '2024-10-23'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0037
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
    - 0.0002
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
  - model: GMN
    model_plain: GMN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2410.11443'
    title: Are High-Degree Representations Really Unnecessary in Equivariant Graph
      Neural Networks?
    date: Oct 15, 2024
    date_iso: '2024-10-15'
    date_display: Oct 2024
    codebase_url: https://github.com/GLAD-RUC/HEGNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.004
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
    - 0.0001
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
  - model: Allegro
    model_plain: Allegro
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.02263'
    title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform for Machine
      Learning Force Fields'
    date: Jul 2, 2024
    date_iso: '2024-07-02'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0046
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
  - model: EGNN
    model_plain: EGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.11443'
    title: Are High-Degree Representations Really Unnecessary in Equivariant Graph
      Neural Networks?
    date: Oct 15, 2024
    date_iso: '2024-10-15'
    date_display: Oct 2024
    codebase_url: https://github.com/GLAD-RUC/HEGNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0047
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
    - 0.0002
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
  - model: rf
    model_plain: rf
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    arxiv_id: '2410.11443'
    title: Are High-Degree Representations Really Unnecessary in Equivariant Graph
      Neural Networks?
    date: Oct 15, 2024
    date_iso: '2024-10-15'
    date_display: Oct 2024
    codebase_url: https://github.com/GLAD-RUC/HEGNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.005
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
    - 0.0001
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
  - model: GNN
    model_plain: GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.17878'
    title: Relaxed Equivariance via Multitask Learning
    date: Oct 23, 2024
    date_iso: '2024-10-23'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0054
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
    - 1.0e-05
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
  - model: REMUL-GNN
    model_plain: REMUL-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.17878'
    title: Relaxed Equivariance via Multitask Learning
    date: Oct 23, 2024
    date_iso: '2024-10-23'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0054
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
    - 1.0e-05
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
  - model: EGNNReg
    model_plain: EGNNReg
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.11443'
    title: Are High-Degree Representations Really Unnecessary in Equivariant Graph
      Neural Networks?
    date: Oct 15, 2024
    date_iso: '2024-10-15'
    date_display: Oct 2024
    codebase_url: https://github.com/GLAD-RUC/HEGNN
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0063
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
    - 0.0001
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
  - model: DA-GNN
    model_plain: DA-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.17878'
    title: Relaxed Equivariance via Multitask Learning
    date: Oct 23, 2024
    date_iso: '2024-10-23'
    date_display: Oct 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0069
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
    - 1.0e-05
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
  - model: GemNet-T
    model_plain: GemNet-T
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.09375'
    title: Symmetry-Informed Geometric Representation for Molecules, Proteins, and
      Crystalline Materials
    date: Jun 15, 2023
    date_iso: '2023-06-15'
    date_display: Jun 2023
    codebase_url: https://github.com/chao1224/Geom3D
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.007
    - null
    - null
    - 0.684
    - null
    - null
    - 0.558
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
  - model: PaiNN
    model_plain: PaiNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.09375'
    title: Symmetry-Informed Geometric Representation for Molecules, Proteins, and
      Crystalline Materials
    date: Jun 15, 2023
    date_iso: '2023-06-15'
    date_display: Jun 2023
    codebase_url: https://github.com/chao1224/Geom3D
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.01
    - null
    - null
    - 27.626
    - null
    - null
    - 0.572
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
  - model: Equiformer
    model_plain: Equiformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.09375'
    title: Symmetry-Informed Geometric Representation for Molecules, Proteins, and
      Crystalline Materials
    date: Jun 15, 2023
    date_iso: '2023-06-15'
    date_display: Jun 2023
    codebase_url: https://github.com/chao1224/Geom3D
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.02
    - null
    - null
    - 0.308
    - null
    - null
    - 0.286
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
  - model: TensorNet 2L (770k)
    model_plain: TensorNet 2L (770k)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.06482'
    title: 'TensorNet: Cartesian Tensor Representations for Efficient Learning of
      Molecular Potentials'
    date: Jun 10, 2023
    date_iso: '2023-06-10'
    date_display: Jun 2023
    codebase_url: https://github.com/torchmd/torchmd-net
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.02
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
  - model: GDML
    model_plain: GDML
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    arxiv_id: '1902.08408'
    title: 'PhysNet: A Neural Network for Predicting Energies, Forces, Dipole Moments
      and Partial Charges'
    date: Feb 22, 2019
    date_iso: '2019-02-22'
    date_display: Feb 2019
    codebase_url: https://github.com/MeuwlyGroup/PhysNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.02
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
  - model: PhysNet-ens5
    model_plain: PhysNet-ens5
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1902.08408'
    title: 'PhysNet: A Neural Network for Predicting Energies, Forces, Dipole Moments
      and Partial Charges'
    date: Feb 22, 2019
    date_iso: '2019-02-22'
    date_display: Feb 2019
    codebase_url: https://github.com/MeuwlyGroup/PhysNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.02
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
  - model: 3D-GSRD
    model_plain: 3D-GSRD
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.16780'
    title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective Re-mask Decoding'
    date: Oct 19, 2025
    date_iso: '2025-10-19'
    date_display: Oct 2025
    codebase_url: https://github.com/WuChang0124/3D-GSRD
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0266
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
  - model: Allegro
    model_plain: Allegro
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.09375'
    title: Symmetry-Informed Geometric Representation for Molecules, Proteins, and
      Crystalline Materials
    date: Jun 15, 2023
    date_iso: '2023-06-15'
    date_display: Jun 2023
    codebase_url: https://github.com/chao1224/Geom3D
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.029
    - null
    - null
    - 1.138
    - null
    - null
    - 3.405
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
  - model: BOTNet
    model_plain: BOTNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.06643'
    title: The design space of E(3)-equivariant atom-centred interatomic potentials
    date: May 13, 2022
    date_iso: '2022-05-13'
    date_display: May 2022
    codebase_url: https://github.com/gncs/botnet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.03
    - null
    - 2.3
    - null
    - 8.5
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
  - model: TensorNet 1L (535k)
    model_plain: TensorNet 1L (535k)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2306.06482'
    title: 'TensorNet: Cartesian Tensor Representations for Efficient Learning of
      Molecular Potentials'
    date: Jun 10, 2023
    date_iso: '2023-06-10'
    date_display: Jun 2023
    codebase_url: https://github.com/torchmd/torchmd-net
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.03
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
  - model: PhysNet
    model_plain: PhysNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1902.08408'
    title: 'PhysNet: A Neural Network for Predicting Energies, Forces, Dipole Moments
      and Partial Charges'
    date: Feb 22, 2019
    date_iso: '2019-02-22'
    date_display: Feb 2019
    codebase_url: https://github.com/MeuwlyGroup/PhysNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.03
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
  - model: FreeCG
    model_plain: FreeCG
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.02263'
    title: 'FreeCG: Free the Design Space of Clebsch–Gordan Transform for Machine
      Learning Force Fields'
    date: Jul 2, 2024
    date_iso: '2024-07-02'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
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
  - model: 3D-EMGP (TorchMD-NET)
    model_plain: 3D-EMGP (TorchMD-NET)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.16780'
    title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective Re-mask Decoding'
    date: Oct 19, 2025
    date_iso: '2025-10-19'
    date_display: Oct 2025
    codebase_url: https://github.com/WuChang0124/3D-GSRD
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0352
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
  - model: AniDS
    model_plain: AniDS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2510.22123'
    title: Learning 3D Anisotropic Noise Distributions Improves Molecular Force Field
      Modeling
    date: Oct 25, 2025
    date_iso: '2025-10-25'
    date_display: Oct 2025
    codebase_url: https://github.com/ZeroKnighting/AniDS
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.036
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
  - model: DeNS (Lmax=3)
    model_plain: DeNS (Lmax=3)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.22123'
    title: Learning 3D Anisotropic Noise Distributions Improves Molecular Force Field
      Modeling
    date: Oct 25, 2025
    date_iso: '2025-10-25'
    date_display: Oct 2025
    codebase_url: https://github.com/ZeroKnighting/AniDS
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.037
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
  - model: TorchMD-Net
    model_plain: TorchMD-Net
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.16780'
    title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective Re-mask Decoding'
    date: Oct 19, 2025
    date_iso: '2025-10-19'
    date_display: Oct 2025
    codebase_url: https://github.com/WuChang0124/3D-GSRD
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.039
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
  - model: NequIP
    model_plain: NequIP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.16511'
    title: 'SE3Set: Harnessing equivariant hypergraph neural networks for molecular
      representation learning'
    date: May 26, 2024
    date_iso: '2024-05-26'
    date_display: May 2024
    codebase_url: ''
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.039
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
  - model: QuinNet
    model_plain: QuinNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.16511'
    title: 'SE3Set: Harnessing equivariant hypergraph neural networks for molecular
      representation learning'
    date: May 26, 2024
    date_iso: '2024-05-26'
    date_display: May 2024
    codebase_url: ''
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.039
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
  - model: SE3Set
    model_plain: SE3Set
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.16511'
    title: 'SE3Set: Harnessing equivariant hypergraph neural networks for molecular
      representation learning'
    date: May 26, 2024
    date_iso: '2024-05-26'
    date_display: May 2024
    codebase_url: ''
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.039
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
    - 0.039
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
  - model: NequIP (Lmax=3)
    model_plain: NequIP (Lmax=3)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.22123'
    title: Learning 3D Anisotropic Noise Distributions Improves Molecular Force Field
      Modeling
    date: Oct 25, 2025
    date_iso: '2025-10-25'
    date_display: Oct 2025
    codebase_url: https://github.com/ZeroKnighting/AniDS
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.039
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
  - model: NequIP
    model_plain: NequIP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 3.0
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.14276'
    title: 'So3krates: Equivariant attention for interactions on arbitrary length-scales
      in molecular systems'
    date: May 28, 2022
    date_iso: '2022-05-28'
    date_display: May 2022
    codebase_url: https://github.com/thorben-frank/mlff
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.04
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
  - model: DTNN
    model_plain: DTNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1712.06113'
    title: SchNet -- a deep learning architecture for molecules and materials
    date: Dec 17, 2017
    date_iso: '2017-12-17'
    date_display: Dec 2017
    codebase_url: https://github.com/atomistic-machine-learning/SchNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.04
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
  - model: 3D-ReTrans
    model_plain: 3D-ReTrans
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.16780'
    title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective Re-mask Decoding'
    date: Oct 19, 2025
    date_iso: '2025-10-19'
    date_display: Oct 2025
    codebase_url: https://github.com/WuChang0124/3D-GSRD
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0417
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
  - model: ENINet
    model_plain: ENINet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.13265'
    title: Molecule Graph Networks with Many-body Equivariant Interactions
    date: Jun 19, 2024
    date_iso: '2024-06-19'
    date_display: Jun 2024
    codebase_url: https://github.com/tsudalab/ENINet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.043
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
  - model: Frad
    model_plain: Frad
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.16780'
    title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective Re-mask Decoding'
    date: Oct 19, 2025
    date_iso: '2025-10-19'
    date_display: Oct 2025
    codebase_url: https://github.com/WuChang0124/3D-GSRD
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.0431
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
  - model: PhysNet-ens5
    model_plain: PhysNet-ens5
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.09575'
    title: Rotation Invariant Graph Neural Networks using Spin Convolutions
    date: Jun 17, 2021
    date_iso: '2021-06-17'
    date_display: Jun 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.044
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
  - model: UniCorn
    model_plain: UniCorn
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.10343'
    title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view Molecular
      Representation Learning'
    date: May 15, 2024
    date_iso: '2024-05-15'
    date_display: May 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
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
    arxiv_id: '2405.16511'
    title: 'SE3Set: Harnessing equivariant hypergraph neural networks for molecular
      representation learning'
    date: May 26, 2024
    date_iso: '2024-05-26'
    date_display: May 2024
    codebase_url: ''
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
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
  row_count: 275
  rows_json: /data/datasets/md17/standard-split-rows.json
  chart_json: /data/datasets/md17/standard-split-chart.json
  arch_counts:
    gnn: 209
    hybrid: 43
    graph_transformer: 1
    llm: 1
    walk: 0
    traditional: 17
  metric_counts:
  - 233
  - 13
  - 13
  - 10
  - 13
  - 12
  - 19
  - 9
  - 1
  - 4
  - 4
  milestones: &id001
  - value: 0.04
    std: null
    model: DTNN
    arxiv_id: '1712.06113'
    title: SchNet -- a deep learning architecture for molecules and materials
    date: '2017-12-17'
  - value: 0.02
    std: null
    model: GDML
    arxiv_id: '1902.08408'
    title: 'PhysNet: A Neural Network for Predicting Energies, Forces, Dipole Moments
      and Partial Charges'
    date: '2019-02-22'
  - value: 8.312e-05
    std: null
    model: QHNet
    arxiv_id: '2306.09549'
    title: 'QH9: A Quantum Hamiltonian Prediction Benchmark for QM9 Molecules'
    date: '2023-06-15'
  - value: 1.036e-05
    std: null
    model: QHNet
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    date: '2025-06-11'
  milestones_by_metric:
    MAE: *id001
    ADE:
    - value: 0.0103
      std: null
      model: empsn (300K)
      arxiv_id: '2402.10011'
      title: Clifford Group Equivariant Simplicial Message Passing Networks
      date: '2024-02-15'
    E:
    - value: 2.3
      std: null
      model: BOTNet
      arxiv_id: '2205.06643'
      title: The design space of E(3)-equivariant atom-centred interatomic potentials
      date: '2022-05-13'
    - value: 0.4
      std: null
      model: MACE
      arxiv_id: '2206.07697'
      title: 'MACE: Higher Order Equivariant Message Passing Neural Networks for Fast
        and Accurate Force Fields'
      date: '2022-06-15'
    Energy:
    - value: 0.244
      std: null
      model: SphereNet
      arxiv_id: '2306.09375'
      title: Symmetry-Informed Geometric Representation for Molecules, Proteins, and
        Crystalline Materials
      date: '2023-06-15'
    F:
    - value: 8.2
      std: null
      model: NequIP
      arxiv_id: '2205.06643'
      title: The design space of E(3)-equivariant atom-centred interatomic potentials
      date: '2022-05-13'
    - value: 0.3
      std: null
      model: MACE
      arxiv_id: '2206.07697'
      title: 'MACE: Higher Order Equivariant Message Passing Neural Networks for Fast
        and Accurate Force Fields'
      date: '2022-06-15'
    FDE:
    - value: 0.0112
      std: null
      model: empsn (300K)
      arxiv_id: '2402.10011'
      title: Clifford Group Equivariant Simplicial Message Passing Networks
      date: '2024-02-15'
    Force:
    - value: 1.1
      std: null
      model: NequIP
      arxiv_id: '2210.07237'
      title: 'Forces are not Enough: Benchmark and Critical Evaluation for Machine
        Learning Force Fields with Molecular Simulations'
      date: '2022-10-13'
    - value: 0.286
      std: null
      model: Equiformer
      arxiv_id: '2306.09375'
      title: Symmetry-Informed Geometric Representation for Molecules, Proteins, and
        Crystalline Materials
      date: '2023-06-15'
    H:
    - value: 1.073e-05
      std: null
      model: PhiSNet (ori)
      arxiv_id: '2406.03794'
      title: Infusing Self-Consistency into Density Functional Theory Hamiltonian
        Prediction via Deep Equilibrium Models
      date: '2024-06-06'
    RMSD:
    - value: 0.00183
      std: 8.0e-06
      model: PAINET
      arxiv_id: '2510.04233'
      title: 'PAINET: A Principled Efficient Transformer for 3D Dynamics Modeling'
      date: '2025-10-05'
    epsilon:
    - value: 3.376e-05
      std: null
      model: QHNet
      arxiv_id: '2502.01171'
      title: Efficient and Scalable Density Functional Theory Hamiltonian Prediction
        through Adaptive Sparsity
      date: '2025-02-03'
    psi:
    - value: 1.0
      std: null
      model: SchNOrb
      arxiv_id: '2502.01171'
      title: Efficient and Scalable Density Functional Theory Hamiltonian Prediction
        through Adaptive Sparsity
      date: '2025-02-03'
---

