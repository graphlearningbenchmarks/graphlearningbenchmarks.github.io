---
title: Squirrel
slug: squirrel
benchmark: Heterophilic Graphs
task_type: node_classification
short_description: Wikipedia Squirrel page node classification (5 classes, heterophilic).
description: '**5-class node classification** Wikipedia Squirrel page node classification
  (5 classes, heterophilic). Uses the Geom-GCN/PyG node features and graph. Evaluated
  by Accuracy.'
detailed_description:
  task: Wikipedia Squirrel page node classification (5 classes, heterophilic). The
    primary catalog metric is Accuracy.
  data: Wikipedia Squirrel page node classification (5 classes, heterophilic). The
    cataloged artifact reports 1 graphs, 5 target classes or tasks.
  features: 'Features and edges follow the Geom-GCN/PyG artifact: WebKB uses webpage
    bag-of-words and hyperlinks, Actor uses film-page keywords and co-occurrence links,
    and WikipediaNetwork uses page features and hyperlinks.'
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split, Filtered split. Evaluation uses Accuracy (higher is better). Exact masks
    or folds must come from the cited release.'
  quirks_and_pitfalls: These small or repurposed graphs have contested preprocessing
    and split conventions. Results across Geom-GCN, PyG, and corrected heterophily
    artifacts are not automatically comparable; class imbalance and high variance
    require multiple splits.
sources:
- title: Heterophilic Graphs benchmark
  arxiv_id: '2110.14446'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric Squirrel loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.WikipediaNetwork.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.WikipediaNetwork.html
stats:
  num_graphs: 1
  avg_nodes: 5201.0
  avg_edges: 217073.0
  num_classes: 5
  extra_stats:
    edge_feature_dim: 0
    edge_feature_type: Wikipedia hyperlinks; no edge attributes
    edge_homophily: 0.22
    heterophily: 0.78
    label_imbalance: five traffic-based classes; duplicate nodes create train-test
      leakage in the original artifact
    node_feature_dim: 2089
    node_feature_type: sparse Wikipedia noun features
    statistic_notes: WikipediaNetwork preprocessing; duplicate-node filtering produces
      a different benchmark
result_count: 445
best_model:
  model: IBG-NN
  value: 0.7763
  metric: Accuracy
  arxiv_id: '2504.18273'
  paper_title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
papers:
- arxiv_id: '2605.20248'
  title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
    Classification'
  date_iso: '2026-05-18'
  venue: ''
- arxiv_id: '2604.19028'
  title: Learning Posterior Predictive Distributions for Node Classification from
    Synthetic Graph Priors
  date_iso: '2026-04-21'
  venue: ICLR 2026
- arxiv_id: '2604.15699'
  title: Frequency-Corrupt Based Graph Self-Supervised Learning
  date_iso: '2026-04-17'
  venue: WWW 2026
- arxiv_id: '2604.01878'
  title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph Contrastive Learning'
  date_iso: '2026-04-02'
  venue: ''
- arxiv_id: '2603.26178'
  title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
    Learning via Ricci Flow'
  date_iso: '2026-03-27'
  venue: ''
- arxiv_id: '2603.09195'
  title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
  date_iso: '2026-03-10'
  venue: ''
- arxiv_id: '2602.15634'
  title: 'Beyond ReLU: Bifurcation, Oversmoothing, and Topological Priors'
  date_iso: '2026-02-17'
  venue: ''
- arxiv_id: '2602.07256'
  title: 'Graph homophily booster: Reimagining the role of discrete features in heterophilic
    graph learning'
  date_iso: '2026-02-06'
  venue: ICLR 2026
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
- arxiv_id: '2512.08798'
  title: Can TabPFN Compete with GNNs for Node Classification via Graph Tabularization?
  date_iso: '2025-12-09'
  venue: LoG 2025
- arxiv_id: '2511.16062'
  title: Gauge-Equivariant Graph Networks via Self-Interference Cancellation
  date_iso: '2025-11-20'
  venue: ''
- arxiv_id: '2509.22416'
  title: 'One Prompt Fits All: Universal Graph Adaptation for Pretrained Models'
  date_iso: '2025-09-26'
  venue: NeurIPS 2025
- arxiv_id: '2509.12530'
  title: 'Graph Homophily Booster: Rethinking the Role of Discrete Features on Heterophilic
    Graphs'
  date_iso: '2025-09-16'
  venue: ''
- arxiv_id: '2506.19343'
  title: Discrepancy-Aware Graph Mask Auto-Encoder
  date_iso: '2025-06-24'
  venue: KDD 2025
- arxiv_id: '2506.14291'
  title: 'Equivariance Everywhere All At Once: A Recipe for Graph Foundation Models'
  date_iso: '2025-06-17'
  venue: ''
- arxiv_id: '2505.22362'
  title: Directed Homophily-Aware Graph Neural Network
  date_iso: '2025-05-28'
  venue: ''
- arxiv_id: '2505.11346'
  title: What Can We Learn From MIMO Graph Convolutions?
  date_iso: '2025-05-16'
  venue: IJCAI 2025
- arxiv_id: '2505.05533'
  title: Rethinking Graph Contrastive Learning through Relative Similarity Preservation
  date_iso: '2025-05-08'
  venue: IJCAI 2025
- arxiv_id: '2504.18273'
  title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
  date_iso: '2025-04-25'
  venue: ''
- arxiv_id: '2412.04064'
  title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
  date_iso: '2024-12-05'
  venue: NeurIPS 2024
- arxiv_id: '2411.19392'
  title: Scale-aware Message Passing For Graph Node Classification
  date_iso: '2024-11-28'
  venue: ''
- arxiv_id: '2410.02158'
  title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation Learning'
  date_iso: '2024-10-03'
  venue: TMLR 2024
- arxiv_id: '2407.19420'
  title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate Over-Smoothing
    in Node Classification Tasks'
  date_iso: '2024-07-28'
  venue: ''
- arxiv_id: '2407.18480'
  title: Scalable Graph Compressed Convolutions
  date_iso: '2024-07-26'
  venue: ''
- arxiv_id: '2407.11907'
  title: 'GraphFM: A generalist graph transformer that learns transferable representations
    across diverse domains'
  date_iso: '2024-07-16'
  venue: TMLR 2024
- arxiv_id: '2407.09381'
  title: The Effectiveness of Curvature-Based Rewiring and the Role of Hyperparameters
    in GNNs Revisited
  date_iso: '2024-07-12'
  venue: ICLR 2024
- arxiv_id: '2406.10871'
  title: Graph Neural Reaction Diffusion Models Submitted to the editors June 2023.
    Accepted in March 2024.
  date_iso: '2024-06-16'
  venue: ''
- arxiv_id: '2406.01899'
  title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models'
  date_iso: '2024-06-04'
  venue: NeurIPS 2024
- arxiv_id: '2404.17099'
  title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
    with FROND
  date_iso: '2024-04-26'
  venue: ICLR 2024
- arxiv_id: '2403.20221'
  title: Graph Neural Aggregation-diffusion with Metastability
  date_iso: '2024-03-29'
  venue: ''
- arxiv_id: '2403.07954'
  title: 'Optimizing Polynomial Graph Filters: A Novel Adaptive Krylov Subspace Approach'
  date_iso: '2024-03-12'
  venue: WWW 2024
- arxiv_id: '2401.09125'
  title: Understanding Heterophily for Graph Neural Networks
  date_iso: '2024-01-17'
  venue: ICML 2024
- arxiv_id: '2312.04111'
  title: Breaking the Entanglement of Homophily and Heterophily in Semi-supervised
    Node Classification
  date_iso: '2023-12-07'
  venue: ''
- arxiv_id: '2401.12780'
  title: 'DeepRicci: Self-supervised Graph Structure-Feature Co-Refinement for Alleviating
    Over-squashing'
  date_iso: '2023-12-01'
  venue: ''
- arxiv_id: '2311.18177'
  title: An Effective Universal Polynomial Basis for Spectral Graph Neural Networks
  date_iso: '2023-11-30'
  venue: ''
- arxiv_id: '2310.13845'
  title: Spectral-Aware Augmentation for Enhanced Graph Representation Learning
  date_iso: '2023-10-20'
  venue: ''
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
- arxiv_id: '2306.05557'
  title: On Performance Discrepancies Across Local Homophily Levels in Graph Neural
    Networks
  date_iso: '2023-06-08'
  venue: ''
- arxiv_id: '2305.13115'
  title: 'Causal-Based Supervision of Attention in Graph Neural Network: A Better
    and Simpler Choice towards Powerful Attention'
  date_iso: '2023-05-22'
  venue: IJCAI 2023
- arxiv_id: '2305.06142'
  title: Feature Expansion for Graph Neural Networks
  date_iso: '2023-05-10'
  venue: ICML 2023
- arxiv_id: '2303.13750'
  title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
  date_iso: '2023-03-24'
  venue: ''
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
- arxiv_id: '2210.09789'
  title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
  date_iso: '2022-10-18'
  venue: ICLR 2022
- arxiv_id: '2210.00513'
  title: Gradient Gating for Deep Multi-Rate Learning on Graphs
  date_iso: '2022-10-02'
  venue: ICLR 2022
- arxiv_id: '2209.15454'
  title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel Geometric Polynomials'
  date_iso: '2022-09-30'
  venue: ''
- arxiv_id: '2206.14418'
  title: Optimization-Induced Graph Implicit Nonlinear Diffusion
  date_iso: '2022-06-29'
  venue: ICML 2022
- arxiv_id: '2206.03601'
  title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
  date_iso: '2022-06-07'
  venue: ''
- arxiv_id: '2206.02386'
  title: Restructuring Graphs for Higher Homophily via Adaptive Spectral Clustering
  date_iso: '2022-06-06'
  venue: AAAI 2022
- arxiv_id: '2204.04874'
  title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
  date_iso: '2022-04-11'
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
- arxiv_id: '2105.07634'
  title: Improving Graph Neural Networks with Simple Architecture Design
  date_iso: '2021-05-17'
  venue: ''
- arxiv_id: '2005.14612'
  title: Non-Local Graph Neural Networks
  date_iso: '2020-05-29'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: Geom-GCN 10 fixed splits.
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 1
    avg_nodes: 5201.0
    avg_edges: 217073.0
    num_classes: 5
    extra_stats:
      edge_feature_dim: 0
      edge_feature_type: Wikipedia hyperlinks; no edge attributes
      edge_homophily: 0.22
      heterophily: 0.78
      label_imbalance: five traffic-based classes; duplicate nodes create train-test
        leakage in the original artifact
      node_feature_dim: 2089
      node_feature_type: sparse Wikipedia noun features
      statistic_notes: WikipediaNetwork preprocessing; duplicate-node filtering produces
        a different benchmark
  metrics:
  - Accuracy
  - F1
  metric_display_names:
  - Accuracy
  - F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: IBG-NN
    model_plain: IBG-NN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: Apr 25, 2025
    date_iso: '2025-04-25'
    date_display: Apr 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7763
    - null
    metric_stds:
    - 0.0179
    - null
  - model: Trans.Conv+CNA
    model_plain: Trans.Conv+CNA
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
    - 0.7747
    - null
    metric_stds:
    - 0.0128
    - null
  - model: DHGNN
    model_plain: DHGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22362'
    title: Directed Homophily-Aware Graph Neural Network
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7684
    - null
    metric_stds:
    - 0.0161
    - null
  - model: FaberNet
    model_plain: FaberNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: Apr 25, 2025
    date_iso: '2025-04-25'
    date_display: Apr 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7671
    - null
    metric_stds:
    - 0.0192
    - null
  - model: ScaleNet
    model_plain: ScaleNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: Nov 28, 2024
    date_iso: '2024-11-28'
    date_display: Nov 2024
    codebase_url: https://github.com/Qin87/ScaleNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.76
    - null
    metric_stds:
    - 0.02
    - null
  - model: LargeScaleNet
    model_plain: LargeScaleNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: Nov 28, 2024
    date_iso: '2024-11-28'
    date_display: Nov 2024
    codebase_url: https://github.com/Qin87/ScaleNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.759
    - null
    metric_stds:
    - 0.02
    - null
  - model: Dir-GNN
    model_plain: Dir-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: Nov 28, 2024
    date_iso: '2024-11-28'
    date_display: Nov 2024
    codebase_url: https://github.com/Qin87/ScaleNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.756
    - null
    metric_stds:
    - 0.019
    - null
  - model: NDDGNN
    model_plain: NDDGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22362'
    title: Directed Homophily-Aware Graph Neural Network
    date: May 28, 2025
    date_iso: '2025-05-28'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7538
    - null
    metric_stds:
    - 0.0195
    - null
  - model: DirGNN
    model_plain: DirGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: Apr 25, 2025
    date_iso: '2025-04-25'
    date_display: Apr 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7513
    - null
    metric_stds:
    - 0.0195
    - null
  - model: GPR-GNN
    model_plain: GPR-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: Apr 25, 2025
    date_iso: '2025-04-25'
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
    - 0.748
    - null
    metric_stds:
    - 0.005
    - null
  - model: FSGNN
    model_plain: FSGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2105.07634'
    title: Improving Graph Neural Networks with Simple Architecture Design
    date: May 17, 2021
    date_iso: '2021-05-17'
    date_display: May 2021
    codebase_url: https://github.com/sunilkmaurya/FSGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.741
    - null
    metric_stds:
    - 0.0189
    - null
  - model: FC-GSSL
    model_plain: FC-GSSL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7403
    - null
    metric_stds:
    - 0.0084
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
    - 0.7298
    - null
    metric_stds:
    - 0.0178
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
    - 0.7295
    - null
    metric_stds:
    - 0.0023
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
    - 0.7254
    - null
    metric_stds:
    - 0.022
    - null
  - model: DGMAE
    model_plain: DGMAE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2506.19343'
    title: Discrepancy-Aware Graph Mask Auto-Encoder
    date: Jun 24, 2025
    date_iso: '2025-06-24'
    date_display: Jun 2025
    codebase_url: https://github.com/zhengziyu77/DGMAE
    published_conference: KDD 2025
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7247
    - null
    metric_stds:
    - 0.0177
    - null
  - model: GraphPAE
    model_plain: GraphPAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7205
    - null
    metric_stds:
    - 0.014
    - null
  - model: GPNet
    model_plain: GPNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2209.15454'
    title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel Geometric Polynomials'
    date: Sep 30, 2022
    date_iso: '2022-09-30'
    date_display: Sep 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7157
    - null
    metric_stds:
    - 0.001
    - null
  - model: GloGNN
    model_plain: GloGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22362'
    title: Directed Homophily-Aware Graph Neural Network
    date: May 28, 2025
    date_iso: '2025-05-28'
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
    - 0.7121
    - null
    metric_stds:
    - 0.0184
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
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7027
    - null
    metric_stds:
    - 0.0088
    - null
  - model: UniGAP
    model_plain: UniGAP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_iso: '2024-07-28'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6967
    - null
    metric_stds:
    - 0.016
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
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.686
    - null
    metric_stds:
    - 0.0056
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
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6853
    - null
    metric_stds:
    - 0.0044
    - null
  - model: UDGNN_GCN
    model_plain: UDGNN_GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2209.15454'
    title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel Geometric Polynomials'
    date: Sep 30, 2022
    date_iso: '2022-09-30'
    date_display: Sep 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6813
    - null
    metric_stds:
    - 0.026
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
    - 0.679
    - null
    metric_stds:
    - 0.0023
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
    arxiv_id: '2505.22362'
    title: Directed Homophily-Aware Graph Neural Network
    date: May 28, 2025
    date_iso: '2025-05-28'
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
    - 0.674
    - null
    metric_stds:
    - 0.0221
    - null
  - model: ACMII-GCN
    model_plain: ACMII-GCN
    is_baseline: true
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
    - 0.674
    - null
    metric_stds:
    - 0.0221
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
    - 0.674
    - null
    metric_stds:
    - 0.0125
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
    - 0.6596
    - null
    metric_stds:
    - 0.0211
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
    - 0.6562
    - null
    metric_stds:
    - 0.0233
    - null
  - model: NWR-GAE
    model_plain: NWR-GAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.16026'
    title: 'MUSE: Multi-View Contrastive Learning for Heterophilic Graphs'
    date: Jul 29, 2023
    date_iso: '2023-07-29'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6481
    - null
    metric_stds:
    - 0.0183
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
    - 0.6464
    - null
    metric_stds:
    - 0.0081
    - null
  - model: G2-GraphSAGE
    model_plain: G2-GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6426
    - null
    metric_stds:
    - 0.0238
    - null
  - model: G2
    model_plain: G2
    is_baseline: true
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
    - 0.6426
    - null
    metric_stds:
    - 0.0238
    - null
  - model: G^2
    model_plain: G^2
    is_baseline: true
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
    - 0.6426
    - null
    metric_stds:
    - 0.0238
    - null
  - model: HopGNN
    model_plain: HopGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.11761'
    title: 'From Node Interaction to Hop Interaction: New Effective and Scalable Graph
      Learning Paradigm'
    date: Nov 21, 2022
    date_iso: '2022-11-21'
    date_display: Nov 2022
    codebase_url: https://github.com/JC-202/HopGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6423
    - null
    metric_stds:
    - 0.0133
    - null
  - model: ICG-NN
    model_plain: ICG-NN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: Apr 25, 2025
    date_iso: '2025-04-25'
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
    - 0.6402
    - null
    metric_stds:
    - 0.0167
    - null
  - model: OptBasisGNN
    model_plain: OptBasisGNN
    is_baseline: true
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
    - 0.6362
    - null
    metric_stds:
    - 0.0076
    - null
  - model: AdaptKry
    model_plain: AdaptKry
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2403.07954'
    title: 'Optimizing Polynomial Graph Filters: A Novel Adaptive Krylov Subspace
      Approach'
    date: Mar 12, 2024
    date_iso: '2024-03-12'
    date_display: Mar 2024
    codebase_url: https://github.com/kkhuang81/AdaptKry
    published_conference: WWW 2024
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6331
    - null
    metric_stds:
    - 0.0076
    - null
  - model: Sp^2GCL
    model_plain: Sp^2GCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6261
    - null
    metric_stds:
    - 0.0087
    - null
  - model: AUG-MAE
    model_plain: AUG-MAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6257
    - null
    metric_stds:
    - 0.0067
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
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: Apr 25, 2025
    date_iso: '2025-04-25'
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
    - 0.619
    - null
    metric_stds:
    - 0.014
    - null
  - model: LINKX
    model_plain: LINKX
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2209.15454'
    title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel Geometric Polynomials'
    date: Sep 30, 2022
    date_iso: '2022-09-30'
    date_display: Sep 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6181
    - null
    metric_stds:
    - 0.018
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
    - 0.6179
    - null
    metric_stds:
    - 0.004
    - null
  - model: AERO-GNN
    model_plain: AERO-GNN
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
    - 0.6176
    - null
    metric_stds:
    - 0.024
    - null
  - model: CCA-SSG
    model_plain: CCA-SSG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6158
    - null
    metric_stds:
    - 0.0198
    - null
  - model: HopGNN+SCL
    model_plain: HopGNN+SCL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2211.11761'
    title: 'From Node Interaction to Hop Interaction: New Effective and Scalable Graph
      Learning Paradigm'
    date: Nov 21, 2022
    date_iso: '2022-11-21'
    date_display: Nov 2022
    codebase_url: https://github.com/JC-202/HopGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6142
    - null
    metric_stds:
    - 0.0198
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
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6113
    - null
    metric_stds:
    - 0.006
    - null
  - model: F-GREAD-BS
    model_plain: F-GREAD-BS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.17099'
    title: Unleashing the Potential of Fractional Calculus in Graph Neural Networks
      with FROND
    date: Apr 26, 2024
    date_iso: '2024-04-26'
    date_display: Apr 2024
    codebase_url: https://github.com/zknus/ICLR2024-FROND
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6086
    - null
    metric_stds:
    - 0.0105
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
    - 0.6081
    - null
    metric_stds:
    - 0.0056
    - null
  row_count: 445
  rows_json: /data/datasets/squirrel/standard-split-rows.json
  chart_json: /data/datasets/squirrel/standard-split-chart.json
  arch_counts:
    gnn: 326
    hybrid: 51
    graph_transformer: 11
    llm: 0
    walk: 7
    traditional: 17
  metric_counts:
  - 439
  - 6
  milestones: &id001
  - value: 0.59
    std: 0.012
    model: NLGCN
    arxiv_id: '2005.14612'
    title: Non-Local Graph Neural Networks
    date: '2020-05-29'
  - value: 0.741
    std: 0.0189
    model: FSGNN
    arxiv_id: '2105.07634'
    title: Improving Graph Neural Networks with Simple Architecture Design
    date: '2021-05-17'
  - value: 0.7416
    std: null
    model: FSGNN
    arxiv_id: '2111.06748'
    title: Simplifying approach to Node Classification in Graph Neural Networks
    date: '2021-11-12'
  - value: 0.76
    std: 0.02
    model: ScaleNet
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: '2024-11-28'
  - value: 0.7747
    std: 0.0128
    model: Trans.Conv+CNA
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: '2024-12-05'
  - value: 0.7763
    std: 0.0179
    model: IBG-NN
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: '2025-04-25'
  milestones_by_metric:
    Accuracy: *id001
    F1:
    - value: 0.4
      std: 0.03
      model: MLP
      arxiv_id: '2306.05557'
      title: On Performance Discrepancies Across Local Homophily Levels in Graph Neural
        Networks
      date: '2023-06-08'
---

