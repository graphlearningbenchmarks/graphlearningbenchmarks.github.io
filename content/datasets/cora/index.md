---
title: Cora
slug: cora
benchmark: Classic
task_type: node_classification
short_description: Predict one of seven research-topic labels for every paper in a
  single citation network.
description: '**Node classification** Predict one of seven research-topic labels for
  every paper in a single citation network. Evaluated by Accuracy.'
detailed_description:
  task: Predict one of seven research-topic labels for every paper in a single citation
    network. The standard Planetoid formulation is transductive, so the features and
    graph position of validation and test nodes are available during training while
    their labels are withheld.
  data: The commonly used Planetoid version contains 2,708 machine-learning papers
    connected by citation links. It is a processed subset of the larger Cora research-paper
    collection; other datasets called Cora, including citation-matching corpora and
    Cora-ML, are not interchangeable with it.
  features: Each paper has a sparse 1,433-dimensional binary bag-of-words vector indicating
    selected vocabulary terms. PyG exposes 10,556 directed edge entries after processing
    the citation relations and reports seven classes.
  splits_and_evaluation: The fixed public Planetoid split uses 20 labeled training
    nodes per class, 500 validation nodes, and 1,000 test nodes. Other common protocols
    include full-label, random, Geom-GCN, and cross-validation splits; their accuracy
    values should not be pooled with the public split.
  quirks_and_pitfalls: Cora is small, highly reused, and sensitive to the exact preprocessing
    and split. Published work sometimes reports results for Cora-ML or a random split
    simply as Cora. The OGB benchmark paper also reports feature-label leakage and
    duplicate-node concerns in this processed dataset, reinforcing the need to state
    the loader and split precisely rather than treating all Cora results as comparable.
sources:
- title: Revisiting Semi-Supervised Learning with Graph Embeddings
  arxiv_id: '1603.08861'
  kind: split_definition
- title: PyTorch Geometric Planetoid documentation and loader
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.Planetoid.html
  kind: loader_documentation
- title: Andrew McCallum's Cora data page
  url: https://people.cs.umass.edu/mccallum/data.html
  kind: upstream_data_source
- title: Open Graph Benchmark
  arxiv_id: '2005.00687'
  kind: dataset_audit
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.Planetoid.html
stats: null
result_count: 1352
best_model:
  model: MATE
  value: 0.946
  metric: Accuracy
  arxiv_id: '2407.20067'
  paper_title: 'xAI-Drop: Don''t Use What You Cannot Explain'
papers:
- arxiv_id: '2606.00757'
  title: 'RADE: Random Add-Drop Edge as a Regularizer'
  date_iso: '2026-05-30'
  venue: ICML 2026
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
- arxiv_id: '2605.03514'
  title: 'Revisiting Graph-Tokenizing Large Language Models: A Systematic Evaluation
    of Graph Token Understanding'
  date_iso: '2026-05-05'
  venue: ''
- arxiv_id: '2605.03076'
  title: Adaptive Negative Scheduling for Graph Contrastive Learning
  date_iso: '2026-05-04'
  venue: ''
- arxiv_id: '2604.24293'
  title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
    via Continuous Phase Transitions'
  date_iso: '2026-04-27'
  venue: ''
- arxiv_id: '2604.19028'
  title: Learning Posterior Predictive Distributions for Node Classification from
    Synthetic Graph Priors
  date_iso: '2026-04-21'
  venue: ICLR 2026
- arxiv_id: '2604.01878'
  title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph Contrastive Learning'
  date_iso: '2026-04-02'
  venue: ''
- arxiv_id: '2603.26178'
  title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
    Learning via Ricci Flow'
  date_iso: '2026-03-27'
  venue: ''
- arxiv_id: '2603.05004'
  title: Poisoning the Inner Prediction Logic of Graph Neural Networks for Clean-Label
    Backdoor Attacks
  date_iso: '2026-03-05'
  venue: TMLR 2026
- arxiv_id: '2603.02938'
  title: 'Beyond One-Size-Fits-All: Adaptive Subgraph Denoising for Zero-Shot Graph
    Learning with Large Language Models'
  date_iso: '2026-03-03'
  venue: ''
- arxiv_id: '2602.15634'
  title: 'Beyond ReLU: Bifurcation, Oversmoothing, and Topological Priors'
  date_iso: '2026-02-17'
  venue: ''
- arxiv_id: '2602.09258'
  title: Generalizing GNNs with Tokenized Mixture of Experts
  date_iso: '2026-02-09'
  venue: KDD 2026
- arxiv_id: '2601.22943'
  title: 'Scalable Topology-Preserving Graph Coarsening: Concepts and Algorithms'
  date_iso: '2026-01-30'
  venue: ''
- arxiv_id: '2601.21369'
  title: 'Rethinking Federated Graph Foundation Models: A Graph-Language Alignment-based
    Approach'
  date_iso: '2026-01-29'
  venue: ''
- arxiv_id: '2602.00064'
  title: 'SPGCL: Simple yet Powerful Graph Contrastive Learning via SVD-Guided Structural
    Perturbation'
  date_iso: '2026-01-20'
  venue: ''
- arxiv_id: '2601.08230'
  title: 'GADPN: Graph Adaptive Denoising and Perturbation Networks via Singular Value
    Decomposition'
  date_iso: '2026-01-13'
  venue: ''
- arxiv_id: '2601.07419'
  title: 'Position: Don''t be Afraid of Over-Smoothing And Over-Squashing'
  date_iso: '2026-01-12'
  venue: ''
- arxiv_id: '2512.13235'
  title: 'CORE: Contrastive Masked Feature Reconstruction on Graphs'
  date_iso: '2025-12-15'
  venue: ''
- arxiv_id: '2511.19976'
  title: Rethinking Semi-Supervised Node Classification with Self-Supervised Graph
    Clustering
  date_iso: '2025-11-25'
  venue: ''
- arxiv_id: '2511.16062'
  title: Gauge-Equivariant Graph Networks via Self-Interference Cancellation
  date_iso: '2025-11-20'
  venue: ''
- arxiv_id: '2510.04522'
  title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
    for Graph Generation and Prediction'
  date_iso: '2025-10-06'
  venue: NeurIPS 2025
- arxiv_id: '2509.22416'
  title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained Models'
  date_iso: '2025-09-26'
  venue: NeurIPS 2025
- arxiv_id: '2508.20597'
  title: Local Virtual Nodes for Alleviating Over-Squashing in Graph Neural Networks
  date_iso: '2025-08-28'
  venue: ''
- arxiv_id: '2508.09320'
  title: Exact Verification of Graph Neural Networks with Incremental Constraint Solving
  date_iso: '2025-08-12'
  venue: ''
- arxiv_id: '2507.14484'
  title: 'ReDiSC: A Reparameterized Masked Diffusion Model for Scalable Node Classification
    with Structured Predictions'
  date_iso: '2025-07-19'
  venue: ''
- arxiv_id: '2506.19343'
  title: Discrepancy-Aware Graph Mask Auto-Encoder
  date_iso: '2025-06-24'
  venue: KDD 2025
- arxiv_id: '2506.14291'
  title: 'Equivariance Everywhere All At Once: A Recipe for Graph Foundation Models'
  date_iso: '2025-06-17'
  venue: ''
- arxiv_id: '2506.07168'
  title: Efficient Text-Attributed Graph Learning through Selective Annotation and
    Graph Alignment
  date_iso: '2025-06-08'
  venue: TMLR 2025
- arxiv_id: '2506.06582'
  title: 'Demystifying Topological Message-Passing with Relational Structures: A Case
    Study on Oversquashing in Simplicial Message-Passing'
  date_iso: '2025-06-06'
  venue: ICLR 2025
- arxiv_id: '2505.14033'
  title: 'Partition-wise Graph Filtering: A Unified Perspective Through the Lens of
    Graph Coarsening'
  date_iso: '2025-05-20'
  venue: KDD 2025
- arxiv_id: '2505.15845'
  title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
    Learning Models'
  date_iso: '2025-05-19'
  venue: ''
- arxiv_id: '2505.05533'
  title: Rethinking Graph Contrastive Learning through Relative Similarity Preservation
  date_iso: '2025-05-08'
  venue: IJCAI 2025
- arxiv_id: '2504.20430'
  title: Learning Laplacian Positional Encodings for Heterophilous Graphs
  date_iso: '2025-04-29'
  venue: ''
- arxiv_id: '2503.19666'
  title: 'Towards Efficient Training of Graph Neural Networks: A Multiscale Approach'
  date_iso: '2025-03-25'
  venue: TMLR 2025
- arxiv_id: '2503.12563'
  title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
  date_iso: '2025-03-16'
  venue: TMLR 2025
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
- arxiv_id: '2501.09178'
  title: Enhancing Graph Representation Learning with Localized Topological Features
  date_iso: '2025-01-15'
  venue: JMLR 2025
- arxiv_id: '2412.06173'
  title: Revisiting the Necessity of Graph Learning and Common Graph Benchmarks
  date_iso: '2024-12-09'
  venue: ''
- arxiv_id: '2412.04064'
  title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
  date_iso: '2024-12-05'
  venue: NeurIPS 2024
- arxiv_id: '2411.04356'
  title: 'GaGSL: Global-augmented Graph Structure Learning via Graph Information Bottleneck'
  date_iso: '2024-11-07'
  venue: ''
- arxiv_id: '2410.05593'
  title: When Graph Neural Networks Meet Dynamic Mode Decomposition
  date_iso: '2024-10-08'
  venue: ICLR 2024
- arxiv_id: '2410.02158'
  title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation Learning'
  date_iso: '2024-10-03'
  venue: TMLR 2024
- arxiv_id: '2411.01157'
  title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
  date_iso: '2024-10-01'
  venue: ''
- arxiv_id: '2409.09111'
  title: 'Transformers from Diffusion: A Unified Framework for Neural Message Passing'
  date_iso: '2024-09-13'
  venue: JMLR 2024
- arxiv_id: '2408.13471'
  title: Disentangled Generative Graph Representation Learning
  date_iso: '2024-08-24'
  venue: ''
- arxiv_id: '2408.07654'
  title: 'Graph Triple Attention Network: A Decoupled Perspective'
  date_iso: '2024-08-14'
  venue: ''
- arxiv_id: '2408.03152'
  title: 'TSC: A Simple Two-Sided Constraint against Over-Smoothing'
  date_iso: '2024-08-06'
  venue: KDD 2024
- arxiv_id: '2407.20067'
  title: 'xAI-Drop: Don''t Use What You Cannot Explain'
  date_iso: '2024-07-29'
  venue: LoG 2024
- arxiv_id: '2407.14996'
  title: 'All Against Some: Efficient Integration of Large Language Models for Message
    Passing in Graph Neural Networks'
  date_iso: '2024-07-20'
  venue: ''
- arxiv_id: '2407.09381'
  title: The Effectiveness of Curvature-Based Rewiring and the Role of Hyperparameters
    in GNNs Revisited
  date_iso: '2024-07-12'
  venue: ICLR 2024
- arxiv_id: '2407.08064'
  title: 'TinyGraph: Joint Feature and Node Condensation for Graph Neural Networks'
  date_iso: '2024-07-10'
  venue: ''
- arxiv_id: '2407.04236'
  title: Graph Pooling via Ricci Flow
  date_iso: '2024-07-05'
  venue: TMLR 2024
- arxiv_id: '2406.10871'
  title: Graph Neural Reaction Diffusion Models Submitted to the editors June 2023.
    Accepted in March 2024.
  date_iso: '2024-06-16'
  venue: ''
- arxiv_id: '2406.10727'
  title: 'Text-space Graph Foundation Models: Comprehensive Benchmarks and New Insights'
  date_iso: '2024-06-15'
  venue: NeurIPS 2024
- arxiv_id: '2406.05346'
  title: 'ProG: A Graph Prompt Learning Benchmark'
  date_iso: '2024-06-08'
  venue: NeurIPS 2024
- arxiv_id: '2406.01899'
  title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models'
  date_iso: '2024-06-04'
  venue: NeurIPS 2024
- arxiv_id: '2405.20445'
  title: Fully-inductive Node Classification on Arbitrary Graphs
  date_iso: '2024-05-30'
  venue: ICLR 2024
- arxiv_id: '2405.18581'
  title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation Decomposition
    via Large Language Models'
  date_iso: '2024-05-28'
  venue: ''
- arxiv_id: '2405.14742'
  title: 'HC-GAE: The Hierarchical Cluster-based Graph Auto-Encoder for Graph Representation
    Learning'
  date_iso: '2024-05-23'
  venue: NeurIPS 2024
- arxiv_id: '2405.13902'
  title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training Framework'
  date_iso: '2024-05-22'
  venue: ''
- arxiv_id: '2405.12474'
  title: 'How Universal Polynomial Bases Enhance Spectral Graph Neural Networks: Heterophily,
    Over-smoothing, and Over-squashing'
  date_iso: '2024-05-21'
  venue: ICML 2024
- arxiv_id: '2405.03401'
  title: 'E2GNN: Efficient Graph Neural Network Ensembles for Semi-Supervised Classification'
  date_iso: '2024-05-06'
  venue: ''
- arxiv_id: '2404.15354'
  title: 'Polynomial Selection in Spectral Graph Neural Networks: An Error-Sum of
    Function Slices Approach'
  date_iso: '2024-04-15'
  venue: WWW 2024
- arxiv_id: '2404.04559'
  title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
  date_iso: '2024-04-06'
  venue: ''
- arxiv_id: '2403.20221'
  title: Graph Neural Aggregation-diffusion with Metastability
  date_iso: '2024-03-29'
  venue: ''
- arxiv_id: '2403.14951'
  title: Simple Graph Condensation
  date_iso: '2024-03-22'
  venue: ''
- arxiv_id: '2403.07943'
  title: Revisiting Edge Perturbation for Graph Neural Network in Graph Data Augmentation
    and Attack
  date_iso: '2024-03-10'
  venue: ''
- arxiv_id: '2403.01079'
  title: 'Teaching MLP More Graph Information: A Three-stage Multitask Knowledge Distillation
    Framework.'
  date_iso: '2024-03-02'
  venue: ''
- arxiv_id: '2402.10468'
  title: Adversarial Curriculum Graph Contrastive Learning with Pair-wise Augmentation
  date_iso: '2024-02-16'
  venue: ''
- arxiv_id: '2402.05894'
  title: Large Language Model Meets Graph Neural Network in Knowledge Distillation
  date_iso: '2024-02-08'
  venue: AAAI 2024
- arxiv_id: '2402.05011'
  title: 'Navigating Complexity: Toward Lossless Graph Condensation via Expanding
    Window Matching'
  date_iso: '2024-02-07'
  venue: ICML 2024
- arxiv_id: '2402.04924'
  title: 'Two Trades are not Baffled: Condensing Graph via Crafting Rational Gradient
    Matching'
  date_iso: '2024-02-07'
  venue: ''
- arxiv_id: '2402.05962'
  title: 'EXGC: Bridging Efficiency and Explainability in Graph Condensation'
  date_iso: '2024-02-05'
  venue: WWW 2024
- arxiv_id: '2401.15569'
  title: Efficient Tuning and Inference for Large Language Models on Textual Graphs
  date_iso: '2024-01-28'
  venue: IJCAI 2024
- arxiv_id: '2401.14580'
  title: 'Design your own universe: a physics-informed agnostic method for enhancing
    graph neural networks'
  date_iso: '2024-01-26'
  venue: ''
- arxiv_id: '2401.09125'
  title: Understanding Heterophily for Graph Neural Networks
  date_iso: '2024-01-17'
  venue: ICML 2024
- arxiv_id: '2312.04737'
  title: Efficient End-to-end Language Model Fine-tuning on Graphs
  date_iso: '2023-12-07'
  venue: KDD 2023
- arxiv_id: '2401.12780'
  title: 'DeepRicci: Self-supervised Graph Structure-Feature Co-Refinement for Alleviating
    Over-squashing'
  date_iso: '2023-12-01'
  venue: ''
- arxiv_id: '2311.18177'
  title: An Effective Universal Polynomial Basis for Spectral Graph Neural Networks
  date_iso: '2023-11-30'
  venue: ''
- arxiv_id: '2311.17781'
  title: 'Propagate & Distill: Towards Effective Graph Learners Using Propagation-Embracing
    MLPs'
  date_iso: '2023-11-29'
  venue: LoG 2023
- arxiv_id: '2311.14864'
  title: Effective Structural Encodings via Local Curvature Profiles
  date_iso: '2023-11-24'
  venue: ICLR 2023
- arxiv_id: '2310.16421'
  title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
  date_iso: '2023-10-25'
  venue: ''
- arxiv_id: '2310.14527'
  title: 'Marginal Nodes Matter: Towards Structure Fairness in Graphs'
  date_iso: '2023-10-23'
  venue: KDD 2023
- arxiv_id: '2310.13845'
  title: Spectral-Aware Augmentation for Enhanced Graph Representation Learning
  date_iso: '2023-10-20'
  venue: ''
- arxiv_id: '2310.11046'
  title: Fast Graph Condensation with Structure-based Neural Tangent Kernel
  date_iso: '2023-10-17'
  venue: WWW 2023
- arxiv_id: '2310.10064'
  title: Shape-aware Graph Spectral Learning
  date_iso: '2023-10-16'
  venue: ''
- arxiv_id: '2310.01089'
  title: 'GraphText: Graph Reasoning in Text Space'
  date_iso: '2023-10-02'
  venue: ''
- arxiv_id: '2310.01618'
  title: 'Operator Learning Meets Numerical Analysis: Improving Neural Networks through
    Iterative Methods'
  date_iso: '2023-10-02'
  venue: ''
- arxiv_id: '2310.00697'
  title: Learning How to Propagate Messages in Graph Neural Networks
  date_iso: '2023-10-01'
  venue: KDD 2023
- arxiv_id: '2310.00183'
  title: On the Equivalence of Graph Convolution and Mixup
  date_iso: '2023-09-29'
  venue: TMLR 2023
- arxiv_id: '2309.04082'
  title: 'Curve Your Attention: Mixed-Curvature Transformers for Graph Representation
    Learning'
  date_iso: '2023-09-08'
  venue: ''
- arxiv_id: '2308.15614'
  title: 'Everything Perturbed All at Once: Enabling Differentiable Graph Attacks'
  date_iso: '2023-08-29'
  venue: WWW 2023
- arxiv_id: '2308.10737'
  title: 'UGSL: A Unified Framework for Benchmarking Graph Structure Learning'
  date_iso: '2023-08-21'
  venue: ''
- arxiv_id: '2308.08235'
  title: 'The Expressive Power of Graph Neural Networks: A Survey'
  date_iso: '2023-08-16'
  venue: ''
- arxiv_id: '2308.07134'
  title: Language is All a Graph Needs
  date_iso: '2023-08-14'
  venue: ''
- arxiv_id: '2308.02117'
  title: 'VQGraph: Rethinking Graph Representation Space for Bridging GNNs and MLPs'
  date_iso: '2023-08-04'
  venue: ICLR 2023
- arxiv_id: '2307.16092'
  title: Feature Transportation Improves Graph Neural Networks
  date_iso: '2023-07-29'
  venue: AAAI 2023
- arxiv_id: '2307.16026'
  title: 'MUSE: Multi-View Contrastive Learning for Heterophilic Graphs'
  date_iso: '2023-07-29'
  venue: ''
- arxiv_id: '2307.09768'
  title: How Curvature Enhance the Adaptation Power of Framelet GCNs
  date_iso: '2023-07-19'
  venue: ''
- arxiv_id: '2307.06631'
  title: Frameless Graph Knowledge Distillation
  date_iso: '2023-07-13'
  venue: ''
- arxiv_id: '2307.01053'
  title: 'ENGAGE: Explanation Guided Data Augmentation for Graph Representation Learning'
  date_iso: '2023-07-03'
  venue: ''
- arxiv_id: '2307.00534'
  title: Shared Growth of Graph Neural Networks via Prompted Free-direction Knowledge
    Distillation
  date_iso: '2023-07-02'
  venue: ''
- arxiv_id: '2306.10466'
  title: 'Graph Ladling: Shockingly Simple Parallel GNN Training without Intermediate
    Communication'
  date_iso: '2023-06-18'
  venue: ICML 2023
- arxiv_id: '2306.09614'
  title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
  date_iso: '2023-06-16'
  venue: KDD 2023
- arxiv_id: '2306.02117'
  title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
  date_iso: '2023-06-03'
  venue: ''
- arxiv_id: '2305.15747'
  title: Union Subgraph Neural Networks
  date_iso: '2023-05-25'
  venue: AAAI 2023
- arxiv_id: '2305.13115'
  title: 'Causal-Based Supervision of Attention in Graph Neural Network: A Better
    and Simpler Choice towards Powerful Attention'
  date_iso: '2023-05-22'
  venue: IJCAI 2023
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
- arxiv_id: '2302.14806'
  title: Framelet Message Passing
  date_iso: '2023-02-28'
  venue: ''
- arxiv_id: '2302.12357'
  title: 'Auto-HeG: Automated Graph Neural Network on Heterophilic Graphs'
  date_iso: '2023-02-23'
  venue: WWW 2023
- arxiv_id: '2302.08727'
  title: Building Shortcuts between Distant Nodes with Biaffine Mapping for Graph
    Convolutional Networks
  date_iso: '2023-02-17'
  venue: ''
- arxiv_id: '2301.09474'
  title: 'Discovering Data Geometry: Energy-Driven Neural Diffusion'
  date_iso: '2023-01-23'
  venue: ICLR 2023
- arxiv_id: '2212.02483'
  title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
  date_iso: '2022-12-05'
  venue: ICML 2022
- arxiv_id: '2211.15335'
  title: 'You Can Have Better Graph Neural Networks by Not Training Weights at All:
    Finding Untrained GNNs Tickets'
  date_iso: '2022-11-28'
  venue: LoG 2022
- arxiv_id: '2211.15081'
  title: Mitigating Overfitting in Graph Neural Networks via Feature and Hyperplane
    Perturbation
  date_iso: '2022-11-28'
  venue: ''
- arxiv_id: '2211.14065'
  title: 'Beyond Smoothing: Unsupervised Graph Representation Learning with Edge Heterophily
    Discriminating'
  date_iso: '2022-11-25'
  venue: AAAI 2022
- arxiv_id: '2211.11761'
  title: 'From Node Interaction to Hop Interaction: New Effective and Scalable Graph
    Learning Paradigm'
  date_iso: '2022-11-21'
  venue: ''
- arxiv_id: '2211.06605'
  title: Comprehensive Analysis of Over-smoothing in Graph Neural Networks from Markov
    Chains Perspective
  date_iso: '2022-11-12'
  venue: ''
- arxiv_id: '2211.03710'
  title: Graph Contrastive Learning with Implicit Augmentations
  date_iso: '2022-11-07'
  venue: ''
- arxiv_id: '2210.10946'
  title: Causally-guided Regularization of Graph Attention Improves Generalizability
  date_iso: '2022-10-20'
  venue: TMLR 2022
- arxiv_id: '2210.07715'
  title: 'Not All Neighbors Are Worth Attending to: Graph Selective Attention Networks
    for Semi-supervised Learning'
  date_iso: '2022-10-14'
  venue: ''
- arxiv_id: '2210.08122'
  title: 'Old can be Gold: Better Gradient Flow can Make Vanilla-GCNs Great Again'
  date_iso: '2022-10-14'
  venue: NeurIPS 2022
- arxiv_id: '2210.03801'
  title: 'Augmentations in Hypergraph Contrastive Learning: Fabricated and Generative'
  date_iso: '2022-10-07'
  venue: NeurIPS 2022
- arxiv_id: '2209.15454'
  title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel Geometric Polynomials'
  date_iso: '2022-09-30'
  venue: ''
- arxiv_id: '2208.10010'
  title: 'NOSMOG: Learning Noise-robust and Structure-aware MLPs on Graphs'
  date_iso: '2022-08-22'
  venue: NeurIPS 2022
- arxiv_id: '2208.06743'
  title: Enhancing Graph Contrastive Learning with Node Similarity
  date_iso: '2022-08-13'
  venue: ''
- arxiv_id: '2206.13510'
  title: Structural Entropy Guided Graph Hierarchical Pooling
  date_iso: '2022-06-26'
  venue: ICML 2022
- arxiv_id: '2206.09166'
  title: 'NAS-Bench-Graph: Benchmarking Graph Neural Architecture Search'
  date_iso: '2022-06-18'
  venue: NeurIPS 2022
- arxiv_id: '2206.07746'
  title: Condensing Graphs via One-Step Gradient Matching
  date_iso: '2022-06-15'
  venue: KDD 2022
- arxiv_id: '2206.03601'
  title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
  date_iso: '2022-06-07'
  venue: ''
- arxiv_id: '2206.02796'
  title: Mixed Graph Contrastive Network for Semi-Supervised Node Classification
  date_iso: '2022-06-06'
  venue: ''
- arxiv_id: '2205.07266'
  title: Discovering the Representation Bottleneck of Graph Neural Networks
  date_iso: '2022-05-15'
  venue: ''
- arxiv_id: '2204.06127'
  title: 'Reinforcement learning on graphs: A survey'
  date_iso: '2022-04-13'
  venue: ''
- arxiv_id: '2204.04874'
  title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
  date_iso: '2022-04-11'
  venue: ''
- arxiv_id: '2203.14082'
  title: Metropolis-Hastings Data Augmentation for Graph Neural Networks
  date_iso: '2022-03-26'
  venue: NeurIPS 2022
- arxiv_id: '2203.12265'
  title: Node Representation Learning in Graph via Node-to-Neighbourhood Mutual Information
    Maximization
  date_iso: '2022-03-23'
  venue: ''
- arxiv_id: '2203.16097'
  title: Neighbor Enhanced Graph Convolutional Networks for Node Classification and
    Recommendation
  date_iso: '2022-03-01'
  venue: ''
- arxiv_id: '2203.00199'
  title: Equivariant and Stable Positional Encoding for More Powerful Graph Neural
    Networks
  date_iso: '2022-03-01'
  venue: ICLR 2022
- arxiv_id: '2202.08391'
  title: Graph Masked Autoencoders with Transformers
  date_iso: '2022-02-17'
  venue: ''
- arxiv_id: '2202.02296'
  title: Graph-Coupled Oscillator Networks
  date_iso: '2022-02-04'
  venue: ICML 2022
- arxiv_id: '2201.13410'
  title: 'Weisfeiler and Leman Go Infinite: Spectral and Combinatorial Pre-Colorings'
  date_iso: '2022-01-31'
  venue: TMLR 2022
- arxiv_id: '2201.05493'
  title: Contrastive Laplacian Eigenmaps
  date_iso: '2022-01-14'
  venue: NeurIPS 2022
- arxiv_id: '2201.01288'
  title: 'Automated Graph Machine Learning: Approaches, Libraries, Benchmarks and
    Directions'
  date_iso: '2022-01-04'
  venue: ''
- arxiv_id: '2112.14531'
  title: 'Designing the Topology of Graph Neural Networks: A Novel Feature Fusion
    Perspective'
  date_iso: '2021-12-29'
  venue: WWW 2021
- arxiv_id: '2112.13507'
  title: Block Modeling-Guided Graph Convolutional Neural Networks
  date_iso: '2021-12-27'
  venue: AAAI 2021
- arxiv_id: '2111.14522'
  title: Understanding over-squashing and bottlenecks on graphs via curvature
  date_iso: '2021-11-29'
  venue: ICLR 2021
- arxiv_id: '2111.06748'
  title: Simplifying approach to Node Classification in Graph Neural Networks
  date_iso: '2021-11-12'
  venue: ''
- arxiv_id: '2110.15777'
  title: 'GBK-GNN: Gated Bi-Kernel Graph Neural Networks for Modeling Both Homophily
    and Heterophily'
  date_iso: '2021-10-29'
  venue: WWW 2021
- arxiv_id: '2110.08727'
  title: 'Graph-less Neural Networks: Teaching Old MLPs New Tricks via Distillation'
  date_iso: '2021-10-17'
  venue: ICLR 2021
- arxiv_id: '2109.11338'
  title: Orthogonal Graph Neural Networks
  date_iso: '2021-09-23'
  venue: AAAI 2021
- arxiv_id: '2108.12055'
  title: Towards Self-Explainable Graph Neural Network
  date_iso: '2021-08-26'
  venue: ''
- arxiv_id: '2108.06280'
  title: Understanding Structural Vulnerability in Graph Convolutional Networks
  date_iso: '2021-08-01'
  venue: IJCAI 2021
- arxiv_id: '2106.10934'
  title: 'GRAND: Graph Neural Diffusion'
  date_iso: '2021-06-21'
  venue: ICML 2021
- arxiv_id: '2106.05150'
  title: Scaling Up Graph Neural Networks Via Graph Coarsening
  date_iso: '2021-06-09'
  venue: KDD 2021
- arxiv_id: '2106.04051'
  title: 'Graph-MLP: Node Classification without Message Passing in Graph'
  date_iso: '2021-06-08'
  venue: ''
- arxiv_id: '2106.02892'
  title: Training Robust Graph Neural Networks with Topology Adaptive Edge Dropping
  date_iso: '2021-06-05'
  venue: ''
- arxiv_id: '2105.07634'
  title: Improving Graph Neural Networks with Simple Architecture Design
  date_iso: '2021-05-17'
  venue: ''
- arxiv_id: '2104.10569'
  title: 'GraphTheta: A Distributed Graph Neural Network Learning System With Flexible
    Training Strategy'
  date_iso: '2021-04-21'
  venue: ''
- arxiv_id: '2104.04987'
  title: 'AutoGL: A Library for Automated Graph Learning'
  date_iso: '2021-04-11'
  venue: ICLR 2021
- arxiv_id: '2103.14958'
  title: 'SelfGNN: Self-supervised Graph Neural Networks without explicit negative
    sampling'
  date_iso: '2021-03-27'
  venue: WWW 2021
- arxiv_id: '2103.14991'
  title: Graph Unlearning
  date_iso: '2021-03-27'
  venue: ''
- arxiv_id: '2103.13355'
  title: Bag of Tricks for Node Classification with Graph Neural Networks
  date_iso: '2021-03-24'
  venue: ''
- arxiv_id: '2103.07295'
  title: Adversarial Graph Disentanglement with Component-specific Aggregation
  date_iso: '2021-03-12'
  venue: ''
- arxiv_id: '2103.06064'
  title: Graph Neural Networks Inspired by Classical Iterative Algorithms
  date_iso: '2021-03-10'
  venue: ICML 2021
- arxiv_id: '2103.02885'
  title: 'Extract the Knowledge of Graph Neural Networks and Go Beyond it: An Effective
    Knowledge Distillation Framework'
  date_iso: '2021-03-04'
  venue: WWW 2021
- arxiv_id: '2102.06986'
  title: How Framelets Enhance Graph Neural Networks
  date_iso: '2021-02-13'
  venue: ICML 2021
- arxiv_id: '2102.03147'
  title: Learning Conjoint Attentions for Graph Neural Nets
  date_iso: '2021-02-05'
  venue: NeurIPS 2021
- arxiv_id: '2012.07437'
  title: Rethinking the Promotion Brought by Contrastive Learning to Semi-Supervised
    Node Classification
  date_iso: '2020-12-14'
  venue: IJCAI 2020
- arxiv_id: '2011.07057'
  title: 'Learning to Drop: Robust Graph Neural Network via Topological Denoising'
  date_iso: '2020-11-13'
  venue: ''
- arxiv_id: '2010.15421'
  title: Scalable Graph Neural Networks via Bidirectional Propagation
  date_iso: '2020-10-29'
  venue: NeurIPS 2020
- arxiv_id: '2010.11797'
  title: Should Graph Convolution Trust Neighbors? A Simple Causal Inference Method
  date_iso: '2020-10-22'
  venue: ''
- arxiv_id: '2010.07565'
  title: 'Bi-GCN: Binary Graph Convolutional Network'
  date_iso: '2020-10-15'
  venue: ''
- arxiv_id: '2009.14332'
  title: Multi-hop Attention Graph Neural Networks
  date_iso: '2020-09-29'
  venue: IJCAI 2020
- arxiv_id: '2009.09232'
  title: Learned Low Precision Graph Neural Networks
  date_iso: '2020-09-19'
  venue: ''
- arxiv_id: '2009.07111'
  title: Contrastive and Generative Graph Convolutional Networks for Graph-based Semi-Supervised
    Learning
  date_iso: '2020-09-15'
  venue: AAAI 2020
- arxiv_id: '2009.02027'
  title: Rethinking Graph Regularization for Graph Neural Networks
  date_iso: '2020-09-04'
  venue: AAAI 2020
- arxiv_id: '2009.00934'
  title: 'SAIL: Self-Augmented Graph Contrastive Learning'
  date_iso: '2020-09-02'
  venue: AAAI 2020
- arxiv_id: '2008.12578'
  title: Graph Convolutional Neural Networks with Node Transition Probability-based
    Message Passing and DropNode Regularization
  date_iso: '2020-08-28'
  venue: ''
- arxiv_id: '2008.09864'
  title: Tackling Over-Smoothing for General Graph Convolutional Networks
  date_iso: '2020-08-22'
  venue: ''
- arxiv_id: '2007.02133'
  title: Simple and Deep Graph Convolutional Networks
  date_iso: '2020-07-04'
  venue: ICML 2020
- arxiv_id: '2006.10141'
  title: 'Self-supervised Learning on Graphs: Deep Insights and New Directions'
  date_iso: '2020-06-17'
  venue: ''
- arxiv_id: '2006.07107'
  title: Understanding and Resolving Performance Degradation in Deep Graph Convolutional
    Networks
  date_iso: '2020-06-12'
  venue: ''
- arxiv_id: '2006.06972'
  title: Towards Deeper Graph Neural Networks with Differentiable Group Normalization
  date_iso: '2020-06-12'
  venue: NeurIPS 2020
- arxiv_id: '2006.03814'
  title: The Impact of Global Structural Information in Graph Neural Networks Applications
  date_iso: '2020-06-06'
  venue: ''
- arxiv_id: '2005.14612'
  title: Non-Local Graph Neural Networks
  date_iso: '2020-05-29'
  venue: ''
- arxiv_id: '2003.13663'
  title: Revisiting Oversmoothing in Deep GCNs
  date_iso: '2020-03-30'
  venue: ''
- arxiv_id: '2003.08414'
  title: 'Scattering GCN: Overcoming Oversmoothness in Graph Convolutional Networks'
  date_iso: '2020-03-18'
  venue: NeurIPS 2020
- arxiv_id: '2003.07450'
  title: Spectral Graph Attention Network with Fast Eigen-approximation
  date_iso: '2020-03-17'
  venue: ''
- arxiv_id: '2002.10413'
  title: Neural Message Passing on High Order Paths
  date_iso: '2020-02-24'
  venue: ''
- arxiv_id: '2001.05140'
  title: 'Graph-Bert: Only Attention is Needed for Learning Graph Representations'
  date_iso: '2020-01-15'
  venue: ''
- arxiv_id: '1912.00967'
  title: Continuous Graph Neural Networks
  date_iso: '2019-12-02'
  venue: ICML 2019
- arxiv_id: '1911.07532'
  title: Graph Neural Ordinary Differential Equations
  date_iso: '2019-11-18'
  venue: AAAI 2019
- arxiv_id: '1910.02370'
  title: 'GraphZoom: A Multi-level Spectral Approach for Accurate and Scalable Graph
    Embedding'
  date_iso: '2019-10-06'
  venue: ICLR 2019
- arxiv_id: '1909.11715'
  title: 'GraphMix: Improved Training of GNNs for Semi-Supervised Learning'
  date_iso: '2019-09-25'
  venue: ''
- arxiv_id: '1909.13021'
  title: Multi-Scale Attributed Node Embedding
  date_iso: '2019-09-25'
  venue: ''
- arxiv_id: '1909.03184'
  title: 'Auto-GNN: Neural Architecture Search of Graph Neural Networks'
  date_iso: '2019-09-07'
  venue: ''
- arxiv_id: '1909.00958'
  title: 'Graph Representation Learning: A Survey'
  date_iso: '2019-09-03'
  venue: ''
- arxiv_id: '2101.03464'
  title: 'SPAGAN: Shortest Path Graph Attention Network'
  date_iso: '2019-08-01'
  venue: IJCAI 2019
- arxiv_id: '1907.04786'
  title: Fast Haar Transforms for Graph Neural Networks
  date_iso: '2019-07-10'
  venue: ''
- arxiv_id: '1905.13728'
  title: Pre-Training Graph Neural Networks for Generic Structural Feature Extraction
  date_iso: '2019-05-31'
  venue: ''
- arxiv_id: '1905.10029'
  title: Power up! Robust Graph Convolutional Network via Graph Powering
  date_iso: '2019-05-24'
  venue: AAAI 2019
- arxiv_id: '1905.05178'
  title: Graph U-Nets
  date_iso: '2019-05-11'
  venue: ''
- arxiv_id: '1903.11960'
  title: Learning Discrete Structures for Graph Neural Networks
  date_iso: '2019-03-28'
  venue: ICML 2019
- arxiv_id: '1901.00596'
  title: A Comprehensive Survey on Graph Neural Networks
  date_iso: '2019-01-01'
  venue: ''
- arxiv_id: '1812.04202'
  title: 'Deep Learning on Graphs: A Survey'
  date_iso: '2018-12-11'
  venue: ''
- arxiv_id: '1802.01572'
  title: 'MotifNet: a motif-based Graph Convolutional Network for directed graphs'
  date_iso: '2018-02-04'
  venue: ''
- arxiv_id: '1711.08920'
  title: 'SplineCNN: Fast Geometric Deep Learning with Continuous B-Spline Kernels'
  date_iso: '2017-11-24'
  venue: ''
- arxiv_id: '1710.10903'
  title: Graph Attention Networks
  date_iso: '2017-10-30'
  venue: ICLR 2017
- arxiv_id: '1710.10370'
  title: Topology Adaptive Graph Convolutional Networks
  date_iso: '2017-10-28'
  venue: ''
- arxiv_id: '1611.08402'
  title: Geometric deep learning on graphs and manifolds using mixture model CNNs
  date_iso: '2016-11-25'
  venue: ''
- arxiv_id: '1603.08861'
  title: Revisiting Semi-Supervised Learning with Graph Embeddings
  date_iso: '2016-03-29'
  venue: ICML 2016
variants:
- slug: planetoid-split
  name: Planetoid split
  notes: Yang et al. 2016 fixed 20-per-class train split.
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - Accuracy
  - AUC
  - F1
  - F1-macro
  - F1-micro
  - Loss
  - NMI
  metric_display_names:
  - Accuracy
  - AUC
  - F1
  - F1-macro
  - F1-micro
  - Loss
  - NMI
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: MATE
    model_plain: MATE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_iso: '2024-07-29'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: LoG 2024
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.946
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
  - model: GraphSAGE+CNA
    model_plain: GraphSAGE+CNA
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9418
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
  - model: DropAggr
    model_plain: DropAggr
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_iso: '2024-07-29'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: LoG 2024
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.938
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.011
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DropNode
    model_plain: DropNode
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_iso: '2024-07-29'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: LoG 2024
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.937
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
  - model: GCN+CNA
    model_plain: GCN+CNA
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9366
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0048
    - null
    - null
    - null
    - null
    - null
    - null
  - model: TransformerConv
    model_plain: TransformerConv
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.935
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
  - model: DropEdge
    model_plain: DropEdge
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_iso: '2024-07-29'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: LoG 2024
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.932
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
  - model: GAT + CNA
    model_plain: GAT + CNA
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
    - 0.9294
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
  - model: DropMess
    model_plain: DropMess
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_iso: '2024-07-29'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: LoG 2024
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2024
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
    - 0.007
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ENGAGE
    model_plain: ENGAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_iso: '2024-07-29'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: LoG 2024
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2024
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
    - 0.007
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GCN Baseline
    model_plain: GCN Baseline
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_iso: '2024-07-29'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: LoG 2024
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.928
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
  - model: ExPass
    model_plain: ExPass
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_iso: '2024-07-29'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: LoG 2024
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.928
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
  - model: PromptGFM
    model_plain: PromptGFM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2503.03313'
    title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed Graph Foundation
      Models'
    date: Mar 5, 2025
    date_iso: '2025-03-05'
    date_display: Mar 2025
    codebase_url: https://github.com/agiresearch/PromptGFM
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
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Policy-GNN
    model_plain: Policy-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2204.06127'
    title: 'Reinforcement learning on graphs: A survey'
    date: Apr 13, 2022
    date_iso: '2022-04-13'
    date_display: Apr 2022
    codebase_url: https://github.com/clvrai/agile
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
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
    - 0.014
    - null
    - null
    - null
    - null
    - null
    - null
  - model: RGCN + RSE (70b)
    model_plain: RGCN + RSE (70b)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_iso: '2024-05-28'
    date_display: May 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9177
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0038
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GraphSAGE_(Llama3)
    model_plain: GraphSAGE_(Llama3)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.05894'
    title: Large Language Model Meets Graph Neural Network in Knowledge Distillation
    date: Feb 8, 2024
    date_iso: '2024-02-08'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.917
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0051
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GAT_(Llama3)
    model_plain: GAT_(Llama3)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.05894'
    title: Large Language Model Meets Graph Neural Network in Knowledge Distillation
    date: Feb 8, 2024
    date_iso: '2024-02-08'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9151
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
  - model: LinguGraph-Llama3 (8B)
    model_plain: LinguGraph-Llama3 (8B)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 8.0
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2402.05894'
    title: Large Language Model Meets Graph Neural Network in Knowledge Distillation
    date: Feb 8, 2024
    date_iso: '2024-02-08'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9151
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0046
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ENGINE
    model_plain: ENGINE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2401.15569'
    title: Efficient Tuning and Inference for Large Language Models on Textual Graphs
    date: Jan 28, 2024
    date_iso: '2024-01-28'
    date_display: Jan 2024
    codebase_url: https://github.com/ZhuYun97/ENGINE
    published_conference: IJCAI 2024
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9148
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
  - model: SeHGNN + RSE (8b)
    model_plain: SeHGNN + RSE (8b)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_iso: '2024-05-28'
    date_display: May 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9138
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
  - model: GIN_(Llama3)
    model_plain: GIN_(Llama3)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.05894'
    title: Large Language Model Meets Graph Neural Network in Knowledge Distillation
    date: Feb 8, 2024
    date_iso: '2024-02-08'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9133
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0028
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ChebNet2D
    model_plain: ChebNet2D
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.04559'
    title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    date: Apr 6, 2024
    date_iso: '2024-04-06'
    date_display: Apr 2024
    codebase_url: https://github.com/jianhao2016/GPRGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9124
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
  - model: TAPE
    model_plain: TAPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    date: Jun 8, 2025
    date_iso: '2025-06-08'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9119
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
  - model: Flan-T5-base
    model_plain: Flan-T5-base
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2308.07134'
    title: Language is All a Graph Needs
    date: Aug 14, 2023
    date_iso: '2023-08-14'
    date_display: Aug 2023
    codebase_url: https://github.com/agiresearch/InstructGLM
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9077
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
  - model: GCN_(Llama3)
    model_plain: GCN_(Llama3)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.05894'
    title: Large Language Model Meets Graph Neural Network in Knowledge Distillation
    date: Feb 8, 2024
    date_iso: '2024-02-08'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: AAAI 2024
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9077
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0028
    - null
    - null
    - null
    - null
    - null
    - null
  - model: InstructGLM
    model_plain: InstructGLM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2310.16421'
    title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    date: Oct 25, 2023
    date_iso: '2023-10-25'
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
    - 0.9077
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
  - model: GA
    model_plain: GA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.16421'
    title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    date: Oct 25, 2023
    date_iso: '2023-10-25'
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
    - 0.9065
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
  - model: HAN + RSE (70b)
    model_plain: HAN + RSE (70b)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_iso: '2024-05-28'
    date_display: May 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9031
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0038
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SSP
    model_plain: SSP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    - 0.9016
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
  - model: Learn2Drop
    model_plain: Learn2Drop
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_iso: '2024-07-29'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: LoG 2024
    published_conference_short: LoG
    published_conference_slug: log
    published_venue: LoG 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.901
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
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_iso: '2024-01-17'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9004
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
  - model: RDGNN-I
    model_plain: RDGNN-I
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.10871'
    title: Graph Neural Reaction Diffusion Models Submitted to the editors June 2023.
      Accepted in March 2024.
    date: Jun 16, 2024
    date_iso: '2024-06-16'
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
    - 0.8991
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.011
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
    - 0.8989
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
  - model: PDNAS-4
    model_plain: PDNAS-4
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2009.09232'
    title: Learned Low Precision Graph Neural Networks
    date: Sep 19, 2020
    date_iso: '2020-09-19'
    date_display: Sep 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.898
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
  - model: LPGNAS
    model_plain: LPGNAS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2009.09232'
    title: Learned Low Precision Graph Neural Networks
    date: Sep 19, 2020
    date_iso: '2020-09-19'
    date_display: Sep 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.898
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
    - 0.8978
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
  - model: ACM-GCN
    model_plain: ACM-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.16421'
    title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    date: Oct 25, 2023
    date_iso: '2023-10-25'
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
    - 0.8975
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
  - model: GAGA
    model_plain: GAGA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    date: Jun 8, 2025
    date_iso: '2025-06-08'
    date_display: Jun 2025
    codebase_url: ''
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8967
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
  - model: Snowball-V3
    model_plain: Snowball-V3
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2308.07134'
    title: Language is All a Graph Needs
    date: Aug 14, 2023
    date_iso: '2023-08-14'
    date_display: Aug 2023
    codebase_url: https://github.com/agiresearch/InstructGLM
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8959
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0158
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ACM-Snowball-3
    model_plain: ACM-Snowball-3
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.16421'
    title: 'Graph Agent: Explicit Reasoning Agent for Graphs'
    date: Oct 25, 2023
    date_iso: '2023-10-25'
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
    - 0.8959
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
  - model: RDGNN-S
    model_plain: RDGNN-S
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.10871'
    title: Graph Neural Reaction Diffusion Models Submitted to the editors June 2023.
      Accepted in March 2024.
    date: Jun 16, 2024
    date_iso: '2024-06-16'
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
    - 0.8953
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0122
    - null
    - null
    - null
    - null
    - null
    - null
  - model: UniMP + RSE (70b)
    model_plain: UniMP + RSE (70b)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_iso: '2024-05-28'
    date_display: May 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8952
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
  - model: UniFilter
    model_plain: UniFilter
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.18177'
    title: An Effective Universal Polynomial Basis for Spectral Graph Neural Networks
    date: Nov 30, 2023
    date_iso: '2023-11-30'
    date_display: Nov 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8949
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0135
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SplineCNN
    model_plain: SplineCNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1711.08920'
    title: 'SplineCNN: Fast Geometric Deep Learning with Continuous B-Spline Kernels'
    date: Nov 24, 2017
    date_iso: '2017-11-24'
    date_display: Nov 2017
    codebase_url: https://github.com/pyg-team/pytorch_geometric
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8948
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0031
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
    - 0.8945
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
  - model: ADR-GNN_S
    model_plain: ADR-GNN_S
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.16092'
    title: Feature Transportation Improves Graph Neural Networks
    date: Jul 29, 2023
    date_iso: '2023-07-29'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8943
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
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.04559'
    title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    date: Apr 6, 2024
    date_iso: '2024-04-06'
    date_display: Apr 2024
    codebase_url: https://github.com/jianhao2016/GPRGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8941
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
  - model: NewtonNet
    model_plain: NewtonNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.10064'
    title: Shape-aware Graph Spectral Learning
    date: Oct 16, 2023
    date_iso: '2023-10-16'
    date_display: Oct 2023
    codebase_url: https://github.com/junjie-xu/NewtonNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8939
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.014
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ReLU-Poly(A)-sh
    model_plain: ReLU-Poly(A)-sh
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
    - 0.8933
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0038
    - null
    - null
    - null
    - null
    - null
    - null
  - model: ReLU-Poly(A)-pl
    model_plain: ReLU-Poly(A)-pl
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
    - 0.8933
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
  row_count: 1352
  rows_json: /data/datasets/cora/planetoid-split-rows.json
  chart_json: /data/datasets/cora/planetoid-split-chart.json
  arch_counts:
    gnn: 841
    hybrid: 158
    graph_transformer: 36
    llm: 45
    walk: 27
    traditional: 144
  metric_counts:
  - 1285
  - 8
  - 46
  - 8
  - 8
  - 6
  - 9
  milestones: &id001
  - value: 0.757
    std: null
    model: Planetoid-T
    arxiv_id: '1603.08861'
    title: Revisiting Semi-Supervised Learning with Graph Embeddings
    date: '2016-03-29'
  - value: 0.8169
    std: 0.0048
    model: mixture model CNNs
    arxiv_id: '1611.08402'
    title: Geometric deep learning on graphs and manifolds using mixture model CNNs
    date: '2016-11-25'
  - value: 0.833
    std: 0.007
    model: TAGCN
    arxiv_id: '1710.10370'
    title: Topology Adaptive Graph Convolutional Networks
    date: '2017-10-28'
  - value: 0.8948
    std: 0.0031
    model: SplineCNN
    arxiv_id: '1711.08920'
    title: 'SplineCNN: Fast Geometric Deep Learning with Continuous B-Spline Kernels'
    date: '2017-11-24'
  - value: 0.898
    std: 0.003
    model: PDNAS-4
    arxiv_id: '2009.09232'
    title: Learned Low Precision Graph Neural Networks
    date: '2020-09-19'
  - value: 0.919
    std: 0.014
    model: Policy-GNN
    arxiv_id: '2204.06127'
    title: 'Reinforcement learning on graphs: A survey'
    date: '2022-04-13'
  - value: 0.946
    std: 0.007
    model: MATE
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: '2024-07-29'
  milestones_by_metric:
    Accuracy: *id001
    AUC:
    - value: 0.973
      std: 0.003
      model: GaGSL
      arxiv_id: '2411.04356'
      title: 'GaGSL: Global-augmented Graph Structure Learning via Graph Information
        Bottleneck'
      date: '2024-11-07'
    F1:
    - value: 0.679
      std: 0.008
      model: Pre-train (Cluster)
      arxiv_id: '1905.13728'
      title: Pre-Training Graph Neural Networks for Generic Structural Feature Extraction
      date: '2019-05-31'
    - value: 0.888
      std: 0.001
      model: APPNP
      arxiv_id: '1909.13021'
      title: Multi-Scale Attributed Node Embedding
      date: '2019-09-25'
    - value: 0.8894
      std: 0.0054
      model: ACM-GCN
      arxiv_id: '2402.05894'
      title: Large Language Model Meets Graph Neural Network in Knowledge Distillation
      date: '2024-02-08'
    F1-macro:
    - value: 0.823
      std: 0.011
      model: GaGSL
      arxiv_id: '2411.04356'
      title: 'GaGSL: Global-augmented Graph Structure Learning via Graph Information
        Bottleneck'
      date: '2024-11-07'
    F1-micro:
    - value: 0.914
      std: 0.02
      model: GEN
      arxiv_id: '2411.04356'
      title: 'GaGSL: Global-augmented Graph Structure Learning via Graph Information
        Bottleneck'
      date: '2024-11-07'
    Loss:
    - value: 1.63
      std: 0.59
      model: GATv2 + CAR
      arxiv_id: '2210.10946'
      title: Causally-guided Regularization of Graph Attention Improves Generalizability
      date: '2022-10-20'
    NMI:
    - value: 0.47
      std: 0.04
      model: ORC (us)
      arxiv_id: '2407.04236'
      title: Graph Pooling via Ricci Flow
      date: '2024-07-05'
---

