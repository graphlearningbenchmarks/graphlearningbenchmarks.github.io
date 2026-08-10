---
title: ogbg-molpcba
slug: ogbg-molpcba
benchmark: OGB
task_type: graph_classification
description: Multi-label classification (128 tasks) on PubChem BioAssay.
primary_metric: AP
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.OGBDataset.html
stats:
  num_graphs: 437929
  avg_nodes: 26.0
  avg_edges: 28.1
  num_classes: 128
result_count: 177
best_model:
  model: HIG with Graphormer
  value: 0.3167
  metric: AP
  arxiv_id: '2205.11678'
  paper_title: Compressing Deep Graph Neural Networks via Adversarial Knowledge Distillation
papers:
- arxiv_id: '2604.24293'
  title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
    via Continuous Phase Transitions'
  date_iso: '2026-04-27'
  venue: ''
- arxiv_id: '2604.17324'
  title: 'SigGate-GT: Taming Over-Smoothing in Graph Transformers via Sigmoid-Gated
    Attention'
  date_iso: '2026-04-19'
  venue: ''
- arxiv_id: '2510.05583'
  title: 'When does global attention help: a unified empirical study on atomistic
    graph learning'
  date_iso: '2025-10-07'
  venue: ''
- arxiv_id: '2509.24886'
  title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
    Networks
  date_iso: '2025-09-29'
  venue: ''
- arxiv_id: '2506.05957'
  title: Pruning Spurious Subgraphs for Graph Out-of-Distribution Generalization
  date_iso: '2025-06-06'
  venue: ''
- arxiv_id: '2502.16233'
  title: Graph Self-Supervised Learning with Learnable Structural and Positional Encodings
  date_iso: '2025-02-22'
  venue: WWW 2025
- arxiv_id: '2406.12059'
  title: A Scalable and Effective Alternative to Graph Transformers
  date_iso: '2024-06-17'
  venue: AAAI 2024
- arxiv_id: '2405.19779'
  title: Automatic Graph Topology-Aware Transformer
  date_iso: '2024-05-30'
  venue: ''
- arxiv_id: '2402.14393'
  title: Graph Parsing Networks
  date_iso: '2024-02-22'
  venue: ICLR 2024
- arxiv_id: '2402.04924'
  title: 'Two Trades are not Baffled: Condensing Graph via Crafting Rational Gradient
    Matching'
  date_iso: '2024-02-07'
  venue: ''
- arxiv_id: '2309.10131'
  title: Deep Prompt Tuning for Graph Transformers
  date_iso: '2023-09-18'
  venue: ''
- arxiv_id: '2309.00738'
  title: Rethinking the Power of Graph Canonization in Graph Representation Learning
    with Stability
  date_iso: '2023-09-01'
  venue: ''
- arxiv_id: '2306.15963'
  title: Fused Gromov-Wasserstein Graph Mixup for Graph-level Classifications
  date_iso: '2023-06-28'
  venue: NeurIPS 2023
- arxiv_id: '2305.06102'
  title: Towards Better Graph Representation Learning with Parameterized Decomposition
    & Filtering
  date_iso: '2023-05-10'
  venue: ICML 2023
- arxiv_id: '2304.02806'
  title: 'Graph Mixture of Experts: Learning on Large-Scale Graphs with Explicit Diversity
    Modeling'
  date_iso: '2023-04-06'
  venue: NeurIPS 2023
- arxiv_id: '2301.11956'
  title: On the Connection Between MPNN and Graph Transformer
  date_iso: '2023-01-27'
  venue: ICML 2023
- arxiv_id: '2211.15335'
  title: 'You Can Have Better Graph Neural Networks by Not Training Weights at All:
    Finding Untrained GNNs Tickets'
  date_iso: '2022-11-28'
  venue: LoG 2022
- arxiv_id: '2210.02997'
  title: Expander Graph Propagation
  date_iso: '2022-10-06'
  venue: LoG 2022
- arxiv_id: '2208.04529'
  title: Motif-based Graph Representation Learning with Application to Chemical Molecules
  date_iso: '2022-08-09'
  venue: ''
- arxiv_id: '2207.08806'
  title: Unified 2D and 3D Pre-Training of Molecular Representations
  date_iso: '2022-07-14'
  venue: KDD 2022
- arxiv_id: '2206.11941'
  title: Affinity-Aware Graph Networks
  date_iso: '2022-06-23'
  venue: NeurIPS 2022
- arxiv_id: '2206.11010'
  title: Agent-based Graph Neural Networks
  date_iso: '2022-06-22'
  venue: ICLR 2022
- arxiv_id: '2206.07746'
  title: Condensing Graphs via One-Step Gradient Matching
  date_iso: '2022-06-15'
  venue: KDD 2022
- arxiv_id: '2205.11678'
  title: Compressing Deep Graph Neural Networks via Adversarial Knowledge Distillation
  date_iso: '2022-05-24'
  venue: KDD 2022
- arxiv_id: '2202.08455'
  title: 'Transformer for Graphs: An Overview from Architecture Perspective'
  date_iso: '2022-02-17'
  venue: ''
- arxiv_id: '2202.00529'
  title: Molecular Representation Learning via Heterogeneous Motif Graph Neural Networks
  date_iso: '2022-02-01'
  venue: ICML 2022
- arxiv_id: '2201.12787'
  title: 'GRPE: Relative Positional Encoding for Graph Transformer'
  date_iso: '2022-01-30'
  venue: ''
- arxiv_id: '2110.07875'
  title: Graph Neural Networks with Learnable Structural and Positional Representations
  date_iso: '2021-10-15'
  venue: ICLR 2021
- arxiv_id: '2110.00577'
  title: Reconstruction for Powerful Graph Representations
  date_iso: '2021-10-01'
  venue: NeurIPS 2021
- arxiv_id: '2103.16584'
  title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
  date_iso: '2021-03-30'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: OGB scaffold split; AP is averaged across all 128 tasks.
  is_standard: true
  primary_metric: AP
  default_metric: AP
  higher_is_better: true
  stats:
    num_graphs: 437929
    avg_nodes: 26.0
    avg_edges: 28.1
    num_classes: 128
  metrics:
  - AP
  - Accuracy
  - ROC-AUC
  metric_display_names:
  - AP
  - Accuracy
  - ROC-AUC
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: HIG with Graphormer
    model_plain: HIG with Graphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.11678'
    title: Compressing Deep Graph Neural Networks via Adversarial Knowledge Distillation
    date: May 24, 2022
    date_iso: '2022-05-24'
    date_display: May 2022
    codebase_url: https://github.com/TencentYoutuResearch/HIG-GraphClassification
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.3167
    - null
    - null
    metric_stds:
    - 0.0034
    - null
    - null
  - model: GRPE-Large
    model_plain: GRPE-Large
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.315
    - null
    - null
    metric_stds:
    - 0.001
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
    arxiv_id: '2207.08806'
    title: Unified 2D and 3D Pre-Training of Molecular Representations
    date: Jul 14, 2022
    date_iso: '2022-07-14'
    date_display: Jul 2022
    codebase_url: https://github.com/teslacool/UnifiedMolPretrain
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.314
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: Graphormer-FLAG
    model_plain: Graphormer-FLAG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 47.0
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
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.3139
    - null
    - null
    metric_stds:
    - 0.0032
    - null
    - null
  - model: Graphormer FT
    model_plain: Graphormer FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 48.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.313
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
  - model: UnifiedMolPretrain
    model_plain: UnifiedMolPretrain
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2207.08806'
    title: Unified 2D and 3D Pre-Training of Molecular Representations
    date: Jul 14, 2022
    date_iso: '2022-07-14'
    date_display: Jul 2022
    codebase_url: https://github.com/teslacool/UnifiedMolPretrain
    published_conference: KDD 2022
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2022
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3125
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GRPE-Standard
    model_plain: GRPE-Standard
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3077
    - null
    - null
    metric_stds:
    - 0.0007
    - null
    - null
  - model: GSO
    model_plain: GSO
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3031
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
  - model: GraphGPS FT
    model_plain: GraphGPS FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 14.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.301
    - null
    - null
    metric_stds:
    - 0.013
    - null
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
    arxiv_id: '2206.11010'
    title: Agent-based Graph Neural Networks
    date: Jun 22, 2022
    date_iso: '2022-06-22'
    date_display: Jun 2022
    codebase_url: https://github.com/KarolisMart/AgentNet
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2986
    - null
    - null
    metric_stds:
    - 0.0025
    - null
    - null
  - model: SigGate-GT
    model_plain: SigGate-GT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2604.17324'
    title: 'SigGate-GT: Taming Over-Smoothing in Graph Transformers via Sigmoid-Gated
      Attention'
    date: Apr 19, 2026
    date_iso: '2026-04-19'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2984
    - null
    - null
    metric_stds:
    - 0.0031
    - null
    - null
  - model: GINE-AP
    model_plain: GINE-AP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 6.2
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2979
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
  - model: GINE
    model_plain: GINE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 6.1
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.2979
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
  - model: GraphGPS DeepGPT
    model_plain: GraphGPS DeepGPT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.05
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.297
    - null
    - null
    metric_stds:
    - 0.02
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
    - 0.2968
    - null
    - null
    metric_stds:
    - 0.0022
    - null
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
    - 0.2961
    - null
    - null
    metric_stds:
    - 0.0008
    - null
    - null
  - model: EGT-Large
    model_plain: EGT-Large
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 110.8
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
    - 0.2961
    - null
    - null
    metric_stds:
    - 0.0024
    - null
    - null
  - model: LiGhT FT
    model_plain: LiGhT FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 90.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.295
    - null
    - null
    metric_stds:
    - 0.006
    - null
    - null
  - model: PHC-GN
    model_plain: PHC-GN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1.7
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2947
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
  - model: PHC-2
    model_plain: PHC-2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.178
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2947
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
  - model: PHC-GNN
    model_plain: PHC-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2947
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
  - model: PHC-2-C
    model_plain: PHC-2-C
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.178
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2941
    - null
    - null
    metric_stds:
    - 0.0015
    - null
    - null
  - model: PHC-3
    model_plain: PHC-3
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.135
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2935
    - null
    - null
    metric_stds:
    - 0.0028
    - null
    - null
  - model: PHC-4
    model_plain: PHC-4
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.111
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.293
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
  - model: Subgraphormer
    model_plain: Subgraphormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2604.24293'
    title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
      via Continuous Phase Transitions'
    date: Apr 27, 2026
    date_iso: '2026-04-27'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.293
    - null
    - null
    metric_stds:
    - 0.004
    - null
    - null
  - model: PHC-4-Q
    model_plain: PHC-4-Q
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.111
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2921
    - null
    - null
    metric_stds:
    - 0.0023
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
    arxiv_id: '2604.17324'
    title: 'SigGate-GT: Taming Over-Smoothing in Graph Transformers via Sigmoid-Gated
      Attention'
    date: Apr 19, 2026
    date_iso: '2026-04-19'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.292
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
  - model: PHC-1
    model_plain: PHC-1
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.313
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2917
    - null
    - null
    metric_stds:
    - 0.0016
    - null
    - null
  - model: PHC-5
    model_plain: PHC-5
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.101
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2913
    - null
    - null
    metric_stds:
    - 0.0024
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
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_iso: '2023-01-27'
    date_display: Jan 2023
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2907
    - null
    - null
    metric_stds:
    - 0.0028
    - null
    - null
  - model: GraphGPS
    model_plain: GraphGPS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.17324'
    title: 'SigGate-GT: Taming Over-Smoothing in Graph Transformers via Sigmoid-Gated
      Attention'
    date: Apr 19, 2026
    date_iso: '2026-04-19'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2907
    - null
    - null
    metric_stds:
    - 0.0028
    - null
    - null
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 510.0
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.2902
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
  - model: Graphormer DeepGPT
    model_plain: Graphormer DeepGPT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.1
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    date: Sep 18, 2023
    date_iso: '2023-09-18'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.289
    - null
    - null
    metric_stds:
    - 0.009
    - null
    - null
  - model: DGN
    model_plain: DGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.114
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2885
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
  - model: novel method to learn motif-level feature embedding
    model_plain: novel method to learn motif-level feature embedding
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.00529'
    title: Molecular Representation Learning via Heterogeneous Motif Graph Neural
      Networks
    date: Feb 1, 2022
    date_iso: '2022-02-01'
    date_display: Feb 2022
    codebase_url: https://github.com/ZhaoningYu1996/HM-GNN
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.287
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
  - model: DeeperG
    model_plain: DeeperG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 5.6
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2842
    - null
    - null
    metric_stds:
    - 0.0043
    - null
    - null
  - model: DeeperGCN+FLAG
    model_plain: DeeperGCN+FLAG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.531
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2842
    - null
    - null
    metric_stds:
    - 0.0043
    - null
    - null
  - model: PNA-LSPE
    model_plain: PNA-LSPE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2110.07875'
    title: Graph Neural Networks with Learnable Structural and Positional Representations
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/vijaydwivedi75/gnn-lspe
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.284
    - null
    - null
    metric_stds:
    - 0.0021
    - null
    - null
  - model: PNA
    model_plain: PNA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.326
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2838
    - null
    - null
    metric_stds:
    - 0.0035
    - null
    - null
  - model: GIN+FLAG
    model_plain: GIN+FLAG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 3.336
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2834
    - null
    - null
    metric_stds:
    - 0.0038
    - null
    - null
  - model: MPNN + Noisy Nodes
    model_plain: MPNN + Noisy Nodes
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.11941'
    title: Affinity-Aware Graph Networks
    date: Jun 23, 2022
    date_iso: '2022-06-23'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2832
    - null
    - null
    metric_stds:
    - 0.0013
    - null
    - null
  - model: MPNN + VN + NoPE
    model_plain: MPNN + VN + NoPE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_iso: '2023-01-27'
    date_display: Jan 2023
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    published_conference: ICML 2023
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2823
    - null
    - null
    metric_stds:
    - 0.0026
    - null
    - null
  - model: MPNN
    model_plain: MPNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.11941'
    title: Affinity-Aware Graph Networks
    date: Jun 23, 2022
    date_iso: '2022-06-23'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2791
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
  - model: MPNN + Random Features + Noisy Nodes
    model_plain: MPNN + Random Features + Noisy Nodes
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.11941'
    title: Affinity-Aware Graph Networks
    date: Jun 23, 2022
    date_iso: '2022-06-23'
    date_display: Jun 2022
    codebase_url: ''
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.279
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
  - model: OAP+GatedGCN
    model_plain: OAP+GatedGCN
    is_baseline: true
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
    - 0.2783
    - null
    - null
    metric_stds:
    - 0.0024
    - null
    - null
  - model: ESAN (GIN + ED)
    model_plain: ESAN (GIN + ED)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2309.00738'
    title: Rethinking the Power of Graph Canonization in Graph Representation Learning
      with Stability
    date: Sep 1, 2023
    date_iso: '2023-09-01'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2782
    - null
    - null
    metric_stds:
    - 0.0036
    - null
    - null
  - model: GN-GIN
    model_plain: GN-GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.00738'
    title: Rethinking the Power of Graph Canonization in Graph Representation Learning
      with Stability
    date: Sep 1, 2023
    date_iso: '2023-09-01'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2781
    - null
    - null
    metric_stds:
    - 0.0043
    - null
    - null
  - model: DeeperGCN
    model_plain: DeeperGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.532
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: Mar 30, 2021
    date_iso: '2021-03-30'
    date_display: Mar 2021
    codebase_url: https://github.com/bayer-science-for-a-better-life/phc-gnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2781
    - null
    - null
    metric_stds:
    - 0.0038
    - null
    - null
  - model: DeeperGCN-VN
    model_plain: DeeperGCN-VN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.07875'
    title: Graph Neural Networks with Learnable Structural and Positional Representations
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/vijaydwivedi75/gnn-lspe
    published_conference: ICLR 2021
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.2781
    - null
    - null
    metric_stds:
    - 0.0038
    - null
    - null
  - model: HGODE
    model_plain: HGODE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.24293'
    title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
      via Continuous Phase Transitions'
    date: Apr 27, 2026
    date_iso: '2026-04-27'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.278
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
  row_count: 177
  rows_json: /data/datasets/ogbg-molpcba/standard-split-rows.json
  chart_json: /data/datasets/ogbg-molpcba/standard-split-chart.json
  arch_counts:
    gnn: 88
    hybrid: 32
    graph_transformer: 24
    llm: 0
    walk: 0
    traditional: 16
  metric_counts:
  - 122
  - 10
  - 45
  milestones: &id001
  - value: 0.2947
    std: 0.0026
    model: PHC-2
    arxiv_id: '2103.16584'
    title: Parameterized Hypercomplex Graph Neural Networks for Graph Classification
    date: '2021-03-30'
  - value: 0.315
    std: 0.001
    model: GRPE-Large
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: '2022-01-30'
  - value: 0.3167
    std: 0.0034
    model: HIG with Graphormer
    arxiv_id: '2205.11678'
    title: Compressing Deep Graph Neural Networks via Adversarial Knowledge Distillation
    date: '2022-05-24'
  milestones_by_metric:
    AP: *id001
    Accuracy:
    - value: 0.2665
      std: 0.0031
      model: GPN
      arxiv_id: '2402.14393'
      title: Graph Parsing Networks
      date: '2024-02-22'
    - value: 0.2745
      std: 0.0195
      model: StructPosGSSL-FA
      arxiv_id: '2502.16233'
      title: Graph Self-Supervised Learning with Learnable Structural and Positional
        Encodings
      date: '2025-02-22'
    ROC-AUC:
    - value: 0.646
      std: 0.004
      model: Whole Dataset
      arxiv_id: '2206.07746'
      title: Condensing Graphs via One-Step Gradient Matching
      date: '2022-06-15'
    - value: 0.784
      std: null
      model: UGTs
      arxiv_id: '2211.15335'
      title: 'You Can Have Better Graph Neural Networks by Not Training Weights at
        All: Finding Untrained GNNs Tickets'
      date: '2022-11-28'
    - value: 0.7919
      std: 0.0137
      model: EGTAS
      arxiv_id: '2405.19779'
      title: Automatic Graph Topology-Aware Transformer
      date: '2024-05-30'
    - value: 0.8159
      std: 0.0535
      model: PrunE
      arxiv_id: '2506.05957'
      title: Pruning Spurious Subgraphs for Graph Out-of-Distribution Generalization
      date: '2025-06-06'
---

