---
title: Tox21
slug: tox21
benchmark: MoleculeNet
task_type: graph_classification
short_description: Multi-task toxicity prediction (12 tasks) on NCI Tox21 challenge
  compounds.
description: '**12-task multi-label graph classification** Multi-task toxicity prediction
  (12 tasks) on NCI Tox21 challenge compounds. SMILES and labels are fixed; molecular
  graph featurization is implementation-defined. Evaluated by ROC-AUC.'
detailed_description:
  task: Multi-task toxicity prediction (12 tasks) on NCI Tox21 challenge compounds.
    The primary catalog metric is ROC-AUC.
  data: Multi-task toxicity prediction (12 tasks) on NCI Tox21 challenge compounds.
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
- title: PyTorch Geometric Tox21 loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
  kind: implementation_documentation
primary_metric: ROC-AUC
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.MoleculeNet.html
stats:
  num_graphs: 7831
  avg_nodes: 18.6
  avg_edges: 19.3
  num_classes: 12
  extra_stats:
    edge_feature_dim: 3
    edge_feature_type: categorical RDKit bond features in the PyG loader
    label_imbalance: 12-task multi-label toxicity assays with substantial missingness
      and task-specific imbalance
    node_feature_dim: 9
    node_feature_type: categorical RDKit atom features in the PyG loader
    statistic_notes: Average edge count is half of the PyG bidirected edge-entry table
result_count: 470
best_model:
  model: HIMP
  value: 0.874
  metric: ROC-AUC
  arxiv_id: '2011.15069'
  paper_title: Graph convolutions that can finally model local structure
papers:
- arxiv_id: '2604.16586'
  title: A Systematic Survey and Benchmark of Deep Learning for Molecular Property
    Prediction in the Foundation Model Era
  date_iso: '2026-04-17'
  venue: ''
- arxiv_id: '2602.01771'
  title: '<SO$ _k$>: One LLM Token for Explicit Graph Structural Understanding'
  date_iso: '2026-02-02'
  venue: ''
- arxiv_id: '2601.02530'
  title: 'Multi-scale Graph Autoregressive Modeling: Molecular Property Prediction
    via Next Token Prediction'
  date_iso: '2026-01-05'
  venue: ''
- arxiv_id: '2510.02565'
  title: On The Expressive Power of GNN Derivatives
  date_iso: '2025-10-02'
  venue: ''
- arxiv_id: '2503.04362'
  title: A Generalist Cross-Domain Molecular Learning Framework for Structure-Based
    Drug Discovery
  date_iso: '2025-03-06'
  venue: ''
- arxiv_id: '2502.16233'
  title: Graph Self-Supervised Learning with Learnable Structural and Positional Encodings
  date_iso: '2025-02-22'
  venue: WWW 2025
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
- arxiv_id: '2410.10365'
  title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
    Samples'
  date_iso: '2024-10-14'
  venue: ''
- arxiv_id: '2407.02013'
  title: 'DiGRAF: Diffeomorphic Graph-Adaptive Activation Function'
  date_iso: '2024-07-02'
  venue: NeurIPS 2024
- arxiv_id: '2406.11714'
  title: Scalable Expressiveness through Preprocessed Graph Perturbations
  date_iso: '2024-06-17'
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
- arxiv_id: '2312.08671'
  title: 'Permutation-Invariant graph partitioning: How graph neural networks capture
    structural interactions?'
  date_iso: '2023-12-14'
  venue: ''
- arxiv_id: '2312.04234'
  title: Graph Convolutions Enrich the Self-Attention in Transformers!
  date_iso: '2023-12-07'
  venue: NeurIPS 2023
- arxiv_id: '2311.01038'
  title: 'Better with Less: A Data-Active Perspective on Pre-Training Graph Neural
    Networks'
  date_iso: '2023-11-02'
  venue: NeurIPS 2023
- arxiv_id: '2310.20082'
  title: Efficient Subgraph GNNs by Learning Effective Selection Policies
  date_iso: '2023-10-30'
  venue: ICLR 2023
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
- arxiv_id: '2306.10767'
  title: 'P-tensors: a General Framework for Higher Order Message Passing in Subgraph
    Neural Networks'
  date_iso: '2023-06-19'
  venue: ''
- arxiv_id: '2305.19903'
  title: Improving Expressivity of GNNs with Subgraph-specific Factor Embedded Normalization
  date_iso: '2023-05-31'
  venue: KDD 2023
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
- arxiv_id: '2305.15747'
  title: Union Subgraph Neural Networks
  date_iso: '2023-05-25'
  venue: AAAI 2023
- arxiv_id: '2304.02806'
  title: 'Graph Mixture of Experts: Learning on Large-Scale Graphs with Explicit Diversity
    Modeling'
  date_iso: '2023-04-06'
  venue: NeurIPS 2023
- arxiv_id: '2212.13350'
  title: A Generalization of ViT/MLP-Mixer to Graphs
  date_iso: '2022-12-27'
  venue: ICML 2022
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
- arxiv_id: '2110.07875'
  title: Graph Neural Networks with Learnable Structural and Positional Representations
  date_iso: '2021-10-15'
  venue: ICLR 2021
- arxiv_id: '2110.07728'
  title: 16 Pre-training Molecular Graph Representation with 3D Geometry
  date_iso: '2021-10-07'
  venue: ICLR 2021
- arxiv_id: '2110.00987'
  title: Motif-based Graph Self-Supervised Learning for Molecular Property Prediction
  date_iso: '2021-10-03'
  venue: NeurIPS 2021
- arxiv_id: '2110.00577'
  title: Reconstruction for Powerful Graph Representations
  date_iso: '2021-10-01'
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
- arxiv_id: '2102.11533'
  title: Accurate Learning of Graph Representations with Graph Multiset Pooling
  date_iso: '2021-02-23'
  venue: ICLR 2021
- arxiv_id: '2011.15069'
  title: Graph convolutions that can finally model local structure
  date_iso: '2020-11-30'
  venue: ''
- arxiv_id: '2009.02027'
  title: Rethinking Graph Regularization for Graph Neural Networks
  date_iso: '2020-09-04'
  venue: AAAI 2020
- arxiv_id: '2002.09518'
  title: Memory-Based Graph Networks
  date_iso: '2020-02-21'
  venue: ICLR 2020
- arxiv_id: '1905.12265'
  title: Strategies for Pre-training Graph Neural Networks
  date_iso: '2019-05-29'
  venue: ICLR 2019
- arxiv_id: '1905.11577'
  title: Towards Interpretable Sparse Graph Representation Learning with Laplacian
    Pooling
  date_iso: '2019-05-28'
  venue: ''
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
    num_graphs: 7831
    avg_nodes: 18.6
    avg_edges: 19.3
    num_classes: 12
    extra_stats:
      edge_feature_dim: 3
      edge_feature_type: categorical RDKit bond features in the PyG loader
      label_imbalance: 12-task multi-label toxicity assays with substantial missingness
        and task-specific imbalance
      node_feature_dim: 9
      node_feature_type: categorical RDKit atom features in the PyG loader
      statistic_notes: Average edge count is half of the PyG bidirected edge-entry
        table
  metrics:
  - ROC-AUC
  - Accuracy
  - ROC
  - ROCAUC
  metric_display_names:
  - ROC-AUC
  - Accuracy
  - ROC
  - ROCAUC
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.874
    - 0.874
    - null
    - null
    metric_stds:
    - 0.005
    - 0.005
    - null
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.872
    - 0.872
    - null
    - null
    metric_stds:
    - 0.003
    - 0.003
    - null
    - null
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.87
    - 0.87
    - null
    - null
    metric_stds:
    - 0.004
    - 0.004
    - null
    - null
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.867
    - 0.867
    - null
    - null
    metric_stds:
    - 0.004
    - 0.004
    - null
    - null
  - model: GINE
    model_plain: GINE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.10767'
    title: 'P-tensors: a General Framework for Higher Order Message Passing in Subgraph
      Neural Networks'
    date: Jun 19, 2023
    date_iso: '2023-06-19'
    date_display: Jun 2023
    codebase_url: https://github.com/arhands/ptensors
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8668
    - null
    - null
    - null
    metric_stds:
    - 0.0077
    - null
    - null
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
    - 0.859
    - 0.859
    - null
    - null
    metric_stds:
    - 0.005
    - 0.005
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
    - 0.85
    - 0.85
    - null
    - null
    metric_stds:
    - 0.009
    - 0.009
    - null
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
    - 0.85
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
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
    arxiv_id: '2306.10767'
    title: 'P-tensors: a General Framework for Higher Order Message Passing in Subgraph
      Neural Networks'
    date: Jun 19, 2023
    date_iso: '2023-06-19'
    date_display: Jun 2023
    codebase_url: https://github.com/arhands/ptensors
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8495
    - null
    - null
    - null
    metric_stds:
    - 0.0058
    - null
    - null
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
    - 0.848
    - null
    - null
    - null
    metric_stds:
    - 0.013
    - null
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
    - 0.848
    - null
    - null
    - null
    metric_stds:
    - null
    - null
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
    - 0.844
    - null
    - null
    - null
    metric_stds:
    - 0.004
    - null
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
    - 0.843
    - null
    - null
    - null
    metric_stds:
    - 0.004
    - null
    - null
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
    - 0.84
    - 0.84
    - null
    - null
    metric_stds:
    - 0.004
    - 0.004
    - null
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
    - 0.84
    - null
    - null
    - null
    metric_stds:
    - 0.023
    - null
    - null
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.838
    - null
    - null
    - null
    metric_stds:
    - 0.017
    - null
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
    - 0.838
    - null
    - null
    - null
    metric_stds:
    - null
    - null
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
    - 0.836
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
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
    - 0.835
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: lapool
    model_plain: lapool
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1905.11577'
    title: Towards Interpretable Sparse Graph Representation Learning with Laplacian
      Pooling
    date: May 28, 2019
    date_iso: '2019-05-28'
    date_display: May 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8342
    - null
    - null
    - null
    metric_stds:
    - 0.0097
    - null
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
    - 0.834
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
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
    - 0.832
    - null
    - null
    - null
    metric_stds:
    - 0.009
    - null
    - null
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
    - 0.832
    - null
    - null
    - null
    metric_stds:
    - 0.012
    - null
    - null
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
    - 0.831
    - 0.831
    - null
    - null
    metric_stds:
    - 0.004
    - 0.004
    - null
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
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_iso: '2020-02-21'
    date_display: Feb 2020
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.829
    - null
    - null
    - null
    metric_stds:
    - 0.006
    - null
    - null
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
    arxiv_id: '1905.11577'
    title: Towards Interpretable Sparse Graph Representation Learning with Laplacian
      Pooling
    date: May 28, 2019
    date_iso: '2019-05-28'
    date_display: May 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.829
    - null
    - null
    - null
    metric_stds:
    - 0.0069
    - null
    - null
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
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.828
    - null
    - null
    - null
    metric_stds:
    - 0.013
    - null
    - null
    - null
  - model: MemGNN
    model_plain: MemGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_iso: '2020-02-21'
    date_display: Feb 2020
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.828
    - null
    - null
    - null
    metric_stds:
    - 0.004
    - null
    - null
    - null
  - model: CamS-LLaMA
    model_plain: CamS-LLaMA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 100.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2601.02530'
    title: 'Multi-scale Graph Autoregressive Modeling: Molecular Property Prediction
      via Next Token Prediction'
    date: Jan 5, 2026
    date_iso: '2026-01-05'
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
    - 0.827
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: OFA
    model_plain: OFA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2406.10727'
    title: 'Text-space Graph Foundation Models: Comprehensive Benchmarks and New Insights'
    date: Jun 15, 2024
    date_iso: '2024-06-15'
    date_display: Jun 2024
    codebase_url: https://github.com/CurryTang/TSGFM
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.825
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.824
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: DiffPool
    model_plain: DiffPool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1905.11577'
    title: Towards Interpretable Sparse Graph Representation Learning with Laplacian
      Pooling
    date: May 28, 2019
    date_iso: '2019-05-28'
    date_display: May 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8237
    - null
    - null
    - null
    metric_stds:
    - 0.009
    - null
    - null
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
    - 0.823
    - null
    - null
    - null
    metric_stds:
    - 0.022
    - null
    - null
    - null
  - model: Kernel SVM
    model_plain: Kernel SVM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_iso: '2020-02-21'
    date_display: Feb 2020
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.822
    - null
    - null
    - null
    metric_stds:
    - 0.006
    - null
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
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_iso: '2020-02-21'
    date_display: Feb 2020
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.82
    - null
    - null
    - null
    metric_stds:
    - 0.01
    - null
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
    - 0.8193
    - null
    - null
    - null
    metric_stds:
    - 0.0179
    - null
    - null
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
    - 0.818
    - null
    - null
    - null
    metric_stds:
    - 0.025
    - null
    - null
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
    - 0.8171
    - null
    - null
    - null
    metric_stds:
    - 0.0179
    - null
    - null
    - null
  - model: Infomax
    model_plain: Infomax
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
    - 0.816
    - null
    - null
    - null
    metric_stds:
    - 0.021
    - null
    - null
    - null
  - model: Graph U-Net
    model_plain: Graph U-Net
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '1905.11577'
    title: Towards Interpretable Sparse Graph Representation Learning with Laplacian
      Pooling
    date: May 28, 2019
    date_iso: '2019-05-28'
    date_display: May 2019
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8141
    - null
    - null
    - null
    metric_stds:
    - 0.006
    - null
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
    - 0.813
    - null
    - null
    - null
    metric_stds:
    - 0.01
    - null
    - null
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
    - 0.8113
    - null
    - null
    - null
    metric_stds:
    - 0.0239
    - null
    - null
    - null
  - model: Bypass
    model_plain: Bypass
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_iso: '2020-02-21'
    date_display: Feb 2020
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.81
    - null
    - null
    - null
    metric_stds:
    - 0.013
    - null
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
    - 0.8094
    - null
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
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
    - 0.8094
    - null
    - null
    - null
    metric_stds:
    - 0.0017
    - null
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
    - 0.809
    - null
    - null
    - null
    metric_stds:
    - null
    - null
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
    - 0.8076
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
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
    - 0.807
    - null
    - null
    - null
    metric_stds:
    - 0.02
    - null
    - null
    - null
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 2.8
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.807
    - null
    - null
    - null
    metric_stds:
    - 0.011
    - null
    - null
    - null
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
    - 0.806
    - null
    - null
    - null
    metric_stds:
    - 0.012
    - null
    - null
    - null
  row_count: 470
  rows_json: /data/datasets/tox21/scaffold-split-rows.json
  chart_json: /data/datasets/tox21/scaffold-split-chart.json
  arch_counts:
    gnn: 281
    hybrid: 94
    graph_transformer: 16
    llm: 14
    walk: 1
    traditional: 27
  metric_counts:
  - 428
  - 46
  - 3
  - 2
  milestones: &id001
  - value: 0.8016
    std: null
    model: AGCN
    arxiv_id: '1801.03226'
    title: Adaptive Graph Convolutional Neural Networks
    date: '2018-01-10'
  - value: 0.8342
    std: 0.0097
    model: lapool
    arxiv_id: '1905.11577'
    title: Towards Interpretable Sparse Graph Representation Learning with Laplacian
      Pooling
    date: '2019-05-28'
  - value: 0.874
    std: 0.005
    model: HIMP
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: '2020-11-30'
  milestones_by_metric:
    ROC-AUC: *id001
    Accuracy:
    - value: 0.874
      std: 0.005
      model: HIMP
      arxiv_id: '2011.15069'
      title: Graph convolutions that can finally model local structure
      date: '2020-11-30'
    - value: 0.9224
      std: 0.0059
      model: GraphSNN
      arxiv_id: '2305.15747'
      title: Union Subgraph Neural Networks
      date: '2023-05-25'
    ROC:
    - value: 0.7545
      std: 0.011
      model: GraphSNN
      arxiv_id: '2312.08671'
      title: 'Permutation-Invariant graph partitioning: How graph neural networks
        capture structural interactions?'
      date: '2023-12-14'
    ROCAUC:
    - value: 0.7895
      std: 0.0069
      model: Graph-ViT + GFSA
      arxiv_id: '2312.04234'
      title: Graph Convolutions Enrich the Self-Attention in Transformers!
      date: '2023-12-07'
---

