---
title: ogbn-proteins
slug: ogbn-proteins
benchmark: OGB
task_type: node_classification
description: Multi-label binary node classification on protein association network
  (112 tasks).
primary_metric: ROC-AUC
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.OGBNodePropPredDataset.html
stats:
  num_graphs: 132534
  avg_nodes: 39561252.0
  avg_edges: null
  num_classes: 112
result_count: 101
best_model:
  model: LD
  value: 0.8942
  metric: ROC-AUC
  arxiv_id: '2309.14907'
  paper_title: Label Deconvolution for Node Representation Learning on Large-scale
    Attributed Graphs against Learning Bias
papers:
- arxiv_id: '2604.24293'
  title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature Evolution
    via Continuous Phase Transitions'
  date_iso: '2026-04-27'
  venue: ''
- arxiv_id: '2602.19622'
  title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with Graph
    Token Attention'
  date_iso: '2026-02-23'
  venue: WWW 2026
- arxiv_id: '2602.17071'
  title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial Synthesis
    and Self-Corrective Propagation'
  date_iso: '2026-02-19'
  venue: ''
- arxiv_id: '2508.17630'
  title: 'Quantum Graph Attention Network: A Novel Quantum Multi-Head Attention Mechanism
    for Graph Learning'
  date_iso: '2025-08-25'
  venue: ''
- arxiv_id: '2505.09361'
  title: Efficient Mixed Precision Quantization in Graph Neural Networks
  date_iso: '2025-05-14'
  venue: ''
- arxiv_id: '2412.17961'
  title: 'Extending Graph Condensation to Multi-Label Datasets: A Benchmark Study'
  date_iso: '2024-12-23'
  venue: TMLR 2024
- arxiv_id: '2409.05573'
  title: Learning to Model Graph Structural Information on MLPs via Graph Structure
    Self-Contrasting
  date_iso: '2024-09-09'
  venue: ''
- arxiv_id: '2405.14260'
  title: Graph Sparsification via Mixture of Graphs
  date_iso: '2024-05-23'
  venue: ICLR 2024
- arxiv_id: '2402.15270'
  title: Smoothed Graph Contrastive Learning via Seamless Proximity Integration
  date_iso: '2024-02-23'
  venue: ''
- arxiv_id: '2309.14907'
  title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
    Graphs against Learning Bias
  date_iso: '2023-09-26'
  venue: ''
- arxiv_id: '2304.02806'
  title: 'Graph Mixture of Experts: Learning on Large-Scale Graphs with Explicit Diversity
    Modeling'
  date_iso: '2023-04-06'
  venue: NeurIPS 2023
- arxiv_id: '2211.14568'
  title: 'BeGin: Extensive Benchmark Scenarios and An Easy-to-use Framework for Graph
    Continual Learning'
  date_iso: '2022-11-26'
  venue: ''
- arxiv_id: '2110.14855'
  title: 'CAP: Co-Adversarial Perturbation on Weights and Features for Improving Generalization
    of Graph Neural Networks'
  date_iso: '2021-10-28'
  venue: ''
- arxiv_id: '2110.07141'
  title: 'SoGCN: Second-Order Graph Convolutional Networks'
  date_iso: '2021-10-14'
  venue: ''
- arxiv_id: '2009.03509'
  title: 'Masked Label Prediction: Unified Message Passing Model for Semi-Supervised
    Classification'
  date_iso: '2020-09-08'
  venue: IJCAI 2020
- arxiv_id: '2006.07107'
  title: Understanding and Resolving Performance Degradation in Deep Graph Convolutional
    Networks
  date_iso: '2020-06-12'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: ROC-AUC
  default_metric: ROC-AUC
  higher_is_better: true
  stats:
    num_graphs: 132534
    avg_nodes: 39561252.0
    avg_edges: null
    num_classes: 112
  metrics:
  - ROC-AUC
  - Accuracy
  - F1-macro
  - F1-micro
  metric_display_names:
  - ROC-AUC
  - Accuracy
  - F1-macro
  - F1-micro
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: LD
    model_plain: LD
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.14907'
    title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
      Graphs against Learning Bias
    date: Sep 26, 2023
    date_iso: '2023-09-26'
    date_display: Sep 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8942
    - null
    - null
    - null
    metric_stds:
    - 0.0007
    - null
    - null
    - null
  - model: X_WO/LD
    model_plain: X_WO/LD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.14907'
    title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
      Graphs against Learning Bias
    date: Sep 26, 2023
    date_iso: '2023-09-26'
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
    - 0.8915
    - null
    - null
    - null
    metric_stds:
    - 0.0012
    - null
    - null
    - null
  - model: MoG
    model_plain: MoG
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.14260'
    title: Graph Sparsification via Mixture of Graphs
    date: May 23, 2024
    date_iso: '2024-05-23'
    date_display: May 2024
    codebase_url: https://github.com/yanweiyue/MoG
    published_conference: ICLR 2024
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8904
    - null
    - null
    - null
    metric_stds:
    - 0.0072
    - null
    - null
    - null
  - model: X_PNE
    model_plain: X_PNE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.14907'
    title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
      Graphs against Learning Bias
    date: Sep 26, 2023
    date_iso: '2023-09-26'
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
    - 0.8894
    - null
    - null
    - null
    metric_stds:
    - 0.0014
    - null
    - null
    - null
  - model: X_GLEM
    model_plain: X_GLEM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.14907'
    title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
      Graphs against Learning Bias
    date: Sep 26, 2023
    date_iso: '2023-09-26'
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
    - 0.8872
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: X_FNE
    model_plain: X_FNE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.14907'
    title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
      Graphs against Learning Bias
    date: Sep 26, 2023
    date_iso: '2023-09-26'
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
    - 0.8866
    - null
    - null
    - null
    metric_stds:
    - 0.0008
    - null
    - null
    - null
  - model: UniMP
    model_plain: UniMP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2009.03509'
    title: 'Masked Label Prediction: Unified Message Passing Model for Semi-Supervised
      Classification'
    date: Sep 8, 2020
    date_iso: '2020-09-08'
    date_display: Sep 2020
    codebase_url: ''
    published_conference: IJCAI 2020
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2020
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8642
    - null
    - null
    - null
    metric_stds:
    - 0.0008
    - null
    - null
    - null
  - model: DeeperGCN
    model_plain: DeeperGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.253743
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.03509'
    title: 'Masked Label Prediction: Unified Message Passing Model for Semi-Supervised
      Classification'
    date: Sep 8, 2020
    date_iso: '2020-09-08'
    date_display: Sep 2020
    codebase_url: ''
    published_conference: IJCAI 2020
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.858
    - null
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
    - null
  - model: STR-Sparse
    model_plain: STR-Sparse
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2409.05573'
    title: Learning to Model Graph Structural Information on MLPs via Graph Structure
      Self-Contrasting
    date: Sep 9, 2024
    date_iso: '2024-09-09'
    date_display: Sep 2024
    codebase_url: https://github.com/LirongWu/GSSC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.855
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: DeepGCN
    model_plain: DeepGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 2.374456
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.03509'
    title: 'Masked Label Prediction: Unified Message Passing Model for Semi-Supervised
      Classification'
    date: Sep 8, 2020
    date_iso: '2020-09-08'
    date_display: Sep 2020
    codebase_url: ''
    published_conference: IJCAI 2020
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8496
    - null
    - null
    - null
    metric_stds:
    - 0.0028
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
    arxiv_id: '2409.05573'
    title: Learning to Model Graph Structural Information on MLPs via Graph Structure
      Self-Contrasting
    date: Sep 9, 2024
    date_iso: '2024-09-09'
    date_display: Sep 2024
    codebase_url: https://github.com/LirongWu/GSSC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.845
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: MWE-DGCN
    model_plain: MWE-DGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.538544
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.03509'
    title: 'Masked Label Prediction: Unified Message Passing Model for Semi-Supervised
      Classification'
    date: Sep 8, 2020
    date_iso: '2020-09-08'
    date_display: Sep 2020
    codebase_url: ''
    published_conference: IJCAI 2020
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8436
    - null
    - null
    - null
    metric_stds:
    - 0.0065
    - null
    - null
    - null
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2409.05573'
    title: Learning to Model Graph Structural Information on MLPs via Graph Structure
      Self-Contrasting
    date: Sep 9, 2024
    date_iso: '2024-09-09'
    date_display: Sep 2024
    codebase_url: https://github.com/LirongWu/GSSC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.843
    - null
    - null
    - null
    metric_stds:
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
    arxiv_id: '2409.05573'
    title: Learning to Model Graph Structural Information on MLPs via Graph Structure
      Self-Contrasting
    date: Sep 9, 2024
    date_iso: '2024-09-09'
    date_display: Sep 2024
    codebase_url: https://github.com/LirongWu/GSSC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.841
    - null
    - null
    - null
    metric_stds:
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
    arxiv_id: '2409.05573'
    title: Learning to Model Graph Structural Information on MLPs via Graph Structure
      Self-Contrasting
    date: Sep 9, 2024
    date_iso: '2024-09-09'
    date_display: Sep 2024
    codebase_url: https://github.com/LirongWu/GSSC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.832
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: NodeNorm
    model_plain: NodeNorm
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.07107'
    title: Understanding and Resolving Performance Degradation in Deep Graph Convolutional
      Networks
    date: Jun 12, 2020
    date_iso: '2020-06-12'
    date_display: Jun 2020
    codebase_url: https://github.com/miafei/NodeNorm
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8226
    - null
    - null
    - null
    metric_stds:
    - 0.0093
    - null
    - null
    - null
  - model: PI-GNN
    model_plain: PI-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.14568'
    title: 'BeGin: Extensive Benchmark Scenarios and An Easy-to-use Framework for
      Graph Continual Learning'
    date: Nov 26, 2022
    date_iso: '2022-11-26'
    date_display: Nov 2022
    codebase_url: https://github.com/ShinhwanKang/BeGin
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.82
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
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
    - 0.8124
    - null
    - null
    - null
    metric_stds:
    - 0.0063
    - null
    - null
    - null
  - model: SS/RD
    model_plain: SS/RD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2409.05573'
    title: Learning to Model Graph Structural Information on MLPs via Graph Structure
      Self-Contrasting
    date: Sep 9, 2024
    date_iso: '2024-09-09'
    date_display: Sep 2024
    codebase_url: https://github.com/LirongWu/GSSC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.812
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: GEM
    model_plain: GEM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.14568'
    title: 'BeGin: Extensive Benchmark Scenarios and An Easy-to-use Framework for
      Graph Continual Learning'
    date: Nov 26, 2022
    date_iso: '2022-11-26'
    date_display: Nov 2022
    codebase_url: https://github.com/ShinhwanKang/BeGin
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.81
    - null
    - null
    - null
    metric_stds:
    - 0.003
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
    - 0.8052
    - null
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
    - null
  - model: DRAGON
    model_plain: DRAGON
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.8046
    - null
    - null
    - null
    metric_stds:
    - 0.0042
    - null
    - null
    - null
  - model: FROND
    model_plain: FROND
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.8026
    - null
    - null
    - null
    metric_stds:
    - 0.0049
    - null
    - null
    - null
  - model: DAGNN
    model_plain: DAGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2409.05573'
    title: Learning to Model Graph Structural Information on MLPs via Graph Structure
      Self-Contrasting
    date: Sep 9, 2024
    date_iso: '2024-09-09'
    date_display: Sep 2024
    codebase_url: https://github.com/LirongWu/GSSC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7995
    - null
    - null
    - null
    metric_stds:
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
    - 0.7953
    - null
    - null
    - null
    metric_stds:
    - 0.0038
    - null
    - null
    - null
  - model: GATv2
    model_plain: GATv2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.17630'
    title: 'Quantum Graph Attention Network: A Novel Quantum Multi-Head Attention
      Mechanism for Graph Learning'
    date: Aug 25, 2025
    date_iso: '2025-08-25'
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
    - 0.7952
    - null
    - null
    - null
    metric_stds:
    - 0.0055
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
    - 0.7941
    - null
    - null
    - null
    metric_stds:
    - 0.0056
    - null
    - null
    - null
  - model: QGAT
    model_plain: QGAT
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.17630'
    title: 'Quantum Graph Attention Network: A Novel Quantum Multi-Head Attention
      Mechanism for Graph Learning'
    date: Aug 25, 2025
    date_iso: '2025-08-25'
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
    - 0.7941
    - null
    - null
    - null
    metric_stds:
    - 0.0021
    - null
    - null
    - null
  - model: GEN
    model_plain: GEN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.07107'
    title: Understanding and Resolving Performance Degradation in Deep Graph Convolutional
      Networks
    date: Jun 12, 2020
    date_iso: '2020-06-12'
    date_display: Jun 2020
    codebase_url: https://github.com/miafei/NodeNorm
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7936
    - null
    - null
    - null
    metric_stds:
    - 0.0086
    - null
    - null
    - null
  - model: SoGCN
    model_plain: SoGCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.07141'
    title: 'SoGCN: Second-Order Graph Convolutional Networks'
    date: Oct 14, 2021
    date_iso: '2021-10-14'
    date_display: Oct 2021
    codebase_url: https://github.com/yuehaowang/SoGCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7928
    - null
    - null
    - null
    metric_stds:
    - 0.0047
    - null
    - null
    - null
  - model: FLODE
    model_plain: FLODE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.7923
    - null
    - null
    - null
    metric_stds:
    - 0.0075
    - null
    - null
    - null
  - model: GREAD-BS
    model_plain: GREAD-BS
    is_baseline: true
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
    - 0.7921
    - null
    - null
    - null
    metric_stds:
    - 0.0074
    - null
    - null
    - null
  - model: Sheaf Diff.
    model_plain: Sheaf Diff.
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.7896
    - null
    - null
    - null
    metric_stds:
    - 0.0056
    - null
    - null
    - null
  - model: 4th-Order GCN
    model_plain: 4th-Order GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.320512
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.07141'
    title: 'SoGCN: Second-Order Graph Convolutional Networks'
    date: Oct 14, 2021
    date_iso: '2021-10-14'
    date_display: Oct 2021
    codebase_url: https://github.com/yuehaowang/SoGCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7895
    - null
    - null
    - null
    metric_stds:
    - 0.0057
    - null
    - null
    - null
  - model: BuNN
    model_plain: BuNN
    is_baseline: true
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
    - 0.7892
    - null
    - null
    - null
    metric_stds:
    - 0.0048
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
    arxiv_id: '2508.17630'
    title: 'Quantum Graph Attention Network: A Novel Quantum Multi-Head Attention
      Mechanism for Graph Learning'
    date: Aug 25, 2025
    date_iso: '2025-08-25'
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
    - 0.7863
    - null
    - null
    - null
    metric_stds:
    - 0.0162
    - null
    - null
    - null
  - model: 6th-Order GCN
    model_plain: 6th-Order GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.448512
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.07141'
    title: 'SoGCN: Second-Order Graph Convolutional Networks'
    date: Oct 14, 2021
    date_iso: '2021-10-14'
    date_display: Oct 2021
    codebase_url: https://github.com/yuehaowang/SoGCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7861
    - null
    - null
    - null
    metric_stds:
    - 0.0042
    - null
    - null
    - null
  - model: GREAD-Exp
    model_plain: GREAD-Exp
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.7861
    - null
    - null
    - null
    metric_stds:
    - 0.0068
    - null
    - null
    - null
  - model: Graph-MLP
    model_plain: Graph-MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2409.05573'
    title: Learning to Model Graph Structural Information on MLPs via Graph Structure
      Self-Contrasting
    date: Sep 9, 2024
    date_iso: '2024-09-09'
    date_display: Sep 2024
    codebase_url: https://github.com/LirongWu/GSSC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.785
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: GeniePath-BS
    model_plain: GeniePath-BS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.316754
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.03509'
    title: 'Masked Label Prediction: Unified Message Passing Model for Semi-Supervised
      Classification'
    date: Sep 8, 2020
    date_iso: '2020-09-08'
    date_display: Sep 2020
    codebase_url: ''
    published_conference: IJCAI 2020
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7825
    - null
    - null
    - null
    metric_stds:
    - 0.0035
    - null
    - null
    - null
  - model: GaAN
    model_plain: GaAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.03509'
    title: 'Masked Label Prediction: Unified Message Passing Model for Semi-Supervised
      Classification'
    date: Sep 8, 2020
    date_iso: '2020-09-08'
    date_display: Sep 2020
    codebase_url: ''
    published_conference: IJCAI 2020
    published_conference_short: IJCAI
    published_conference_slug: ijcai
    published_venue: IJCAI 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7803
    - null
    - null
    - null
    metric_stds:
    - 0.0073
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
    - 0.7784
    - null
    - null
    - null
    metric_stds:
    - 0.0056
    - null
    - null
    - null
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.07141'
    title: 'SoGCN: Second-Order Graph Convolutional Networks'
    date: Oct 14, 2021
    date_iso: '2021-10-14'
    date_display: Oct 2021
    codebase_url: https://github.com/yuehaowang/SoGCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7753
    - null
    - null
    - null
    metric_stds:
    - 0.003
    - null
    - null
    - null
  - model: GraphSAGE +CAP
    model_plain: GraphSAGE +CAP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.14855'
    title: 'CAP: Co-Adversarial Perturbation on Weights and Features for Improving
      Generalization of Graph Neural Networks'
    date: Oct 28, 2021
    date_iso: '2021-10-28'
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
    - 0.7753
    - null
    - null
    - null
    metric_stds:
    - 0.007
    - null
    - null
    - null
  - model: NodeFormer
    model_plain: NodeFormer
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
    - 0.7745
    - null
    - null
    - null
    metric_stds:
    - 0.0115
    - null
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
    - 0.7725
    - null
    - null
    - null
    metric_stds:
    - 0.0042
    - null
    - null
    - null
  - model: LinkDist
    model_plain: LinkDist
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2409.05573'
    title: Learning to Model Graph Structural Information on MLPs via Graph Structure
      Self-Contrasting
    date: Sep 9, 2024
    date_iso: '2024-09-09'
    date_display: Sep 2024
    codebase_url: https://github.com/LirongWu/GSSC
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.772
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
  - model: CGNN
    model_plain: CGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.7712
    - null
    - null
    - null
    metric_stds:
    - 0.0061
    - null
    - null
    - null
  - model: GraphSAGE + Vanilla
    model_plain: GraphSAGE + Vanilla
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.14855'
    title: 'CAP: Co-Adversarial Perturbation on Weights and Features for Improving
      Generalization of Graph Neural Networks'
    date: Oct 28, 2021
    date_iso: '2021-10-28'
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
    - 0.7691
    - null
    - null
    - null
    metric_stds:
    - 0.0102
    - null
    - null
    - null
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.07141'
    title: 'SoGCN: Second-Order Graph Convolutional Networks'
    date: Oct 14, 2021
    date_iso: '2021-10-14'
    date_display: Oct 2021
    codebase_url: https://github.com/yuehaowang/SoGCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7677
    - null
    - null
    - null
    metric_stds:
    - 0.002
    - null
    - null
    - null
  row_count: 101
  rows_json: /data/datasets/ogbn-proteins/standard-split-rows.json
  chart_json: /data/datasets/ogbn-proteins/standard-split-chart.json
  arch_counts:
    gnn: 70
    hybrid: 12
    graph_transformer: 7
    llm: 0
    walk: 0
    traditional: 11
  metric_counts:
  - 74
  - 19
  - 2
  - 8
  milestones: &id001
  - value: 0.8226
    std: 0.0093
    model: NodeNorm
    arxiv_id: '2006.07107'
    title: Understanding and Resolving Performance Degradation in Deep Graph Convolutional
      Networks
    date: '2020-06-12'
  - value: 0.8642
    std: 0.0008
    model: UniMP
    arxiv_id: '2009.03509'
    title: 'Masked Label Prediction: Unified Message Passing Model for Semi-Supervised
      Classification'
    date: '2020-09-08'
  - value: 0.8942
    std: 0.0007
    model: LD
    arxiv_id: '2309.14907'
    title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
      Graphs against Learning Bias
    date: '2023-09-26'
  milestones_by_metric:
    ROC-AUC: *id001
    Accuracy:
    - value: 0.9464
      std: 0.002
      model: SGCL-T
      arxiv_id: '2402.15270'
      title: Smoothed Graph Contrastive Learning via Seamless Proximity Integration
      date: '2024-02-23'
    F1-macro:
    - value: 0.0747
      std: null
      model: GCond
      arxiv_id: '2412.17961'
      title: 'Extending Graph Condensation to Multi-Label Datasets: A Benchmark Study'
      date: '2024-12-23'
    F1-micro:
    - value: 0.3104
      std: null
      model: Coreset (K-Center)
      arxiv_id: '2412.17961'
      title: 'Extending Graph Condensation to Multi-Label Datasets: A Benchmark Study'
      date: '2024-12-23'
---

