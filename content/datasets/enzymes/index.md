---
title: ENZYMES
slug: enzymes
benchmark: TU Dortmund
task_type: graph_classification
short_description: TU Dortmund graph classification on 6 enzyme reaction classes (600
  graphs, subset of BRENDA database).
description: '**6-class graph classification** TU Dortmund graph classification on
  6 enzyme reaction classes (600 graphs, subset of BRENDA database). Uses the released
  node/edge labels or attributes; several social datasets are featureless. Evaluated
  by Accuracy.'
detailed_description:
  task: TU Dortmund graph classification on 6 enzyme reaction classes (600 graphs,
    subset of BRENDA database). The primary catalog metric is Accuracy.
  data: TU Dortmund graph classification on 6 enzyme reaction classes (600 graphs,
    subset of BRENDA database). The cataloged artifact reports 600 graphs, 6 target
    classes or tasks.
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
- title: PyTorch Geometric ENZYMES loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
stats:
  num_graphs: 600
  avg_nodes: 32.6
  avg_edges: 62.1
  num_classes: 6
result_count: 445
best_model:
  model: GMN
  value: 0.7866
  metric: Accuracy
  arxiv_id: '2002.09518'
  paper_title: Memory-Based Graph Networks
papers:
- arxiv_id: '2605.13383'
  title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
  date_iso: '2026-05-13'
  venue: ''
- arxiv_id: '2602.05567'
  title: 'MAGPrompt: Message-Adaptive Graph Prompt Tuning for Graph Neural Networks'
  date_iso: '2026-02-05'
  venue: ''
- arxiv_id: '2601.07419'
  title: 'Position: Don''t be Afraid of Over-Smoothing And Over-Squashing'
  date_iso: '2026-01-12'
  venue: ''
- arxiv_id: '2510.22643'
  title: Enhancing Graph Classification Robustness with Singular Pooling
  date_iso: '2025-10-26'
  venue: NeurIPS 2025
- arxiv_id: '2510.21207'
  title: 'Adaptive Graph Mixture of Residual Experts: Unsupervised Learning on Diverse
    Graphs with Heterogeneous Specialization'
  date_iso: '2025-10-24'
  venue: ''
- arxiv_id: '2509.24886'
  title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
    Networks
  date_iso: '2025-09-29'
  venue: ''
- arxiv_id: '2508.20597'
  title: Local Virtual Nodes for Alleviating Over-Squashing in Graph Neural Networks
  date_iso: '2025-08-28'
  venue: ''
- arxiv_id: '2508.09320'
  title: Exact Verification of Graph Neural Networks with Incremental Constraint Solving
  date_iso: '2025-08-12'
  venue: ''
- arxiv_id: '2506.16110'
  title: Mitigating Over-Squashing in Graph Neural Networks by Spectrum-Preserving
    Sparsification
  date_iso: '2025-06-19'
  venue: ICML 2025
- arxiv_id: '2506.06582'
  title: 'Demystifying Topological Message-Passing with Relational Structures: A Case
    Study on Oversquashing in Simplicial Message-Passing'
  date_iso: '2025-06-06'
  venue: ICLR 2025
- arxiv_id: '2505.21285'
  title: Learnable Kernel Density Estimation for Graphs
  date_iso: '2025-05-27'
  venue: ICML 2025
- arxiv_id: '2501.15142'
  title: 'DAGPrompT: Pushing the Limits of Graph Prompting with a Distribution-aware
    Graph Prompt Tuning Approach'
  date_iso: '2025-01-25'
  venue: WWW 2025
- arxiv_id: '2408.16288'
  title: 'OpenFGL: A Comprehensive Benchmark for Federated Graph Learning'
  date_iso: '2024-08-29'
  venue: ''
- arxiv_id: '2407.02057'
  title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised Graph-Level
    Anomaly Detection'
  date_iso: '2024-07-02'
  venue: ''
- arxiv_id: '2406.15523'
  title: 'Unifying Unsupervised Graph-Level Anomaly Detection and Out-of-Distribution
    Detection: A Benchmark'
  date_iso: '2024-06-21'
  venue: ICLR 2024
- arxiv_id: '2406.08897'
  title: Motif-driven Subgraph Structure Learning for Graph Classification
  date_iso: '2024-06-13'
  venue: ''
- arxiv_id: '2406.05346'
  title: 'ProG: A Graph Prompt Learning Benchmark'
  date_iso: '2024-06-08'
  venue: NeurIPS 2024
- arxiv_id: '2406.04843'
  title: Variational Flow Matching for Graph Generation
  date_iso: '2024-06-07'
  venue: NeurIPS 2024
- arxiv_id: '2406.01899'
  title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models'
  date_iso: '2024-06-04'
  venue: NeurIPS 2024
- arxiv_id: '2406.01249'
  title: Equivariant Machine Learning on Graphs with Nonlinear Spectral Filters
  date_iso: '2024-06-03'
  venue: NeurIPS 2024
- arxiv_id: '2402.16346'
  title: Boosting Graph Pooling with Persistent Homology
  date_iso: '2024-02-26'
  venue: NeurIPS 2024
- arxiv_id: '2402.15270'
  title: Smoothed Graph Contrastive Learning via Seamless Proximity Integration
  date_iso: '2024-02-23'
  venue: ''
- arxiv_id: '2402.07568'
  title: '--Leman at the margin: When more expressivity matters'
  date_iso: '2024-02-12'
  venue: ICML 2024
- arxiv_id: '2401.17580'
  title: Graph Contrastive Learning with Cohesive Subgraph Awareness
  date_iso: '2024-01-31'
  venue: WWW 2024
- arxiv_id: '2312.13583'
  title: Fine-tuning Graph Neural Networks by Preserving Graph Generative Patterns
  date_iso: '2023-12-21'
  venue: AAAI 2023
- arxiv_id: '2311.14864'
  title: Effective Structural Encodings via Local Curvature Profiles
  date_iso: '2023-11-24'
  venue: ICLR 2023
- arxiv_id: '2310.10434'
  title: Equivariant Matrix Function Neural Networks
  date_iso: '2023-10-16'
  venue: ICLR 2023
- arxiv_id: '2310.01668'
  title: Locality-Aware Graph Rewiring in GNNs
  date_iso: '2023-10-02'
  venue: ICLR 2023
- arxiv_id: '2309.09384'
  title: Mitigating Over-Smoothing and Over-Squashing using Augmentations of Forman-Ricci
    Curvature
  date_iso: '2023-09-17'
  venue: ''
- arxiv_id: '2309.00738'
  title: Rethinking the Power of Graph Canonization in Graph Representation Learning
    with Stability
  date_iso: '2023-09-01'
  venue: ''
- arxiv_id: '2305.15747'
  title: Union Subgraph Neural Networks
  date_iso: '2023-05-25'
  venue: AAAI 2023
- arxiv_id: '2305.06102'
  title: Towards Better Graph Representation Learning with Parameterized Decomposition
    & Filtering
  date_iso: '2023-05-10'
  venue: ICML 2023
- arxiv_id: '2304.01575'
  title: The expressive power of pooling in Graph Neural Networks
  date_iso: '2023-04-04'
  venue: NeurIPS 2023
- arxiv_id: '2301.11039'
  title: WL meet VC
  date_iso: '2023-01-26'
  venue: ICML 2023
- arxiv_id: '2003.00982'
  title: GNNBenchmark
  date_iso: '2023-01-01'
  venue: JMLR 2023
- arxiv_id: '2211.15779'
  title: Revisiting Over-smoothing and Over-squashing using Ollivier's Ricci Curvature
  date_iso: '2022-11-28'
  venue: ICML 2022
- arxiv_id: '2210.11790'
  title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing in GNNs'
  date_iso: '2022-10-21'
  venue: ICLR 2022
- arxiv_id: '2210.00084'
  title: Contrastive Graph Few-Shot Learning
  date_iso: '2022-09-30'
  venue: ''
- arxiv_id: '2205.15733'
  title: Template based Graph Neural Network with Optimal Transport Distances
  date_iso: '2022-05-31'
  venue: NeurIPS 2022
- arxiv_id: '2204.10390'
  title: 'SoftEdge: Regularizing Graph Classification with Random Soft Edges'
  date_iso: '2022-04-21'
  venue: ''
- arxiv_id: '2201.00491'
  title: 'KerGNNs: Interpretable Graph Neural Networks with Graph Kernels'
  date_iso: '2022-01-03'
  venue: AAAI 2022
- arxiv_id: '2112.07160'
  title: A New Perspective on the Effects of Spectrum in Graph Neural Networks
  date_iso: '2021-12-14'
  venue: ICML 2021
- arxiv_id: '2110.09344'
  title: 'ifMixup: Interpolating Graph Pair to Regularize Graph Classification'
  date_iso: '2021-10-18'
  venue: AAAI 2021
- arxiv_id: '2106.04319'
  title: Breaking the Limits of Message Passing Graph Neural Networks
  date_iso: '2021-06-08'
  venue: ICML 2021
- arxiv_id: '2102.07835'
  title: Topological Graph Neural Networks
  date_iso: '2021-02-15'
  venue: ICLR 2021
- arxiv_id: '2012.08734'
  title: Hierarchical Graph Capsule Network
  date_iso: '2020-12-16'
  venue: AAAI 2020
- arxiv_id: '2009.10564'
  title: 'GraphCrop: Subgraph Cropping for Graph Classification'
  date_iso: '2020-09-22'
  venue: ''
- arxiv_id: '2008.12578'
  title: Graph Convolutional Neural Networks with Node Transition Probability-based
    Message Passing and DropNode Regularization
  date_iso: '2020-08-28'
  venue: ''
- arxiv_id: '2007.11202'
  title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for Graph Representation
    and Learning'
  date_iso: '2020-07-22'
  venue: ''
- arxiv_id: '2006.09430'
  title: Wasserstein Embedding for Graph Learning
  date_iso: '2020-06-16'
  venue: ICLR 2020
- arxiv_id: '2006.05205'
  title: On the Bottleneck of Graph Neural Networks and its Practical Implications
  date_iso: '2020-06-09'
  venue: ICLR 2020
- arxiv_id: '2002.09518'
  title: Memory-Based Graph Networks
  date_iso: '2020-02-21'
  venue: ICLR 2020
- arxiv_id: '2001.08184'
  title: 'GraphGen: A Scalable Approach to Domain-agnostic Labeled Graph Generation'
  date_iso: '2020-01-22'
  venue: WWW 2020
- arxiv_id: '1910.11436'
  title: Hierarchical Representation Learning in Graph Neural Networks with Node Decimation
    Pooling
  date_iso: '2019-10-24'
  venue: ''
- arxiv_id: '1906.02319'
  title: 'DEMO-Net: Degree-specific Graph Neural Networks for Node and Graph Classification'
  date_iso: '2019-06-05'
  venue: KDD 2019
- arxiv_id: '1906.01277'
  title: Wasserstein Weisfeiler-Lehman Graph Kernels
  date_iso: '2019-06-04'
  venue: NeurIPS 2019
- arxiv_id: '1904.13107'
  title: Graph Convolutional Networks with EigenPooling
  date_iso: '2019-04-30'
  venue: KDD 2019
- arxiv_id: '1901.01343'
  title: Graph Neural Networks With Convolutional ARMA Filters
  date_iso: '2019-01-05'
  venue: ''
- arxiv_id: '1805.11921'
  title: Anonymous Walk Embeddings
  date_iso: '2018-05-30'
  venue: ICML 2018
- arxiv_id: '1805.08090'
  title: Graph Capsule Convolutional Neural Networks
  date_iso: '2018-05-21'
  venue: ICML 2018
- arxiv_id: '1704.02901'
  title: Dynamic Edge-Conditioned Filters in Convolutional Neural Networks on Graphs
  date_iso: '2017-04-10'
  venue: ''
- arxiv_id: '1606.01141'
  title: On Valid Optimal Assignment Kernels and Applications to Graph Classification
  date_iso: '2016-06-03'
  venue: NeurIPS 2016
- arxiv_id: '1603.06186'
  title: The Multiscale Laplacian Graph Kernel
  date_iso: '2016-03-01'
  venue: NeurIPS 2016
- arxiv_id: '1511.02136'
  title: Diffusion-Convolutional Neural Networks
  date_iso: '2015-11-06'
  venue: NeurIPS 2015
variants:
- slug: 10-fold-cv
  name: 10-fold CV
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 600
    avg_nodes: 32.6
    avg_edges: 62.1
    num_classes: 6
  metrics:
  - Accuracy
  - AUC
  - AUROC
  - Clustering
  - Degree
  - F (macro)
  - F (micro)
  - Joint Node Label & Degree
  - NSPDK
  - Orbit
  - Uniqueness
  metric_display_names:
  - Accuracy
  - AUC
  - AUROC
  - Clustering
  - Degree
  - F (macro)
  - F (micro)
  - Joint Node Label & Degree
  - NSPDK
  - Orbit
  - Uniqueness
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GMN
    model_plain: GMN
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7866
    - null
    - null
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
    - null
    - null
  - model: MemGNN
    model_plain: MemGNN
    is_baseline: true
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
    - 0.755
    - null
    - null
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
    - null
    - null
  - model: TFGW SP
    model_plain: TFGW SP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15733'
    title: Template based Graph Neural Network with Optimal Transport Distances
    date: May 31, 2022
    date_iso: '2022-05-31'
    date_display: May 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.751
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.05
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: TFGW ADJ
    model_plain: TFGW ADJ
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15733'
    title: Template based Graph Neural Network with Optimal Transport Distances
    date: May 31, 2022
    date_iso: '2022-05-31'
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
    - 0.738
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.046
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PDF
    model_plain: PDF
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.06102'
    title: Towards Better Graph Representation Learning with Parameterized Decomposition
      & Filtering
    date: May 10, 2023
    date_iso: '2023-05-10'
    date_display: May 2023
    codebase_url: https://github.com/qslim/PDF
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.735
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0639
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Norm-GN
    model_plain: Norm-GN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.07160'
    title: A New Perspective on the Effects of Spectrum in Graph Neural Networks
    date: Dec 14, 2021
    date_iso: '2021-12-14'
    date_display: Dec 2021
    codebase_url: https://github.com/qslim/gnn-spectrum
    published_conference: ICML 2021
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2021
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7333
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0796
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: WWL
    model_plain: WWL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1906.01277'
    title: Wasserstein Weisfeiler-Lehman Graph Kernels
    date: Jun 4, 2019
    date_iso: '2019-06-04'
    date_display: Jun 2019
    codebase_url: https://github.com/BorgwardtLab/WWL
    published_conference: NeurIPS 2019
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7325
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0087
    - null
    - null
    - null
    - null
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
    - 0.7301
    - null
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
    - null
  - model: MFN
    model_plain: MFN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2310.10434'
    title: Equivariant Matrix Function Neural Networks
    date: Oct 16, 2023
    date_iso: '2023-10-16'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.729
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0755
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: Spec-GN
    model_plain: Spec-GN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.07160'
    title: A New Perspective on the Effects of Spectrum in Graph Neural Networks
    date: Dec 14, 2021
    date_iso: '2021-12-14'
    date_display: Dec 2021
    codebase_url: https://github.com/qslim/gnn-spectrum
    published_conference: ICML 2021
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.725
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0579
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: FGW - ADJ
    model_plain: FGW - ADJ
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.15733'
    title: Template based Graph Neural Network with Optimal Transport Distances
    date: May 31, 2022
    date_iso: '2022-05-31'
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
    - 0.722
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.04
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: MEAN
    model_plain: MEAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2508.09320'
    title: Exact Verification of Graph Neural Networks with Incremental Constraint
      Solving
    date: Aug 12, 2025
    date_iso: '2025-08-12'
    date_display: Aug 2025
    codebase_url: https://github.com/minghao-liu/GNNev
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7167
    - null
    - null
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
    - null
    - null
  - model: UniAug
    model_plain: UniAug
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.01899'
    title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models'
    date: Jun 4, 2024
    date_iso: '2024-06-04'
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
    - 0.715
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0585
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: PGCN_g+DropNode
    model_plain: PGCN_g+DropNode
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2008.12578'
    title: Graph Convolutional Neural Networks with Node Transition Probability-based
      Message Passing and DropNode Regularization
    date: Aug 28, 2020
    date_iso: '2020-08-28'
    date_display: Aug 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.705
    - null
    - null
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
    - null
    - null
  - model: FGW - SP
    model_plain: FGW - SP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.15733'
    title: Template based Graph Neural Network with Optimal Transport Distances
    date: May 31, 2022
    date_iso: '2022-05-31'
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
    - 0.705
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.062
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GFN
    model_plain: GFN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.08734'
    title: Hierarchical Graph Capsule Network
    date: Dec 16, 2020
    date_iso: '2020-12-16'
    date_display: Dec 2020
    codebase_url: https://github.com/uta-smile/HGCN
    published_conference: AAAI 2020
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7017
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0558
    - null
    - null
    - null
    - null
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
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_iso: '2023-01-01'
    date_display: Jan 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.04944
    - null
    - null
    - null
    - null
    - null
    - null
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
    - 0.6994
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
  - model: WL
    model_plain: WL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2205.15733'
    title: Template based Graph Neural Network with Optimal Transport Distances
    date: May 31, 2022
    date_iso: '2022-05-31'
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
    - 0.695
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.032
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GCN_g+DropNode
    model_plain: GCN_g+DropNode
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2008.12578'
    title: Graph Convolutional Neural Networks with Node Transition Probability-based
      Message Passing and DropNode Regularization
    date: Aug 28, 2020
    date_iso: '2020-08-28'
    date_display: Aug 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.69
    - null
    - null
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
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_iso: '2023-01-01'
    date_display: Jan 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.685
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.05241
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: RBF-WL
    model_plain: RBF-WL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1906.01277'
    title: Wasserstein Weisfeiler-Lehman Graph Kernels
    date: Jun 4, 2019
    date_iso: '2019-06-04'
    date_display: Jun 2019
    codebase_url: https://github.com/BorgwardtLab/WWL
    published_conference: NeurIPS 2019
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6843
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0147
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: FLAG
    model_plain: FLAG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.01899'
    title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models'
    date: Jun 4, 2024
    date_iso: '2024-06-04'
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
    - 0.6835
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0745
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SUM
    model_plain: SUM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.09320'
    title: Exact Verification of Graph Neural Networks with Incremental Constraint
      Solving
    date: Aug 12, 2025
    date_iso: '2025-08-12'
    date_display: Aug 2025
    codebase_url: https://github.com/minghao-liu/GNNev
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6833
    - null
    - null
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
    - null
    - null
  - model: MAX
    model_plain: MAX
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.09320'
    title: Exact Verification of Graph Neural Networks with Incremental Constraint
      Solving
    date: Aug 12, 2025
    date_iso: '2025-08-12'
    date_display: Aug 2025
    codebase_url: https://github.com/minghao-liu/GNNev
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6833
    - null
    - null
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
    - null
    - null
  - model: UnionSNN
    model_plain: UnionSNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.15747'
    title: Union Subgraph Neural Networks
    date: May 25, 2023
    date_iso: '2023-05-25'
    date_display: May 2023
    codebase_url: https://github.com/AngusMonroe/UnionSNN
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6817
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.057
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GraphAug
    model_plain: GraphAug
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.01899'
    title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models'
    date: Jun 4, 2024
    date_iso: '2024-06-04'
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
    - 0.6814
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0792
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: UnionGatedGCN
    model_plain: UnionGatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.15747'
    title: Union Subgraph Neural Networks
    date: May 25, 2023
    date_iso: '2023-05-25'
    date_display: May 2023
    codebase_url: https://github.com/AngusMonroe/UnionSNN
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6783
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0687
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: UnionGIN
    model_plain: UnionGIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.15747'
    title: Union Subgraph Neural Networks
    date: May 25, 2023
    date_iso: '2023-05-25'
    date_display: May 2023
    codebase_url: https://github.com/AngusMonroe/UnionSNN
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6783
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.061
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GIN + FA
    model_plain: GIN + FA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2006.05205'
    title: On the Bottleneck of Graph Neural Networks and its Practical Implications
    date: Jun 9, 2020
    date_iso: '2020-06-09'
    date_display: Jun 2020
    codebase_url: https://github.com/tech-srl/bottleneck
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.677
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.053
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GraphSNN
    model_plain: GraphSNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.15747'
    title: Union Subgraph Neural Networks
    date: May 25, 2023
    date_iso: '2023-05-25'
    date_display: May 2023
    codebase_url: https://github.com/AngusMonroe/UnionSNN
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6767
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0374
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: OT-GNN
    model_plain: OT-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15733'
    title: Template based Graph Neural Network with Optimal Transport Distances
    date: May 31, 2022
    date_iso: '2022-05-31'
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
    - 0.673
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.043
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: S-Mixup
    model_plain: S-Mixup
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2406.01899'
    title: 'Cross-Domain Graph Data Scaling: A Showcase with Diffusion Models'
    date: Jun 4, 2024
    date_iso: '2024-06-04'
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
    - 0.6685
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0704
    - null
    - null
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
    arxiv_id: '2012.08734'
    title: Hierarchical Graph Capsule Network
    date: Dec 16, 2020
    date_iso: '2020-12-16'
    date_display: Dec 2020
    codebase_url: https://github.com/uta-smile/HGCN
    published_conference: AAAI 2020
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.665
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0691
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GCN + 2FC
    model_plain: GCN + 2FC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2008.12578'
    title: Graph Convolutional Neural Networks with Node Transition Probability-based
      Message Passing and DropNode Regularization
    date: Aug 28, 2020
    date_iso: '2020-08-28'
    date_display: Aug 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6645
    - null
    - null
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
    - null
    - null
  - model: HGK-SP
    model_plain: HGK-SP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1906.01277'
    title: Wasserstein Weisfeiler-Lehman Graph Kernels
    date: Jun 4, 2019
    date_iso: '2019-06-04'
    date_display: Jun 2019
    codebase_url: https://github.com/BorgwardtLab/WWL
    published_conference: NeurIPS 2019
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6636
    - null
    - null
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
    - null
    - null
  - model: FCN (2FC)
    model_plain: FCN (2FC)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2008.12578'
    title: Graph Convolutional Neural Networks with Node Transition Probability-based
      Message Passing and DropNode Regularization
    date: Aug 28, 2020
    date_iso: '2020-08-28'
    date_display: Aug 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6617
    - null
    - null
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
    - null
    - null
  - model: PGCN_g+2FC
    model_plain: PGCN_g+2FC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2008.12578'
    title: Graph Convolutional Neural Networks with Node Transition Probability-based
      Message Passing and DropNode Regularization
    date: Aug 28, 2020
    date_iso: '2020-08-28'
    date_display: Aug 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6617
    - null
    - null
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
    - null
    - null
  - model: NLSF
    model_plain: NLSF
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
    - 0.6594
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
  - model: att-Graph-level NLSFs
    model_plain: att-Graph-level NLSFs
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
    - 0.6594
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
  - model: vanilla GCN
    model_plain: vanilla GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_iso: '2023-01-01'
    date_display: Jan 2023
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.65833
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0461
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GCN-4
    model_plain: GCN-4
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2102.07835'
    title: Topological Graph Neural Networks
    date: Feb 15, 2021
    date_iso: '2021-02-15'
    date_display: Feb 2021
    codebase_url: https://github.com/BorgwardtLab/TOGL
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.658
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.046
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DropGIN
    model_plain: DropGIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.15733'
    title: Template based Graph Neural Network with Optimal Transport Distances
    date: May 31, 2022
    date_iso: '2022-05-31'
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
    - 0.658
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.027
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: GATED-GCN-4
    model_plain: GATED-GCN-4
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2102.07835'
    title: Topological Graph Neural Networks
    date: Feb 15, 2021
    date_iso: '2021-02-15'
    date_display: Feb 2021
    codebase_url: https://github.com/BorgwardtLab/TOGL
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.657
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.049
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DiffPool +FA
    model_plain: DiffPool +FA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.05205'
    title: On the Bottleneck of Graph Neural Networks and its Practical Implications
    date: Jun 9, 2020
    date_iso: '2020-06-09'
    date_display: Jun 2020
    codebase_url: https://github.com/tech-srl/bottleneck
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.657
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.048
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: gh
    model_plain: gh
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1906.01277'
    title: Wasserstein Weisfeiler-Lehman Graph Kernels
    date: Jun 4, 2019
    date_iso: '2019-06-04'
    date_display: Jun 2019
    codebase_url: https://github.com/BorgwardtLab/WWL
    published_conference: NeurIPS 2019
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2019
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6565
    - null
    - null
    - null
    - null
    - null
    - null
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
    - null
    - null
    - null
    - null
    - null
    - null
  - model: SGCL-T
    model_plain: SGCL-T
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.15270'
    title: Smoothed Graph Contrastive Learning via Seamless Proximity Integration
    date: Feb 23, 2024
    date_iso: '2024-02-23'
    date_display: Feb 2024
    codebase_url: https://github.com/maysambehmanesh/SGCL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.653
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.036
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: No Struct
    model_plain: No Struct
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2006.05205'
    title: On the Bottleneck of Graph Neural Networks and its Practical Implications
    date: Jun 9, 2020
    date_iso: '2020-06-09'
    date_display: Jun 2020
    codebase_url: https://github.com/tech-srl/bottleneck
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.652
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.064
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: DiffPool-TIP
    model_plain: DiffPool-TIP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.16346'
    title: Boosting Graph Pooling with Persistent Homology
    date: Feb 26, 2024
    date_iso: '2024-02-26'
    date_display: Feb 2024
    codebase_url: https://github.com/LOGO-CUHKSZ/TIP
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6505
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - 0.0424
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
  - model: EigenPool
    model_plain: EigenPool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2007.11202'
    title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for Graph Representation
      and Learning'
    date: Jul 22, 2020
    date_iso: '2020-07-22'
    date_display: Jul 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.65
    - null
    - null
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
    - null
    - null
  row_count: 445
  rows_json: /data/datasets/enzymes/10-fold-cv-rows.json
  chart_json: /data/datasets/enzymes/10-fold-cv-chart.json
  arch_counts:
    gnn: 258
    hybrid: 63
    graph_transformer: 3
    llm: 1
    walk: 4
    traditional: 103
  metric_counts:
  - 401
  - 10
  - 31
  - 1
  - 1
  - 5
  - 5
  - 2
  - 2
  - 3
  - 2
  milestones: &id001
  - value: 0.2155
    std: null
    model: deepwl
    arxiv_id: '1511.02136'
    title: Diffusion-Convolutional Neural Networks
    date: '2015-11-06'
  - value: 0.6181
    std: 0.0099
    model: MLG
    arxiv_id: '1603.06186'
    title: The Multiscale Laplacian Graph Kernel
    date: '2016-03-01'
  - value: 0.6183
    std: 0.0539
    model: GCAPS-CNN
    arxiv_id: '1805.08090'
    title: Graph Capsule Convolutional Neural Networks
    date: '2018-05-21'
  - value: 0.65
    std: null
    model: EigenPooling-1
    arxiv_id: '1904.13107'
    title: Graph Convolutional Networks with EigenPooling
    date: '2019-04-30'
  - value: 0.7325
    std: 0.0087
    model: WWL
    arxiv_id: '1906.01277'
    title: Wasserstein Weisfeiler-Lehman Graph Kernels
    date: '2019-06-04'
  - value: 0.7866
    std: null
    model: GMN
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: '2020-02-21'
  milestones_by_metric:
    Accuracy: *id001
    AUC:
    - value: 0.6539
      std: 0.0623
      model: HC-GLAD
      arxiv_id: '2407.02057'
      title: 'HC-GLAD: Dual Hyperbolic Contrastive Learning for Unsupervised Graph-Level
        Anomaly Detection'
      date: '2024-07-02'
    AUROC:
    - value: 0.6856
      std: null
      model: CVTGAD
      arxiv_id: '2406.15523'
      title: 'Unifying Unsupervised Graph-Level Anomaly Detection and Out-of-Distribution
        Detection: A Benchmark'
      date: '2024-06-21'
    - value: 0.7104
      std: 0.0045
      model: LGKDE
      arxiv_id: '2505.21285'
      title: Learnable Kernel Density Estimation for Graphs
      date: '2025-05-27'
    Clustering:
    - value: 0.062
      std: 0.011
      model: CatFlow
      arxiv_id: '2406.04843'
      title: Variational Flow Matching for Graph Generation
      date: '2024-06-07'
    Degree:
    - value: 0.013
      std: 0.012
      model: CatFlow
      arxiv_id: '2406.04843'
      title: Variational Flow Matching for Graph Generation
      date: '2024-06-07'
    F (macro):
    - value: 0.1431
      std: null
      model: deepwl
      arxiv_id: '1511.02136'
      title: Diffusion-Convolutional Neural Networks
      date: '2015-11-06'
    F (micro):
    - value: 0.2155
      std: null
      model: deepwl
      arxiv_id: '1511.02136'
      title: Diffusion-Convolutional Neural Networks
      date: '2015-11-06'
    Joint Node Label & Degree:
    - value: 0.249
      std: null
      model: GraphGen
      arxiv_id: '2001.08184'
      title: 'GraphGen: A Scalable Approach to Domain-agnostic Labeled Graph Generation'
      date: '2020-01-22'
    NSPDK:
    - value: 0.051
      std: null
      model: GraphGen
      arxiv_id: '2001.08184'
      title: 'GraphGen: A Scalable Approach to Domain-agnostic Labeled Graph Generation'
      date: '2020-01-22'
    Orbit:
    - value: 0.016
      std: null
      model: GraphGen
      arxiv_id: '2001.08184'
      title: 'GraphGen: A Scalable Approach to Domain-agnostic Labeled Graph Generation'
      date: '2020-01-22'
    - value: 0.008
      std: 0.007
      model: CatFlow
      arxiv_id: '2406.04843'
      title: Variational Flow Matching for Graph Generation
      date: '2024-06-07'
    Uniqueness:
    - value: 0.99
      std: null
      model: GraphGen
      arxiv_id: '2001.08184'
      title: 'GraphGen: A Scalable Approach to Domain-agnostic Labeled Graph Generation'
      date: '2020-01-22'
---

