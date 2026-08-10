---
title: CLUSTER
slug: cluster
benchmark: GNNBenchmark
task_type: node_classification
description: Semi-supervised node classification on stochastic block model graphs
  (6 classes).
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.GNNBenchmarkDataset.html
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 6
result_count: 172
best_model:
  model: GRPE-Small
  value: 0.81586
  metric: Accuracy
  arxiv_id: '2201.12787'
  paper_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
papers:
- arxiv_id: '2606.04647'
  title: 'ALINC: Active Learning for Inductive Node Classification via Graph Sampling'
  date_iso: '2026-06-03'
  venue: ''
- arxiv_id: '2605.05689'
  title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive Consistency
    Model'
  date_iso: '2026-05-07'
  venue: ''
- arxiv_id: '2510.14336'
  title: 'DARTS-GT: Differentiable Architecture Search for Graph Transformers with
    Quantifiable Instance-Specific Interpretability Analysis'
  date_iso: '2025-10-16'
  venue: ''
- arxiv_id: '2508.05070'
  title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
  date_iso: '2025-08-07'
  venue: ''
- arxiv_id: '2504.12588'
  title: Plain Transformers Can be Powerful Graph Learners
  date_iso: '2025-04-17'
  venue: ''
- arxiv_id: '2502.08092'
  title: 'GCoT: Chain-of-Thought Prompt Learning for Graphs'
  date_iso: '2025-02-12'
  venue: KDD 2025
- arxiv_id: '2411.12732'
  title: Benchmarking Positional Encodings for GNNs and Graph Transformers
  date_iso: '2024-11-19'
  venue: KDD 2024
- arxiv_id: '2405.19779'
  title: Automatic Graph Topology-Aware Transformer
  date_iso: '2024-05-30'
  venue: ''
- arxiv_id: '2405.19121'
  title: Spatio-Spectral Graph Neural Networks
  date_iso: '2024-05-29'
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
- arxiv_id: '2312.01538'
  title: Recurrent Distance Filtering for Graph Representation Learning
  date_iso: '2023-12-03'
  venue: ICML 2023
- arxiv_id: '2310.20519'
  title: Enhancing Graph Neural Networks with Quantum Computed Encodings
  date_iso: '2023-10-31'
  venue: ''
- arxiv_id: '2305.11424'
  title: IJCAI--23 Formatting Instructions
  date_iso: '2023-05-19'
  venue: IJCAI 2023
- arxiv_id: '2303.00579'
  title: Are More Layers Beneficial to Graph Transformers?
  date_iso: '2023-03-01'
  venue: ICLR 2023
- arxiv_id: '2003.00982'
  title: GNNBenchmark
  date_iso: '2023-01-01'
  venue: JMLR 2023
- arxiv_id: '2206.02059'
  title: Empowering GNNs via Edge-Aware Weisfeiler-Leman Algorithm
  date_iso: '2022-06-04'
  venue: TMLR 2022
- arxiv_id: '2205.12454'
  title: Recipe for a General, Powerful, Scalable Graph Transformer
  date_iso: '2022-05-25'
  venue: NeurIPS 2022
- arxiv_id: '2202.03036'
  title: Structure-Aware Transformer for Graph Representation Learning
  date_iso: '2022-02-07'
  venue: ICML 2022
- arxiv_id: '2201.12787'
  title: 'GRPE: Relative Positional Encoding for Graph Transformer'
  date_iso: '2022-01-30'
  venue: ''
- arxiv_id: '2201.12674'
  title: Rewiring with Positional Encodings for Graph Neural Networks
  date_iso: '2022-01-29'
  venue: TMLR 2022
- arxiv_id: '2201.09332'
  title: How Expressive are Transformers in Spectral Domain for Graphs?
  date_iso: '2022-01-23'
  venue: TMLR 2022
- arxiv_id: '2110.07141'
  title: 'SoGCN: Second-Order Graph Convolutional Networks'
  date_iso: '2021-10-14'
  venue: ''
- arxiv_id: '2107.04755'
  title: 'Beyond Low-pass Filtering: Graph Convolutional Networks with Automatic Filtering'
  date_iso: '2021-07-10'
  venue: ''
- arxiv_id: '2102.07835'
  title: Topological Graph Neural Networks
  date_iso: '2021-02-15'
  venue: ICLR 2021
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
    num_classes: 6
  metrics:
  - Accuracy
  - ACC
  - AULC
  - W. Accuracy
  metric_display_names:
  - Accuracy
  - ACC
  - AULC
  - W. Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GRPE-Small
    model_plain: GRPE-Small
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 489.0
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.81586
    - null
    - null
    - null
    metric_stds:
    - 0.0019
    - null
    - null
    - null
  - model: TANGO-GPS
    model_plain: TANGO-GPS
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.05070'
    title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
    date: Aug 7, 2025
    date_iso: '2025-08-07'
    date_display: Aug 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.80113
    - null
    - null
    - null
    metric_stds:
    - 0.00138
    - null
    - null
    - null
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
    - 0.80026
    - null
    - null
    - null
    metric_stds:
    - 0.00277
    - null
    - null
    - null
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
    - 0.79777
    - null
    - null
    - null
    metric_stds:
    - 0.00171
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
    - 0.79236
    - null
    - null
    - null
    metric_stds:
    - 0.00215
    - null
    - null
    - null
  - model: EGT
    model_plain: EGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 500.0
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
    - 0.79232
    - null
    - null
    - null
    metric_stds:
    - 0.00348
    - null
    - null
    - null
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
    - 0.78895
    - null
    - null
    - null
    metric_stds:
    - 0.001145
    - null
    - null
    - null
  - model: SparseGRIT + SignNet
    model_plain: SparseGRIT + SignNet
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
    - 0.78882
    - null
    - null
    - null
    metric_stds:
    - 0.00146
    - null
    - null
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
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7882
    - null
    - null
    - null
    metric_stds:
    - 0.00187
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
    - 0.78592
    - null
    - null
    - null
    metric_stds:
    - 0.00052
    - null
    - null
    - null
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
    - 0.78495
    - null
    - null
    - null
    metric_stds:
    - 0.00103
    - null
    - null
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
    - 0.78308
    - null
    - null
    - null
    metric_stds:
    - 0.00111
    - null
    - null
    - null
  - model: DARTS-GT
    model_plain: DARTS-GT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.14336'
    title: 'DARTS-GT: Differentiable Architecture Search for Graph Transformers with
      Quantifiable Instance-Specific Interpretability Analysis'
    date: Oct 16, 2025
    date_iso: '2025-10-16'
    date_display: Oct 2025
    codebase_url: https://github.com/shrutiOx/DARTS_GT
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.78299
    - null
    - null
    - null
    metric_stds:
    - 0.0007
    - null
    - null
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
    - 0.7828
    - null
    - null
    - null
    metric_stds:
    - 0.00211
    - null
    - null
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
    - 0.78218
    - null
    - null
    - null
    metric_stds:
    - 0.00267
    - null
    - null
    - null
  - model: TANGO-GatedGCN
    model_plain: TANGO-GatedGCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.05070'
    title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
    date: Aug 7, 2025
    date_iso: '2025-08-07'
    date_display: Aug 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.78194
    - null
    - null
    - null
    metric_stds:
    - 0.00307
    - null
    - null
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
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.78171
    - null
    - null
    - null
    metric_stds:
    - 0.00231
    - null
    - null
    - null
  - model: UGAS
    model_plain: UGAS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.14336'
    title: 'DARTS-GT: Differentiable Architecture Search for Graph Transformers with
      Quantifiable Instance-Specific Interpretability Analysis'
    date: Oct 16, 2025
    date_iso: '2025-10-16'
    date_display: Oct 2025
    codebase_url: https://github.com/shrutiOx/DARTS_GT
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7814
    - null
    - null
    - null
    metric_stds:
    - 0.0021
    - null
    - null
    - null
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
    - 0.78098
    - null
    - null
    - null
    metric_stds:
    - 0.00211
    - null
    - null
    - null
  - model: S² GatedGCN
    model_plain: S² GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.19121'
    title: Spatio-Spectral Graph Neural Networks
    date: May 29, 2024
    date_iso: '2024-05-29'
    date_display: May 2024
    codebase_url: ''
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7808
    - null
    - null
    - null
    metric_stds:
    - 0.0005
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
    arxiv_id: '2405.19121'
    title: Spatio-Spectral Graph Neural Networks
    date: May 29, 2024
    date_iso: '2024-05-29'
    date_display: May 2024
    codebase_url: ''
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7807
    - null
    - null
    - null
    metric_stds:
    - 0.0004
    - null
    - null
    - null
  - model: GPTrans-Nano
    model_plain: GPTrans-Nano
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.11424'
    title: IJCAI--23 Formatting Instructions
    date: May 19, 2023
    date_iso: '2023-05-19'
    date_display: May 2023
    codebase_url: https://github.com/czczup/GPTrans
    published_conference: IJCAI 2023
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.78069
    - null
    - null
    - null
    metric_stds:
    - 0.00154
    - null
    - null
    - null
  - model: TIGT
    model_plain: TIGT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2405.19121'
    title: Spatio-Spectral Graph Neural Networks
    date: May 29, 2024
    date_iso: '2024-05-29'
    date_display: May 2024
    codebase_url: ''
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7803
    - null
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
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
    - 0.78016
    - null
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
    - null
  - model: SAT
    model_plain: SAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    - 0.77856
    - null
    - null
    - null
    metric_stds:
    - 0.00104
    - null
    - null
    - null
  - model: K-Subgraph SAT
    model_plain: K-Subgraph SAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.77856
    - null
    - null
    - null
    metric_stds:
    - 0.00104
    - null
    - null
    - null
  - model: SAN + RandAlign
    model_plain: SAN + RandAlign
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
    - 0.77847
    - null
    - null
    - null
    metric_stds:
    - 0.00073
    - null
    - null
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
    - 0.778
    - null
    - null
    - null
    metric_stds:
    - 0.00107
    - null
    - null
    - null
  - model: K-Subtree SAT
    model_plain: K-Subtree SAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.03036'
    title: Structure-Aware Transformer for Graph Representation Learning
    date: Feb 7, 2022
    date_iso: '2022-02-07'
    date_display: Feb 2022
    codebase_url: https://github.com/BorgwardtLab/SAT
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.77751
    - null
    - null
    - null
    metric_stds:
    - 0.00121
    - null
    - null
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
    - 0.7769
    - null
    - null
    - null
    metric_stds:
    - 0.00147
    - null
    - null
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
    - 0.7759
    - null
    - null
    - null
    metric_stds:
    - 0.00158
    - null
    - null
    - null
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
    - 0.77575
    - null
    - null
    - null
    metric_stds:
    - 0.00149
    - null
    - null
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
    - 0.7755
    - null
    - null
    - null
    metric_stds:
    - 0.00057
    - null
    - null
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
    - 0.7755
    - null
    - null
    - null
    metric_stds:
    - 0.00195
    - null
    - null
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
    - 0.77514
    - null
    - null
    - null
    metric_stds:
    - 0.00182
    - null
    - null
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
    - 0.775
    - null
    - null
    - null
    metric_stds:
    - 0.00151
    - null
    - null
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
    - 0.77478
    - null
    - null
    - null
    metric_stds:
    - 0.0015
    - null
    - null
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
    - 0.7747
    - null
    - null
    - null
    metric_stds:
    - 0.00067
    - null
    - null
    - null
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
    - 0.77434
    - null
    - null
    - null
    metric_stds:
    - 0.00056
    - null
    - null
    - null
  - model: GraphGPS + RRWP
    model_plain: GraphGPS + RRWP
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
    - 0.7742
    - null
    - null
    - null
    metric_stds:
    - 0.0008
    - null
    - null
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
    - 0.77402
    - null
    - null
    - null
    metric_stds:
    - 0.0012
    - null
    - null
    - null
  - model: ARGNP
    model_plain: ARGNP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2405.19121'
    title: Spatio-Spectral Graph Neural Networks
    date: May 29, 2024
    date_iso: '2024-05-29'
    date_display: May 2024
    codebase_url: ''
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7735
    - null
    - null
    - null
    metric_stds:
    - 0.0005
    - null
    - null
    - null
  - model: SparseGRIT + noPE
    model_plain: SparseGRIT + noPE
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
    - 0.77274
    - null
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
    - null
  - model: FeTA + LPE + Sparse
    model_plain: FeTA + LPE + Sparse
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.77224
    - null
    - null
    - null
    metric_stds:
    - 0.00111
    - null
    - null
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
    - 0.77175
    - null
    - null
    - null
    metric_stds:
    - 0.00165
    - null
    - null
    - null
  - model: SparseGRIT + RWSE
    model_plain: SparseGRIT + RWSE
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
    - 0.77148
    - null
    - null
    - null
    metric_stds:
    - 0.00174
    - null
    - null
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
    - 0.76866
    - null
    - null
    - null
    metric_stds:
    - 0.00171
    - null
    - null
    - null
  - model: GraphGPS + PPR
    model_plain: GraphGPS + PPR
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
    - 0.76828
    - null
    - null
    - null
    metric_stds:
    - 0.0025
    - null
    - null
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
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.76773
    - null
    - null
    - null
    metric_stds:
    - 0.00301
    - null
    - null
    - null
  - model: FeTA + LPE + Full
    model_plain: FeTA + LPE + Full
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.7675
    - null
    - null
    - null
    metric_stds:
    - 0.00296
    - null
    - null
    - null
  row_count: 172
  rows_json: /data/datasets/cluster/standard-split-rows.json
  chart_json: /data/datasets/cluster/standard-split-chart.json
  arch_counts:
    gnn: 73
    hybrid: 36
    graph_transformer: 46
    llm: 0
    walk: 0
    traditional: 11
  metric_counts:
  - 140
  - 10
  - 11
  - 11
  milestones: &id001
  - value: 0.7639
    std: 0.0013
    model: LRGA + GatedGCN
    arxiv_id: '2006.07846'
    title: Formatting Instructions for ICLR 2021 Conference Submissions
    date: '2020-06-14'
  - value: 0.77224
    std: 0.00111
    model: FeTA + LPE + Sparse
    arxiv_id: '2201.09332'
    title: How Expressive are Transformers in Spectral Domain for Graphs?
    date: '2022-01-23'
  - value: 0.77575
    std: 0.00149
    model: Ours(100K)
    arxiv_id: '2201.12674'
    title: Rewiring with Positional Encodings for Graph Neural Networks
    date: '2022-01-29'
  - value: 0.81586
    std: 0.0019
    model: GRPE-Small
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: '2022-01-30'
  milestones_by_metric:
    Accuracy: *id001
    ACC:
    - value: 0.741
      std: 0.002
      model: AutoGCN
      arxiv_id: '2107.04755'
      title: 'Beyond Low-pass Filtering: Graph Convolutional Networks with Automatic
        Filtering'
      date: '2021-07-10'
    AULC:
    - value: 62.36
      std: 0.26
      model: Degree (Max)
      arxiv_id: '2606.04647'
      title: 'ALINC: Active Learning for Inductive Node Classification via Graph Sampling'
      date: '2026-06-03'
    W. Accuracy:
    - value: 0.80027
      std: 0.00114
      model: PPGT
      arxiv_id: '2504.12588'
      title: Plain Transformers Can be Powerful Graph Learners
      date: '2025-04-17'
---

