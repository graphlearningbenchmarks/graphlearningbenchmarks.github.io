---
title: COLLAB
slug: collab
benchmark: TU Dortmund
task_type: graph_classification
short_description: Graph classification of scientific collaboration networks (3 classes).
description: '**3-class graph classification** Graph classification of scientific
  collaboration networks (3 classes). Uses the released node/edge labels or attributes;
  several social datasets are featureless. Evaluated by Accuracy.'
detailed_description:
  task: Graph classification of scientific collaboration networks (3 classes). The
    primary catalog metric is Accuracy.
  data: Graph classification of scientific collaboration networks (3 classes). The
    cataloged artifact reports 5,000 graphs, 2 target classes or tasks.
  features: The TU text format may contain discrete node or edge labels and optional
    continuous attributes. Social-network datasets commonly have no intrinsic node
    attributes, so papers often add constant or degree features; that choice changes
    the input.
  splits_and_evaluation: 'The catalog records these protocols or variants: 10-fold
    CV. Evaluation uses Accuracy (higher is better). Exact masks or folds must come
    from the cited release.'
  quirks_and_pitfalls: TU datasets have no canonical train/test split. Report cross-validation
    folds, seeds, feature construction, and whether duplicate or isomorphic graphs
    were removed; published results can otherwise differ for protocol rather than
    model quality.
sources:
- title: TU Dortmund benchmark
  arxiv_id: '2007.08663'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric COLLAB loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
stats:
  num_graphs: 5000
  avg_nodes: 74.5
  avg_edges: 2457.8
  num_classes: 3
result_count: 520
best_model:
  model: WL-MLP
  value: 0.9792
  metric: Accuracy
  arxiv_id: '2202.10156'
  paper_title: 1-WL Expressiveness Is (Almost) All You Need
papers:
- arxiv_id: '2512.13235'
  title: 'CORE: Contrastive Masked Feature Reconstruction on Graphs'
  date_iso: '2025-12-15'
  venue: ''
- arxiv_id: '2510.03987'
  title: 'ICEPool: Enhancing Graph Pooling Networks with Inter-cluster Connectivity'
  date_iso: '2025-10-05'
  venue: ''
- arxiv_id: '2509.22100'
  title: 'SHAKE-GNN: Scalable Hierarchical Kirchhoff-Forest Graph Neural Network'
  date_iso: '2025-09-26'
  venue: ''
- arxiv_id: '2512.04530'
  title: Explainable Graph Representation Learning via Graph Pattern Analysis
  date_iso: '2025-09-01'
  venue: IJCAI 2025
- arxiv_id: '2508.20597'
  title: Local Virtual Nodes for Alleviating Over-Squashing in Graph Neural Networks
  date_iso: '2025-08-28'
  venue: ''
- arxiv_id: '2506.20362'
  title: Self-Supervised Graph Learning via Spectral Bootstrapping and Laplacian-Based
    Augmentations
  date_iso: '2025-06-25'
  venue: ''
- arxiv_id: '2506.06212'
  title: Model-Driven Graph Contrastive Learning
  date_iso: '2025-06-06'
  venue: ''
- arxiv_id: '2505.21285'
  title: Learnable Kernel Density Estimation for Graphs
  date_iso: '2025-05-27'
  venue: ICML 2025
- arxiv_id: '2505.15015'
  title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
  date_iso: '2025-05-21'
  venue: ''
- arxiv_id: '2504.13426'
  title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
  date_iso: '2025-04-18'
  venue: ''
- arxiv_id: '2502.16233'
  title: Graph Self-Supervised Learning with Learnable Structural and Positional Encodings
  date_iso: '2025-02-22'
  venue: WWW 2025
- arxiv_id: '2501.18739'
  title: 'Beyond Message Passing: Neural Graph Pattern Machine'
  date_iso: '2025-01-30'
  venue: ICML 2025
- arxiv_id: '2412.17856'
  title: Graph Structure Refinement with Energy-based Contrastive Learning
  date_iso: '2024-12-20'
  venue: AAAI 2024
- arxiv_id: '2410.10241'
  title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
  date_iso: '2024-10-14'
  venue: KDD 2024
- arxiv_id: '2410.10365'
  title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
    Samples'
  date_iso: '2024-10-14'
  venue: ''
- arxiv_id: '2410.06746'
  title: Cluster-wise Graph Transformer with Dual-granularity Kernelized Attention
  date_iso: '2024-10-09'
  venue: NeurIPS 2024
- arxiv_id: '2408.16288'
  title: 'OpenFGL: A Comprehensive Benchmark for Federated Graph Learning'
  date_iso: '2024-08-29'
  venue: ''
- arxiv_id: '2408.13471'
  title: Disentangled Generative Graph Representation Learning
  date_iso: '2024-08-24'
  venue: ''
- arxiv_id: '2408.11370'
  title: 'Graph Classification via Reference Distribution Learning: Theory and Practice'
  date_iso: '2024-08-21'
  venue: NeurIPS 2024
- arxiv_id: '2407.18480'
  title: Scalable Graph Compressed Convolutions
  date_iso: '2024-07-26'
  venue: ''
- arxiv_id: '2407.04236'
  title: Graph Pooling via Ricci Flow
  date_iso: '2024-07-05'
  venue: TMLR 2024
- arxiv_id: '2406.15523'
  title: 'Unifying Unsupervised Graph-Level Anomaly Detection and Out-of-Distribution
    Detection: A Benchmark'
  date_iso: '2024-06-21'
  venue: ICLR 2024
- arxiv_id: '2406.11714'
  title: Scalable Expressiveness through Preprocessed Graph Perturbations
  date_iso: '2024-06-17'
  venue: ''
- arxiv_id: '2406.05346'
  title: 'ProG: A Graph Prompt Learning Benchmark'
  date_iso: '2024-06-08'
  venue: NeurIPS 2024
- arxiv_id: '2406.01899'
  title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models'
  date_iso: '2024-06-04'
  venue: NeurIPS 2024
- arxiv_id: '2406.01249'
  title: Equivariant Machine Learning on Graphs with Nonlinear Spectral Filters
  date_iso: '2024-06-03'
  venue: NeurIPS 2024
- arxiv_id: '2406.00403'
  title: Dual-perspective Cross Contrastive Learning in Graph Transformers
  date_iso: '2024-06-01'
  venue: ''
- arxiv_id: '2405.14742'
  title: 'HC-GAE: The Hierarchical Cluster-based Graph Auto-Encoder for Graph Representation
    Learning'
  date_iso: '2024-05-23'
  venue: NeurIPS 2024
- arxiv_id: '2405.01350'
  title: Community-Invariant Graph Contrastive Learning
  date_iso: '2024-05-02'
  venue: ICML 2024
- arxiv_id: '2404.15806'
  title: 'Where to Mask: Structure-Guided Masking for Graph Masked Autoencoders'
  date_iso: '2024-04-24'
  venue: IJCAI 2024
- arxiv_id: '2412.03864'
  title: Training MLPs on Graphs without Supervision
  date_iso: '2024-02-14'
  venue: ''
- arxiv_id: '2402.08023'
  title: 'UGMAE: A Unified Framework for Graph Masked Autoencoders'
  date_iso: '2024-02-12'
  venue: ''
- arxiv_id: '2402.07225'
  title: Rethinking Graph Masked Autoencoders through Alignment and Uniformity
  date_iso: '2024-02-11'
  venue: AAAI 2024
- arxiv_id: '2401.17580'
  title: Graph Contrastive Learning with Cohesive Subgraph Awareness
  date_iso: '2024-01-31'
  venue: WWW 2024
- arxiv_id: '2401.03638'
  title: Unifying Graph Contrastive Learning via Graph Message Augmentation
  date_iso: '2024-01-08'
  venue: ''
- arxiv_id: '2311.01038'
  title: 'Better with Less: A Data-Active Perspective on Pre-Training Graph Neural
    Networks'
  date_iso: '2023-11-02'
  venue: NeurIPS 2023
- arxiv_id: '2310.15523'
  title: Generative and Contrastive Paradigms Are Complementary for Graph Self-Supervised
    Learning
  date_iso: '2023-10-24'
  venue: ''
- arxiv_id: '2310.11025'
  title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
    Learning'
  date_iso: '2023-10-17'
  venue: ''
- arxiv_id: '2310.01668'
  title: Locality-Aware Graph Rewiring in GNNs
  date_iso: '2023-10-02'
  venue: ICLR 2023
- arxiv_id: '2309.02304'
  title: Graph Self-Contrast Representation Learning
  date_iso: '2023-09-05'
  venue: ''
- arxiv_id: '2307.01053'
  title: 'ENGAGE: Explanation Guided Data Augmentation for Graph Representation Learning'
  date_iso: '2023-07-03'
  venue: ''
- arxiv_id: '2305.17437'
  title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
  date_iso: '2023-05-27'
  venue: ''
- arxiv_id: '2304.01575'
  title: The expressive power of pooling in Graph Neural Networks
  date_iso: '2023-04-04'
  venue: NeurIPS 2023
- arxiv_id: '2302.12449'
  title: 'SGL-PT: A Strong Graph Learner with Graph Prompt Tuning'
  date_iso: '2023-02-24'
  venue: ''
- arxiv_id: '2302.02369'
  title: Deep Graph-Level Clustering Using Pseudo-Label-Guided Mutual Information
    Maximization Network
  date_iso: '2023-02-05'
  venue: ''
- arxiv_id: '2211.06218'
  title: Total Variation Graph Neural Networks
  date_iso: '2022-11-11'
  venue: ICML 2022
- arxiv_id: '2210.11790'
  title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing in GNNs'
  date_iso: '2022-10-21'
  venue: ICLR 2022
- arxiv_id: '2210.00643'
  title: Spectral Augmentation for Self-Supervised Learning on Graphs
  date_iso: '2022-10-02'
  venue: ICLR 2022
- arxiv_id: '2209.06560'
  title: Graph Contrastive Learning with Personalized Augmentation
  date_iso: '2022-09-14'
  venue: ''
- arxiv_id: '2206.12933'
  title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised Learning
  date_iso: '2022-06-26'
  venue: AAAI 2022
- arxiv_id: '2206.13510'
  title: Structural Entropy Guided Graph Hierarchical Pooling
  date_iso: '2022-06-26'
  venue: ICML 2022
- arxiv_id: '2206.07869'
  title: Let Invariant Rationale Discovery Inspire Graph Contrastive Learning
  date_iso: '2022-06-16'
  venue: ICML 2022
- arxiv_id: '2206.07369'
  title: 'DiffWire: Inductive Graph Rewiring via the Lovász Bound'
  date_iso: '2022-06-15'
  venue: LoG 2022
- arxiv_id: '2206.02059'
  title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
  date_iso: '2022-06-04'
  venue: TMLR 2022
- arxiv_id: '2205.15746'
  title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
    Learning
  date_iso: '2022-05-31'
  venue: ICML 2022
- arxiv_id: '2205.14368'
  title: Going Deeper into Permutation-Sensitive Graph Neural Networks
  date_iso: '2022-05-28'
  venue: ICML 2022
- arxiv_id: '2205.10803'
  title: 'GraphMAE: Self-Supervised Masked Graph Autoencoders'
  date_iso: '2022-05-22'
  venue: KDD 2022
- arxiv_id: '2205.09802'
  title: Label-invariant Augmentation for Semi-Supervised Graph Classification
  date_iso: '2022-05-19'
  venue: NeurIPS 2022
- arxiv_id: '2205.15068'
  title: Embedding Graphs on Grassmann Manifold
  date_iso: '2022-05-01'
  venue: ''
- arxiv_id: '2203.07678'
  title: Incorporating Heterophily into Graph Neural Networks for Graph Classification
  date_iso: '2022-03-15'
  venue: ''
- arxiv_id: '2202.13248'
  title: Automated Data Augmentations for Graph Classification
  date_iso: '2022-02-26'
  venue: ICLR 2022
- arxiv_id: '2202.10156'
  title: 1-WL Expressiveness Is (Almost) All You Need
  date_iso: '2022-02-21'
  venue: ''
- arxiv_id: '2202.08333'
  title: Self-Supervised Representation Learning via Latent Graph Prediction
  date_iso: '2022-02-16'
  venue: ICML 2022
- arxiv_id: '2201.13410'
  title: 'Weisfeiler and Leman Go Infinite: Spectral and Combinatorial Pre-Colorings'
  date_iso: '2022-01-31'
  venue: TMLR 2022
- arxiv_id: '2201.09830'
  title: Learning Graph Augmentations to Learn Graph Representations
  date_iso: '2022-01-24'
  venue: ''
- arxiv_id: '2201.00491'
  title: 'KerGNNs: Interpretable Graph Neural Networks with Graph Kernels'
  date_iso: '2022-01-03'
  venue: AAAI 2022
- arxiv_id: '2112.09899'
  title: Improving Subgraph Recognition with Variational Graph Information Bottleneck
  date_iso: '2021-12-18'
  venue: ''
- arxiv_id: '2112.08903'
  title: Graph Structure Learning with Variational Information Bottleneck
  date_iso: '2021-12-16'
  venue: AAAI 2021
- arxiv_id: '2112.03806'
  title: 'OOD-GNN: Out-of-Distribution Generalized Graph Neural Network'
  date_iso: '2021-12-07'
  venue: ''
- arxiv_id: '2110.15438'
  title: 'InfoGCL: Information-Aware Graph Contrastive Learning'
  date_iso: '2021-10-28'
  venue: NeurIPS 2021
- arxiv_id: '2106.09645'
  title: Prototypical Graph Contrastive Learning
  date_iso: '2021-06-17'
  venue: ''
- arxiv_id: '2106.05819'
  title: Adversarial Graph Augmentation to Improve Graph Contrastive Learning
  date_iso: '2021-06-10'
  venue: NeurIPS 2021
- arxiv_id: '2106.07594'
  title: Graph Contrastive Learning Automated
  date_iso: '2021-06-10'
  venue: ICML 2021
- arxiv_id: '2105.07519'
  title: Graph-Free Knowledge Distillation for Graph Neural Networks
  date_iso: '2021-05-16'
  venue: IJCAI 2021
- arxiv_id: '2103.00959'
  title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
  date_iso: '2021-03-01'
  venue: WWW 2021
- arxiv_id: '2103.00111'
  title: 'Graph Self-Supervised Learning: A Survey'
  date_iso: '2021-02-27'
  venue: ''
- arxiv_id: '2010.15116'
  title: On Graph Neural Networks versus Graph-Augmented MLPs
  date_iso: '2020-10-28'
  venue: ICLR 2020
- arxiv_id: '2010.05421'
  title: Factorizable Graph Convolutional Networks
  date_iso: '2020-10-12'
  venue: NeurIPS 2020
- arxiv_id: '2009.10564'
  title: 'GraphCrop: Subgraph Cropping for Graph Classification'
  date_iso: '2020-09-22'
  venue: ''
- arxiv_id: '2009.03294'
  title: 'GraphNorm: A Principled Approach to Accelerating Graph Neural Network Training'
  date_iso: '2020-09-07'
  venue: ICML 2020
- arxiv_id: '2008.05089'
  title: Quaternion Graph Neural Networks
  date_iso: '2020-08-12'
  venue: ''
- arxiv_id: '2007.08349'
  title: Natural Graph Networks
  date_iso: '2020-07-16'
  venue: NeurIPS 2020
- arxiv_id: '2006.09963'
  title: 'GCC: Graph Contrastive Coding for Graph Neural Network Pre-Training'
  date_iso: '2020-06-17'
  venue: KDD 2020
- arxiv_id: '2006.09430'
  title: Wasserstein Embedding for Graph Learning
  date_iso: '2020-06-16'
  venue: ICLR 2020
- arxiv_id: '2002.09518'
  title: Memory-Based Graph Networks
  date_iso: '2020-02-21'
  venue: ICLR 2020
- arxiv_id: '1909.11855'
  title: Universal Graph Transformer Self-Attention Networks
  date_iso: '2019-09-26'
  venue: WWW 2019
- arxiv_id: '1905.13192'
  title: 'Graph Neural Tangent Kernel: Fusing Graph Neural Networks with Graph Kernels'
  date_iso: '2019-05-30'
  venue: NeurIPS 2019
- arxiv_id: '1905.12560'
  title: On the Equivalence between Graph Isomorphism Testing and Function Approximation
    with GNNs
  date_iso: '2019-05-29'
  venue: NeurIPS 2019
- arxiv_id: '1905.10990'
  title: Edge Contraction Pooling for Graph Neural Networks
  date_iso: '2019-05-27'
  venue: ''
- arxiv_id: '1905.05178'
  title: Graph U-Nets
  date_iso: '2019-05-11'
  venue: ''
- arxiv_id: '1903.02428'
  title: Fast Graph Representation Learning with PyTorch Geometric
  date_iso: '2019-03-06'
  venue: ICLR 2019
- arxiv_id: '1810.00826'
  title: How Powerful are Graph Neural Networks?
  date_iso: '2018-10-01'
  venue: ICLR 2018
- arxiv_id: '1805.11921'
  title: Anonymous Walk Embeddings
  date_iso: '2018-05-30'
  venue: ICML 2018
- arxiv_id: '1805.08090'
  title: Graph Capsule Convolutional Neural Networks
  date_iso: '2018-05-21'
  venue: ICML 2018
- arxiv_id: '1606.01141'
  title: On Valid Optimal Assignment Kernels and Applications to Graph Classification
  date_iso: '2016-06-03'
  venue: NeurIPS 2016
variants:
- slug: 10-fold-cv
  name: 10-fold CV
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 5000
    avg_nodes: 74.5
    avg_edges: 2457.8
    num_classes: 3
  metrics:
  - Accuracy
  - AUROC
  - F1
  - equivalence classes
  - ing Accuracy
  metric_display_names:
  - Accuracy
  - AUROC
  - F1
  - equivalence classes
  - ing Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: WL-MLP
    model_plain: WL-MLP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_iso: '2022-02-21'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9792
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
  - model: MSH-GNN
    model_plain: MSH-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_iso: '2025-05-21'
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
    - 0.964
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
  - model: CoCN
    model_plain: CoCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.18480'
    title: Scalable Graph Compressed Convolutions
    date: Jul 26, 2024
    date_iso: '2024-07-26'
    date_display: Jul 2024
    codebase_url: https://github.com/sunjss/CoCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8722
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0013
    - null
    - null
    - null
    - null
  - model: N^2
    model_plain: N^2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_iso: '2025-05-21'
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
    - 0.867
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
  - model: CoCN vanilla
    model_plain: CoCN vanilla
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.18480'
    title: Scalable Graph Compressed Convolutions
    date: Jul 26, 2024
    date_iso: '2024-07-26'
    date_display: Jul 2024
    codebase_url: https://github.com/sunjss/CoCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8615
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    - null
    - null
  - model: graph2vec
    model_plain: graph2vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2103.00959'
    title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    date: Mar 1, 2021
    date_iso: '2021-03-01'
    date_display: Mar 2021
    codebase_url: https://github.com/THUDM/cogdl
    published_conference: WWW 2021
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8558
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
  - model: GSN
    model_plain: GSN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_iso: '2025-05-21'
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
    - 0.855
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.012
    - null
    - null
    - null
    - null
  - model: OEPG
    model_plain: OEPG
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15746'
    title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
      Learning
    date: May 31, 2022
    date_iso: '2022-05-31'
    date_display: May 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.847
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
  - model: CORE (GraphMAE2 + CORE)
    model_plain: CORE (GraphMAE2 + CORE)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2512.13235'
    title: 'CORE: Contrastive Masked Feature Reconstruction on Graphs'
    date: Dec 15, 2025
    date_iso: '2025-12-15'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.843
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    - null
    - null
  - model: GraphMAE2
    model_plain: GraphMAE2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.13235'
    title: 'CORE: Contrastive Masked Feature Reconstruction on Graphs'
    date: Dec 15, 2025
    date_iso: '2025-12-15'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.841
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
    - null
    - null
  - model: PXGL-GNN
    model_plain: PXGL-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2512.04530'
    title: Explainable Graph Representation Learning via Graph Pattern Analysis
    date: Sep 1, 2025
    date_iso: '2025-09-01'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: IJCAI 2025
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8396
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0159
    - null
    - null
    - null
    - null
  - model: DiGGR
    model_plain: DiGGR
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_iso: '2024-08-24'
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
    - 0.8376
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.037
    - null
    - null
    - null
    - null
  - model: GNTK
    model_plain: GNTK
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    arxiv_id: '1905.13192'
    title: 'Graph Neural Tangent Kernel: Fusing Graph Neural Networks with Graph Kernels'
    date: May 30, 2019
    date_iso: '2019-05-30'
    date_display: May 2019
    codebase_url: https://github.com/KangchengHou/gntk
    published_conference: NeurIPS 2019
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.836
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
  - model: SE2P-C3
    model_plain: SE2P-C3
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.11714'
    title: Scalable Expressiveness through Preprocessed Graph Perturbations
    date: Jun 17, 2024
    date_iso: '2024-06-17'
    date_display: Jun 2024
    codebase_url: https://github.com/Danial-sb/SE2P
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.835
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.017
    - null
    - null
    - null
    - null
  - model: SE2P-C2
    model_plain: SE2P-C2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.11714'
    title: Scalable Expressiveness through Preprocessed Graph Perturbations
    date: Jun 17, 2024
    date_iso: '2024-06-17'
    date_display: Jun 2024
    codebase_url: https://github.com/Danial-sb/SE2P
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.833
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
  - model: Attention
    model_plain: Attention
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2205.15068'
    title: Embedding Graphs on Grassmann Manifold
    date: May 1, 2022
    date_iso: '2022-05-01'
    date_display: May 2022
    codebase_url: https://github.com/conf20/Egg
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8322
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
    - null
    - null
  - model: ECL-GSR
    model_plain: ECL-GSR
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2412.17856'
    title: Graph Structure Refinement with Energy-based Contrastive Learning
    date: Dec 20, 2024
    date_iso: '2024-12-20'
    date_display: Dec 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.83
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0143
    - null
    - null
    - null
    - null
  - model: EGG
    model_plain: EGG
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15068'
    title: Embedding Graphs on Grassmann Manifold
    date: May 1, 2022
    date_iso: '2022-05-01'
    date_display: May 2022
    codebase_url: https://github.com/conf20/Egg
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8294
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0106
    - null
    - null
    - null
    - null
  - model: GraphAug
    model_plain: GraphAug
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.13248'
    title: Automated Data Augmentations for Graph Classification
    date: Feb 26, 2022
    date_iso: '2022-02-26'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.829
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
    - null
    - null
  - model: SE2P-C4
    model_plain: SE2P-C4
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.11714'
    title: Scalable Expressiveness through Preprocessed Graph Perturbations
    date: Jun 17, 2024
    date_iso: '2024-06-17'
    date_display: Jun 2024
    codebase_url: https://github.com/Danial-sb/SE2P
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.828
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
  - model: SAN
    model_plain: SAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2512.04530'
    title: Explainable Graph Representation Learning via Graph Pattern Analysis
    date: Sep 1, 2025
    date_iso: '2025-09-01'
    date_display: Sep 2025
    codebase_url: ''
    published_conference: IJCAI 2025
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8273
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
  - model: GraphMAE
    model_plain: GraphMAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10241'
    title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: https://github.com/EdisonLeeeee/lrGAE
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.827
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
  - model: Empowering GNNs
    model_plain: Empowering GNNs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.02059'
    title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
    date: Jun 4, 2022
    date_iso: '2022-06-04'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: TMLR 2022
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.825
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.012
    - null
    - null
    - null
    - null
  - model: LaplaceGNN
    model_plain: LaplaceGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.20362'
    title: Self-Supervised Graph Learning via Spectral Bootstrapping and Laplacian-Based
      Augmentations
    date: Jun 25, 2025
    date_iso: '2025-06-25'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8241
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0042
    - null
    - null
    - null
    - null
  - model: SignGT
    model_plain: SignGT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: Oct 17, 2023
    date_iso: '2023-10-17'
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
    - 0.824
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0014
    - null
    - null
    - null
    - null
  - model: lrGAE 6
    model_plain: lrGAE 6
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10241'
    title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: https://github.com/EdisonLeeeee/lrGAE
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.823
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
  - model: lrGAE 7
    model_plain: lrGAE 7
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10241'
    title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: https://github.com/EdisonLeeeee/lrGAE
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.823
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
  - model: lrGAE 8
    model_plain: lrGAE 8
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2410.10241'
    title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: https://github.com/EdisonLeeeee/lrGAE
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.822
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
    - null
    - null
  - model: S2GAE
    model_plain: S2GAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10241'
    title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: https://github.com/EdisonLeeeee/lrGAE
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.822
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
  - model: att-Pooling-NLSFs
    model_plain: att-Pooling-NLSFs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.8219
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.013
    - null
    - null
    - null
    - null
  - model: JOAOv2
    model_plain: JOAOv2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09802'
    title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8216
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0017
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
    arxiv_id: '2407.18480'
    title: Scalable Graph Compressed Convolutions
    date: Jul 26, 2024
    date_iso: '2024-07-26'
    date_display: Jul 2024
    codebase_url: https://github.com/sunjss/CoCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8213
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0043
    - null
    - null
    - null
    - null
  - model: DiffPool-Det
    model_plain: DiffPool-Det
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '1905.05178'
    title: Graph U-Nets
    date: May 11, 2019
    date_iso: '2019-05-11'
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
    - 0.8213
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
  - model: MaskGAE
    model_plain: MaskGAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10241'
    title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: https://github.com/EdisonLeeeee/lrGAE
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.82
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
  - model: CTAug-JOAO
    model_plain: CTAug-JOAO
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2401.17580'
    title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/wuyucheng2002/CTAug
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.819
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
  - model: SimGRACE
    model_plain: SimGRACE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09802'
    title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8188
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0023
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
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: Oct 17, 2023
    date_iso: '2023-10-17'
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
    - 0.818
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0224
    - null
    - null
    - null
    - null
  - model: WGDN
    model_plain: WGDN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.12933'
    title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised Learning
    date: Jun 26, 2022
    date_iso: '2022-06-26'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: AAAI 2022
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8176
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0024
    - null
    - null
    - null
    - null
  - model: SEP-G ICE
    model_plain: SEP-G ICE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.03987'
    title: 'ICEPool: Enhancing Graph Pooling Networks with Inter-cluster Connectivity'
    date: Oct 5, 2025
    date_iso: '2025-10-05'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8176
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0081
    - null
    - null
    - null
    - null
  - model: SAGPool
    model_plain: SAGPool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.15068'
    title: Embedding Graphs on Grassmann Manifold
    date: May 1, 2022
    date_iso: '2022-05-01'
    date_display: May 2022
    codebase_url: https://github.com/conf20/Egg
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8176
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0157
    - null
    - null
    - null
    - null
  - model: CTAug-GraphCL
    model_plain: CTAug-GraphCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2401.17580'
    title: Graph Contrastive Learning with Cohesive Subgraph Awareness
    date: Jan 31, 2024
    date_iso: '2024-01-31'
    date_display: Jan 2024
    codebase_url: https://github.com/wuyucheng2002/CTAug
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8172
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
    - null
    - null
  - model: GraphMAE2
    model_plain: GraphMAE2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10241'
    title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: https://github.com/EdisonLeeeee/lrGAE
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.817
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
    - null
    - null
  - model: GCKM
    model_plain: GCKM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_iso: '2025-04-18'
    date_display: Apr 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.817
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
  - model: Teacher (100% training data)
    model_plain: Teacher (100% training data)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2105.07519'
    title: Graph-Free Knowledge Distillation for Graph Neural Networks
    date: May 16, 2021
    date_iso: '2021-05-16'
    date_display: May 2021
    codebase_url: https://github.com/Xiang-Deng-DL/GFKD
    published_conference: IJCAI 2021
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.817
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
  - model: UGMAE
    model_plain: UGMAE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.08023'
    title: 'UGMAE: A Unified Framework for Graph Masked Autoencoders'
    date: Feb 12, 2024
    date_iso: '2024-02-12'
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
    - 0.8166
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0012
    - null
    - null
    - null
    - null
  - model: Uniform PerturbEdge
    model_plain: Uniform PerturbEdge
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.13248'
    title: Automated Data Augmentations for Graph Classification
    date: Feb 26, 2022
    date_iso: '2022-02-26'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.816
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
    - null
    - null
  - model: GLA
    model_plain: GLA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09802'
    title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    date: May 19, 2022
    date_iso: '2022-05-19'
    date_display: May 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8154
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0014
    - null
    - null
    - null
    - null
  - model: BGRL
    model_plain: BGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.10241'
    title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
    date: Oct 14, 2024
    date_iso: '2024-10-14'
    date_display: Oct 2024
    codebase_url: https://github.com/EdisonLeeeee/lrGAE
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.815
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
  - model: WL-PM
    model_plain: WL-PM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    arxiv_id: '2502.16233'
    title: Graph Self-Supervised Learning with Learnable Structural and Positional
      Encodings
    date: Feb 22, 2025
    date_iso: '2025-02-22'
    date_display: Feb 2025
    codebase_url: https://github.com/wokas36/StructPosGSSL
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.815
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
  - model: Uniform MaskNF
    model_plain: Uniform MaskNF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.13248'
    title: Automated Data Augmentations for Graph Classification
    date: Feb 26, 2022
    date_iso: '2022-02-26'
    date_display: Feb 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.815
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
    - null
    - null
  row_count: 520
  rows_json: /data/datasets/collab/10-fold-cv-rows.json
  chart_json: /data/datasets/collab/10-fold-cv-chart.json
  arch_counts:
    gnn: 326
    hybrid: 83
    graph_transformer: 13
    llm: 1
    walk: 14
    traditional: 75
  metric_counts:
  - 485
  - 31
  - 2
  - 2
  - 1
  milestones: &id001
  - value: 0.807
    std: 0.001
    model: WL-OA
    arxiv_id: '1606.01141'
    title: On Valid Optimal Assignment Kernels and Applications to Graph Classification
    date: '2016-06-03'
  - value: 0.8213
    std: null
    model: DiffPool-Det
    arxiv_id: '1905.05178'
    title: Graph U-Nets
    date: '2019-05-11'
  - value: 0.836
    std: 0.01
    model: GNTK
    arxiv_id: '1905.13192'
    title: 'Graph Neural Tangent Kernel: Fusing Graph Neural Networks with Graph Kernels'
    date: '2019-05-30'
  - value: 0.8558
    std: null
    model: graph2vec
    arxiv_id: '2103.00959'
    title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    date: '2021-03-01'
  - value: 0.9792
    std: null
    model: WL-MLP
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: '2022-02-21'
  milestones_by_metric:
    Accuracy: *id001
    AUROC:
    - value: 0.7245
      std: null
      model: SIGNET
      arxiv_id: '2406.15523'
      title: 'Unifying Unsupervised Graph-Level Anomaly Detection and Out-of-Distribution
        Detection: A Benchmark'
      date: '2024-06-21'
    F1:
    - value: 0.8123
      std: 0.0086
      model: APT (Mole-BERT)
      arxiv_id: '2311.01038'
      title: 'Better with Less: A Data-Active Perspective on Pre-Training Graph Neural
        Networks'
      date: '2023-11-02'
    equivalence classes:
    - value: 294.0
      std: null
      model: GNN
      arxiv_id: '2010.15116'
      title: On Graph Neural Networks versus Graph-Augmented MLPs
      date: '2020-10-28'
    ing Accuracy:
    - value: 0.799
      std: null
      model: GRDL
      arxiv_id: '2408.11370'
      title: 'Graph Classification via Reference Distribution Learning: Theory and
        Practice'
      date: '2024-08-21'
---

