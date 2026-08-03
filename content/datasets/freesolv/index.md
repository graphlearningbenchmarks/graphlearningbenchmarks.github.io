---
title: FreeSolv
slug: freesolv
benchmark: MoleculeNet
task_type: graph_regression
description: Hydration free energy regression (kcal/mol) on 642 molecules.
primary_metric: RMSE
higher_is_better: false
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
stats: null
result_count: 179
best_model:
  model: 10% ZINC + 10% PubChem
  value: 0.205
  metric: RMSE
  arxiv_id: '2106.09553'
  paper_title: How Much Structural Information Large Scale Molecular Language Representations
    Can Capture?
papers:
- arxiv_id: '2604.15699'
  title: Frequency-Corrupt Based Graph Self-Supervised Learning
  date_iso: '2026-04-17'
  venue: WWW 2026
- arxiv_id: '2602.20344'
  title: Hierarchical Molecular Representation Learning via Fragment-Based Self-Supervised
    Embedding Prediction
  date_iso: '2026-02-23'
  venue: ''
- arxiv_id: '2510.16885'
  title: 'UniGTE: Unified Graph–Text Encoding for Zero-Shot Generalization across
    Graph Tasks and Domains'
  date_iso: '2025-10-19'
  venue: NeurIPS 2025
- arxiv_id: '2510.07289'
  title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D Graph Encoder'
  date_iso: '2025-10-08'
  venue: ''
- arxiv_id: '2505.23345'
  title: Graph Positional Autoencoders as Self-supervised Learners
  date_iso: '2025-05-29'
  venue: KDD 2025
- arxiv_id: '2502.12638'
  title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation'
  date_iso: '2025-02-18'
  venue: ICLR 2025
- arxiv_id: '2412.15589'
  title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
    Graph Information Bottleneck
  date_iso: '2024-12-20'
  venue: AAAI 2024
- arxiv_id: '2406.01899'
  title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models'
  date_iso: '2024-06-04'
  venue: NeurIPS 2024
- arxiv_id: '2405.10343'
  title: 'UniCorn: A Unified Contrastive Learning Approach for Multi-view Molecular
    Representation Learning'
  date_iso: '2024-05-15'
  venue: ICML 2024
- arxiv_id: '2405.01350'
  title: Community-Invariant Graph Contrastive Learning
  date_iso: '2024-05-02'
  venue: ICML 2024
- arxiv_id: '2402.01975'
  title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
  date_iso: '2024-02-03'
  venue: ICML 2024
- arxiv_id: '2312.07633'
  title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive Molecular
    Property Prediction
  date_iso: '2023-12-12'
  venue: NeurIPS 2023
- arxiv_id: '2311.04837'
  title: Identifying Semantic Component for Robust Molecular Property Prediction
  date_iso: '2023-11-08'
  venue: ''
- arxiv_id: '2310.16401'
  title: Graph Neural Networks with a Distribution of Parametrized Graphs
  date_iso: '2023-10-25'
  venue: ICML 2023
- arxiv_id: '2309.10131'
  title: Deep Prompt Tuning for Graph Transformers
  date_iso: '2023-09-18'
  venue: ''
- arxiv_id: '2309.04062'
  title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising and
    Cross-Modal Distillation'
  date_iso: '2023-09-08'
  venue: AAAI 2023
- arxiv_id: '2309.04589'
  title: Motif-aware Attribute Masking for Molecular Graph Pre-training
  date_iso: '2023-09-08'
  venue: ''
- arxiv_id: '2307.07107'
  title: Graph Positional and Structural Encoder
  date_iso: '2023-07-14'
  venue: ICML 2023
- arxiv_id: '2202.09346'
  title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation and
    Decomposed Fragment Contrast
  date_iso: '2022-02-18'
  venue: ''
- arxiv_id: '2112.03806'
  title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
  date_iso: '2021-12-07'
  venue: ''
- arxiv_id: '2110.04126'
  title: 3D Infomax improves GNNs for Molecular Property Prediction
  date_iso: '2021-10-08'
  venue: ICML 2021
- arxiv_id: '2109.11730'
  title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
  date_iso: '2021-09-24'
  venue: AAAI 2021
- arxiv_id: '2106.09553'
  title: How Much Structural Information Large Scale Molecular Language Representations
    Can Capture?
  date_iso: '2021-06-17'
  venue: ''
- arxiv_id: '2106.06130'
  title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
    Prediction'
  date_iso: '2021-06-11'
  venue: ''
- arxiv_id: '1709.03741'
  title: Learning Graph-Level Representation for Drug Discovery
  date_iso: '2017-09-12'
  venue: ''
- arxiv_id: '1703.00564'
  title: MoleculeNet
  date_iso: '2017-03-02'
  venue: ''
variants:
- slug: scaffold-split
  name: Scaffold split
  notes: ''
  is_standard: true
  primary_metric: RMSE
  default_metric: RMSE
  higher_is_better: false
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - RMSE
  - MAE
  metric_display_names:
  - RMSE
  - MAE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: 10% ZINC + 10% PubChem
    model_plain: 10% ZINC + 10% PubChem
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_iso: '2021-06-17'
    date_display: Jun 2021
    codebase_url: https://github.com/IBM/molformer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.205
    - null
    metric_stds:
    - null
    - null
  - model: MoLFormer-XL
    model_plain: MoLFormer-XL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_iso: '2021-06-17'
    date_display: Jun 2021
    codebase_url: https://github.com/IBM/molformer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2308
    - null
    metric_stds:
    - null
    - null
  - model: MoLFormer-Base
    model_plain: MoLFormer-Base
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_iso: '2021-06-17'
    date_display: Jun 2021
    codebase_url: https://github.com/IBM/molformer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2596
    - null
    metric_stds:
    - null
    - null
  - model: 100% ZINC
    model_plain: 100% ZINC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_iso: '2021-06-17'
    date_display: Jun 2021
    codebase_url: https://github.com/IBM/molformer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2981
    - null
    metric_stds:
    - null
    - null
  - model: SE(3)-I MPPH
    model_plain: SE(3)-I MPPH
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: Dec 12, 2023
    date_iso: '2023-12-12'
    date_display: Dec 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.354
    - null
    metric_stds:
    - 0.053
    - null
  - model: ECFP-4 + RF
    model_plain: ECFP-4 + RF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: Dec 12, 2023
    date_iso: '2023-12-12'
    date_display: Dec 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.56
    - null
    metric_stds:
    - 0.066
    - null
  - model: GPSE + GPS
    model_plain: GPSE + GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.07107'
    title: Graph Positional and Structural Encoder
    date: Jul 14, 2023
    date_iso: '2023-07-14'
    date_display: Jul 2023
    codebase_url: https://github.com/G-Taxonomy-Workgroup/GPSE
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.682
    - null
    metric_stds:
    - null
    - null
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.07107'
    title: Graph Positional and Structural Encoder
    date: Jul 14, 2023
    date_iso: '2023-07-14'
    date_display: Jul 2023
    codebase_url: https://github.com/G-Taxonomy-Workgroup/GPSE
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.743
    - null
    metric_stds:
    - null
    - null
  - model: GeomGCL
    model_plain: GeomGCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_iso: '2021-06-17'
    date_display: Jun 2021
    codebase_url: https://github.com/IBM/molformer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.866
    - null
    metric_stds:
    - null
    - null
  - model: GeomMPNN
    model_plain: GeomMPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.913
    - null
    metric_stds:
    - null
    - null
  - model: dummy super node
    model_plain: dummy super node
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1709.03741'
    title: Learning Graph-Level Representation for Drug Discovery
    date: Sep 12, 2017
    date_iso: '2017-09-12'
    date_display: Sep 2017
    codebase_url: https://github.com/ZJULearning/graph_level_drug_discovery
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.933
    - null
    metric_stds:
    - null
    - null
  - model: LiGhT FT
    model_plain: LiGhT FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 90.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.955
    - null
    metric_stds:
    - 0.051
    - null
  - model: GraphConv
    model_plain: GraphConv
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1709.03741'
    title: Learning Graph-Level Representation for Drug Discovery
    date: Sep 12, 2017
    date_iso: '2017-09-12'
    date_display: Sep 2017
    codebase_url: https://github.com/ZJULearning/graph_level_drug_discovery
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.963
    - null
    metric_stds:
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
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_iso: '2021-06-17'
    date_display: Jun 2021
    codebase_url: https://github.com/IBM/molformer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.978
    - null
    metric_stds:
    - null
    - null
  - model: LiGhT DeepGPT
    model_plain: LiGhT DeepGPT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.37
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.983
    - null
    metric_stds:
    - 0.079
    - null
  - model: D-MPNN
    model_plain: D-MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: Dec 12, 2023
    date_iso: '2023-12-12'
    date_display: Dec 2023
    codebase_url: ''
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.01
    - null
    metric_stds:
    - 0.064
    - null
  - model: AttentiveFP
    model_plain: AttentiveFP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.034
    - null
    metric_stds:
    - null
    - null
  - model: MAT
    model_plain: MAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.059
    - null
    metric_stds:
    - null
    - null
  - model: DMPNN
    model_plain: DMPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.092
    - null
    metric_stds:
    - null
    - null
  - model: CoMPT
    model_plain: CoMPT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.103
    - null
    metric_stds:
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
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: Mar 2, 2017
    date_iso: '2017-03-02'
    date_display: Mar 2017
    codebase_url: https://github.com/deepchem/deepchem
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.15
    - null
    metric_stds:
    - 0.12
    - null
  - model: HMGNN
    model_plain: HMGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.207
    - null
    metric_stds:
    - null
    - null
  - model: Weave
    model_plain: Weave
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: Mar 2, 2017
    date_iso: '2017-03-02'
    date_display: Mar 2017
    codebase_url: https://github.com/deepchem/deepchem
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.22
    - null
    metric_stds:
    - 0.28
    - null
  - model: GraSPNet
    model_plain: GraSPNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.20344'
    title: Hierarchical Molecular Representation Learning via Fragment-Based Self-Supervised
      Embedding Prediction
    date: Feb 23, 2026
    date_iso: '2026-02-23'
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
    - 1.232
    - null
    metric_stds:
    - 0.05
    - null
  - model: GraphGPS FT
    model_plain: GraphGPS FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 14.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.38
    - null
    metric_stds:
    - 0.234
    - null
  - model: GC
    model_plain: GC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: Mar 2, 2017
    date_iso: '2017-03-02'
    date_display: Mar 2017
    codebase_url: https://github.com/deepchem/deepchem
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.4
    - null
    metric_stds:
    - 0.16
    - null
  - model: GraphGPS DeepGPT
    model_plain: GraphGPS DeepGPT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.05
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.415
    - null
    metric_stds:
    - 0.254
    - null
  - model: conan-FGW
    model_plain: conan-FGW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.423
    - null
    metric_stds:
    - 0.272
    - null
  - model: MoCL
    model_plain: MoCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: Sep 24, 2021
    date_iso: '2021-09-24'
    date_display: Sep 2021
    codebase_url: ''
    published_conference: AAAI 2021
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.478
    - null
    metric_stds:
    - null
    - null
  - model: UniMol
    model_plain: UniMol
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.48
    - null
    metric_stds:
    - 0.048
    - null
  - model: conan
    model_plain: conan
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.548
    - null
    metric_stds:
    - 0.281
    - null
  - model: UniCorn(DFT + RDKit)
    model_plain: UniCorn(DFT + RDKit)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.555
    - null
    metric_stds:
    - 0.075
    - null
  - model: SchNet-emb
    model_plain: SchNet-emb
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.587
    - null
    metric_stds:
    - 0.136
    - null
  - model: MoLlama
    model_plain: MoLlama
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2502.12638'
    title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation'
    date: Feb 18, 2025
    date_iso: '2025-02-18'
    date_display: Feb 2025
    codebase_url: https://github.com/acharkq/NExT-Mol
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.59
    - null
    metric_stds:
    - 0.04
    - null
  - model: SchNet-scalar
    model_plain: SchNet-scalar
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.01975'
    title: Structure-Aware E(3)-Invariant Molecular Conformer Aggregation Networks
    date: Feb 3, 2024
    date_iso: '2024-02-03'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.608
    - null
    metric_stds:
    - 0.158
    - null
  - model: DAG
    model_plain: DAG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: Mar 2, 2017
    date_iso: '2017-03-02'
    date_display: Mar 2017
    codebase_url: https://github.com/deepchem/deepchem
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.63
    - null
    metric_stds:
    - 0.18
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
    - 1.648
    - null
    metric_stds:
    - 0.074
    - null
  - model: Graphormer DeepGPT
    model_plain: Graphormer DeepGPT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.668
    - null
    metric_stds:
    - 0.114
    - null
  - model: Graphormer FT
    model_plain: Graphormer FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 48.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.68
    - null
    metric_stds:
    - 0.013
    - null
  - model: MolPROP
    model_plain: MolPROP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2502.12638'
    title: 'NExT-Mol: 3D Diffusion Meets 1D Language Modeling for 3D Molecule Generation'
    date: Feb 18, 2025
    date_iso: '2025-02-18'
    date_display: Feb 2025
    codebase_url: https://github.com/acharkq/NExT-Mol
    published_conference: ICLR 2025
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2025
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.7
    - null
    metric_stds:
    - 0.09
    - null
  - model: Geometry
    model_plain: Geometry
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: Jun 11, 2021
    date_iso: '2021-06-11'
    date_display: Jun 2021
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.701
    - null
    metric_stds:
    - 0.147
    - null
  - model: XGBoost
    model_plain: XGBoost
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: Mar 2, 2017
    date_iso: '2017-03-02'
    date_display: Mar 2017
    codebase_url: https://github.com/deepchem/deepchem
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.74
    - null
    metric_stds:
    - 0.15
    - null
  - model: OOD-GNN
    model_plain: OOD-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.04837'
    title: Identifying Semantic Component for Robust Molecular Property Prediction
    date: Nov 8, 2023
    date_iso: '2023-11-08'
    date_display: Nov 2023
    codebase_url: https://github.com/DMIRLAB-Group/SCI
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.81
    - null
    metric_stds:
    - 0.14
    - null
  - model: MoleBlend
    model_plain: MoleBlend
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.07289'
    title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D Graph Encoder'
    date: Oct 8, 2025
    date_iso: '2025-10-08'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.851
    - null
    metric_stds:
    - 0.068
    - null
  - model: GeoGNN
    model_plain: GeoGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: Jun 11, 2021
    date_iso: '2021-06-11'
    date_display: Jun 2021
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.857
    - null
    metric_stds:
    - 0.071
    - null
  - model: MICRO-Graph
    model_plain: MICRO-Graph
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 1.865
    - null
    metric_stds:
    - 0.061
    - null
  - model: Multitask
    model_plain: Multitask
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1703.00564'
    title: MoleculeNet
    date: Mar 2, 2017
    date_iso: '2017-03-02'
    date_display: Mar 2017
    codebase_url: https://github.com/deepchem/deepchem
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.87
    - null
    metric_stds:
    - 0.07
    - null
  - model: Geometry+Graph
    model_plain: Geometry+Graph
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: Jun 11, 2021
    date_iso: '2021-06-11'
    date_display: Jun 2021
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.876
    - null
    metric_stds:
    - 0.094
    - null
  - model: GEM
    model_plain: GEM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.09553'
    title: How Much Structural Information Large Scale Molecular Language Representations
      Can Capture?
    date: Jun 17, 2021
    date_iso: '2021-06-17'
    date_display: Jun 2021
    codebase_url: https://github.com/IBM/molformer
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.877
    - null
    metric_stds:
    - null
    - null
  - model: ChemRL-GEM
    model_plain: ChemRL-GEM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: Jun 11, 2021
    date_iso: '2021-06-11'
    date_display: Jun 2021
    codebase_url: https://github.com/PaddlePaddle/PaddleHelix
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.877
    - null
    metric_stds:
    - 0.094
    - null
  row_count: 179
  rows_json: /data/datasets/freesolv/scaffold-split-rows.json
  chart_json: /data/datasets/freesolv/scaffold-split-chart.json
  arch_counts:
    gnn: 118
    hybrid: 33
    graph_transformer: 8
    llm: 6
    walk: 1
    traditional: 10
  metric_counts:
  - 168
  - 11
  milestones: &id001
  - value: 1.701
    std: 0.147
    model: Geometry
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: '2021-06-11'
  - value: 0.866
    std: null
    model: GeomGCL
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: '2021-09-24'
  - value: 0.354
    std: 0.053
    model: SE(3)-I MPPH
    arxiv_id: '2312.07633'
    title: SE(3)-Invariant Multiparameter Persistent Homology for Chiral-Sensitive
      Molecular Property Prediction
    date: '2023-12-12'
  milestones_by_metric:
    RMSE: *id001
    MAE:
    - value: 1.339
      std: 0.075
      model: DCT
      arxiv_id: '2406.01899'
      title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models'
      date: '2024-06-04'
---

