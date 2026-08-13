---
title: PascalVOC-SP
slug: pascalvoc-sp
benchmark: LRGB
task_type: node_classification
short_description: Assign one of 21 semantic-segmentation labels, including background,
  to every superpixel node.
description: '**21-class node classification** Assign one of 21 semantic-segmentation
  labels, including background, to every superpixel node. Evaluated by F1.'
detailed_description:
  task: Assign one of 21 semantic-segmentation labels, including background, to every
    superpixel node. A superpixel receives the ground-truth class of the pixel at
    the superpixel's center-of-mass coordinate.
  data: Each of 11,355 images from the Semantic Boundaries Dataset augmentation of
    Pascal VOC 2011 becomes one graph. SLIC with compactness 30 produces at most 500
    image regions, and two regions are connected when they share a boundary in the
    default region-adjacency graph.
  features: Each node has 12 RGB summary values—the mean, standard deviation, maximum,
    and minimum in each channel—plus its two-dimensional center-of-mass coordinate.
    Each edge stores the average Sobel response and pixel count along the shared boundary.
  splits_and_evaluation: The original training set remains training data. The original
    validation set is divided equally into validation and test subsets using a stratified
    image-level meta-label obtained by majority vote over non-background node labels,
    yielding 8,498/1,428/1,429 graphs. The score is class-weighted macro F1 over nodes.
  quirks_and_pitfalls: This is not pixel-level segmentation; labels and predictions
    are quantized to superpixels, and labeling only from the center pixel can misrepresent
    mixed regions. LRGB also releases compactness-10 and 8-nearest-neighbor graph
    variants, whose structures and edge features differ from the default compactness-30
    region-boundary version.
sources:
- title: Long Range Graph Benchmark
  arxiv_id: '2206.08164'
  kind: benchmark_definition
- title: The PASCAL Visual Object Classes Challenge
  url: http://host.robots.ox.ac.uk/pascal/VOC/pubs/everingham10.pdf
  kind: upstream_data_source
primary_metric: F1
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.LRGBDataset.html
stats:
  num_graphs: 11355
  avg_nodes: 479.4
  avg_edges: 2710.48
  num_classes: 21
result_count: 130
best_model:
  model: NeuralWalker
  value: 0.4912
  metric: F1
  arxiv_id: '2510.12111'
  paper_title: 'Chimera: State Space Models Beyond Sequences'
papers:
- arxiv_id: '2606.05046'
  title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for Structure-Aware
    Graph Machine Learning'
  date_iso: '2026-06-03'
  venue: ''
- arxiv_id: '2605.13383'
  title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
  date_iso: '2026-05-13'
  venue: ''
- arxiv_id: '2605.05689'
  title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive Consistency
    Model'
  date_iso: '2026-05-07'
  venue: ''
- arxiv_id: '2601.19094'
  title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
  date_iso: '2026-01-27'
  venue: ''
- arxiv_id: '2510.12111'
  title: 'Chimera: State Space Models Beyond Sequences'
  date_iso: '2025-10-14'
  venue: TMLR 2025
- arxiv_id: '2506.01231'
  title: Towards Efficient Few-shot Graph Neural Architecture Search via Partitioning
    Gradient Contribution
  date_iso: '2025-06-02'
  venue: KDD 2025
- arxiv_id: '2505.12880'
  title: AdS-GNN - a Conformally Equivariant Graph Neural Network
  date_iso: '2025-05-19'
  venue: ''
- arxiv_id: '2504.12588'
  title: Plain Transformers Can be Powerful Graph Learners
  date_iso: '2025-04-17'
  venue: ''
- arxiv_id: '2411.12732'
  title: Benchmarking Positional Encodings for GNNs and Graph Transformers
  date_iso: '2024-11-19'
  venue: KDD 2024
- arxiv_id: '2410.05593'
  title: When Graph Neural Networks Meet Dynamic Mode Decomposition
  date_iso: '2024-10-08'
  venue: ICLR 2024
- arxiv_id: '2406.12059'
  title: A Scalable and Effective Alternative to Graph Transformers
  date_iso: '2024-06-17'
  venue: AAAI 2024
- arxiv_id: '2406.01977'
  title: What Improves the Generalization of Graph Transformers? A Theoretical Dive
    into the Self-attention and Positional Encoding
  date_iso: '2024-06-04'
  venue: ICML 2024
- arxiv_id: '2405.21061'
  title: Graph External Attention Enhanced Transformer
  date_iso: '2024-05-31'
  venue: ICML 2024
- arxiv_id: '2405.17404'
  title: Spectral Greedy Coresets for Graph Neural Networks
  date_iso: '2024-05-27'
  venue: ''
- arxiv_id: '2405.15540'
  title: Bundle Neural Networks for message diffusion on graphs
  date_iso: '2024-05-24'
  venue: ''
- arxiv_id: '2405.11951'
  title: 'Distinguished In Uniform: Self Attention Vs. Virtual Nodes'
  date_iso: '2024-05-20'
  venue: ICLR 2024
- arxiv_id: '2404.09774'
  title: 'RandAlign: A Parameter-Free Method for Regularizing Graph Convolutional
    Networks'
  date_iso: '2024-04-15'
  venue: ''
- arxiv_id: '2402.08678'
  title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
  date_iso: '2024-02-13'
  venue: KDD 2024
- arxiv_id: '2310.01618'
  title: 'Operator Learning Meets Numerical Analysis: Improving Neural Networks through
    Iterative Methods'
  date_iso: '2023-10-02'
  venue: ''
- arxiv_id: '2309.00367'
  title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
  date_iso: '2023-09-01'
  venue: TMLR 2023
- arxiv_id: '2301.11956'
  title: On the Connection Between MPNN and Graph Transformer
  date_iso: '2023-01-27'
  venue: ICML 2023
- arxiv_id: '2206.08164'
  title: LRGB
  date_iso: '2022-06-16'
  venue: NeurIPS 2022
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: F1
  default_metric: F1
  higher_is_better: true
  stats:
    num_graphs: 11355
    avg_nodes: 479.4
    avg_edges: 2710.48
    num_classes: 21
  metrics:
  - F1
  - fraction of nodes satisfying $\Delta_n(z_m)>0$
  metric_display_names:
  - F1
  - fraction of nodes satisfying $\Delta_n(z_m)>0$
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: NeuralWalker
    model_plain: NeuralWalker
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2510.12111'
    title: 'Chimera: State Space Models Beyond Sequences'
    date: Oct 14, 2025
    date_iso: '2025-10-14'
    date_display: Oct 2025
    codebase_url: https://github.com/goombalab/chimera
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.4912
    - null
    metric_stds:
    - 0.0042
    - null
  - model: PPGT
    model_plain: PPGT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2504.12588'
    title: Plain Transformers Can be Powerful Graph Learners
    date: Apr 17, 2025
    date_iso: '2025-04-17'
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
    - 0.4641
    - null
    metric_stds:
    - 0.0033
    - null
  - model: CRaWl
    model_plain: CRaWl
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2309.00367'
    title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    date: Sep 1, 2023
    date_iso: '2023-09-01'
    date_display: Sep 2023
    codebase_url: https://github.com/toenshoff/LRGB
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4588
    - null
    metric_stds:
    - 0.0079
    - null
  - model: GEAET
    model_plain: GEAET
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.113235
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2405.21061'
    title: Graph External Attention Enhanced Transformer
    date: May 31, 2024
    date_iso: '2024-05-31'
    date_display: May 2024
    codebase_url: https://github.com/icm1018/GEAET
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4585
    - null
    metric_stds:
    - null
    - null
  - model: GraphGPS
    model_plain: GraphGPS
    is_baseline: true
    is_overridden: true
    override_reason: Table 1 reports 45.38 +/- 0.83 percent; normalize both values
      to fractions.
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4538
    - null
    metric_stds:
    - 0.0083
    - null
  - model: GraphGPS + ESLapPE
    model_plain: GraphGPS + ESLapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4538
    - null
    metric_stds:
    - 0.0083
    - null
  - model: GraphGPS + RWSE
    model_plain: GraphGPS + RWSE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4531
    - null
    metric_stds:
    - 0.0073
    - null
  - model: GraphGPS + (noPE)
    model_plain: GraphGPS + (noPE)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4517
    - null
    metric_stds:
    - 0.0112
    - null
  - model: GraphGPS + GCKN
    model_plain: GraphGPS + GCKN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4515
    - null
    metric_stds:
    - 0.0053
    - null
  - model: GraphGPS+LapPE
    model_plain: GraphGPS+LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4501
    - null
    metric_stds:
    - 0.0057
    - null
  - model: GraphGPS + RWDIFF
    model_plain: GraphGPS + RWDIFF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4488
    - null
    metric_stds:
    - 0.0097
    - null
  - model: GatedGCN-VN
    model_plain: GatedGCN-VN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.11951'
    title: 'Distinguished In Uniform: Self Attention Vs. Virtual Nodes'
    date: May 20, 2024
    date_iso: '2024-05-20'
    date_display: May 2024
    codebase_url: https://github.com/toenshoff/VN-vs-GT
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4477
    - null
    metric_stds:
    - 0.0137
    - null
  - model: Chimera
    model_plain: Chimera
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.12111'
    title: 'Chimera: State Space Models Beyond Sequences'
    date: Oct 14, 2025
    date_iso: '2025-10-14'
    date_display: Oct 2025
    codebase_url: https://github.com/goombalab/chimera
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.446
    - null
    metric_stds:
    - 0.007
    - null
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.00367'
    title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    date: Sep 1, 2023
    date_iso: '2023-09-01'
    date_display: Sep 2023
    codebase_url: https://github.com/toenshoff/LRGB
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.444
    - null
    metric_stds:
    - 0.0065
    - null
  - model: GraphGPS+Transformer
    model_plain: GraphGPS+Transformer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.12111'
    title: 'Chimera: State Space Models Beyond Sequences'
    date: Oct 14, 2025
    date_iso: '2025-10-14'
    date_display: Oct 2025
    codebase_url: https://github.com/goombalab/chimera
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.444
    - null
    metric_stds:
    - 0.0054
    - null
  - model: GMN
    model_plain: GMN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4393
    - null
    metric_stds:
    - 0.0112
    - null
  - model: Graph Mamba
    model_plain: Graph Mamba
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.12111'
    title: 'Chimera: State Space Models Beyond Sequences'
    date: Oct 14, 2025
    date_iso: '2025-10-14'
    date_display: Oct 2025
    codebase_url: https://github.com/goombalab/chimera
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4393
    - null
    metric_stds:
    - 0.0112
    - null
  - model: GraphGPS + SignNet
    model_plain: GraphGPS + SignNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4291
    - null
    metric_stds:
    - 0.0056
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
    - 0.4288
    - null
    metric_stds:
    - 0.0062
    - null
  - model: Exphormer
    model_plain: Exphormer
    is_baseline: true
    is_overridden: true
    override_reason: Table 1 reports 42.42 +/- 0.44 percent; normalize both values
      to fractions.
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4242
    - null
    metric_stds:
    - 0.0044
    - null
  - model: Exphormer + LapPE
    model_plain: Exphormer + LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4242
    - null
    metric_stds:
    - 0.0044
    - null
  - model: GCCM
    model_plain: GCCM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2605.05689'
    title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive Consistency
      Model'
    date: May 7, 2026
    date_iso: '2026-05-07'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4219
    - null
    metric_stds:
    - 0.0102
    - null
  - model: Exphormer + RWSE
    model_plain: Exphormer + RWSE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4218
    - null
    metric_stds:
    - 0.0063
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
    - 0.421
    - null
    metric_stds:
    - 0.008
    - null
  - model: EXPHORMER + GCN
    model_plain: EXPHORMER + GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4196
    - null
    metric_stds:
    - 0.0049
    - null
  - model: GPS-PCL
    model_plain: GPS-PCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.05689'
    title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive Consistency
      Model'
    date: May 7, 2026
    date_iso: '2026-05-07'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4196
    - null
    metric_stds:
    - 0.0086
    - null
  - model: Graph-Mamba
    model_plain: Graph-Mamba
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_iso: '2026-01-27'
    date_display: Jan 2026
    codebase_url: https://github.com/ocx-lab/FloydNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4191
    - null
    metric_stds:
    - null
    - null
  - model: GPS + Mamba
    model_plain: GPS + Mamba
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.418
    - null
    metric_stds:
    - 0.012
    - null
  - model: Exphormer + RWDIFF
    model_plain: Exphormer + RWDIFF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4165
    - null
    metric_stds:
    - 0.0059
    - null
  - model: Exphormer + noPE
    model_plain: Exphormer + noPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4149
    - null
    metric_stds:
    - 0.0047
    - null
  - model: Exphormer + ESLapPE
    model_plain: Exphormer + ESLapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4141
    - null
    metric_stds:
    - 0.0054
    - null
  - model: Exphormer + WLPE
    model_plain: Exphormer + WLPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4104
    - null
    metric_stds:
    - 0.0071
    - null
  - model: CRaWl
    model_plain: CRaWl
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4088
    - null
    metric_stds:
    - 0.0079
    - null
  - model: BuNN
    model_plain: BuNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.15540'
    title: Bundle Neural Networks for message diffusion on graphs
    date: May 24, 2024
    date_iso: '2024-05-24'
    date_display: May 2024
    codebase_url: https://github.com/jacobbamberger/BuNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4049
    - null
    metric_stds:
    - 0.0046
    - null
  - model: FloydNet
    model_plain: FloydNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_iso: '2026-01-27'
    date_display: Jan 2026
    codebase_url: https://github.com/ocx-lab/FloydNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4046
    - null
    metric_stds:
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
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4006
    - null
    metric_stds:
    - 0.0061
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
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_iso: '2024-02-13'
    date_display: Feb 2024
    codebase_url: ''
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3975
    - null
    metric_stds:
    - 0.0037
    - null
  - model: Exphormer + SignNet
    model_plain: Exphormer + SignNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3966
    - null
    metric_stds:
    - 0.002
    - null
  - model: GatedGCN + GCKN
    model_plain: GatedGCN + GCKN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3933
    - null
    metric_stds:
    - 0.0044
    - null
  - model: GatedGCN + ESLapPE
    model_plain: GatedGCN + ESLapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.393
    - null
    metric_stds:
    - 0.0041
    - null
  - model: GatedGCN + noPE
    model_plain: GatedGCN + noPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3923
    - null
    metric_stds:
    - 0.002
    - null
  - model: GatedGCN+LapPE
    model_plain: GatedGCN+LapPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.392
    - null
    metric_stds:
    - 0.0033
    - null
  - model: GatedGCN + RWDIFF
    model_plain: GatedGCN + RWDIFF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3919
    - null
    metric_stds:
    - 0.0019
    - null
  - model: GPS-LGD
    model_plain: GPS-LGD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.05689'
    title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive Consistency
      Model'
    date: May 7, 2026
    date_iso: '2026-05-07'
    date_display: May 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3912
    - null
    metric_stds:
    - 0.0207
    - null
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_iso: '2026-05-13'
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
    - 0.3884
    - null
    metric_stds:
    - 0.0055
    - null
  - model: GatedGCN+RWSE
    model_plain: GatedGCN+RWSE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3882
    - null
    metric_stds:
    - 0.0041
    - null
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.00367'
    title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    date: Sep 1, 2023
    date_iso: '2023-09-01'
    date_display: Sep 2023
    codebase_url: https://github.com/toenshoff/LRGB
    published_conference: TMLR 2023
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.388
    - null
    metric_stds:
    - 0.004
    - null
  - model: Gated-GCN
    model_plain: Gated-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.12111'
    title: 'Chimera: State Space Models Beyond Sequences'
    date: Oct 14, 2025
    date_iso: '2025-10-14'
    date_display: Oct 2025
    codebase_url: https://github.com/goombalab/chimera
    published_conference: TMLR 2025
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.388
    - null
    metric_stds:
    - 0.004
    - null
  - model: GatedGCN + SignNet
    model_plain: GatedGCN + SignNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3814
    - null
    metric_stds:
    - 0.0005
    - null
  - model: GatedGCN + WLPE
    model_plain: GatedGCN + WLPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_iso: '2024-11-19'
    date_display: Nov 2024
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    published_conference: KDD 2024
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3805
    - null
    metric_stds:
    - 0.0018
    - null
  row_count: 130
  rows_json: /data/datasets/pascalvoc-sp/standard-split-rows.json
  chart_json: /data/datasets/pascalvoc-sp/standard-split-chart.json
  arch_counts:
    gnn: 46
    hybrid: 30
    graph_transformer: 44
    llm: 0
    walk: 1
    traditional: 8
  metric_counts:
  - 129
  - 1
  milestones: &id001
  - value: 0.323
    std: 0.0039
    model: SAN+LapPE
    arxiv_id: '2206.08164'
    title: LRGB
    date: '2022-06-16'
  - value: 0.4588
    std: 0.0079
    model: CRaWl
    arxiv_id: '2309.00367'
    title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    date: '2023-09-01'
  - value: 0.4641
    std: 0.0033
    model: PPGT
    arxiv_id: '2504.12588'
    title: Plain Transformers Can be Powerful Graph Learners
    date: '2025-04-17'
  - value: 0.4912
    std: 0.0042
    model: NeuralWalker
    arxiv_id: '2510.12111'
    title: 'Chimera: State Space Models Beyond Sequences'
    date: '2025-10-14'
  milestones_by_metric:
    F1: *id001
    fraction of nodes satisfying $\Delta_n(z_m)>0$:
    - value: 0.9854
      std: null
      model: GT
      arxiv_id: '2406.01977'
      title: What Improves the Generalization of Graph Transformers? A Theoretical
        Dive into the Self-attention and Positional Encoding
      date: '2024-06-04'
---

