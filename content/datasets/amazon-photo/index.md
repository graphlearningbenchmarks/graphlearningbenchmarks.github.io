---
title: Amazon-Photo
slug: amazon-photo
benchmark: Classic
task_type: node_classification
short_description: Predict each product’s category from review-derived features and
  product links on one co-purchase graph.
description: '**Node classification** on one co-purchase graph, predicting each product’s
  category from review-derived features and product links. Evaluated by Accuracy.'
detailed_description:
  task: Amazon co-purchase graph (Photo) node classification. The primary catalog
    metric is Accuracy.
  data: Amazon co-purchase graph (Photo) node classification.
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
- title: PyTorch Geometric Amazon-Photo loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.Amazon.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.Amazon.html
stats:
  num_graphs: 1
  avg_nodes: 7650.0
  avg_edges: 119081.0
  num_classes: 8
  extra_stats:
    avg_degree: 31.132
    edge_feature_dim: 0
    edge_feature_type: co-purchase links; no edge attributes
    edge_homophily: 0.8365
    node_feature_dim: 745
    node_feature_type: sparse bag-of-words product-review features
    statistic_notes: PyG exposes 238,162 bidirected edge entries; this record stores
      119,081 unique undirected links
result_count: 871
best_model:
  model: GraphTARIF
  value: 0.9703
  metric: Accuracy
  arxiv_id: '2510.10631'
  paper_title: 'GraphTARIF: Linear Graph Transformer with Augmented Rank and Improved
    Focus'
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
- arxiv_id: '2605.06814'
  title: 'From Model to Data (M2D): Shifting Complexity from GNNs to Graphs for Transparent
    Graph Learning'
  date_iso: '2026-05-07'
  venue: ''
- arxiv_id: '2605.03076'
  title: Adaptive Negative Scheduling for Graph Contrastive Learning
  date_iso: '2026-05-04'
  venue: ''
- arxiv_id: '2604.19028'
  title: Learning Posterior Predictive Distributions for Node Classification from
    Synthetic Graph Priors
  date_iso: '2026-04-21'
  venue: ICLR 2026
- arxiv_id: '2603.26178'
  title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
    Learning via Ricci Flow'
  date_iso: '2026-03-27'
  venue: ''
- arxiv_id: '2603.16849'
  title: 'GIST: Gauge-Invariant Spectral Transformers for Scalable Graph Neural Operators'
  date_iso: '2026-03-17'
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
- arxiv_id: '2602.05571'
  title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures via Adversarial
    Edge Masking'
  date_iso: '2026-02-05'
  venue: TMLR 2026
- arxiv_id: '2602.00064'
  title: 'SPGCL: Simple yet Powerful Graph Contrastive Learning via SVD-Guided Structural
    Perturbation'
  date_iso: '2026-01-20'
  venue: ''
- arxiv_id: '2512.24062'
  title: Energy-Balanced Hyperspherical Graph Representation Learning via Structural
    Binding and Entropic Dispersion
  date_iso: '2025-12-30'
  venue: ''
- arxiv_id: '2512.13235'
  title: 'CORE: Contrastive Masked Feature Reconstruction on Graphs'
  date_iso: '2025-12-15'
  venue: ''
- arxiv_id: '2512.11561'
  title: 'View Space: Learning Representation across Arbitrary Graphs'
  date_iso: '2025-12-12'
  venue: ICML 2025
- arxiv_id: '2512.08798'
  title: Can TabPFN Compete with GNNs for Node Classification via Graph Tabularization?
  date_iso: '2025-12-09'
  venue: LoG 2025
- arxiv_id: '2511.19976'
  title: Rethinking Semi-Supervised Node Classification with Self-Supervised Graph
    Clustering
  date_iso: '2025-11-25'
  venue: ''
- arxiv_id: '2510.10631'
  title: 'GraphTARIF: Linear Graph Transformer with Augmented Rank and Improved Focus'
  date_iso: '2025-10-12'
  venue: WWW 2025
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
- arxiv_id: '2506.15448'
  title: Semi-supervised Graph Anomaly Detection via Robust Homophily Learning
  date_iso: '2025-06-18'
  venue: NeurIPS 2025
- arxiv_id: '2506.13083'
  title: 'Uncertainty-Aware Graph Neural Networks: A Multi-Hop Evidence Fusion Approach'
  date_iso: '2025-06-16'
  venue: ''
- arxiv_id: '2506.06212'
  title: Model-Driven Graph Contrastive Learning
  date_iso: '2025-06-06'
  venue: ''
- arxiv_id: '2505.23014'
  title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in the Perspective of
    A System of Hyperbolic Partial Differential Equations'
  date_iso: '2025-05-29'
  venue: ICML 2025
- arxiv_id: '2505.19024'
  title: Learn Beneficial Noise as Graph Augmentation
  date_iso: '2025-05-25'
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
- arxiv_id: '2505.04808'
  title: Piecewise Constant Spectral Graph Neural Network
  date_iso: '2025-05-07'
  venue: TMLR 2025
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
- arxiv_id: '2503.03313'
  title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed Graph Foundation
    Models'
  date_iso: '2025-03-05'
  venue: ''
- arxiv_id: '2502.08092'
  title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
  date_iso: '2025-02-12'
  venue: KDD 2025
- arxiv_id: '2501.19089'
  title: Resolving Oversmoothing with Opinion Dissensus
  date_iso: '2025-01-31'
  venue: ''
- arxiv_id: '2501.15755'
  title: 'GraphICL: Unlocking Graph Learning Potential in LLMs through Structured
    Prompt Design'
  date_iso: '2025-01-27'
  venue: ''
- arxiv_id: '2412.21151'
  title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
  date_iso: '2024-12-30'
  venue: ''
- arxiv_id: '2412.19211'
  title: 'Large Language Models Meet Graph Neural Networks: A Perspective of Graph
    Mining'
  date_iso: '2024-12-26'
  venue: ''
- arxiv_id: '2412.16441'
  title: 'Towards Graph Foundation Models: Learning Generalities Across Graphs via
    Task-Trees'
  date_iso: '2024-12-21'
  venue: ICML 2024
- arxiv_id: '2412.07188'
  title: 'Graph Neural Networks Are More Than Filters: Revisiting and Benchmarking
    from A Spectral Perspective'
  date_iso: '2024-12-10'
  venue: ICLR 2024
- arxiv_id: '2412.06173'
  title: Revisiting the Necessity of Graph Learning and Common Graph Benchmarks
  date_iso: '2024-12-09'
  venue: ''
- arxiv_id: '2412.04064'
  title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
  date_iso: '2024-12-05'
  venue: NeurIPS 2024
- arxiv_id: '2411.17296'
  title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
  date_iso: '2024-11-26'
  venue: ICML 2024
- arxiv_id: '2411.16278'
  title: Even Sparser Graph Transformers
  date_iso: '2024-11-25'
  venue: NeurIPS 2024
- arxiv_id: '2411.05274'
  title: Distributed-Order Fractional Graph Operating Network
  date_iso: '2024-11-08'
  venue: NeurIPS 2024
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
- arxiv_id: '2408.01697'
  title: Invariant Graph Learning Meets Information Bottleneck for Out-of-Distribution
    Generalization
  date_iso: '2024-08-03'
  venue: ''
- arxiv_id: '2408.00165'
  title: Non-convolutional Graph Neural Networks
  date_iso: '2024-07-31'
  venue: NeurIPS 2024
- arxiv_id: '2407.19944'
  title: Noise-Resilient Unsupervised Graph Representation Learning via Multi-Hop
    Feature Quality Estimation
  date_iso: '2024-07-29'
  venue: ''
- arxiv_id: '2407.16726'
  title: Topology Reorganized Graph Contrastive Learning with Mitigating Semantic
    Drift
  date_iso: '2024-07-23'
  venue: ''
- arxiv_id: '2407.15431'
  title: Pre-Training and Prompting for Few-Shot Node Classification on Text-Attributed
    Graphs
  date_iso: '2024-07-22'
  venue: KDD 2024
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
- arxiv_id: '2407.11596'
  title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
  date_iso: '2024-06-30'
  venue: ''
- arxiv_id: '2406.19249'
  title: 'NTFormer: A Composite Node Tokenized Graph Transformer for Node Classification'
  date_iso: '2024-06-27'
  venue: ''
- arxiv_id: '2406.15044'
  title: 'From Overfitting to Robustness: Quantity, Quality, and Variety Oriented
    Negative Sample Selection in Graph Contrastive Learning'
  date_iso: '2024-06-21'
  venue: ''
- arxiv_id: '2406.12052'
  title: 'UniGLM: Training One Unified Language Model for Text-Attributed Graph Embedding'
  date_iso: '2024-06-17'
  venue: ''
- arxiv_id: '2406.10727'
  title: 'Text-space Graph Foundation Models: Comprehensive Benchmarks and New Insights'
  date_iso: '2024-06-15'
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
- arxiv_id: '2412.03864'
  title: Training MLPs on Graphs without Supervision
  date_iso: '2024-02-14'
  venue: ''
- arxiv_id: '2402.04621'
  title: 'Feature Distribution on Graph Topology Mediates the Effect of Graph Convolution:
    Homophily Perspective'
  date_iso: '2024-02-07'
  venue: ICML 2024
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
- arxiv_id: '2310.14527'
  title: 'Marginal Nodes Matter: Towards Structure Fairness in Graphs'
  date_iso: '2023-10-23'
  venue: KDD 2023
- arxiv_id: '2310.13845'
  title: Spectral-Aware Augmentation for Enhanced Graph Representation Learning
  date_iso: '2023-10-20'
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
- arxiv_id: '2310.00800'
  title: 'GraphPatcher: Mitigating Degree Bias for Graph Neural Networks via Test-time
    Augmentation'
  date_iso: '2023-10-01'
  venue: NeurIPS 2023
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
- arxiv_id: '2306.12091'
  title: Structure-Aware DropEdge Towards Deep Graph Convolutional Networks
  date_iso: '2023-06-21'
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
- arxiv_id: '2306.04004'
  title: Randomized Schur Complement Views for Graph Contrastive Learning
  date_iso: '2023-06-06'
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
- arxiv_id: '2305.17437'
  title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
  date_iso: '2023-05-27'
  venue: ''
- arxiv_id: '2305.15747'
  title: Union Subgraph Neural Networks
  date_iso: '2023-05-25'
  venue: AAAI 2023
- arxiv_id: '2305.06142'
  title: Feature Expansion for Graph Neural Networks
  date_iso: '2023-05-10'
  venue: ICML 2023
- arxiv_id: '2305.02866'
  title: Hierarchical Transformer for Scalable Graph Learning
  date_iso: '2023-05-04'
  venue: IJCAI 2023
- arxiv_id: '2305.00139'
  title: Leveraging Label Non-Uniformity for Node Classification in Graph Neural Networks
  date_iso: '2023-04-29'
  venue: ICML 2023
- arxiv_id: '2303.13750'
  title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
  date_iso: '2023-03-24'
  venue: ''
- arxiv_id: '2302.08727'
  title: Building Shortcuts between Distant Nodes with Biaffine Mapping for Graph
    Convolutional Networks
  date_iso: '2023-02-17'
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
- arxiv_id: '2212.07035'
  title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive Learning'
  date_iso: '2022-12-14'
  venue: AAAI 2022
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
- arxiv_id: '2211.14065'
  title: 'Beyond Smoothing: Unsupervised Graph Representation Learning with Edge Heterophily
    Discriminating'
  date_iso: '2022-11-25'
  venue: AAAI 2022
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
- arxiv_id: '2207.05887'
  title: Tuning the Geometry of Graph Neural Networks
  date_iso: '2022-07-12'
  venue: ''
- arxiv_id: '2206.12933'
  title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised Learning
  date_iso: '2022-06-26'
  venue: AAAI 2022
- arxiv_id: '2206.09166'
  title: 'NAS-Bench-Graph: Benchmarking Graph Neural Architecture Search'
  date_iso: '2022-06-18'
  venue: NeurIPS 2022
- arxiv_id: '2206.05437'
  title: 'ACMP: Allen-Cahn Message Passing with Attractive and Repulsive Forces for
    Graph Neural Networks'
  date_iso: '2022-06-11'
  venue: ICLR 2022
- arxiv_id: '2206.04355'
  title: Graph Attention Multi-Layer Perceptron
  date_iso: '2022-06-09'
  venue: KDD 2022
- arxiv_id: '2206.04471'
  title: 'Towards Understanding Graph Neural Networks: An Algorithm Unrolling Perspective'
  date_iso: '2022-06-09'
  venue: ''
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
- arxiv_id: '2205.09335'
  title: A Simple Yet Effective SVD-GCN for Directed Graphs
  date_iso: '2022-05-19'
  venue: ''
- arxiv_id: '2203.00638'
  title: 'PaSca: a Graph Neural Architecture Search System under the Scalable Paradigm'
  date_iso: '2022-03-01'
  venue: WWW 2022
- arxiv_id: '2202.08391'
  title: Graph Masked Autoencoders with Transformers
  date_iso: '2022-02-17'
  venue: ''
- arxiv_id: '2202.08480'
  title: Eliciting Structural and Semantic Global Knowledge in Unsupervised Graph
    Contrastive Learning
  date_iso: '2022-02-17'
  venue: AAAI 2022
- arxiv_id: '2201.12843'
  title: Graph Representation Learning via Aggregation Enhancement
  date_iso: '2022-01-30'
  venue: ''
- arxiv_id: '2201.09830'
  title: Learning Graph Augmentations to Learn Graph Representations
  date_iso: '2022-01-24'
  venue: ''
- arxiv_id: '2112.02472'
  title: Augmentation-Free Self-Supervised Learning on Graphs
  date_iso: '2021-12-05'
  venue: AAAI 2021
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
- arxiv_id: '2105.05682'
  title: Multi-Scale Contrastive Siamese Networks for Self-Supervised Graph Representation
    Learning
  date_iso: '2021-05-12'
  venue: IJCAI 2021
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
- arxiv_id: '2003.07450'
  title: Spectral Graph Attention Network with Fast Eigen-approximation
  date_iso: '2020-03-17'
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
    avg_nodes: 7650.0
    avg_edges: 119081.0
    num_classes: 8
    extra_stats:
      avg_degree: 31.132
      edge_feature_dim: 0
      edge_feature_type: co-purchase links; no edge attributes
      edge_homophily: 0.8365
      node_feature_dim: 745
      node_feature_type: sparse bag-of-words product-review features
      statistic_notes: PyG exposes 238,162 bidirected edge entries; this record stores
        119,081 unique undirected links
  metrics:
  - Accuracy
  - ACC
  - AUROC
  - Macro-F1
  - Micro-F1
  - Normalized AUAC
  - ROC-AUC
  - Recall
  - Weighted-F1
  metric_display_names:
  - Accuracy
  - ACC
  - AUROC
  - Macro-F1
  - Micro-F1
  - Normalized AUAC
  - ROC-AUC
  - Recall
  - Weighted-F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GraphTARIF
    model_plain: GraphTARIF
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.10631'
    title: 'GraphTARIF: Linear Graph Transformer with Augmented Rank and Improved
      Focus'
    date: Oct 12, 2025
    date_iso: '2025-10-12'
    date_display: Oct 2025
    codebase_url: ''
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9703
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
    - 0.9669
    - null
    - null
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
    - 0.9666
    - null
    - null
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
    - 0.966
    - null
    - null
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
    - 0.9657
    - null
    - null
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
    - 0.9651
    - null
    - null
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
    - 0.9646
    - null
    - null
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
    - 0.9643
    - null
    - null
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
    - 0.9632
    - null
    - null
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
    - 0.9621
    - null
    - null
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
    - 0.9617
    - null
    - null
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
    - 0.9614
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
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
    - 0.9611
    - null
    - null
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
    - 0.9611
    - null
    - null
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
    - 0.9609
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
    - null
    - null
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
    - 0.9601
    - null
    - null
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
    - 0.9596
    - null
    - null
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
    - null
    - null
  - model: ChebNetII
    model_plain: ChebNetII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.23014'
    title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in the Perspective
      of A System of Hyperbolic Partial Differential Equations'
    date: May 29, 2025
    date_iso: '2025-05-29'
    date_display: May 2025
    codebase_url: https://github.com/YueAWu/Hyperbolic-GNN
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9588
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0058
    - null
    - null
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
    - 0.9584
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0041
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: VCR-Graphormer-LGTL
    model_plain: VCR-Graphormer-LGTL
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
    - 0.9582
    - null
    - null
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
    - null
    - null
  - model: Specformer
    model_plain: Specformer
    is_baseline: true
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
    - 0.958
    - null
    - null
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
    - null
    - null
  - model: GRAND
    model_plain: GRAND
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_iso: '2025-04-22'
    date_display: Apr 2025
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9579
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0059
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: APPNP
    model_plain: APPNP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.9573
    - null
    - null
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
    - null
    - null
  - model: CGT
    model_plain: CGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.9573
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0084
    - null
    - null
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
    - 0.957
    - null
    - null
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
    - null
    - null
  - model: Sine-Poly(A)-sh
    model_plain: Sine-Poly(A)-sh
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
    - 0.9569
    - null
    - null
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
    - 0.9568
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0036
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PieCoN
    model_plain: PieCoN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.04808'
    title: Piecewise Constant Spectral Graph Neural Network
    date: May 7, 2025
    date_iso: '2025-05-07'
    date_display: May 2025
    codebase_url: https://github.com/vmart20/PieCoN
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9565
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0034
    - null
    - null
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
    - 0.9564
    - null
    - null
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
    - null
    - null
  - model: GIST
    model_plain: GIST
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.16849'
    title: 'GIST: Gauge-Invariant Spectral Transformers for Scalable Graph Neural
      Operators'
    date: Mar 17, 2026
    date_iso: '2026-03-17'
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
    - 0.9561
    - null
    - null
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
    - null
    - null
  - model: GWN-fa
    model_plain: GWN-fa
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_iso: '2025-04-22'
    date_display: Apr 2025
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9561
    - null
    - null
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
    - 0.956
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
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GOAL
    model_plain: GOAL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.07608'
    title: 'Finding the Missing-half: Graph Complementary Learning for Homophily-prone
      and Heterophily-prone Graphs'
    date: Jun 13, 2023
    date_iso: '2023-06-13'
    date_display: Jun 2023
    codebase_url: https://github.com/zyzisastudyreallyhardguy/GOAL-Graph-Complementary-Learning
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.956
    - null
    - null
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
    - 0.9558
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0036
    - null
    - null
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
    - 0.9555
    - null
    - null
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
    - 0.9553
    - null
    - null
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
    - null
    - null
  - model: GrokFormer
    model_plain: GrokFormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_iso: '2024-11-26'
    date_display: Nov 2024
    codebase_url: https://github.com/GGA23/GrokFormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9552
    - null
    - null
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
    - 0.955
    - null
    - null
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
    - 0.9549
    - null
    - null
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
    - null
    - null
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.9549
    - null
    - null
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
    - null
    - null
  - model: H2GCN
    model_plain: H2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_iso: '2023-06-04'
    date_display: Jun 2023
    codebase_url: https://github.com/GISec-Team/NCGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9548
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
  - model: FE-GNN
    model_plain: FE-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2305.06142'
    title: Feature Expansion for Graph Neural Networks
    date: May 10, 2023
    date_iso: '2023-05-10'
    date_display: May 2023
    codebase_url: https://github.com/sajqavril/Feature-Extension-Graph-Neural-Networks
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9545
    - null
    - null
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
    - 0.9544
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
  - model: JacobiConv
    model_plain: JacobiConv
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.13750'
    title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
    date: Mar 24, 2023
    date_iso: '2023-03-24'
    date_display: Mar 2023
    codebase_url: https://github.com/TaoLbr1993/LON-GNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9543
    - null
    - null
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
    - null
    - null
  - model: GNSN
    model_plain: GNSN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.21247'
    title: Graph Navier–Stokes Networks
    date: May 20, 2026
    date_iso: '2026-05-20'
    date_display: May 2026
    codebase_url: https://github.com/Duckbluee/Graph-Navier-Stokes-Networks
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9543
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0126
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SGT
    model_plain: SGT
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
    - 0.9537
    - null
    - null
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
    - 0.9535
    - null
    - null
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
    - null
    - null
  - model: GAT+GPL
    model_plain: GAT+GPL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.11361'
    title: 'Graph Structure Prompt Learning: A Novel Methodology to Improve Performance
      of Graph Neural Networks'
    date: Jul 16, 2024
    date_iso: '2024-07-16'
    date_display: Jul 2024
    codebase_url: https://github.com/PreckLi/graph_prompt_learning
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9535
    - null
    - null
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
    - null
    - null
  - model: HiGCN
    model_plain: HiGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.17296'
    title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    date: Nov 26, 2024
    date_iso: '2024-11-26'
    date_display: Nov 2024
    codebase_url: https://github.com/GGA23/GrokFormer
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9533
    - null
    - null
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
    - null
    - null
  - model: ADC
    model_plain: ADC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_iso: '2025-04-22'
    date_display: Apr 2025
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    published_conference: WWW 2025
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9533
    - null
    - null
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
    - null
    - null
  row_count: 871
  rows_json: /data/datasets/amazon-photo/standard-split-rows.json
  chart_json: /data/datasets/amazon-photo/standard-split-chart.json
  arch_counts:
    gnn: 586
    hybrid: 126
    graph_transformer: 48
    llm: 17
    walk: 16
    traditional: 50
  metric_counts:
  - 807
  - 4
  - 12
  - 12
  - 12
  - 14
  - 16
  - 1
  - 6
  milestones: &id001
  - value: 0.915
    std: 0.005
    model: acc
    arxiv_id: '1909.03211'
    title: Measuring and Relieving the Over-smoothing Problem for Graph Neural Networks
      from the Topological View
    date: '2019-09-07'
  - value: 0.928
    std: 0.002
    model: SpGAT-Cheby-MAX
    arxiv_id: '2003.07450'
    title: Spectral Graph Attention Network with Fast Eigen-approximation
    date: '2020-03-17'
  - value: 0.9308
    std: null
    model: NCGNN-A
    arxiv_id: '2012.03476'
    title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised Classification'
    date: '2020-12-07'
  - value: 0.9313
    std: 0.0032
    model: GCA
    arxiv_id: '2101.11525'
    title: Calibrating and Improving Graph Contrastive Learning
    date: '2021-01-27'
  - value: 0.932
    std: 0.007
    model: ROD
    arxiv_id: '2107.11789'
    title: 'ROD: Reception-aware Online Distillation for Sparse Graphs'
    date: '2021-07-25'
  - value: 0.9322
    std: 0.0028
    model: AFGRL
    arxiv_id: '2112.02472'
    title: Augmentation-Free Self-Supervised Learning on Graphs
    date: '2021-12-05'
  - value: 0.941
    std: 0.004
    model: LG2AR + GRU
    arxiv_id: '2201.09830'
    title: Learning Graph Augmentations to Learn Graph Representations
    date: '2022-01-24'
  - value: 0.956
    std: 0.001
    model: GIRL
    arxiv_id: '2201.12843'
    title: Graph Representation Learning via Aggregation Enhancement
    date: '2022-01-30'
  - value: 0.9564
    std: 0.0027
    model: STAGNN
    arxiv_id: '2310.05296'
    title: Tailoring Self-Attention for Graph via Rooted Subtrees
    date: '2023-10-08'
  - value: 0.9568
    std: 0.0036
    model: SignGT
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: '2023-10-17'
  - value: 0.9646
    std: 0.0026
    model: Polynormer-r
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: '2024-03-02'
  - value: 0.9666
    std: 0.0013
    model: DAM-GT
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: '2025-05-23'
  - value: 0.9703
    std: null
    model: GraphTARIF
    arxiv_id: '2510.10631'
    title: 'GraphTARIF: Linear Graph Transformer with Augmented Rank and Improved
      Focus'
    date: '2025-10-12'
  milestones_by_metric:
    Accuracy: *id001
    ACC:
    - value: 0.9109
      std: null
      model: SAGE
      arxiv_id: '2310.14527'
      title: 'Marginal Nodes Matter: Towards Structure Fairness in Graphs'
      date: '2023-10-23'
    AUROC:
    - value: 0.7129
      std: null
      model: RHO
      arxiv_id: '2506.15448'
      title: Semi-supervised Graph Anomaly Detection via Robust Homophily Learning
      date: '2025-06-18'
    Macro-F1:
    - value: 0.9205
      std: 0.0017
      model: gCooL_c
      arxiv_id: '2110.14863'
      title: Graph Communal Contrastive Learning
      date: '2021-10-28'
    Micro-F1:
    - value: 0.9318
      std: 0.0012
      model: gCooL_c
      arxiv_id: '2110.14863'
      title: Graph Communal Contrastive Learning
      date: '2021-10-28'
    Normalized AUAC:
    - value: 0.6903
      std: 0.023
      model: GCNII
      arxiv_id: '2412.07188'
      title: 'Graph Neural Networks Are More Than Filters: Revisiting and Benchmarking
        from A Spectral Perspective'
      date: '2024-12-10'
    ROC-AUC:
    - value: 0.955
      std: 0.004
      model: GraphSAGE
      arxiv_id: '2504.19785'
      title: Heterophily-informed Message Passing
      date: '2025-04-28'
    Recall:
    - value: 0.786
      std: 0.0015
      model: PATTON
      arxiv_id: '2412.19211'
      title: 'Large Language Models Meet Graph Neural Networks: A Perspective of Graph
        Mining'
      date: '2024-12-26'
    Weighted-F1:
    - value: 0.897
      std: 0.01
      model: PPNP w/ RN
      arxiv_id: '2110.04099'
      title: Topology-Imbalance Learning for Semi-Supervised Node Classification
      date: '2021-10-08'
---

