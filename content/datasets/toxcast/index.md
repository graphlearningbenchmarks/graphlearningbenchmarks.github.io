---
title: ToxCast
slug: toxcast
benchmark: MoleculeNet
task_type: graph_classification
description: Multi-task toxicological profile prediction (617 tasks) from the EPA
  ToxCast program.
primary_metric: ROC-AUC
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 617
result_count: 299
best_model:
  model: SCI
  value: 0.8073
  metric: ROC-AUC
  arxiv_id: '2311.04837'
  paper_title: Identifying Semantic Component for Robust Molecular Property Prediction
papers:
- arxiv_id: '2503.04362'
  title: A Generalist Cross-Domain Molecular Learning Framework for Structure-Based
    Drug Discovery
  date_iso: '2025-03-06'
  venue: ''
- arxiv_id: '2501.01073'
  title: Graph Generative Pre-trained Transformer
  date_iso: '2025-01-02'
  venue: ICML 2025
- arxiv_id: '2412.16441'
  title: 'Towards Graph Foundation Models: Learning Generalities Across Graphs via
    Task-Trees'
  date_iso: '2024-12-21'
  venue: ICML 2024
- arxiv_id: '2412.15589'
  title: Pre-training Graph Neural Networks on Molecules by Using Subgraph-Conditioned
    Graph Information Bottleneck
  date_iso: '2024-12-20'
  venue: AAAI 2024
- arxiv_id: '2412.07407'
  title: 'Towards Graph Foundation Models: A Study on the Generalization of Positional
    and Structural Encodings'
  date_iso: '2024-12-10'
  venue: TMLR 2024
- arxiv_id: '2410.13761'
  title: 'GDeR: Safeguarding Efficiency, Balancing, and Robustness via Prototypical
    Graph Pruning'
  date_iso: '2024-10-17'
  venue: NeurIPS 2024
- arxiv_id: '2410.10365'
  title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
    Samples'
  date_iso: '2024-10-14'
  venue: ''
- arxiv_id: '2407.12136'
  title: Molecular Topological Profile (MOLTOP) - Simple and Strong Baseline for Molecular
    Graph Classification
  date_iso: '2024-07-16'
  venue: ''
- arxiv_id: '2406.10727'
  title: 'Text-space Graph Foundation Models: Comprehensive Benchmarks and New Insights'
  date_iso: '2024-06-15'
  venue: NeurIPS 2024
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
- arxiv_id: '2405.01350'
  title: Community-Invariant Graph Contrastive Learning
  date_iso: '2024-05-02'
  venue: ICML 2024
- arxiv_id: '2403.01400'
  title: Decoupling Weighing and Selecting for Integrating Multiple Graph Pre-training
    Tasks
  date_iso: '2024-03-03'
  venue: ICLR 2024
- arxiv_id: '2402.10380'
  title: Subgraph-level Universal Prompt Tuning
  date_iso: '2024-02-16'
  venue: ''
- arxiv_id: '2402.08023'
  title: 'UGMAE: A Unified Framework for Graph Masked Autoencoders'
  date_iso: '2024-02-12'
  venue: ''
- arxiv_id: '2402.07249'
  title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent Molecular Property
    Prediction: A Systematic Survey'
  date_iso: '2024-02-11'
  venue: ''
- arxiv_id: '2312.13583'
  title: Fine-tuning Graph Neural Networks by Preserving Graph Generative Patterns
  date_iso: '2023-12-21'
  venue: AAAI 2023
- arxiv_id: '2311.04837'
  title: Identifying Semantic Component for Robust Molecular Property Prediction
  date_iso: '2023-11-08'
  venue: ''
- arxiv_id: '2310.14753'
  title: Rethinking Tokenizer and Decoder in Masked Graph Modeling for Molecules
  date_iso: '2023-10-23'
  venue: NeurIPS 2023
- arxiv_id: '2310.14216'
  title: 'UniMAP: Universal SMILES-Graph Representation Learning'
  date_iso: '2023-10-22'
  venue: ''
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
- arxiv_id: '2309.02304'
  title: Graph Self-Contrast Representation Learning
  date_iso: '2023-09-05'
  venue: ''
- arxiv_id: '2306.03506'
  title: Subgraph Networks Based Contrastive Learning
  date_iso: '2023-06-06'
  venue: ''
- arxiv_id: '2305.18407'
  title: A Group Symmetric Stochastic Differential Equation Model for Molecule Multi-modal
    Pretraining
  date_iso: '2023-05-28'
  venue: ICML 2023
- arxiv_id: '2306.13089'
  title: 'gimlet: A Unified Graph-Text Model for Instruction-Based Molecule Zero-Shot
    Learning'
  date_iso: '2023-05-28'
  venue: ''
- arxiv_id: '2305.15745'
  title: Robust Ante-hoc Graph Explainer using Bilevel Optimization
  date_iso: '2023-05-25'
  venue: ''
- arxiv_id: '2209.15240'
  title: Universal Prompt Tuning for Graph Neural Networks
  date_iso: '2022-09-30'
  venue: NeurIPS 2022
- arxiv_id: '2209.15101'
  title: Improving Molecular Pretraining with Complementary Featurizations
  date_iso: '2022-09-29'
  venue: ''
- arxiv_id: '2207.06010'
  title: Does GNN Pretraining Help Molecular Representation?
  date_iso: '2022-07-13'
  venue: NeurIPS 2022
- arxiv_id: '2206.07869'
  title: Let Invariant Rationale Discovery Inspire Graph Contrastive Learning
  date_iso: '2022-06-16'
  venue: ICML 2022
- arxiv_id: '2206.08005'
  title: Evaluating Self-Supervised Learning for Molecular Graph Embeddings
  date_iso: '2022-06-16'
  venue: NeurIPS 2022
- arxiv_id: '2206.03364'
  title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer for Molecular Property
    Prediction'
  date_iso: '2022-06-02'
  venue: KDD 2022
- arxiv_id: '2205.15746'
  title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
    Learning
  date_iso: '2022-05-31'
  venue: ICML 2022
- arxiv_id: '2205.10803'
  title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
  date_iso: '2022-05-22'
  venue: KDD 2022
- arxiv_id: '2202.02989'
  title: Graph Self-supervised Learning with Accurate Discrepancy Learning
  date_iso: '2022-02-07'
  venue: NeurIPS 2022
- arxiv_id: '2112.03806'
  title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
  date_iso: '2021-12-07'
  venue: ''
- arxiv_id: '2110.07728'
  title: 16 Pre-training Molecular Graph Representation with 3D Geometry
  date_iso: '2021-10-07'
  venue: ICLR 2021
- arxiv_id: '2110.00987'
  title: Motif-based Graph Self-Supervised Learning for Molecular Property Prediction
  date_iso: '2021-10-03'
  venue: NeurIPS 2021
- arxiv_id: '2109.11730'
  title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
  date_iso: '2021-09-24'
  venue: AAAI 2021
- arxiv_id: '2106.06130'
  title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
    Prediction'
  date_iso: '2021-06-11'
  venue: ''
- arxiv_id: '2106.05819'
  title: Adversarial Graph Augmentation to Improve Graph Contrastive Learning
  date_iso: '2021-06-10'
  venue: NeurIPS 2021
- arxiv_id: '2106.04509'
  title: 'MoCL: Data-driven Molecular Fingerprint via Knowledge-aware Contrastive
    Learning from Molecular Graph'
  date_iso: '2021-06-05'
  venue: KDD 2021
- arxiv_id: '2011.15069'
  title: Graph convolutions that can finally model local structure
  date_iso: '2020-11-30'
  venue: ''
variants:
- slug: scaffold-split
  name: Scaffold split
  notes: ''
  is_standard: true
  primary_metric: ROC-AUC
  default_metric: ROC-AUC
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: 617
  metrics:
  - ROC-AUC
  - Accuracy
  metric_display_names:
  - ROC-AUC
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: SCI
    model_plain: SCI
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8073
    - null
    metric_stds:
    - 0.0006
    - null
  - model: PharmHGT
    model_plain: PharmHGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.8023
    - null
    metric_stds:
    - 0.0009
    - null
  - model: StableGNN-Graph
    model_plain: StableGNN-Graph
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
    - 0.7986
    - null
    metric_stds:
    - 0.001
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
    - 0.787
    - null
    metric_stds:
    - 0.003
    - null
  - model: FFiNet
    model_plain: FFiNet
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
    - 0.7712
    - null
    metric_stds:
    - 0.0048
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
    - 0.7678
    - null
    metric_stds:
    - 0.0037
    - null
  - model: GeomGCL
    model_plain: GeomGCL
    is_baseline: false
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
    - 0.763
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
    - 0.757
    - null
    metric_stds:
    - 0.011
    - null
  - model: D&D-Node +vn
    model_plain: D&D-Node +vn
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.04062'
    title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising
      and Cross-Modal Distillation'
    date: Sep 8, 2023
    date_iso: '2023-09-08'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7556
    - null
    metric_stds:
    - 0.0068
    - null
  - model: D&D-Graph +vn
    model_plain: D&D-Graph +vn
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.04062'
    title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising
      and Cross-Modal Distillation'
    date: Sep 8, 2023
    date_iso: '2023-09-08'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7554
    - null
    metric_stds:
    - 0.0003
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
    - 0.755
    - null
    metric_stds:
    - null
    - null
  - model: D&D-Node +mp
    model_plain: D&D-Node +mp
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.04062'
    title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising
      and Cross-Modal Distillation'
    date: Sep 8, 2023
    date_iso: '2023-09-08'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7549
    - null
    metric_stds:
    - 0.0055
    - null
  - model: D&D-Graph +mp
    model_plain: D&D-Graph +mp
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.04062'
    title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising
      and Cross-Modal Distillation'
    date: Sep 8, 2023
    date_iso: '2023-09-08'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7541
    - null
    metric_stds:
    - 0.0014
    - null
  - model: GINE w/ VN
    model_plain: GINE w/ VN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_iso: '2020-11-30'
    date_display: Nov 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.749
    - 0.749
    metric_stds:
    - 0.002
    - 0.002
  - model: GINe+ K=1 w/ VN
    model_plain: GINe+ K=1 w/ VN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_iso: '2020-11-30'
    date_display: Nov 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.749
    - 0.749
    metric_stds:
    - 0.008
    - 0.008
  - model: KPGT
    model_plain: KPGT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.03364'
    title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer for Molecular
      Property Prediction'
    date: Jun 2, 2022
    date_iso: '2022-06-02'
    date_display: Jun 2022
    codebase_url: https://github.com/lihan97/KPGT
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.746
    - null
    metric_stds:
    - 0.002
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
    - 0.745
    - null
    metric_stds:
    - 0.005
    - null
  - model: GCN w/ VN
    model_plain: GCN w/ VN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_iso: '2020-11-30'
    date_display: Nov 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.743
    - 0.743
    metric_stds:
    - 0.003
    - 0.003
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
    - 0.743
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
    - 0.743
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
    - 0.743
    - null
    metric_stds:
    - null
    - null
  - model: GINE
    model_plain: GINE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_iso: '2020-11-30'
    date_display: Nov 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.741
    - 0.741
    metric_stds:
    - 0.004
    - 0.004
  - model: NaiveGINe+ K=3 w/ VN
    model_plain: NaiveGINe+ K=3 w/ VN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_iso: '2020-11-30'
    date_display: Nov 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.737
    - 0.737
    metric_stds:
    - 0.007
    - 0.007
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_iso: '2020-11-30'
    date_display: Nov 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.735
    - 0.735
    metric_stds:
    - 0.002
    - 0.002
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
    - 0.735
    - null
    metric_stds:
    - 0.005
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
    - 0.735
    - null
    metric_stds:
    - null
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
    - 0.725
    - null
    metric_stds:
    - 0.011
    - null
  - model: Contextpred+Sup
    model_plain: Contextpred+Sup
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.03364'
    title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer for Molecular
      Property Prediction'
    date: Jun 2, 2022
    date_iso: '2022-06-02'
    date_display: Jun 2022
    codebase_url: https://github.com/lihan97/KPGT
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.724
    - null
    metric_stds:
    - 0.015
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
    - 0.722
    - null
    metric_stds:
    - 0.011
    - null
  - model: Context Prediction + Supervised
    model_plain: Context Prediction + Supervised
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.06010'
    title: Does GNN Pretraining Help Molecular Representation?
    date: Jul 13, 2022
    date_iso: '2022-07-13'
    date_display: Jul 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7219
    - null
    metric_stds:
    - 0.0079
    - null
  - model: RandInit +mp
    model_plain: RandInit +mp
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.04062'
    title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising
      and Cross-Modal Distillation'
    date: Sep 8, 2023
    date_iso: '2023-09-08'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7219
    - null
    metric_stds:
    - 0.0035
    - null
  - model: HIMP
    model_plain: HIMP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_iso: '2020-11-30'
    date_display: Nov 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.721
    - 0.721
    metric_stds:
    - 0.004
    - 0.004
  - model: RandInit +vn
    model_plain: RandInit +vn
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.04062'
    title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising
      and Cross-Modal Distillation'
    date: Sep 8, 2023
    date_iso: '2023-09-08'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.719
    - null
    metric_stds:
    - 0.0051
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
    - 0.718
    - null
    metric_stds:
    - null
    - null
  - model: Masking Node + Supervised
    model_plain: Masking Node + Supervised
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.06010'
    title: Does GNN Pretraining Help Molecular Representation?
    date: Jul 13, 2022
    date_iso: '2022-07-13'
    date_display: Jul 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7166
    - null
    metric_stds:
    - 0.0073
    - null
  - model: Supervised
    model_plain: Supervised
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2207.06010'
    title: Does GNN Pretraining Help Molecular Representation?
    date: Jul 13, 2022
    date_iso: '2022-07-13'
    date_display: Jul 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7164
    - null
    metric_stds:
    - 0.0046
    - null
  - model: 3D Infomax
    model_plain: 3D Infomax
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.03364'
    title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer for Molecular
      Property Prediction'
    date: Jun 2, 2022
    date_iso: '2022-06-02'
    date_display: Jun 2022
    codebase_url: https://github.com/lihan97/KPGT
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.716
    - null
    metric_stds:
    - 0.013
    - null
  - model: Masking+Sup
    model_plain: Masking+Sup
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.03364'
    title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer for Molecular
      Property Prediction'
    date: Jun 2, 2022
    date_iso: '2022-06-02'
    date_display: Jun 2022
    codebase_url: https://github.com/lihan97/KPGT
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.715
    - null
    metric_stds:
    - 0.007
    - null
  - model: DeeperGCN
    model_plain: DeeperGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_iso: '2020-11-30'
    date_display: Nov 2020
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
    - 0.714
    metric_stds:
    - 0.005
    - 0.005
  - model: ContextPred
    model_plain: ContextPred
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.03364'
    title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer for Molecular
      Property Prediction'
    date: Jun 2, 2022
    date_iso: '2022-06-02'
    date_display: Jun 2022
    codebase_url: https://github.com/lihan97/KPGT
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.714
    - null
    metric_stds:
    - 0.018
    - null
  - model: EdgePred
    model_plain: EdgePred
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.03364'
    title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer for Molecular
      Property Prediction'
    date: Jun 2, 2022
    date_iso: '2022-06-02'
    date_display: Jun 2022
    codebase_url: https://github.com/lihan97/KPGT
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.712
    - null
    metric_stds:
    - 0.011
    - null
  - model: JOAO
    model_plain: JOAO
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.03364'
    title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer for Molecular
      Property Prediction'
    date: Jun 2, 2022
    date_iso: '2022-06-02'
    date_display: Jun 2022
    codebase_url: https://github.com/lihan97/KPGT
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.711
    - null
    metric_stds:
    - 0.014
    - null
  - model: scratch
    model_plain: scratch
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.04509'
    title: 'MoCL: Data-driven Molecular Fingerprint via Knowledge-aware Contrastive
      Learning from Molecular Graph'
    date: Jun 5, 2021
    date_iso: '2021-06-05'
    date_display: Jun 2021
    codebase_url: https://github.com/illidanlab/MoCL-DK
    published_conference: KDD 2021
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.71
    - null
    metric_stds:
    - null
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
    - 0.7095
    - null
    metric_stds:
    - 0.0027
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
    - 0.7095
    - null
    metric_stds:
    - 0.0027
    - null
  - model: GROVER
    model_plain: GROVER
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 100.0
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.03364'
    title: 'KPGT: Knowledge-Guided Pre-training of Graph Transformer for Molecular
      Property Prediction'
    date: Jun 2, 2022
    date_iso: '2022-06-02'
    date_display: Jun 2022
    codebase_url: https://github.com/lihan97/KPGT
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.708
    - null
    metric_stds:
    - 0.015
    - null
  - model: InfoGraph
    model_plain: InfoGraph
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
    - 0.705
    - null
    metric_stds:
    - null
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
    - 0.702
    - null
    metric_stds:
    - null
    - null
  - model: Context Prediction
    model_plain: Context Prediction
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2207.06010'
    title: Does GNN Pretraining Help Molecular Representation?
    date: Jul 13, 2022
    date_iso: '2022-07-13'
    date_display: Jul 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7018
    - null
    metric_stds:
    - 0.0044
    - null
  - model: GT
    model_plain: GT
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
    - 0.6999
    - null
    metric_stds:
    - 0.0037
    - null
  row_count: 299
  rows_json: /data/datasets/toxcast/scaffold-split-rows.json
  chart_json: /data/datasets/toxcast/scaffold-split-chart.json
  arch_counts:
    gnn: 195
    hybrid: 64
    graph_transformer: 7
    llm: 9
    walk: 0
    traditional: 16
  metric_counts:
  - 286
  - 21
  milestones: &id001
  - value: 0.749
    std: 0.002
    model: GINE w/ VN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: '2020-11-30'
  - value: 0.763
    std: null
    model: GeomGCL
    arxiv_id: '2109.11730'
    title: 'GeomGCL: Geometric Graph Contrastive Learning for Molecular Property Prediction'
    date: '2021-09-24'
  - value: 0.8073
    std: 0.0006
    model: SCI
    arxiv_id: '2311.04837'
    title: Identifying Semantic Component for Robust Molecular Property Prediction
    date: '2023-11-08'
  milestones_by_metric:
    ROC-AUC: *id001
    Accuracy:
    - value: 0.749
      std: 0.002
      model: GINE w/ VN
      arxiv_id: '2011.15069'
      title: Graph convolutions that can finally model local structure
      date: '2020-11-30'
---

