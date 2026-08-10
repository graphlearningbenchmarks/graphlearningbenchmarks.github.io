---
title: ogbg-molhiv
slug: ogbg-molhiv
benchmark: OGB
task_type: graph_classification
description: 'Binary graph classification on HIV inhibition (molecules). Highly imbalanced
  dataset: only ~3.5% of molecules are active (HIV inhibitors). Evaluated with ROC-AUC
  to account for class imbalance.'
primary_metric: ROC-AUC
higher_is_better: true
pyg_url: https://ogb.stanford.edu/docs/leader_graphprop/#ogbg-molhiv
stats:
  num_graphs: 41127
  avg_nodes: 25.5
  avg_edges: 27.5
  num_classes: 2
result_count: 370
best_model:
  model: Multi-RF Fusion with Multi-GNN Blending
  value: 0.8476
  metric: ROC-AUC
  arxiv_id: '2603.20724'
  paper_title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
papers:
- arxiv_id: '2606.00757'
  title: 'RADE: Random Add-Drop Edge as a Regularizer'
  date_iso: '2026-05-30'
  venue: ICML 2026
- arxiv_id: '2604.17324'
  title: 'SigGate-GT: Taming Over-Smoothing in Graph Transformers via Sigmoid-Gated
    Attention'
  date_iso: '2026-04-19'
  venue: ''
- arxiv_id: '2603.20724'
  title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
  date_iso: '2026-03-21'
  venue: ''
- arxiv_id: '2510.04567'
  title: 'GILT: An LLM-Free, Tuning-Free Graph Foundational Model for In-Context Learning'
  date_iso: '2025-10-06'
  venue: ICML 2025
- arxiv_id: '2509.24886'
  title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
    Networks
  date_iso: '2025-09-29'
  venue: ''
- arxiv_id: '2506.05814'
  title: Positional Encoding meets Persistent Homology on Graphs
  date_iso: '2025-06-06'
  venue: ICML 2025
- arxiv_id: '2506.06127'
  title: Flow-Attentional Graph Neural Networks
  date_iso: '2025-06-06'
  venue: TMLR 2025
- arxiv_id: '2505.18289'
  title: Convexified Message-Passing Graph Neural Networks
  date_iso: '2025-05-23'
  venue: ''
- arxiv_id: '2502.16233'
  title: Graph Self-Supervised Learning with Learnable Structural and Positional Encodings
  date_iso: '2025-02-22'
  venue: WWW 2025
- arxiv_id: '2502.07968'
  title: Generative Risk Minimization for Out-of-Distribution Generalization on Graphs
  date_iso: '2025-02-11'
  venue: TMLR 2025
- arxiv_id: '2501.04102'
  title: Enhancing Distribution and Label Consistency for Graph Out-of-Distribution
    Generalization
  date_iso: '2024-12-09'
  venue: ''
- arxiv_id: '2410.22372'
  title: A Hierarchical Language Model For Interpretable Graph Reasoning
  date_iso: '2024-10-29'
  venue: ''
- arxiv_id: '2408.07340'
  title: Towards Few-shot Self-explaining Graph Neural Networks
  date_iso: '2024-08-14'
  venue: ''
- arxiv_id: '2407.04236'
  title: Graph Pooling via Ricci Flow
  date_iso: '2024-07-05'
  venue: TMLR 2024
- arxiv_id: '2407.02013'
  title: 'DiGRAF: Diffeomorphic Graph-Adaptive Activation Function'
  date_iso: '2024-07-02'
  venue: NeurIPS 2024
- arxiv_id: '2406.12059'
  title: A Scalable and Effective Alternative to Graph Transformers
  date_iso: '2024-06-17'
  venue: AAAI 2024
- arxiv_id: '2406.11714'
  title: Scalable Expressiveness through Preprocessed Graph Perturbations
  date_iso: '2024-06-17'
  venue: ''
- arxiv_id: '2406.07955'
  title: How Interpretable Are Interpretable Graph Neural Networks?
  date_iso: '2024-06-12'
  venue: ICML 2024
- arxiv_id: '2405.19779'
  title: Automatic Graph Topology-Aware Transformer
  date_iso: '2024-05-30'
  venue: ''
- arxiv_id: '2404.13344'
  title: 'GRANOLA: Adaptive Normalization for Graph Neural Networks'
  date_iso: '2024-04-20'
  venue: NeurIPS 2024
- arxiv_id: '2404.09774'
  title: 'RandAlign: A Parameter-Free Method for Regularizing Graph Convolutional
    Networks'
  date_iso: '2024-04-15'
  venue: ''
- arxiv_id: '2403.12529'
  title: Contextualized Messages Boost Graph Representations
  date_iso: '2024-03-19'
  venue: TMLR 2024
- arxiv_id: '2402.16402'
  title: Graph Learning with Distributional Edge Layouts
  date_iso: '2024-02-26'
  venue: ''
- arxiv_id: '2402.04924'
  title: 'Two Trades are not Baffled: Condensing Graph via Crafting Rational Gradient
    Matching'
  date_iso: '2024-02-07'
  venue: ''
- arxiv_id: '2401.17752'
  title: 'PF-GNN: Differentiable particle filtering based approximation of universal
    graph representations'
  date_iso: '2024-01-31'
  venue: ICLR 2024
- arxiv_id: '2312.08671'
  title: 'Permutation-Invariant graph partitioning: How graph neural networks capture
    structural interactions?'
  date_iso: '2023-12-14'
  venue: ''
- arxiv_id: '2310.20082'
  title: Efficient Subgraph GNNs by Learning Effective Selection Policies
  date_iso: '2023-10-30'
  venue: ICLR 2023
- arxiv_id: '2310.19142'
  title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
  date_iso: '2023-10-29'
  venue: NeurIPS 2023
- arxiv_id: '2310.17132'
  title: 'BiKT: Unleashing the potential of GNNs via Bi-directional Knowledge Transfer'
  date_iso: '2023-10-26'
  venue: ''
- arxiv_id: '2310.01794'
  title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based Gnn Explainers
    through In-depth Benchmarking'
  date_iso: '2023-10-03'
  venue: ICLR 2023
- arxiv_id: '2309.10131'
  title: Deep Prompt Tuning for Graph Transformers
  date_iso: '2023-09-18'
  venue: ''
- arxiv_id: '2309.00738'
  title: Rethinking the Power of Graph Canonization in Graph Representation Learning
    with Stability
  date_iso: '2023-09-01'
  venue: ''
- arxiv_id: '2308.06838'
  title: 'Weisfeiler and Lehman Go Paths: Learning Topological Features via Path Complexes'
  date_iso: '2023-08-13'
  venue: AAAI 2023
- arxiv_id: '2306.15963'
  title: Fused Gromov-Wasserstein Graph Mixup for Graph-level Classifications
  date_iso: '2023-06-28'
  venue: NeurIPS 2023
- arxiv_id: '2306.06788'
  title: Graph Mixup with Soft Alignments
  date_iso: '2023-06-11'
  venue: ICML 2023
- arxiv_id: '2305.19903'
  title: Improving Expressivity of GNNs with Subgraph-specific Factor Embedded Normalization
  date_iso: '2023-05-31'
  venue: KDD 2023
- arxiv_id: '2305.15747'
  title: Union Subgraph Neural Networks
  date_iso: '2023-05-25'
  venue: AAAI 2023
- arxiv_id: '2305.15066'
  title: 'GPT4Graph: Can Large Language Models Understand Graph Structured Data? An
    Empirical Evaluation and Benchmarking'
  date_iso: '2023-05-24'
  venue: ''
- arxiv_id: '2305.04963'
  title: 'From Relational Pooling to Subgraph GNNs: A Universal Framework for More
    Expressive Graph Neural Networks'
  date_iso: '2023-05-08'
  venue: ICML 2023
- arxiv_id: '2304.02806'
  title: 'Graph Mixture of Experts: Learning on Large-Scale Graphs with Explicit Diversity
    Modeling'
  date_iso: '2023-04-06'
  venue: NeurIPS 2023
- arxiv_id: '2303.10576'
  title: An Efficient Subgraph GNN with Provable Substructure Counting Power
  date_iso: '2023-03-19'
  venue: KDD 2023
- arxiv_id: '2302.07090'
  title: A Complete Expressiveness Hierarchy for Subgraph GNNs via Subgraph Weisfeiler-Lehman
    Tests
  date_iso: '2023-02-14'
  venue: ICML 2023
- arxiv_id: '2301.11956'
  title: On the Connection Between MPNN and Graph Transformer
  date_iso: '2023-01-27'
  venue: ICML 2023
- arxiv_id: '2211.15335'
  title: 'You Can Have Better Graph Neural Networks by Not Training Weights at All:
    Finding Untrained GNNs Tickets'
  date_iso: '2022-11-28'
  venue: LoG 2022
- arxiv_id: '2211.06605'
  title: Comprehensive Analysis of Over-smoothing in Graph Neural Networks from Markov
    Chains Perspective
  date_iso: '2022-11-12'
  venue: ''
- arxiv_id: '2210.13978'
  title: Boosting the Cycle Counting Power of Graph Neural Networks with I$^2$-GNNs
  date_iso: '2022-10-22'
  venue: ICLR 2022
- arxiv_id: '2210.02636'
  title: Geodesic Graph Neural Network for Efficient Graph Representation Learning
  date_iso: '2022-10-06'
  venue: NeurIPS 2022
- arxiv_id: '2210.02997'
  title: Expander Graph Propagation
  date_iso: '2022-10-06'
  venue: LoG 2022
- arxiv_id: '2209.06560'
  title: Graph Contrastive Learning with Personalized Augmentation
  date_iso: '2022-09-14'
  venue: ''
- arxiv_id: '2208.04529'
  title: Motif-based Graph Representation Learning with Application to Chemical Molecules
  date_iso: '2022-08-09'
  venue: ''
- arxiv_id: '2206.11010'
  title: Agent-based Graph Neural Networks
  date_iso: '2022-06-22'
  venue: ICLR 2022
- arxiv_id: '2206.07746'
  title: Condensing Graphs via One-Step Gradient Matching
  date_iso: '2022-06-15'
  venue: KDD 2022
- arxiv_id: '2206.02886'
  title: Graph Rationalization with Environment-based Augmentations
  date_iso: '2022-06-06'
  venue: KDD 2022
- arxiv_id: '2205.15746'
  title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
    Learning
  date_iso: '2022-05-31'
  venue: ICML 2022
- arxiv_id: '2205.11678'
  title: Compressing Deep Graph Neural Networks via Adversarial Knowledge Distillation
  date_iso: '2022-05-24'
  venue: KDD 2022
- arxiv_id: '2205.15068'
  title: Embedding Graphs on Grassmann Manifold
  date_iso: '2022-05-01'
  venue: ''
- arxiv_id: '2202.13248'
  title: Automated Data Augmentations for Graph Classification
  date_iso: '2022-02-26'
  venue: ICLR 2022
- arxiv_id: '2202.08455'
  title: 'Transformer for Graphs: An Overview from Architecture Perspective'
  date_iso: '2022-02-17'
  venue: ''
- arxiv_id: '2202.00529'
  title: Molecular Representation Learning via Heterogeneous Motif Graph Neural Networks
  date_iso: '2022-02-01'
  venue: ICML 2022
- arxiv_id: '2201.12787'
  title: 'GRPE: Relative Positional Encoding for Graph Transformer'
  date_iso: '2022-01-30'
  venue: ''
- arxiv_id: '2201.12872'
  title: Discovering Invariant Rationales for Graph Neural Networks
  date_iso: '2022-01-30'
  venue: ICLR 2022
- arxiv_id: '2201.09332'
  title: How Expressive are Transformers in Spectral Domain for Graphs?
  date_iso: '2022-01-23'
  venue: TMLR 2022
- arxiv_id: '2110.07141'
  title: 'SoGCN: Second-Order Graph Convolutional Networks'
  date_iso: '2021-10-14'
  venue: ''
- arxiv_id: '2110.00577'
  title: Reconstruction for Powerful Graph Representations
  date_iso: '2021-10-01'
  venue: NeurIPS 2021
- arxiv_id: '2104.01481'
  title: Do We Need Anisotropic Graph Neural Networks?
  date_iso: '2021-04-03'
  venue: ICLR 2021
- arxiv_id: '2103.16584'
  title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
  date_iso: '2021-03-30'
  venue: ''
- arxiv_id: '2103.01488'
  title: 'Multi-Level Attention Pooling for Graph Neural Networks: Unifying Graph
    Representations with Multiple Localities'
  date_iso: '2021-03-02'
  venue: ''
- arxiv_id: '2102.06986'
  title: How Framelets Enhance Graph Neural Networks
  date_iso: '2021-02-13'
  venue: ICML 2021
- arxiv_id: '2011.15069'
  title: Graph convolutions that can finally model local structure
  date_iso: '2020-11-30'
  venue: ''
- arxiv_id: '2009.03294'
  title: 'GraphNorm: A Principled Approach to Accelerating Graph Neural Network Training'
  date_iso: '2020-09-07'
  venue: ICML 2020
- arxiv_id: '2009.02027'
  title: Rethinking Graph Regularization for Graph Neural Networks
  date_iso: '2020-09-04'
  venue: AAAI 2020
- arxiv_id: '2006.09430'
  title: Wasserstein Embedding for Graph Learning
  date_iso: '2020-06-16'
  venue: ICLR 2020
variants:
- slug: standard-split
  name: Standard split
  notes: OGB scaffold split; use the official default task and features.
  is_standard: true
  primary_metric: ROC-AUC
  default_metric: ROC-AUC
  higher_is_better: true
  stats:
    num_graphs: 41127
    avg_nodes: 25.5
    avg_edges: 27.5
    num_classes: 2
  metrics:
  - ROC-AUC
  - AUC
  - AUC-ROC
  - Accuracy
  - Size
  - Sparsity
  - Suffic.
  metric_display_names:
  - ROC-AUC
  - AUC
  - AUC-ROC
  - Accuracy
  - Size
  - Sparsity
  - Suffic.
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: Multi-RF Fusion with Multi-GNN Blending
    model_plain: Multi-RF Fusion with Multi-GNN Blending
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_iso: '2026-03-21'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8476
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
  - model: HyperFusion
    model_plain: HyperFusion
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_iso: '2026-03-21'
    date_display: Mar 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8475
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0003
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PAS+FPs
    model_plain: PAS+FPs
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: Mar 21, 2026
    date_iso: '2026-03-21'
    date_display: Mar 2026
    codebase_url: ''
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
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0015
    - null
    - null
    - null
    - null
    - null
    - null
  - model: HIG with DeeperGCN
    model_plain: HIG with DeeperGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.11678'
    title: Compressing Deep Graph Neural Networks via Adversarial Knowledge Distillation
    date: May 24, 2022
    date_iso: '2022-05-24'
    date_display: May 2022
    codebase_url: https://github.com/TencentYoutuResearch/HIG-GraphClassification
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8403
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0021
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SigGate-GT
    model_plain: SigGate-GT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    - 0.8247
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0063
    - null
    - null
    - null
    - null
    - null
    - null
  - model: two augmentation methods based on environment subgraphs
    model_plain: two augmentation methods based on environment subgraphs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8191
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.024
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GRPE-Standard
    model_plain: GRPE-Standard
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_iso: '2022-01-30'
    date_display: Jan 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8139
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0049
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GSN + Granola
    model_plain: GSN + Granola
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.13344'
    title: 'GRANOLA: Adaptive Normalization for Graph Neural Networks'
    date: Apr 20, 2024
    date_iso: '2024-04-20'
    date_display: Apr 2024
    codebase_url: https://github.com/MosheEliasof/GRANOLA
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8112
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0079
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GRM
    model_plain: GRM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.07968'
    title: Generative Risk Minimization for Out-of-Distribution Generalization on
      Graphs
    date: Feb 11, 2025
    date_iso: '2025-02-11'
    date_display: Feb 2025
    codebase_url: https://github.com/SongW-SW/GRM
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8102
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
  - model: OOD-GNN
    model_plain: OOD-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8096
    - 0.7799
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0132
    - 0.0078
    - null
    - null
    - null
    - null
    - null
  - model: CIN
    model_plain: CIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.13978'
    title: Boosting the Cycle Counting Power of Graph Neural Networks with I$^2$-GNNs
    date: Oct 22, 2022
    date_iso: '2022-10-22'
    date_display: Oct 2022
    codebase_url: https://github.com/GraphPKU/I2GNN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8094
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0057
    - null
    - null
    - null
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
    - 0.809
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.016
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Exphormer
    model_plain: Exphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    - 0.8075
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0094
    - null
    - null
    - null
    - null
    - null
    - null
  - model: EGT-Large
    model_plain: EGT-Large
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 110.8
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_iso: '2022-01-30'
    date_display: Jan 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.806
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0065
    - null
    - null
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
    - 0.806
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.007
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GMT-sam
    model_plain: GMT-sam
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.07955'
    title: How Interpretable Are Interpretable Graph Neural Networks?
    date: Jun 12, 2024
    date_iso: '2024-06-12'
    date_display: Jun 2024
    codebase_url: https://github.com/LFhase/GMT
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8058
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0083
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GALA
    model_plain: GALA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.07968'
    title: Generative Risk Minimization for Out-of-Distribution Generalization on
      Graphs
    date: Feb 11, 2025
    date_iso: '2025-02-11'
    date_display: Feb 2025
    codebase_url: https://github.com/SongW-SW/GRM
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8053
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
  - model: Graphormer-FLAG
    model_plain: Graphormer-FLAG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 47.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_iso: '2022-01-30'
    date_display: Jan 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8051
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0053
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Graphormer
    model_plain: Graphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2201.09332'
    title: How Expressive are Transformers in Spectral Domain for Graphs?
    date: Jan 23, 2022
    date_iso: '2022-01-23'
    date_display: Jan 2022
    codebase_url: ''
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8051
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0053
    - null
    - null
    - null
    - null
    - null
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
    - 0.805
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.005
    - null
    - null
    - null
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
    - 0.804
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.021
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GSN
    model_plain: GSN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.13978'
    title: Boosting the Cycle Counting Power of Graph Neural Networks with I$^2$-GNNs
    date: Oct 22, 2022
    date_iso: '2022-10-22'
    date_display: Oct 2022
    codebase_url: https://github.com/GraphPKU/I2GNN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8039
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.009
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DGSN
    model_plain: DGSN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.02636'
    title: Geodesic Graph Neural Network for Efficient Graph Representation Learning
    date: Oct 6, 2022
    date_iso: '2022-10-06'
    date_display: Oct 2022
    codebase_url: https://github.com/woodcutter1998/gdgnn
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8039
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.009
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Directional GSN
    model_plain: Directional GSN
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
    - 0.8039
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.009
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DiGRAF
    model_plain: DiGRAF
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.02013'
    title: 'DiGRAF: Diffeomorphic Graph-Adaptive Activation Function'
    date: Jul 2, 2024
    date_iso: '2024-07-02'
    date_display: Jul 2024
    codebase_url: https://github.com/ipsitmantri/DiGRAF
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8028
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0144
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GPS + RandAlign
    model_plain: GPS + RandAlign
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.09774'
    title: 'RandAlign: A Parameter-Free Method for Regularizing Graph Convolutional
      Networks'
    date: Apr 15, 2024
    date_iso: '2024-04-15'
    date_display: Apr 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8021
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0305
    - null
    - null
    - null
    - null
    - null
    - null
  - model: novel method to learn motif-level feature embedding
    model_plain: novel method to learn motif-level feature embedding
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.00529'
    title: Molecular Representation Learning via Heterogeneous Motif Graph Neural
      Networks
    date: Feb 1, 2022
    date_iso: '2022-02-01'
    date_display: Feb 2022
    codebase_url: https://github.com/ZhaoningYu1996/HM-GNN
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.802
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0118
    - null
    - null
    - null
    - null
    - null
    - null
  - model: A-NLSF
    model_plain: A-NLSF
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: Sep 29, 2025
    date_iso: '2025-09-29'
    date_display: Sep 2025
    codebase_url: https://github.com/ywelld/_ac
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8019
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0152
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PF-GNN
    model_plain: PF-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.02636'
    title: Geodesic Graph Neural Network for Efficient Graph Representation Learning
    date: Oct 6, 2022
    date_iso: '2022-10-06'
    date_display: Oct 2022
    codebase_url: https://github.com/woodcutter1998/gdgnn
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8015
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0068
    - null
    - null
    - null
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
    - 0.801
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.015
    - null
    - null
    - null
    - null
    - null
    - null
  - model: CIN-Small
    model_plain: CIN-Small
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.13978'
    title: Boosting the Cycle Counting Power of Graph Neural Networks with I$^2$-GNNs
    date: Oct 22, 2022
    date_iso: '2022-10-22'
    date_display: Oct 2022
    codebase_url: https://github.com/GraphPKU/I2GNN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8005
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0104
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GMT-lin
    model_plain: GMT-lin
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.07955'
    title: How Interpretable Are Interpretable Graph Neural Networks?
    date: Jun 12, 2024
    date_iso: '2024-06-12'
    date_display: Jun 2024
    codebase_url: https://github.com/LFhase/GMT
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8005
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0071
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SUN (EGO)
    model_plain: SUN (EGO)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.13978'
    title: Boosting the Cycle Counting Power of Graph Neural Networks with I$^2$-GNNs
    date: Oct 22, 2022
    date_iso: '2022-10-22'
    date_display: Oct 2022
    codebase_url: https://github.com/GraphPKU/I2GNN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8003
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0055
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SUN
    model_plain: SUN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.526
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.07090'
    title: A Complete Expressiveness Hierarchy for Subgraph GNNs via Subgraph Weisfeiler-Lehman
      Tests
    date: Feb 14, 2023
    date_iso: '2023-02-14'
    date_display: Feb 2023
    codebase_url: https://github.com/subgraph23/SWL
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8003
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0055
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SUN(EGO)
    model_plain: SUN(EGO)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.04963'
    title: 'From Relational Pooling to Subgraph GNNs: A Universal Framework for More
      Expressive Graph Neural Networks'
    date: May 8, 2023
    date_iso: '2023-05-08'
    date_display: May 2023
    codebase_url: ''
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8003
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0055
    - null
    - null
    - null
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
    - 0.799
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.01
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GSAT
    model_plain: GSAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.07955'
    title: How Interpretable Are Interpretable Graph Neural Networks?
    date: Jun 12, 2024
    date_iso: '2024-06-12'
    date_display: Jun 2024
    codebase_url: https://github.com/LFhase/GMT
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7982
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0067
    - null
    - null
    - null
    - null
    - null
    - null
  - model: EGTAS
    model_plain: EGTAS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2405.19779'
    title: Automatic Graph Topology-Aware Transformer
    date: May 30, 2024
    date_iso: '2024-05-30'
    date_display: May 2024
    codebase_url: https://github.com/xiaofangxd/EGTAS
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7981
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0117
    - null
    - null
    - null
    - null
    - null
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
    - 0.798
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.02
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DLG
    model_plain: DLG
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2501.04102'
    title: Enhancing Distribution and Label Consistency for Graph Out-of-Distribution
      Generalization
    date: Dec 9, 2024
    date_iso: '2024-12-09'
    date_display: Dec 2024
    codebase_url: https://github.com/SongW-SW/DLG
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.798
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0178
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PiPE
    model_plain: PiPE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2506.05814'
    title: Positional Encoding meets Persistent Homology on Graphs
    date: Jun 6, 2025
    date_iso: '2025-06-06'
    date_display: Jun 2025
    codebase_url: https://github.com/Aalto-QuML/PIPE
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.798
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.004
    - null
    - null
    - null
    - null
    - null
    - null
  - model: CIGA
    model_plain: CIGA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2501.04102'
    title: Enhancing Distribution and Label Consistency for Graph Out-of-Distribution
      Generalization
    date: Dec 9, 2024
    date_iso: '2024-12-09'
    date_display: Dec 2024
    codebase_url: https://github.com/SongW-SW/DLG
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.797
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0192
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DGN
    model_plain: DGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.114
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.797
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0097
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GNNAK+
    model_plain: GNNAK+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.13978'
    title: Boosting the Cycle Counting Power of Graph Neural Networks with I$^2$-GNNs
    date: Oct 22, 2022
    date_iso: '2022-10-22'
    date_display: Oct 2022
    codebase_url: https://github.com/GraphPKU/I2GNN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7961
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0119
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GNN-AK+
    model_plain: GNN-AK+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.07090'
    title: A Complete Expressiveness Hierarchy for Subgraph GNNs via Subgraph Weisfeiler-Lehman
      Tests
    date: Feb 14, 2023
    date_iso: '2023-02-14'
    date_display: Feb 2023
    codebase_url: https://github.com/subgraph23/SWL
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7961
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0119
    - null
    - null
    - null
    - null
    - null
    - null
  - model: AT Mask-1
    model_plain: AT Mask-1
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.08455'
    title: 'Transformer for Graphs: An Overview from Architecture Perspective'
    date: Feb 17, 2022
    date_iso: '2022-02-17'
    date_display: Feb 2022
    codebase_url: https://github.com/qwerfdsaplking/Graph-Trans
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.796
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
  - model: GNN-SSWL+
    model_plain: GNN-SSWL+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.07090'
    title: A Complete Expressiveness Hierarchy for Subgraph GNNs via Subgraph Weisfeiler-Lehman
      Tests
    date: Feb 14, 2023
    date_iso: '2023-02-14'
    date_display: Feb 2023
    codebase_url: https://github.com/subgraph23/SWL
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7958
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0035
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SSWL+
    model_plain: SSWL+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.19142'
    title: 'MAG-GNN: Reinforcement Learning Boosted Graph Neural Network'
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/LechengKong/MAG-GNN
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7958
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0035
    - null
    - null
    - null
    - null
    - null
    - null
  - model: IRM
    model_plain: IRM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02886'
    title: Graph Rationalization with Environment-based Augmentations
    date: Jun 6, 2022
    date_iso: '2022-06-06'
    date_display: Jun 2022
    codebase_url: https://github.com/liugangcode/GREA
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7947
    - 0.7817
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0186
    - 0.012
    - null
    - null
    - null
    - null
    - null
  - model: GraphAKD
    model_plain: GraphAKD
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.11678'
    title: Compressing Deep Graph Neural Networks via Adversarial Knowledge Distillation
    date: May 24, 2022
    date_iso: '2022-05-24'
    date_display: May 2022
    codebase_url: https://github.com/TencentYoutuResearch/HIG-GraphClassification
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7946
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0097
    - null
    - null
    - null
    - null
    - null
    - null
  row_count: 370
  rows_json: /data/datasets/ogbg-molhiv/standard-split-rows.json
  chart_json: /data/datasets/ogbg-molhiv/standard-split-chart.json
  arch_counts:
    gnn: 214
    hybrid: 80
    graph_transformer: 32
    llm: 4
    walk: 0
    traditional: 22
  metric_counts:
  - 348
  - 9
  - 8
  - 10
  - 2
  - 2
  - 2
  milestones: &id001
  - value: 0.791
    std: 0.003
    model: WL + Virtual Node + AutoML
    arxiv_id: '2006.09430'
    title: Wasserstein Embedding for Graph Learning
    date: '2020-06-16'
  - value: 0.797
    std: 0.0097
    model: DGN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: '2021-03-30'
  - value: 0.8051
    std: 0.0053
    model: Graphormer
    arxiv_id: '2201.09332'
    title: How Expressive are Transformers in Spectral Domain for Graphs?
    date: '2022-01-23'
  - value: 0.8139
    std: 0.0049
    model: GRPE-Standard
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: '2022-01-30'
  - value: 0.8403
    std: 0.0021
    model: HIG with DeeperGCN
    arxiv_id: '2205.11678'
    title: Compressing Deep Graph Neural Networks via Adversarial Knowledge Distillation
    date: '2022-05-24'
  - value: 0.8476
    std: 0.0002
    model: Multi-RF Fusion with Multi-GNN Blending
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    date: '2026-03-21'
  milestones_by_metric:
    ROC-AUC: *id001
    AUC:
    - value: 0.7817
      std: 0.012
      model: IRM
      arxiv_id: '2206.02886'
      title: Graph Rationalization with Environment-based Augmentations
      date: '2022-06-06'
    AUC-ROC:
    - value: 0.6818
      std: 0.008
      model: ASMAML
      arxiv_id: '2408.07340'
      title: Towards Few-shot Self-explaining Graph Neural Networks
      date: '2024-08-14'
    Accuracy:
    - value: 0.79
      std: 0.0243
      model: StructPosGSSL-FA
      arxiv_id: '2502.16233'
      title: Graph Self-Supervised Learning with Learnable Structural and Positional
        Encodings
      date: '2025-02-22'
    - value: 0.98
      std: null
      model: MPNNs
      arxiv_id: '2505.18289'
      title: Convexified Message-Passing Graph Neural Networks
      date: '2025-05-23'
    Size:
    - value: 1.0
      std: 0.0
      model: RCExplainer
      arxiv_id: '2310.01794'
      title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based Gnn Explainers
        through In-depth Benchmarking'
      date: '2023-10-03'
    Sparsity:
    - value: 0.96
      std: 0.0
      model: RCExplainer
      arxiv_id: '2310.01794'
      title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based Gnn Explainers
        through In-depth Benchmarking'
      date: '2023-10-03'
    Suffic.:
    - value: 0.9
      std: 0.02
      model: RCExplainer
      arxiv_id: '2310.01794'
      title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based Gnn Explainers
        through In-depth Benchmarking'
      date: '2023-10-03'
---

