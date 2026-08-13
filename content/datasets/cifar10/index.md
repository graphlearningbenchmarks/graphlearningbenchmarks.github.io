---
title: CIFAR10
slug: cifar10
benchmark: GNNBenchmark
task_type: graph_classification
short_description: Graph classification on CIFAR10 superpixel graphs (10 classes,
  60k graphs).
description: '**10-class graph classification** Graph classification on CIFAR10 superpixel
  graphs (10 classes, 60k graphs). Uses the benchmark-provided synthetic or superpixel
  node/edge features. Evaluated by Accuracy.'
detailed_description:
  task: Graph classification on CIFAR10 superpixel graphs (10 classes, 60k graphs).
    The primary catalog metric is Accuracy.
  data: Graph classification on CIFAR10 superpixel graphs (10 classes, 60k graphs).
  features: The benchmark release supplies fixed graph tensors and task-specific node
    or edge inputs. Image graphs use superpixel appearance and position, synthetic
    node tasks use generated signals, TSP uses coordinates, and CSL is intentionally
    featureless.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses Accuracy (higher is better). Exact masks or folds must
    come from the cited release.'
  quirks_and_pitfalls: Use the released train/validation/test files rather than resplitting.
    These tasks were designed to expose specific architectural limitations, and preprocessing
    such as changing superpixels, adding positional encodings, or balancing edge labels
    changes the benchmark.
sources:
- title: GNNBenchmark benchmark
  arxiv_id: '2003.00982'
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric CIFAR10 loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.GNNBenchmarkDataset.html
  kind: implementation_documentation
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.GNNBenchmarkDataset.html
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 10
result_count: 160
best_model:
  model: RandAlign
  value: 0.7942
  metric: Accuracy
  arxiv_id: '2404.09774'
  paper_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph Convolutional
    Networks'
papers:
- arxiv_id: '2605.05689'
  title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive Consistency
    Model'
  date_iso: '2026-05-07'
  venue: ''
- arxiv_id: '2510.12369'
  title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive Graph Representation
    Learning
  date_iso: '2025-10-14'
  venue: ''
- arxiv_id: '2504.12588'
  title: Plain Transformers Can be Powerful Graph Learners
  date_iso: '2025-04-17'
  venue: ''
- arxiv_id: '2411.12732'
  title: Benchmarking Positional Encodings for GNNs and Graph Transformers
  date_iso: '2024-11-19'
  venue: KDD 2024
- arxiv_id: '2409.19117'
  title: 'Range-aware Positional Encoding via High-order Pretraining: Theory and Practice'
  date_iso: '2024-09-27'
  venue: ''
- arxiv_id: '2408.07654'
  title: 'Graph Triple Attention Network: A Decoupled Perspective'
  date_iso: '2024-08-14'
  venue: ''
- arxiv_id: '2407.02758'
  title: Differential Encoding for Improved Representation Learning Over Graphs
  date_iso: '2024-07-03'
  venue: ''
- arxiv_id: '2407.11596'
  title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
  date_iso: '2024-06-30'
  venue: ''
- arxiv_id: '2405.19779'
  title: Automatic Graph Topology-Aware Transformer
  date_iso: '2024-05-30'
  venue: ''
- arxiv_id: '2404.09774'
  title: 'RandAlign: A Parameter-Free Method for Regularizing Graph Convolutional
    Networks'
  date_iso: '2024-04-15'
  venue: ''
- arxiv_id: '2403.12529'
  title: Contextualized Messages Boost Graph Representations
  date_iso: '2024-03-19'
  venue: TMLR 2024
- arxiv_id: '2402.08678'
  title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
  date_iso: '2024-02-13'
  venue: KDD 2024
- arxiv_id: '2402.02005'
  title: Topology-Informed Graph Transformer
  date_iso: '2024-02-03'
  venue: ''
- arxiv_id: '2312.05905'
  title: Improving Subgraph-GNNs via Edge-Level Ego-Network Encodings
  date_iso: '2023-12-10'
  venue: TMLR 2023
- arxiv_id: '2312.01538'
  title: Recurrent Distance Filtering for Graph Representation Learning
  date_iso: '2023-12-03'
  venue: ICML 2023
- arxiv_id: '2310.20519'
  title: Enhancing Graph Neural Networks with Quantum Computed Encodings
  date_iso: '2023-10-31'
  venue: ''
- arxiv_id: '2003.00982'
  title: GNNBenchmark
  date_iso: '2023-01-01'
  venue: JMLR 2023
- arxiv_id: '2212.13350'
  title: A Generalization of ViT/MLP-Mixer to Graphs
  date_iso: '2022-12-27'
  venue: ICML 2022
- arxiv_id: '2206.07746'
  title: Condensing Graphs via One-Step Gradient Matching
  date_iso: '2022-06-15'
  venue: KDD 2022
- arxiv_id: '2205.12454'
  title: Recipe for a General, Powerful, Scalable Graph Transformer
  date_iso: '2022-05-25'
  venue: NeurIPS 2022
- arxiv_id: '2201.12674'
  title: Rewiring with Positional Encodings for Graph Neural Networks
  date_iso: '2022-01-29'
  venue: TMLR 2022
- arxiv_id: '2110.07875'
  title: Graph Neural Networks with Learnable Structural and Positional Representations
  date_iso: '2021-10-15'
  venue: ICLR 2021
- arxiv_id: '2110.07141'
  title: 'SoGCN: Second-Order Graph Convolutional Networks'
  date_iso: '2021-10-14'
  venue: ''
- arxiv_id: '2110.03753'
  title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
  date_iso: '2021-10-07'
  venue: ICLR 2021
- arxiv_id: '2107.04755'
  title: 'Beyond Low-pass Filtering: Graph Convolutional Networks with Automatic Filtering'
  date_iso: '2021-07-10'
  venue: ''
- arxiv_id: '2103.16584'
  title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
  date_iso: '2021-03-30'
  venue: ''
- arxiv_id: '2006.07846'
  title: Formatting Instructions for ICLR 2021 Conference Submissions
  date_iso: '2020-06-14'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: 10
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: RandAlign
    model_plain: RandAlign
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.7942
    metric_stds:
    - 0.00072
  - model: differential encoding
    model_plain: differential encoding
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.02758'
    title: Differential Encoding for Improved Representation Learning Over Graphs
    date: Jul 3, 2024
    date_iso: '2024-07-03'
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
    - 0.79067
    metric_stds:
    - 0.00269
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
    - 0.7856
    metric_stds:
    - 0.007
  - model: TAU-GRIT
    model_plain: TAU-GRIT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.12369'
    title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive Graph
      Representation Learning
    date: Oct 14, 2025
    date_iso: '2025-10-14'
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
    - 0.77784
    metric_stds:
    - 0.0049
  - model: GRED
    model_plain: GRED
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.01538'
    title: Recurrent Distance Filtering for Graph Representation Learning
    date: Dec 3, 2023
    date_iso: '2023-12-03'
    date_display: Dec 2023
    codebase_url: https://github.com/skeletondyh/GRED
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.76853
    metric_stds:
    - 0.00185
  - model: DeGTA
    model_plain: DeGTA
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2408.07654'
    title: 'Graph Triple Attention Network: A Decoupled Perspective'
    date: Aug 14, 2024
    date_iso: '2024-08-14'
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
    - 0.76756
    metric_stds:
    - 0.00927
  - model: GRIT
    model_plain: GRIT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_iso: '2023-10-31'
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
    - 0.76468
    metric_stds:
    - 0.00881
  - model: GRIT 2-QiQRW
    model_plain: GRIT 2-QiQRW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_iso: '2023-10-31'
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
    - 0.76442
    metric_stds:
    - 0.0107
  - model: GatedGCN + RandAlign
    model_plain: GatedGCN + RandAlign
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.76395
    metric_stds:
    - 0.00186
  - model: GatedGCN-16 + RandAlign
    model_plain: GatedGCN-16 + RandAlign
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.76395
    metric_stds:
    - 0.00186
  - model: GRIT 1-CQRW
    model_plain: GRIT 1-CQRW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_iso: '2023-10-31'
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
    - 0.76347
    metric_stds:
    - 0.00704
  - model: EdgeGCN
    model_plain: EdgeGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.02758'
    title: Differential Encoding for Improved Representation Learning Over Graphs
    date: Jul 3, 2024
    date_iso: '2024-07-03'
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
    - 0.76127
    metric_stds:
    - 0.00402
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
    - 0.7576
    metric_stds:
    - 0.0042
  - model: GRIT+RRWP
    model_plain: GRIT+RRWP
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
    - 0.7566
    metric_stds:
    - 0.0041
  - model: Exphormer + (LapPE)
    model_plain: Exphormer + (LapPE)
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
    - 0.7521
    metric_stds:
    - 0.001
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
    - 0.75205
    metric_stds:
    - 0.00095
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
    - 0.74962
    metric_stds:
    - 0.00631
  - model: SparseGRIT + (RRWP)
    model_plain: SparseGRIT + (RRWP)
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
    - 0.7495
    metric_stds:
    - 0.0026
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
    - 0.74926
    metric_stds:
    - 0.00288
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
    - 0.74886
    metric_stds:
    - 0.0081
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
    - 0.7488
    metric_stds:
    - 0.00322
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
    - 0.74794
    metric_stds:
    - 0.00358
  - model: PNA*-AK+-S
    model_plain: PNA*-AK+-S
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2110.03753'
    title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
    date: Oct 7, 2021
    date_iso: '2021-10-07'
    date_display: Oct 2021
    codebase_url: https://github.com/LingxiaoShawn/GNNAsKernel
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7479
    metric_stds:
    - 0.0018
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
    - 0.7469
    metric_stds:
    - 0.0013
  - model: Exphormer + RRWP
    model_plain: Exphormer + RRWP
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
    - 0.74504
    metric_stds:
    - 0.00369
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
    - 0.74434
    metric_stds:
    - 0.00205
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
    - 0.74308
    metric_stds:
    - 0.00575
  - model: Exphormer + PPR
    model_plain: Exphormer + PPR
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
    - 0.74076
    metric_stds:
    - 0.00104
  - model: Graph MLP-Mixer
    model_plain: Graph MLP-Mixer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.01538'
    title: Recurrent Distance Filtering for Graph Representation Learning
    date: Dec 3, 2023
    date_iso: '2023-12-03'
    date_display: Dec 2023
    codebase_url: https://github.com/skeletondyh/GRED
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7396
    metric_stds:
    - 0.0033
  - model: GraphTrans-MLP-Mixer
    model_plain: GraphTrans-MLP-Mixer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.13350'
    title: A Generalization of ViT/MLP-Mixer to Graphs
    date: Dec 27, 2022
    date_iso: '2022-12-27'
    date_display: Dec 2022
    codebase_url: https://github.com/XiaoxinHe/Graph-ViT-MLPMixer
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7396
    metric_stds:
    - 0.0033
  - model: TIGT
    model_plain: TIGT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: Feb 3, 2024
    date_iso: '2024-02-03'
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
    - 0.73955
    metric_stds:
    - 0.0036
  - model: ARGNP
    model_plain: ARGNP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2407.02758'
    title: Differential Encoding for Improved Representation Learning Over Graphs
    date: Jul 3, 2024
    date_iso: '2024-07-03'
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
    - 0.739
    metric_stds:
    - 0.0015
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
    - 0.73842
    metric_stds:
    - 0.00317
  - model: Ours(100K)
    model_plain: Ours(100K)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2201.12674'
    title: Rewiring with Positional Encodings for Graph Neural Networks
    date: Jan 29, 2022
    date_iso: '2022-01-29'
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
    - 0.73808
    metric_stds:
    - 0.00193
  - model: LRGA + GatedGCN
    model_plain: LRGA + GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.07846'
    title: Formatting Instructions for ICLR 2021 Conference Submissions
    date: Jun 14, 2020
    date_iso: '2020-06-14'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7348
    metric_stds:
    - 0.0029
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
    - 0.7341
    metric_stds:
    - 0.0015
  - model: PNA
    model_plain: PNA*
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.03753'
    title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
    date: Oct 7, 2021
    date_iso: '2021-10-07'
    date_display: Oct 2021
    codebase_url: https://github.com/LingxiaoShawn/GNNAsKernel
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7311
    metric_stds:
    - 0.0011
  - model: GPS + HOPE-WavePE
    model_plain: GPS + HOPE-WavePE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2409.19117'
    title: 'Range-aware Positional Encoding via High-order Pretraining: Theory and
      Practice'
    date: Sep 27, 2024
    date_iso: '2024-09-27'
    date_display: Sep 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7301
    metric_stds:
    - 0.0081
  - model: DGN
    model_plain: DGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.03753'
    title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
    date: Oct 7, 2021
    date_iso: '2021-10-07'
    date_display: Oct 2021
    codebase_url: https://github.com/LingxiaoShawn/GNNAsKernel
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7284
    metric_stds:
    - 0.0042
  - model: CKGCN
    model_plain: CKGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.72785
    metric_stds:
    - 0.00436
  - model: GCN-AK+
    model_plain: GCN-AK+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2110.03753'
    title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
    date: Oct 7, 2021
    date_iso: '2021-10-07'
    date_display: Oct 2021
    codebase_url: https://github.com/LingxiaoShawn/GNNAsKernel
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.727
    metric_stds:
    - 0.0029
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
    - 0.72502
    metric_stds:
    - 0.00287
  - model: Graph MLP-Mixer
    model_plain: Graph MLP-Mixer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2409.19117'
    title: 'Range-aware Positional Encoding via High-order Pretraining: Theory and
      Practice'
    date: Sep 27, 2024
    date_iso: '2024-09-27'
    date_display: Sep 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7246
    metric_stds:
    - 0.0036
  - model: GIN-AK+-S
    model_plain: GIN-AK+-S
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2110.03753'
    title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
    date: Oct 7, 2021
    date_iso: '2021-10-07'
    date_display: Oct 2021
    codebase_url: https://github.com/LingxiaoShawn/GNNAsKernel
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7239
    metric_stds:
    - 0.0038
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
    - 0.7231
    metric_stds:
    - 0.00198
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
    - 0.7231
    metric_stds:
    - 0.0053
  - model: GPS + (RWSE/LapPE)
    model_plain: GPS + (RWSE/LapPE)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2409.19117'
    title: 'Range-aware Positional Encoding via High-order Pretraining: Theory and
      Practice'
    date: Sep 27, 2024
    date_iso: '2024-09-27'
    date_display: Sep 2024
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.723
    metric_stds:
    - 0.0036
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.12454'
    title: Recipe for a General, Powerful, Scalable Graph Transformer
    date: May 25, 2022
    date_iso: '2022-05-25'
    date_display: May 2022
    codebase_url: https://github.com/rampasek/GraphGPS
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.72298
    metric_stds:
    - 0.00356
  - model: GraphGPS
    model_plain: GraphGPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2408.07654'
    title: 'Graph Triple Attention Network: A Decoupled Perspective'
    date: Aug 14, 2024
    date_iso: '2024-08-14'
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
    - 0.72298
    metric_stds:
    - 0.00356
  - model: GIN-AK+
    model_plain: GIN-AK+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.03753'
    title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
    date: Oct 7, 2021
    date_iso: '2021-10-07'
    date_display: Oct 2021
    codebase_url: https://github.com/LingxiaoShawn/GNNAsKernel
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7219
    metric_stds:
    - 0.0013
  row_count: 160
  rows_json: /data/datasets/cifar10/standard-split-rows.json
  chart_json: /data/datasets/cifar10/standard-split-chart.json
  arch_counts:
    gnn: 88
    hybrid: 41
    graph_transformer: 19
    llm: 0
    walk: 0
    traditional: 8
  metric_counts:
  - 160
  milestones: &id001
  - value: 0.7348
    std: 0.0029
    model: LRGA + GatedGCN
    arxiv_id: '2006.07846'
    title: Formatting Instructions for ICLR 2021 Conference Submissions
    date: '2020-06-14'
  - value: 0.7479
    std: 0.0018
    model: PNA*-AK+-S
    arxiv_id: '2110.03753'
    title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
    date: '2021-10-07'
  - value: 0.76468
    std: 0.00881
    model: GRIT
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: '2023-10-31'
  - value: 0.76853
    std: 0.00185
    model: GRED
    arxiv_id: '2312.01538'
    title: Recurrent Distance Filtering for Graph Representation Learning
    date: '2023-12-03'
  - value: 0.7942
    std: 0.00072
    model: RandAlign
    arxiv_id: '2404.09774'
    title: 'RandAlign: A Parameter-Free Method for Regularizing Graph Convolutional
      Networks'
    date: '2024-04-15'
  milestones_by_metric:
    Accuracy: *id001
---

