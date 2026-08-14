---
title: SIDER
slug: sider
benchmark: MoleculeNet
task_type: graph_classification
short_description: Multi-label classification of marketed drug side effects (27 tasks).
description: '**27-label graph classification** Multi-label classification of marketed
  drug side effects (27 tasks). SMILES and labels are fixed; molecular graph featurization
  is implementation-defined. Missing labels are not negatives; report split and featurizer.
  Evaluated by ROC-AUC.'
detailed_description:
  task: Multi-label classification of marketed drug side effects (27 tasks). The primary
    catalog metric is ROC-AUC.
  data: Multi-label classification of marketed drug side effects (27 tasks).
  features: MoleculeNet distributes SMILES and targets, not one mandatory graph featurization.
    A graph implementation normally derives atom and bond fields with RDKit or DeepChem;
    results depend on featurizer, salt handling, stereochemistry, and invalid-molecule
    policy.
  splits_and_evaluation: 'The catalog records these protocols or variants: Scaffold
    split. Evaluation uses ROC-AUC (higher is better). Exact masks or folds must come
    from the cited release.'
  quirks_and_pitfalls: Small samples, imbalance, missing assay labels, duplicate compounds,
    and scaffold leakage are common. Missing labels are not negatives. Always report
    split algorithm, featurizer, metric aggregation, and dataset version; random and
    scaffold results are not comparable.
sources:
- title: MoleculeNet benchmark
  arxiv_id: '1703.00564'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric SIDER loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
  kind: implementation_documentation
primary_metric: ROC-AUC
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
stats:
  num_graphs: 1427
  avg_nodes: 33.6
  avg_edges: 35.35
  num_classes: 27
  extra_stats:
    edge_feature_dim: 3
    edge_feature_type: categorical RDKit bond features in the PyG loader
    label_imbalance: 27-task multi-label adverse-reaction data with missingness and
      task-specific imbalance
    node_feature_dim: 9
    node_feature_type: categorical RDKit atom features in the PyG loader
    statistic_notes: Average edge count is half of the PyG bidirected edge-entry table
result_count: 303
best_model:
  model: KA-GAT
  value: 0.847
  metric: ROC-AUC
  arxiv_id: '2604.16586'
  paper_title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
    Prediction in the Foundation Model Era
papers:
- arxiv_id: '2604.16586'
  title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
    Prediction in the Foundation Model Era
  date_iso: '2026-04-17'
  venue: ''
- arxiv_id: '2602.05567'
  title: 'MAGPrompt: Message-Adaptive Graph Prompt Tuning for Graph Neural Networks'
  date_iso: '2026-02-05'
  venue: ''
- arxiv_id: '2510.07289'
  title: 'MolGA: Molecular Graph Adaptation with Pre-trained 2D Graph Encoder'
  date_iso: '2025-10-08'
  venue: ''
- arxiv_id: '2505.06283'
  title: 'Soft causal learning for generalized molecule property prediction: An environment
    modeling perspective'
  date_iso: '2025-05-07'
  venue: ''
- arxiv_id: '2503.04362'
  title: A Generalist Cross-Domain Molecular Learning Framework for Structure-Based
    Drug Discovery
  date_iso: '2025-03-06'
  venue: ''
- arxiv_id: '2501.01073'
  title: Graph Generative Pre-trained Transformer
  date_iso: '2025-01-02'
  venue: ICML 2025
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
- arxiv_id: '2410.10365'
  title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
    Samples'
  date_iso: '2024-10-14'
  venue: ''
- arxiv_id: '2406.00403'
  title: Dual-perspective Cross Contrastive Learning in Graph Transformers
  date_iso: '2024-06-01'
  venue: ''
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
- arxiv_id: '2404.15806'
  title: 'Where to Mask: Structure-Guided Masking for Graph Masked Autoencoders'
  date_iso: '2024-04-24'
  venue: IJCAI 2024
- arxiv_id: '2404.11568'
  title: On the Scalability of GNNs for Molecular Graphs
  date_iso: '2024-04-17'
  venue: NeurIPS 2024
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
- arxiv_id: '2311.01038'
  title: 'Better with Less: A Data-Active Perspective on Pre-Training Graph Neural
    Networks'
  date_iso: '2023-11-02'
  venue: NeurIPS 2023
- arxiv_id: '2310.14753'
  title: Rethinking Tokenizer and Decoder in Masked Graph Modeling for Molecules
  date_iso: '2023-10-23'
  venue: NeurIPS 2023
- arxiv_id: '2310.14216'
  title: 'UniMAP: Universal SMILES-Graph Representation Learning'
  date_iso: '2023-10-22'
  venue: ''
- arxiv_id: '2310.07351'
  title: Atom-Motif Contrastive Transformer for Molecular Property Prediction
  date_iso: '2023-10-11'
  venue: ''
- arxiv_id: '2309.10131'
  title: Deep Prompt Tuning for Graph Transformers
  date_iso: '2023-09-18'
  venue: ''
- arxiv_id: '2309.04589'
  title: Motif-aware Attribute Masking for Molecular Graph Pre-training
  date_iso: '2023-09-08'
  venue: ''
- arxiv_id: '2309.04062'
  title: '3D Denoisers are Good 2D Teachers: Molecular Pretraining via Denoising and
    Cross-Modal Distillation'
  date_iso: '2023-09-08'
  venue: AAAI 2023
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
- arxiv_id: '2209.15240'
  title: Universal Prompt Tuning for Graph Neural Networks
  date_iso: '2022-09-30'
  venue: NeurIPS 2022
- arxiv_id: '2209.15101'
  title: Improving Molecular Pretraining with Complementary Featurizations
  date_iso: '2022-09-29'
  venue: ''
- arxiv_id: '2208.04529'
  title: Motif-based Graph Representation Learning with Application to Chemical Molecules
  date_iso: '2022-08-09'
  venue: ''
- arxiv_id: '2207.08806'
  title: Unified 2D and 3D Pre-Training of Molecular Representations
  date_iso: '2022-07-14'
  venue: KDD 2022
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
- arxiv_id: '2202.09346'
  title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation and
    Decomposed Fragment Contrast
  date_iso: '2022-02-18'
  venue: ''
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
- arxiv_id: '2106.04509'
  title: 'MoCL: Data-driven Molecular Fingerprint via Knowledge-aware Contrastive
    Learning from Molecular Graph'
  date_iso: '2021-06-05'
  venue: KDD 2021
- arxiv_id: '1905.12265'
  title: Strategies for Pre-training Graph Neural Networks
  date_iso: '2019-05-29'
  venue: ICLR 2019
- arxiv_id: '1801.03226'
  title: Adaptive Graph Convolutional Neural Networks
  date_iso: '2018-01-10'
  venue: AAAI 2018
variants:
- slug: scaffold-split
  name: Scaffold split
  notes: ''
  is_standard: true
  primary_metric: ROC-AUC
  default_metric: ROC-AUC
  higher_is_better: true
  stats:
    num_graphs: 1427
    avg_nodes: 33.6
    avg_edges: 35.35
    num_classes: 27
    extra_stats:
      edge_feature_dim: 3
      edge_feature_type: categorical RDKit bond features in the PyG loader
      label_imbalance: 27-task multi-label adverse-reaction data with missingness
        and task-specific imbalance
      node_feature_dim: 9
      node_feature_type: categorical RDKit atom features in the PyG loader
      statistic_notes: Average edge count is half of the PyG bidirected edge-entry
        table
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
  - model: KA-GAT
    model_plain: KA-GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.847
    - null
    metric_stds:
    - 0.002
    - null
  - model: KA-GCN
    model_plain: KA-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.842
    - null
    metric_stds:
    - 0.001
    - null
  - model: GraphKAN
    model_plain: GraphKAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.837
    - null
    metric_stds:
    - 0.001
    - null
  - model: Mol-GDL
    model_plain: Mol-GDL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.831
    - null
    metric_stds:
    - 0.002
    - null
  - model: KA-GNNs
    model_plain: KA-GNNs
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.831
    - null
    metric_stds:
    - 0.004
    - null
  - model: MolLM
    model_plain: MolLM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.07249'
    title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent Molecular
      Property Prediction: A Systematic Survey'
    date: Feb 11, 2024
    date_iso: '2024-02-11'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: null
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.71
    - null
    metric_stds:
    - null
    - null
  - model: iMolCLR
    model_plain: iMolCLR
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09346'
    title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation
      and Decomposed Fragment Contrast
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.699
    - null
    metric_stds:
    - 0.015
    - null
  - model: GPF
    model_plain: GPF
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2209.15240'
    title: Universal Prompt Tuning for Graph Neural Networks
    date: Sep 30, 2022
    date_iso: '2022-09-30'
    date_display: Sep 2022
    codebase_url: https://github.com/zjunet/GPF
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6913
    - null
    metric_stds:
    - 0.0116
    - null
  - model: AttrMasking SUPT_hard
    model_plain: AttrMasking SUPT_hard
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6882
    - null
    metric_stds:
    - null
    - null
  - model: AttrMasking SUPT_soft
    model_plain: AttrMasking SUPT_soft
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6868
    - null
    metric_stds:
    - null
    - null
  - model: GPF-plus
    model_plain: GPF-plus
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2209.15240'
    title: Universal Prompt Tuning for Graph Neural Networks
    date: Sep 30, 2022
    date_iso: '2022-09-30'
    date_display: Sep 2022
    codebase_url: https://github.com/zjunet/GPF
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6865
    - null
    metric_stds:
    - 0.0072
    - null
  - model: AttrMasking GPF-plus
    model_plain: AttrMasking GPF-plus
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6853
    - null
    metric_stds:
    - null
    - null
  - model: AttrMasking GPF
    model_plain: AttrMasking GPF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6819
    - null
    metric_stds:
    - null
    - null
  - model: MolCLR
    model_plain: MolCLR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09346'
    title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation
      and Decomposed Fragment Contrast
    date: Feb 18, 2022
    date_iso: '2022-02-18'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.68
    - null
    metric_stds:
    - 0.011
    - null
  - model: SMPT
    model_plain: SMPT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.676
    - null
    metric_stds:
    - 0.05
    - null
  - model: UnifiedMolPretrain
    model_plain: UnifiedMolPretrain
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2207.08806'
    title: Unified 2D and 3D Pre-Training of Molecular Representations
    date: Jul 14, 2022
    date_iso: '2022-07-14'
    date_display: Jul 2022
    codebase_url: https://github.com/teslacool/UnifiedMolPretrain
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.674
    - null
    metric_stds:
    - 0.005
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
    - 0.672
    - null
    metric_stds:
    - 0.004
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
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.672
    - null
    metric_stds:
    - 0.004
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
    - 0.671
    - null
    metric_stds:
    - 0.011
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
    - 0.67
    - null
    metric_stds:
    - 0.005
    - null
  - model: 1B MolGPS
    model_plain: 1B MolGPS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 1000.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.11568'
    title: On the Scalability of GNNs for Molecular Graphs
    date: Apr 17, 2024
    date_iso: '2024-04-17'
    date_display: Apr 2024
    codebase_url: ''
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.67
    - null
    metric_stds:
    - null
    - null
  - model: EdgePred SUPT_soft
    model_plain: EdgePred SUPT_soft
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6695
    - null
    metric_stds:
    - null
    - null
  - model: EdgePred SUPT_hard
    model_plain: EdgePred SUPT_hard
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6685
    - null
    metric_stds:
    - null
    - null
  - model: N-Gram_RF
    model_plain: N-Gram_RF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
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
    - 0.668
    - null
    metric_stds:
    - 0.007
    - null
  - model: GROVER(large)
    model_plain: GROVER(large)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.14216'
    title: 'UniMAP: Universal SMILES-Graph Representation Learning'
    date: Oct 22, 2023
    date_iso: '2023-10-22'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.668
    - null
    metric_stds:
    - 0.001
    - null
  - model: N-GramRF
    model_plain: N-GramRF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: random_forest
    architecture_label: RF
    architecture_title: Random forest
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.668
    - null
    metric_stds:
    - 0.007
    - null
  - model: FT
    model_plain: FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2209.15240'
    title: Universal Prompt Tuning for Graph Neural Networks
    date: Sep 30, 2022
    date_iso: '2022-09-30'
    date_display: Sep 2022
    codebase_url: https://github.com/zjunet/GPF
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6677
    - null
    metric_stds:
    - 0.0013
    - null
  - model: AttrMasking FT
    model_plain: AttrMasking FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6677
    - null
    metric_stds:
    - null
    - null
  - model: EdgePred GPF
    model_plain: EdgePred GPF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6671
    - null
    metric_stds:
    - null
    - null
  - model: EdgePred GPF-plus
    model_plain: EdgePred GPF-plus
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6661
    - null
    metric_stds:
    - null
    - null
  - model: 3B MolGPS
    model_plain: 3B MolGPS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 3000.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.11568'
    title: On the Scalability of GNNs for Molecular Graphs
    date: Apr 17, 2024
    date_iso: '2024-04-17'
    date_display: Apr 2024
    codebase_url: ''
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.666
    - null
    metric_stds:
    - null
    - null
  - model: UniMAP
    model_plain: UniMAP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.14216'
    title: 'UniMAP: Universal SMILES-Graph Representation Learning'
    date: Oct 22, 2023
    date_iso: '2023-10-22'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.666
    - null
    metric_stds:
    - 0.008
    - null
  - model: ContextPred SUPT_soft
    model_plain: ContextPred SUPT_soft
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6648
    - null
    metric_stds:
    - null
    - null
  - model: ContextPred SUPT_hard
    model_plain: ContextPred SUPT_hard
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6637
    - null
    metric_stds:
    - null
    - null
  - model: ContextPred GPF-plus
    model_plain: ContextPred GPF-plus
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6632
    - null
    metric_stds:
    - null
    - null
  - model: GraphFP
    model_plain: GraphFP
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
    - 0.6593
    - null
    metric_stds:
    - 0.0309
    - null
  - model: CI-GCL
    model_plain: CI-GCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.01350'
    title: Community-Invariant Graph Contrastive Learning
    date: May 2, 2024
    date_iso: '2024-05-02'
    date_display: May 2024
    codebase_url: https://github.com/ShiyinTan/CI-GCL.git
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6591
    - null
    metric_stds:
    - 0.0082
    - null
  - model: Uni-Mol
    model_plain: Uni-Mol
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.659
    - null
    metric_stds:
    - 0.013
    - null
  - model: Infomax GPF-plus
    model_plain: Infomax GPF-plus
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6589
    - null
    metric_stds:
    - null
    - null
  - model: Infomax SUPT_soft
    model_plain: Infomax SUPT_soft
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6588
    - null
    metric_stds:
    - null
    - null
  - model: Infomax SUPT_hard
    model_plain: Infomax SUPT_hard
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6578
    - null
    metric_stds:
    - null
    - null
  - model: Infomax GPF
    model_plain: Infomax GPF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6564
    - null
    metric_stds:
    - null
    - null
  - model: N-Gram_XGB
    model_plain: N-Gram_XGB
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
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
    - 0.655
    - null
    metric_stds:
    - 0.007
    - null
  - model: N-GramXGB
    model_plain: N-GramXGB
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: boosting
    architecture_label: Boost
    architecture_title: Boosting ensemble
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/Zongru-Li/Survey-and-Benchmarks-of-DL-for-Molecular-Property-Prediction-in-the-Foundation-Model-Era
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.655
    - null
    metric_stds:
    - 0.007
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
    - 0.6534
    - null
    metric_stds:
    - 0.0017
    - null
  - model: ContextPred GPF
    model_plain: ContextPred GPF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.10380'
    title: Subgraph-level Universal Prompt Tuning
    date: Feb 16, 2024
    date_iso: '2024-02-16'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6531
    - null
    metric_stds:
    - null
    - null
  - model: Hu et al.
    model_plain: Hu et al.
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.09346'
    title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation
      and Decomposed Fragment Contrast
    date: Feb 18, 2022
    date_iso: '2022-02-18'
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
    - 0.652
    - null
    metric_stds:
    - 0.009
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
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6519
    - null
    metric_stds:
    - 0.0017
    - null
  - model: Node Prediction
    model_plain: Node Prediction
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
    - 0.6508
    - null
    metric_stds:
    - 0.0012
    - null
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
    - 0.649
    - null
    metric_stds:
    - 0.009
    - null
  row_count: 303
  rows_json: /data/datasets/sider/scaffold-split-rows.json
  chart_json: /data/datasets/sider/scaffold-split-chart.json
  arch_counts:
    gnn: 191
    hybrid: 73
    graph_transformer: 10
    llm: 5
    walk: 1
    traditional: 15
  metric_counts:
  - 290
  - 13
  milestones: &id001
  - value: 0.5921
    std: null
    model: AGCN
    arxiv_id: '1801.03226'
    title: Adaptive Graph Convolutional Neural Networks
    date: '2018-01-10'
  - value: 0.639
    std: 0.009
    model: GIN (Graph-level Supervised AttrMasking)
    arxiv_id: '1905.12265'
    title: Strategies for Pre-training Graph Neural Networks
    date: '2019-05-29'
  - value: 0.672
    std: 0.004
    model: ChemRL-GEM
    arxiv_id: '2106.06130'
    title: 'ChemRL-GEM: Geometry Enhanced Molecular Representation Learning for Property
      Prediction'
    date: '2021-06-11'
  - value: 0.699
    std: 0.015
    model: iMolCLR
    arxiv_id: '2202.09346'
    title: Improving Molecular Contrastive Learning via Faulty Negative Mitigation
      and Decomposed Fragment Contrast
    date: '2022-02-18'
  - value: 0.71
    std: null
    model: MolLM
    arxiv_id: '2402.07249'
    title: 'Impact of Domain Knowledge and Multi-Modality on Intelligent Molecular
      Property Prediction: A Systematic Survey'
    date: '2024-02-11'
  - value: 0.847
    std: 0.002
    model: KA-GAT
    arxiv_id: '2604.16586'
    title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
      Prediction in the Foundation Model Era
    date: '2026-04-17'
  milestones_by_metric:
    ROC-AUC: *id001
    Accuracy:
    - value: 0.6473
      std: 0.0042
      model: SpeGCL
      arxiv_id: '2410.10365'
      title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without
        Positive Samples'
      date: '2024-10-14'
---

