---
title: Amazon-Computers
slug: amazon-computers
benchmark: Classic
task_type: node_classification
short_description: Predict each product’s category from review-derived features and
  product links on one co-purchase graph.
description: '**Node classification** on one co-purchase graph, predicting each product’s
  category from review-derived features and product links. Evaluated by Accuracy.'
detailed_description:
  task: Amazon co-purchase graph (Computers) node classification. The primary catalog
    metric is Accuracy.
  data: Amazon co-purchase graph (Computers) node classification.
  features: The representation follows the cited PyG loader or benchmark release.
    Node and edge fields are dataset-specific; preprocessing, graph direction, and
    any feature normalization must be kept fixed when reproducing a result.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses Accuracy (higher is better). Exact masks or folds must
    come from the cited release.'
  quirks_and_pitfalls: The same short dataset name is used for incompatible processed
    artifacts and split protocols. Report the loader/version, directedness, feature
    preprocessing, and exact masks; transductive results should not be described as
    inductive.
sources:
- title: Pitfalls of Graph Neural Network Evaluation
  arxiv_id: '1811.05868'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric Amazon-Computers loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.Amazon.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.Amazon.html
stats:
  num_graphs: 1
  avg_nodes: 13752.0
  avg_edges: 245861.0
  num_classes: 10
  extra_stats:
    avg_degree: 35.758
    edge_feature_dim: 0
    edge_feature_type: co-purchase links; no edge attributes
    edge_homophily: 0.7853
    node_feature_dim: 767
    node_feature_type: sparse bag-of-words product-review features
    statistic_notes: PyG exposes 491,722 bidirected edge entries; this record stores
      245,861 unique undirected links
result_count: 789
best_model:
  model: GraphTARIF
  value: 0.9461
  metric: Accuracy
  arxiv_id: '2605.20248'
  paper_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in
    Node Classification'
papers:
- arxiv_id: '2605.21247'
  title: Graph Navier–Stokes Networks
  date_iso: '2026-05-20'
  venue: ''
- arxiv_id: '2605.20248'
  title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
    Classification'
  date_iso: '2026-05-18'
  venue: ''
- arxiv_id: '2605.03076'
  title: Adaptive Negative Scheduling for Graph Contrastive Learning
  date_iso: '2026-05-04'
  venue: ''
- arxiv_id: '2602.19622'
  title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with Graph
    Token Attention'
  date_iso: '2026-02-23'
  venue: WWW 2026
- arxiv_id: '2602.15634'
  title: 'Beyond ReLU: Bifurcation, Oversmoothing, and Topological Priors'
  date_iso: '2026-02-17'
  venue: ''
- arxiv_id: '2512.13235'
  title: 'CORE: Contrastive Masked Feature Reconstruction on Graphs'
  date_iso: '2025-12-15'
  venue: ''
- arxiv_id: '2512.08798'
  title: Can TabPFN Compete with GNNs for Node Classification via Graph Tabularization?
  date_iso: '2025-12-09'
  venue: LoG 2025
- arxiv_id: '2511.19976'
  title: Rethinking Semi-Supervised Node Classification with Self-Supervised Graph
    Clustering
  date_iso: '2025-11-25'
  venue: ''
- arxiv_id: '2510.17457'
  title: 'Deeper with Riemannian Geometry: Overcoming Oversmoothing and Oversquashing
    for Graph Foundation Models'
  date_iso: '2025-10-20'
  venue: NeurIPS 2025
- arxiv_id: '2507.14484'
  title: 'ReDiSC: A Reparameterized Masked Diffusion Model for Scalable Node Classification
    with Structured Predictions'
  date_iso: '2025-07-19'
  venue: ''
- arxiv_id: '2506.20362'
  title: Self-Supervised Graph Learning via Spectral Bootstrapping and Laplacian-Based
    Augmentations
  date_iso: '2025-06-25'
  venue: ''
- arxiv_id: '2506.22510'
  title: 'Towards Text-free Graph Foundation Models: Rethinking Multi-Domain Graph
    Contrastive Learning'
  date_iso: '2025-06-25'
  venue: ''
- arxiv_id: '2506.19343'
  title: Discrepancy-Aware Graph Mask Auto-Encoder
  date_iso: '2025-06-24'
  venue: KDD 2025
- arxiv_id: '2506.13083'
  title: 'Uncertainty-Aware Graph Neural Networks: A Multi-Hop Evidence Fusion Approach'
  date_iso: '2025-06-16'
  venue: ''
- arxiv_id: '2505.23014'
  title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in the Perspective of
    A System of Hyperbolic Partial Differential Equations'
  date_iso: '2025-05-29'
  venue: ICML 2025
- arxiv_id: '2505.17660'
  title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
    for Node Classification'
  date_iso: '2025-05-23'
  venue: ''
- arxiv_id: '2505.15845'
  title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
    Learning Models'
  date_iso: '2025-05-19'
  venue: ''
- arxiv_id: '2505.10307'
  title: Negative Metric Learning for Graphs
  date_iso: '2025-05-15'
  venue: IJCAI 2025
- arxiv_id: '2505.05533'
  title: Rethinking Graph Contrastive Learning through Relative Similarity Preservation
  date_iso: '2025-05-08'
  venue: IJCAI 2025
- arxiv_id: '2504.20430'
  title: Learning Laplacian Positional Encodings for Heterophilous Graphs
  date_iso: '2025-04-29'
  venue: ''
- arxiv_id: '2504.19785'
  title: Heterophily-informed Message Passing
  date_iso: '2025-04-28'
  venue: TMLR 2025
- arxiv_id: '2505.20034'
  title: Graph Wave Networks
  date_iso: '2025-04-22'
  venue: WWW 2025
- arxiv_id: '2507.07141'
  title: 'Str-GCL: Structural Commonsense Driven Graph Contrastive Learning'
  date_iso: '2025-04-22'
  venue: WWW 2025
- arxiv_id: '2504.12011'
  title: Balancing Graph Embedding Smoothness in Self-Supervised Learning via Information-Theoretic
    Decomposition
  date_iso: '2025-04-16'
  venue: WWW 2025
- arxiv_id: '2501.19089'
  title: Resolving Oversmoothing with Opinion Dissensus
  date_iso: '2025-01-31'
  venue: ''
- arxiv_id: '2501.15755'
  title: 'GraphICL: Unlocking Graph Learning Potential in LLMs through Structured
    Prompt Design'
  date_iso: '2025-01-27'
  venue: ''
- arxiv_id: '2412.16441'
  title: 'Towards Graph Foundation Models: Learning Generalities Across Graphs via
    Task-Trees'
  date_iso: '2024-12-21'
  venue: ICML 2024
- arxiv_id: '2412.06173'
  title: Revisiting the Necessity of Graph Learning and Common Graph Benchmarks
  date_iso: '2024-12-09'
  venue: ''
- arxiv_id: '2412.04064'
  title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
  date_iso: '2024-12-05'
  venue: NeurIPS 2024
- arxiv_id: '2411.16278'
  title: Even Sparser Graph Transformers
  date_iso: '2024-11-25'
  venue: NeurIPS 2024
- arxiv_id: '2411.05274'
  title: Distributed-Order Fractional Graph Operating Network
  date_iso: '2024-11-08'
  venue: NeurIPS 2024
- arxiv_id: '2410.19723'
  title: Sparse Decomposition of Graph Neural Networks
  date_iso: '2024-10-25'
  venue: TMLR 2024
- arxiv_id: '2410.15355'
  title: 'LAC: Graph Contrastive Learning with Learnable Augmentation in Continuous
    Space'
  date_iso: '2024-10-20'
  venue: ''
- arxiv_id: '2410.10241'
  title: Revisiting Graph Autoencoders as Implicit Contrastive Learners
  date_iso: '2024-10-14'
  venue: KDD 2024
- arxiv_id: '2410.02622'
  title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic Transforms'
  date_iso: '2024-10-03'
  venue: ICML 2024
- arxiv_id: '2409.08010'
  title: Multiplex Graph Contrastive Learning with Soft Negatives
  date_iso: '2024-09-12'
  venue: ''
- arxiv_id: '2408.05087'
  title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised Learning
  date_iso: '2024-08-09'
  venue: ''
- arxiv_id: '2408.00165'
  title: Non-convolutional Graph Neural Networks
  date_iso: '2024-07-31'
  venue: NeurIPS 2024
- arxiv_id: '2407.16726'
  title: Topology Reorganized Graph Contrastive Learning with Mitigating Semantic
    Drift
  date_iso: '2024-07-23'
  venue: ''
- arxiv_id: '2407.11361'
  title: 'Graph Structure Prompt Learning: A Novel Methodology to Improve Performance
    of Graph Neural Networks'
  date_iso: '2024-07-16'
  venue: ''
- arxiv_id: '2407.11907'
  title: 'GraphFM: A generalist graph transformer that learns transferable representations
    across diverse domains'
  date_iso: '2024-07-16'
  venue: TMLR 2024
- arxiv_id: '2406.19249'
  title: 'NTFormer: A Composite Node Tokenized Graph Transformer for Node Classification'
  date_iso: '2024-06-27'
  venue: ''
- arxiv_id: '2406.12052'
  title: 'UniGLM: Training One Unified Language Model for Text-Attributed Graph Embedding'
  date_iso: '2024-06-17'
  venue: ''
- arxiv_id: '2406.10727'
  title: 'Text-space Graph Foundation Models: Comprehensive Benchmarks and New Insights'
  date_iso: '2024-06-15'
  venue: NeurIPS 2024
- arxiv_id: '2405.19779'
  title: Automatic Graph Topology-Aware Transformer
  date_iso: '2024-05-30'
  venue: ''
- arxiv_id: '2405.14742'
  title: 'HC-GAE: The Hierarchical Cluster-based Graph Auto-Encoder for Graph Representation
    Learning'
  date_iso: '2024-05-23'
  venue: NeurIPS 2024
- arxiv_id: '2405.13806'
  title: A General Graph Spectral Wavelet Convolution via Chebyshev Order Decomposition
  date_iso: '2024-05-22'
  venue: ICML 2024
- arxiv_id: '2404.17099'
  title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
    with FROND
  date_iso: '2024-04-26'
  venue: ICLR 2024
- arxiv_id: '2403.20221'
  title: Graph Neural Aggregation-diffusion with Metastability
  date_iso: '2024-03-29'
  venue: ''
- arxiv_id: '2403.05064'
  title: Unsupervised Graph Neural Architecture Search with Disentangled Self-supervision
  date_iso: '2024-03-08'
  venue: NeurIPS 2024
- arxiv_id: '2403.01400'
  title: Decoupling Weighing and Selecting for Integrating Multiple Graph Pre-training
    Tasks
  date_iso: '2024-03-03'
  venue: ICLR 2024
- arxiv_id: '2403.01232'
  title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
  date_iso: '2024-03-02'
  venue: ICLR 2024
- arxiv_id: '2403.01079'
  title: 'Teaching MLP More Graph Information: A Three-stage Multitask Knowledge Distillation
    Framework.'
  date_iso: '2024-03-02'
  venue: ''
- arxiv_id: '2402.15270'
  title: Smoothed Graph Contrastive Learning via Seamless Proximity Integration
  date_iso: '2024-02-23'
  venue: ''
- arxiv_id: '2402.10468'
  title: Adversarial Curriculum Graph Contrastive Learning with Pair-wise Augmentation
  date_iso: '2024-02-16'
  venue: ''
- arxiv_id: '2402.09711'
  title: Node Duplication Improves Cold-start Link Prediction
  date_iso: '2024-02-15'
  venue: TMLR 2024
- arxiv_id: '2412.03864'
  title: Training MLPs on Graphs without Supervision
  date_iso: '2024-02-14'
  venue: ''
- arxiv_id: '2402.04621'
  title: 'Feature Distribution on Graph Topology Mediates the Effect of Graph Convolution:
    Homophily Perspective'
  date_iso: '2024-02-07'
  venue: ICML 2024
- arxiv_id: '2401.17580'
  title: Graph Contrastive Learning with Cohesive Subgraph Awareness
  date_iso: '2024-01-31'
  venue: WWW 2024
- arxiv_id: '2401.15203'
  title: 'FedGT: Federated Node Classification with Scalable Graph Transformer'
  date_iso: '2024-01-26'
  venue: ICLR 2024
- arxiv_id: '2401.11750'
  title: 'AdaFGL: A New Paradigm for Federated Node Classification with Topology Heterogeneity'
  date_iso: '2024-01-22'
  venue: ''
- arxiv_id: '2312.02619'
  title: Rethinking and Simplifying Bootstrapped Graph Latents
  date_iso: '2023-12-05'
  venue: ''
- arxiv_id: '2311.02687'
  title: 'Architecture Matters: Uncovering Implicit Mechanisms in Graph Contrastive
    Learning'
  date_iso: '2023-11-05'
  venue: NeurIPS 2023
- arxiv_id: '2310.18884'
  title: Simple and Asymmetric Graph Contrastive Learning without Augmentations
  date_iso: '2023-10-29'
  venue: NeurIPS 2023
- arxiv_id: '2310.17132'
  title: 'BiKT: Unleashing the potential of GNNs via Bi-directional Knowledge Transfer'
  date_iso: '2023-10-26'
  venue: ''
- arxiv_id: '2310.11762'
  title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
  date_iso: '2023-10-18'
  venue: WWW 2023
- arxiv_id: '2310.11025'
  title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
    Learning'
  date_iso: '2023-10-17'
  venue: ''
- arxiv_id: '2310.05296'
  title: Tailoring Self-Attention for Graph via Rooted Subtrees
  date_iso: '2023-10-08'
  venue: NeurIPS 2023
- arxiv_id: '2310.03977'
  title: Perfect Alignment May be Poisonous to Graph Contrastive Learning
  date_iso: '2023-10-06'
  venue: ICML 2023
- arxiv_id: '2401.11755'
  title: 'FedGTA: Topology-aware Averaging for Federated Graph Learning'
  date_iso: '2023-09-01'
  venue: ''
- arxiv_id: '2307.06631'
  title: Frameless Graph Knowledge Distillation
  date_iso: '2023-07-13'
  venue: ''
- arxiv_id: '2307.01053'
  title: 'ENGAGE: Explanation Guided Data Augmentation for Graph Representation Learning'
  date_iso: '2023-07-03'
  venue: ''
- arxiv_id: '2306.09614'
  title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
  date_iso: '2023-06-16'
  venue: KDD 2023
- arxiv_id: '2306.07608'
  title: 'Finding the Missing-half: Graph Complementary Learning for Homophily-prone
    and Heterophily-prone Graphs'
  date_iso: '2023-06-13'
  venue: ICML 2023
- arxiv_id: '2306.02285'
  title: Clarify Confused Nodes via Separated Learning
  date_iso: '2023-06-04'
  venue: ''
- arxiv_id: '2306.02376'
  title: 'Towards Deep Attention in Graph Neural Networks: Problems and Remedies'
  date_iso: '2023-06-04'
  venue: ICML 2023
- arxiv_id: '2306.02117'
  title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
  date_iso: '2023-06-03'
  venue: ''
- arxiv_id: '2305.17284'
  title: 'GC-Flow: A Graph-Based Flow Network for Effective Clustering'
  date_iso: '2023-05-26'
  venue: ICML 2023
- arxiv_id: '2305.15747'
  title: Union Subgraph Neural Networks
  date_iso: '2023-05-25'
  venue: AAAI 2023
- arxiv_id: '2305.06142'
  title: Feature Expansion for Graph Neural Networks
  date_iso: '2023-05-10'
  venue: ICML 2023
- arxiv_id: '2303.13750'
  title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
  date_iso: '2023-03-24'
  venue: ''
- arxiv_id: '2301.12458'
  title: 'SeeGera: Self-supervised Semi-implicit Graph Variational Auto-encoders with
    Masking'
  date_iso: '2023-01-29'
  venue: WWW 2023
- arxiv_id: '2301.12063'
  title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical Adaptive
    Masking and Trainable Corruption'
  date_iso: '2023-01-28'
  venue: ''
- arxiv_id: '2212.04604'
  title: Localized Graph Contrastive Learning
  date_iso: '2022-12-08'
  venue: ''
- arxiv_id: '2212.03654'
  title: Node-oriented Spectral Filtering for Graph Neural Networks
  date_iso: '2022-12-07'
  venue: ''
- arxiv_id: '2212.02483'
  title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
  date_iso: '2022-12-05'
  venue: ICML 2022
- arxiv_id: '2211.16494'
  title: On the Ability of Graph Neural Networks to Model Interactions Between Vertices
  date_iso: '2022-11-29'
  venue: NeurIPS 2022
- arxiv_id: '2210.08792'
  title: Unifying Graph Contrastive Learning with Flexible Contextual Scopes
  date_iso: '2022-10-17'
  venue: ''
- arxiv_id: '2210.00643'
  title: Spectral Augmentation for Self-Supervised Learning on Graphs
  date_iso: '2022-10-02'
  venue: ICLR 2022
- arxiv_id: '2209.13964'
  title: Graph Soft-Contrastive Learning via Neighborhood Ranking
  date_iso: '2022-09-28'
  venue: ''
- arxiv_id: '2208.10493'
  title: Relational Self-Supervised Learning on Graphs
  date_iso: '2022-08-21'
  venue: ''
- arxiv_id: '2206.12933'
  title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised Learning
  date_iso: '2022-06-26'
  venue: AAAI 2022
- arxiv_id: '2206.05437'
  title: 'ACMP: Allen-Cahn Message Passing with Attractive and Repulsive Forces for
    Graph Neural Networks'
  date_iso: '2022-06-11'
  venue: ICLR 2022
- arxiv_id: '2206.04355'
  title: Graph Attention Multi-Layer Perceptron
  date_iso: '2022-06-09'
  venue: KDD 2022
- arxiv_id: '2206.03638'
  title: Alternately Optimized Graph Neural Networks
  date_iso: '2022-06-08'
  venue: ICML 2022
- arxiv_id: '2206.02796'
  title: Mixed Graph Contrastive Network for Semi-Supervised Node Classification
  date_iso: '2022-06-06'
  venue: ''
- arxiv_id: '2206.01535'
  title: 'Rethinking and Scaling Up Graph Contrastive Learning: An Extremely Efficient
    Approach with Group Discrimination'
  date_iso: '2022-06-03'
  venue: NeurIPS 2022
- arxiv_id: '2205.15746'
  title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
    Learning
  date_iso: '2022-05-31'
  venue: ICML 2022
- arxiv_id: '2203.00638'
  title: 'PaSca: a Graph Neural Architecture Search System under the Scalable Paradigm'
  date_iso: '2022-03-01'
  venue: WWW 2022
- arxiv_id: '2202.08391'
  title: Graph Masked Autoencoders with Transformers
  date_iso: '2022-02-17'
  venue: ''
- arxiv_id: '2201.12843'
  title: Graph Representation Learning via Aggregation Enhancement
  date_iso: '2022-01-30'
  venue: ''
- arxiv_id: '2112.14531'
  title: 'Designing the Topology of Graph Neural Networks: A Novel Feature Fusion
    Perspective'
  date_iso: '2021-12-29'
  venue: WWW 2021
- arxiv_id: '2112.03499'
  title: A Piece-wise Polynomial Filtering Approach for Graph Neural Networks
  date_iso: '2021-12-07'
  venue: ''
- arxiv_id: '2112.02472'
  title: Augmentation-Free Self-Supervised Learning on Graphs
  date_iso: '2021-12-05'
  venue: AAAI 2021
- arxiv_id: '2111.12128'
  title: On the Unreasonable Effectiveness of Feature Propagation in Learning on Graphs
    with Missing Node Features
  date_iso: '2021-11-23'
  venue: ''
- arxiv_id: '2110.15742'
  title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
  date_iso: '2021-10-29'
  venue: ''
- arxiv_id: '2110.14863'
  title: Graph Communal Contrastive Learning
  date_iso: '2021-10-28'
  venue: WWW 2021
- arxiv_id: '2110.11842'
  title: Multi-view Contrastive Graph Clustering
  date_iso: '2021-10-22'
  venue: NeurIPS 2021
- arxiv_id: '2110.09443'
  title: Beltrami Flow and Neural Diffusion on Graphs
  date_iso: '2021-10-18'
  venue: NeurIPS 2021
- arxiv_id: '2110.08727'
  title: 'Graph-less Neural Networks: Teaching Old MLPs New Tricks via Distillation'
  date_iso: '2021-10-17'
  venue: ICLR 2021
- arxiv_id: '2110.04099'
  title: Topology-Imbalance Learning for Semi-Supervised Node Classification
  date_iso: '2021-10-08'
  venue: NeurIPS 2021
- arxiv_id: '2108.10521'
  title: 'Bag of Tricks for Training Deeper Graph Neural Networks: A Comprehensive
    Benchmark Study'
  date_iso: '2021-08-24'
  venue: ''
- arxiv_id: '2107.11789'
  title: 'ROD: Reception-aware Online Distillation for Sparse Graphs'
  date_iso: '2021-07-25'
  venue: KDD 2021
- arxiv_id: '2107.06996'
  title: Elastic Graph Neural Networks
  date_iso: '2021-07-05'
  venue: ICML 2021
- arxiv_id: '2103.02885'
  title: 'Extract the Knowledge of Graph Neural Networks and Go Beyond it: An Effective
    Knowledge Distillation Framework'
  date_iso: '2021-03-04'
  venue: WWW 2021
- arxiv_id: '2101.11525'
  title: Calibrating and Improving Graph Contrastive Learning
  date_iso: '2021-01-27'
  venue: TMLR 2021
- arxiv_id: '2012.03476'
  title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised Classification'
  date_iso: '2020-12-07'
  venue: ''
- arxiv_id: '2010.14945'
  title: Graph Contrastive Learning with Adaptive Augmentation
  date_iso: '2020-10-27'
  venue: WWW 2020
- arxiv_id: '2010.01777'
  title: A Unified View on Graph Neural Networks as Graph Signal Denoising
  date_iso: '2020-10-05'
  venue: ''
- arxiv_id: '2011.01623'
  title: Learning on Attribute-Missing Graphs
  date_iso: '2020-10-01'
  venue: ''
- arxiv_id: '2009.09232'
  title: Learned Low Precision Graph Neural Networks
  date_iso: '2020-09-19'
  venue: ''
- arxiv_id: '2007.04583'
  title: Graph Convolutional Networks for Graphs Containing Missing Features
  date_iso: '2020-07-09'
  venue: ''
- arxiv_id: '2007.09296'
  title: Towards Deeper Graph Neural Networks
  date_iso: '2020-07-06'
  venue: KDD 2020
- arxiv_id: '2006.10222'
  title: Class-Attentive Diffusion Network for Semi-Supervised Classification
  date_iso: '2020-06-18'
  venue: AAAI 2020
- arxiv_id: '2004.13970'
  title: Directed Graph Convolutional Network
  date_iso: '2020-04-29'
  venue: ''
- arxiv_id: '2002.10306'
  title: Adaptive Propagation Graph Convolutional Network
  date_iso: '2020-02-24'
  venue: ''
- arxiv_id: '1911.07123'
  title: Graph-Revised Convolutional Network
  date_iso: '2019-11-17'
  venue: ''
- arxiv_id: '1909.03211'
  title: Measuring and Relieving the Over-smoothing Problem for Graph Neural Networks
    from the Topological View
  date_iso: '2019-09-07'
  venue: AAAI 2019
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 13752.0
    avg_edges: 245861.0
    num_classes: 10
    extra_stats:
      avg_degree: 35.758
      edge_feature_dim: 0
      edge_feature_type: co-purchase links; no edge attributes
      edge_homophily: 0.7853
      node_feature_dim: 767
      node_feature_type: sparse bag-of-words product-review features
      statistic_notes: PyG exposes 491,722 bidirected edge entries; this record stores
        245,861 unique undirected links
  metrics:
  - Accuracy
  - ACC
  - F1
  - Macro-F1
  - Micro-F1
  - ROC-AUC
  - Weighted-F1
  metric_display_names:
  - Accuracy
  - ACC
  - F1
  - Macro-F1
  - Micro-F1
  - ROC-AUC
  - Weighted-F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GraphTARIF
    model_plain: GraphTARIF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9461
    - null
    - null
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
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9412
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0008
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9398
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GCN+TS
    model_plain: GCN+TS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9398
    - null
    - null
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
    - null
    - null
  - model: GAT+T
    model_plain: GAT+T
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9386
    - null
    - null
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
    - null
    - null
  - model: Polynormer
    model_plain: Polynormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9378
    - null
    - null
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
    - null
    - null
  - model: Polynormer-r
    model_plain: Polynormer-r
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/cornell-zhang/Polynormer
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9368
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
  - model: SAGE
    model_plain: SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9351
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0006
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SAGE+T
    model_plain: SAGE+T
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9343
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0011
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Polynormer-v2
    model_plain: Polynormer-v2
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/cornell-zhang/Polynormer
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9325
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Polynormer
    model_plain: Polynormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/cornell-zhang/Polynormer
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9318
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Polynormer-v1
    model_plain: Polynormer-v1
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/cornell-zhang/Polynormer
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9318
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
    - null
    - null
    - null
    - null
  - model: OGFormer
    model_plain: OGFormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.929
    - null
    - null
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
    - null
    - null
  - model: TabPFN-GN
    model_plain: TabPFN-GN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2512.08798'
    title: Can TabPFN Compete with GNNs for Node Classification via Graph Tabularization?
    date: Dec 9, 2025
    date_iso: '2025-12-09'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: LoG 2025
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2025
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9271
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
  - model: CNA (TransformerConv)
    model_plain: CNA (TransformerConv)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_iso: '2024-12-05'
    date_display: Dec 2024
    codebase_url: https://github.com/ml-research/cna_modules
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9268
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0027
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
    - 0.9253
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0066
    - null
    - null
    - null
    - null
    - null
    - null
  - model: VecFormer
    model_plain: VecFormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_iso: '2026-02-23'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9251
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0054
    - null
    - null
    - null
    - null
    - null
    - null
  - model: BGAE + Att
    model_plain: BGAE + Att
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.15742'
    title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9244
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
  - model: DAM-GT
    model_plain: DAM-GT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_iso: '2025-05-23'
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
    - 0.9243
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SGFormer
    model_plain: SGFormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9242
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0066
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.02622'
    title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic Transforms'
    date: Oct 3, 2024
    date_iso: '2024-10-03'
    date_display: Oct 2024
    codebase_url: https://github.com/aidos-lab/Diss-l-ECT
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.924
    - null
    - null
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
    - 0.923
    - null
    - null
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
    - null
    - null
  - model: GOAT
    model_plain: GOAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9229
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0037
    - null
    - null
    - null
    - null
    - null
    - null
  - model: WaveGC
    model_plain: WaveGC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13806'
    title: A General Graph Spectral Wavelet Convolution via Chebyshev Order Decomposition
    date: May 22, 2024
    date_iso: '2024-05-22'
    date_display: May 2024
    codebase_url: https://github.com/liun-online/WaveGC
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9226
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Matrix-valued
    model_plain: Matrix-valued
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.13806'
    title: A General Graph Spectral Wavelet Convolution via Chebyshev Order Decomposition
    date: May 22, 2024
    date_iso: '2024-05-22'
    date_display: May 2024
    codebase_url: https://github.com/liun-online/WaveGC
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9226
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
  - model: BGAE
    model_plain: BGAE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.15742'
    title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    date: Oct 29, 2021
    date_iso: '2021-10-29'
    date_display: Oct 2021
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9224
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
  - model: LECT_1+LECT_2
    model_plain: LECT_1+LECT_2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2410.02622'
    title: 'Diss-l-ECT: Dissecting Graph Data with local Euler Characteristic Transforms'
    date: Oct 3, 2024
    date_iso: '2024-10-03'
    date_display: Oct 2024
    codebase_url: https://github.com/aidos-lab/Diss-l-ECT
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.922
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.006
    - null
    - null
    - null
    - null
    - null
    - null
  - model: WaveNet
    model_plain: WaveNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13806'
    title: A General Graph Spectral Wavelet Convolution via Chebyshev Order Decomposition
    date: May 22, 2024
    date_iso: '2024-05-22'
    date_display: May 2024
    codebase_url: https://github.com/liun-online/WaveGC
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9206
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0033
    - null
    - null
    - null
    - null
    - null
    - null
  - model: F^2GAT
    model_plain: F^2GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.14531'
    title: 'Designing the Topology of Graph Neural Networks: A Novel Feature Fusion
      Perspective'
    date: Dec 29, 2021
    date_iso: '2021-12-29'
    date_display: Dec 2021
    codebase_url: https://github.com/AutoML-Research/F2GNN
    published_conference: WWW 2021
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9204
    - null
    - null
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
    - null
    - null
  - model: OrderedGNN
    model_plain: OrderedGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/cornell-zhang/Polynormer
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9203
    - null
    - null
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
    - null
    - null
  - model: DIFFormer
    model_plain: DIFFormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/cornell-zhang/Polynormer
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9199
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0076
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Sine-Poly(A)-pl
    model_plain: Sine-Poly(A)-pl
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.15634'
    title: 'Beyond ReLU: Bifurcation, Oversmoothing, and Topological Priors'
    date: Feb 17, 2026
    date_iso: '2026-02-17'
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
    - 0.9194
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0007
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Polynormer
    model_plain: Polynormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_iso: '2026-02-23'
    date_display: Feb 2026
    codebase_url: ''
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9192
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0025
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GNNII (L4)
    model_plain: GNNII (L4)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.14531'
    title: 'Designing the Topology of Graph Neural Networks: A Novel Feature Fusion
      Perspective'
    date: Dec 29, 2021
    date_iso: '2021-12-29'
    date_display: Dec 2021
    codebase_url: https://github.com/AutoML-Research/F2GNN
    published_conference: WWW 2021
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9191
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0011
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GCNII-GAT
    model_plain: GCNII-GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.9191
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0011
    - null
    - null
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
    - 0.919
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
  - model: F^2SAGE
    model_plain: F^2SAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2112.14531'
    title: 'Designing the Topology of Graph Neural Networks: A Novel Feature Fusion
      Perspective'
    date: Dec 29, 2021
    date_iso: '2021-12-29'
    date_display: Dec 2021
    codebase_url: https://github.com/AutoML-Research/F2GNN
    published_conference: WWW 2021
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9181
    - null
    - null
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
    - null
    - null
  - model: GGCN
    model_plain: GGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_iso: '2024-03-02'
    date_display: Mar 2024
    codebase_url: https://github.com/cornell-zhang/Polynormer
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9181
    - null
    - null
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
    - null
    - null
  - model: GIRL
    model_plain: GIRL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2201.12843'
    title: Graph Representation Learning via Aggregation Enhancement
    date: Jan 30, 2022
    date_iso: '2022-01-30'
    date_display: Jan 2022
    codebase_url: https://github.com/Anonymous1252022/KR_for_GNNs
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.918
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0
    - null
    - null
    - null
    - null
    - null
    - null
  - model: JK (L4)
    model_plain: JK (L4)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.14531'
    title: 'Designing the Topology of Graph Neural Networks: A Novel Feature Fusion
      Perspective'
    date: Dec 29, 2021
    date_iso: '2021-12-29'
    date_display: Dec 2021
    codebase_url: https://github.com/AutoML-Research/F2GNN
    published_conference: WWW 2021
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.918
    - null
    - null
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
    - null
    - null
  - model: JK-GAT
    model_plain: JK-GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.918
    - null
    - null
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
    - null
    - null
  - model: NAGphormer-LGTL
    model_plain: NAGphormer-LGTL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_iso: '2025-05-19'
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
    - 0.9178
    - null
    - null
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
    - null
    - null
  - model: AdNGCL
    model_plain: AdNGCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.03076'
    title: Adaptive Negative Scheduling for Graph Contrastive Learning
    date: May 4, 2026
    date_iso: '2026-05-04'
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
    - 0.9176
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0029
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Random
    model_plain: Random
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2112.14531'
    title: 'Designing the Topology of Graph Neural Networks: A Novel Feature Fusion
      Perspective'
    date: Dec 29, 2021
    date_iso: '2021-12-29'
    date_display: Dec 2021
    codebase_url: https://github.com/AutoML-Research/F2GNN
    published_conference: WWW 2021
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9176
    - null
    - null
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
    - null
    - null
  - model: VCR-Graphormer
    model_plain: VCR-Graphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_iso: '2025-05-23'
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
    - 0.9175
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
  - model: STAGNN
    model_plain: STAGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.05296'
    title: Tailoring Self-Attention for Graph via Rooted Subtrees
    date: Oct 8, 2023
    date_iso: '2023-10-08'
    date_display: Oct 2023
    codebase_url: https://github.com/LUMIA-Group/SubTree-Attention
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9172
    - null
    - null
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
    - 0.9171
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0044
    - null
    - null
    - null
    - null
    - null
    - null
  - model: NTFormer
    model_plain: NTFormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.19249'
    title: 'NTFormer: A Composite Node Tokenized Graph Transformer for Node Classification'
    date: Jun 27, 2024
    date_iso: '2024-06-27'
    date_display: Jun 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9169
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0032
    - null
    - null
    - null
    - null
    - null
    - null
  - model: NAGphormer
    model_plain: NAGphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_iso: '2026-05-18'
    date_display: May 2026
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9169
    - null
    - null
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
    - null
    - null
  - model: DEFT
    model_plain: DEFT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13806'
    title: A General Graph Spectral Wavelet Convolution via Chebyshev Order Decomposition
    date: May 22, 2024
    date_iso: '2024-05-22'
    date_display: May 2024
    codebase_url: https://github.com/liun-online/WaveGC
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9163
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0052
    - null
    - null
    - null
    - null
    - null
    - null
  row_count: 789
  rows_json: /data/datasets/amazon-computers/standard-split-rows.json
  chart_json: /data/datasets/amazon-computers/standard-split-chart.json
  arch_counts:
    gnn: 521
    hybrid: 129
    graph_transformer: 45
    llm: 16
    walk: 12
    traditional: 42
  metric_counts:
  - 727
  - 18
  - 7
  - 12
  - 15
  - 16
  - 6
  milestones: &id001
  - value: 0.824
    std: 0.011
    model: acc
    arxiv_id: '1909.03211'
    title: Measuring and Relieving the Over-smoothing Problem for Graph Neural Networks
      from the Topological View
    date: '2019-09-07'
  - value: 0.837
    std: 0.018
    model: GRCN
    arxiv_id: '1911.07123'
    title: Graph-Revised Convolutional Network
    date: '2019-11-17'
  - value: 0.8518
    std: 0.0023
    model: AP-GCN
    arxiv_id: '2002.10306'
    title: Adaptive Propagation Graph Convolutional Network
    date: '2020-02-24'
  - value: 0.8641
    std: null
    model: GCNmf
    arxiv_id: '2007.04583'
    title: Graph Convolutional Networks for Graphs Containing Missing Features
    date: '2020-07-09'
  - value: 0.905
    std: 0.0
    model: LPGNAS
    arxiv_id: '2009.09232'
    title: Learned Low Precision Graph Neural Networks
    date: '2020-09-19'
  - value: 0.9244
    std: null
    model: BGAE + Att
    arxiv_id: '2110.15742'
    title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    date: '2021-10-29'
  - value: 0.9368
    std: 0.0021
    model: Polynormer-r
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: '2024-03-02'
  - value: 0.9461
    std: 0.0017
    model: GraphTARIF
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: '2026-05-18'
  milestones_by_metric:
    Accuracy: *id001
    ACC:
    - value: 0.9176
      std: 0.0063
      model: BORF
      arxiv_id: '2510.17457'
      title: 'Deeper with Riemannian Geometry: Overcoming Oversmoothing and Oversquashing
        for Graph Foundation Models'
      date: '2025-10-20'
    F1:
    - value: 0.9429
      std: 0.0052
      model: SDGNN
      arxiv_id: '2410.19723'
      title: Sparse Decomposition of Graph Neural Networks
      date: '2024-10-25'
    Macro-F1:
    - value: 0.8753
      std: 0.26
      model: gCooL_e
      arxiv_id: '2110.14863'
      title: Graph Communal Contrastive Learning
      date: '2021-10-28'
    Micro-F1:
    - value: 0.8885
      std: 0.14
      model: gCooL_c
      arxiv_id: '2110.14863'
      title: Graph Communal Contrastive Learning
      date: '2021-10-28'
    ROC-AUC:
    - value: 0.916
      std: 0.005
      model: GCN
      arxiv_id: '2504.19785'
      title: Heterophily-informed Message Passing
      date: '2025-04-28'
    Weighted-F1:
    - value: 0.79
      std: 0.011
      model: PPNP w/ RN
      arxiv_id: '2110.04099'
      title: Topology-Imbalance Learning for Semi-Supervised Node Classification
      date: '2021-10-08'
---

