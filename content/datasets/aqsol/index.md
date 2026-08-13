---
title: AQSOL
slug: aqsol
benchmark: Classic
task_type: graph_regression
short_description: Predict measured aqueous solubility on molecular graphs.
description: '**Graph regression** on molecular graphs, predicting measured aqueous
  solubility. Atom and bond types form the graph input. Evaluated by MAE.'
detailed_description:
  task: Aqueous solubility regression on 9,982 molecular graphs from the LRGB paper.
    The primary catalog metric is MAE.
  data: Aqueous solubility regression on 9,982 molecular graphs from the LRGB paper.
  features: The representation follows the cited PyG loader or benchmark release.
    Node and edge fields are dataset-specific; preprocessing, graph direction, and
    any feature normalization must be kept fixed when reproducing a result.
  splits_and_evaluation: 'The catalog records these protocols or variants: Standard
    split. Evaluation uses MAE (lower is better). Exact masks or folds must come from
    the cited release.'
  quirks_and_pitfalls: The same short dataset name is used for incompatible processed
    artifacts and split protocols. Report the loader/version, directedness, feature
    preprocessing, and exact masks; transductive results should not be described as
    inductive.
sources:
- title: AqSolDB, a curated reference set of aqueous solubility
  url: https://doi.org/10.1038/s41597-019-0151-1
  kind: benchmark_or_upstream_source
- title: PyTorch Geometric AQSOL loader documentation
  url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.AQSOL.html
  kind: implementation_documentation
primary_metric: MAE
higher_is_better: false
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.AQSOL.html
stats: null
result_count: 34
best_model:
  model: Ours(100K)
  value: 0.92
  metric: MAE
  arxiv_id: '2201.12674'
  paper_title: Rewiring with Positional Encodings for Graph Neural Networks
papers:
- arxiv_id: '2505.13087'
  title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
    Encodings
  date_iso: '2025-05-19'
  venue: ICML 2025
- arxiv_id: '2003.00982'
  title: GNNBenchmark
  date_iso: '2023-01-01'
  venue: JMLR 2023
- arxiv_id: '2201.12674'
  title: Rewiring with Positional Encodings for Graph Neural Networks
  date_iso: '2022-01-29'
  venue: TMLR 2022
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: MAE
  default_metric: MAE
  higher_is_better: false
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - MAE
  metric_display_names:
  - MAE
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.92
    metric_stds:
    - 0.009
  - model: GatedGCN-PE/E(500K)
    model_plain: GatedGCN-PE/E(500K)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.996
    metric_stds:
    - 0.008
  - model: GatedGCN-E-PE
    model_plain: GatedGCN-E-PE
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
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.996
    metric_stds:
    - 0.008
  - model: 3WLGNN-E
    model_plain: 3WLGNN-E
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
    - 1.042
    metric_stds:
    - 0.064
  - model: GAPE + RWPE
    model_plain: GAPE + RWPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.13087'
    title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
      Encodings
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.069
    metric_stds:
    - 0.009
  - model: PNA(100K)
    model_plain: PNA(100K)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 1.083
    metric_stds:
    - 0.011
  - model: GAPE
    model_plain: GAPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.13087'
    title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
      Encodings
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.085
    metric_stds:
    - 0.009
  - model: 3WLGNN
    model_plain: 3WLGNN
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
    - 1.108
    metric_stds:
    - 0.036
  - model: GraphTransformer(500K)
    model_plain: GraphTransformer(500K)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    - 1.11
    metric_stds:
    - 0.01
  - model: RWPE
    model_plain: RWPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.13087'
    title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
      Encodings
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.12
    metric_stds:
    - 0.004
  - model: R-LAP
    model_plain: R-LAP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2505.13087'
    title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
      Encodings
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.23
    metric_stds:
    - 0.007
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.13087'
    title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
      Encodings
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.24
    metric_stds:
    - 0.011
  - model: SignNet
    model_plain: SignNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.13087'
    title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
      Encodings
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.26
    metric_stds:
    - 0.006
  - model: ABS-LAP
    model_plain: ABS-LAP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2505.13087'
    title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
      Encodings
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.27
    metric_stds:
    - 0.009
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.13087'
    title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
      Encodings
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.28
    metric_stds:
    - 0.011
  - model: GatedGCN(100K)
    model_plain: GatedGCN(100K)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 1.295
    metric_stds:
    - 0.016
  - model: GatedGCN-E
    model_plain: GatedGCN-E
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
    - 1.295
    metric_stds:
    - 0.016
  - model: LAP
    model_plain: LAP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2505.13087'
    title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
      Encodings
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.31
    metric_stds:
    - 0.006
  - model: LaplacianPE
    model_plain: LaplacianPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.13087'
    title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
      Encodings
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.31
    metric_stds:
    - 0.039
  - model: GCN
    model_plain: GCN
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
    - 1.333
    metric_stds:
    - 0.013
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
    - 1.352
    metric_stds:
    - 0.034
  - model: MoNet(100K)
    model_plain: MoNet(100K)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 1.395
    metric_stds:
    - 0.027
  - model: MoNet
    model_plain: MoNet
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
    - 1.395
    metric_stds:
    - 0.027
  - model: GraphSAGE
    model_plain: GraphSAGE
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
    - 1.402
    metric_stds:
    - 0.013
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
    - 1.403
    metric_stds:
    - 0.008
  - model: GraphSage(100K)
    model_plain: GraphSage(100K)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 1.431
    metric_stds:
    - 0.01
  - model: GAT(100K)
    model_plain: GAT(100K)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 1.441
    metric_stds:
    - 0.023
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
    - 1.458
    metric_stds:
    - 0.011
  - model: None
    model_plain: None
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.13087'
    title: Graph Alignment for Benchmarking Graph Neural Networks and Learning Positional
      Encodings
    date: May 19, 2025
    date_iso: '2025-05-19'
    date_display: May 2025
    codebase_url: ''
    published_conference: ICML 2025
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 1.71
    metric_stds:
    - 0.05
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    - 1.744
    metric_stds:
    - 0.016
  - model: GIN(100K)
    model_plain: GIN(100K)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 1.894
    metric_stds:
    - 0.024
  - model: GIN
    model_plain: GIN
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
    - 1.894
    metric_stds:
    - 0.024
  - model: RingGNN-E
    model_plain: RingGNN-E
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
    is_std_outlier: true
    metric_values:
    - 3.769
    metric_stds:
    - 1.012
  - model: RingGNN
    model_plain: RingGNN
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
    is_std_outlier: true
    metric_values:
    - 20.264
    metric_stds:
    - 7.549
  row_count: 34
  rows_json: ''
  chart_json: /data/datasets/aqsol/standard-split-chart.json
  arch_counts:
    gnn: 26
    hybrid: 3
    graph_transformer: 1
    llm: 0
    walk: 0
    traditional: 1
  metric_counts:
  - 34
  milestones: &id001
  - value: 0.92
    std: 0.009
    model: Ours(100K)
    arxiv_id: '2201.12674'
    title: Rewiring with Positional Encodings for Graph Neural Networks
    date: '2022-01-29'
  milestones_by_metric:
    MAE: *id001
---

