---
title: ogbl-collab
slug: ogbl-collab
benchmark: OGB
task_type: link_prediction
description: Link prediction on academic collaboration network (author co-authorship).
primary_metric: Hits@50
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.OGBLinkPropPredDataset.html
stats:
  num_graphs: 235868
  avg_nodes: 1285465.0
  avg_edges: null
  num_classes: null
result_count: 163
best_model:
  model: PROXI
  value: 0.765
  metric: Hits@50
  arxiv_id: '2410.01802'
  paper_title: 'PROXI: Challenging the GNNs for Link Prediction'
papers:
- arxiv_id: '2508.17630'
  title: 'Quantum Graph Attention Network: A Novel Quantum Multi-Head Attention Mechanism
    for Graph Learning'
  date_iso: '2025-08-25'
  venue: ''
- arxiv_id: '2506.24018'
  title: Bridging Theory and Practice in Link Representation with Graph Neural Networks
  date_iso: '2025-06-30'
  venue: NeurIPS 2025
- arxiv_id: '2504.06193'
  title: 'Weak Models Can be Good Teachers: A Case Study on Link Prediction with MLPs'
  date_iso: '2025-04-08'
  venue: ''
- arxiv_id: '2501.18739'
  title: 'Beyond Message Passing: Neural Graph Pattern Machine'
  date_iso: '2025-01-30'
  venue: ICML 2025
- arxiv_id: '2411.03845'
  title: Reconsidering the Performance of GAE in Link Prediction
  date_iso: '2024-11-06'
  venue: ''
- arxiv_id: '2410.01802'
  title: 'PROXI: Challenging the GNNs for Link Prediction'
  date_iso: '2024-10-02'
  venue: TMLR 2024
- arxiv_id: '2409.17475'
  title: On the Impact of Feature Heterophily on Link Prediction with Graph Neural
    Networks
  date_iso: '2024-09-26'
  venue: NeurIPS 2024
- arxiv_id: '2406.16687'
  title: Link Prediction with Untrained Message Passing Layers
  date_iso: '2024-06-24'
  venue: ''
- arxiv_id: '2310.11009'
  title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
  date_iso: '2023-10-17'
  venue: KDD 2023
- arxiv_id: '2310.09516'
  title: Efficient Link Prediction via GNN Layers Induced by Negative Sampling
  date_iso: '2023-10-14'
  venue: ''
- arxiv_id: '2305.19903'
  title: Improving Expressivity of GNNs with Subgraph-specific Factor Embedded Normalization
  date_iso: '2023-05-31'
  venue: KDD 2023
- arxiv_id: '2303.00170'
  title: Asymmetric Learning for Graph Neural Network based Link Prediction
  date_iso: '2023-03-01'
  venue: ''
- arxiv_id: '2003.00982'
  title: GNNBenchmark
  date_iso: '2023-01-01'
  venue: JMLR 2023
- arxiv_id: '2212.12488'
  title: 'Bring Your Own View: Graph Neural Networks for Link Prediction with Personalized
    Subgraph Selection'
  date_iso: '2022-12-23'
  venue: ''
- arxiv_id: '2210.02636'
  title: Geodesic Graph Neural Network for Efficient Graph Representation Learning
  date_iso: '2022-10-06'
  venue: NeurIPS 2022
- arxiv_id: '2210.01301'
  title: 'GIDN: A Lightweight Graph Inception Diffusion Network for High-efficient
    Link Prediction'
  date_iso: '2022-10-04'
  venue: ''
- arxiv_id: '2206.04216'
  title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks for Link Prediction'
  date_iso: '2022-06-09'
  venue: NeurIPS 2022
- arxiv_id: '2203.00199'
  title: Equivariant and Stable Positional Encoding for More Powerful Graph Neural
    Networks
  date_iso: '2022-03-01'
  venue: ICLR 2022
- arxiv_id: '2202.13538'
  title: Algorithm and System Co-design for Efficient Subgraph-based Graph Representation
    Learning
  date_iso: '2022-02-28'
  venue: ''
- arxiv_id: '2201.07858'
  title: Decoupling the Depth and Scope of Graph Neural Networks
  date_iso: '2022-01-19'
  venue: NeurIPS 2022
- arxiv_id: '2201.02534'
  title: 'MGAE: Masked Autoencoders for Self-Supervised Learning on Graphs'
  date_iso: '2022-01-07'
  venue: ''
- arxiv_id: '2112.02936'
  title: Pairwise Learning for Neural Link Prediction
  date_iso: '2021-12-06'
  venue: ''
- arxiv_id: '2110.14363'
  title: 'VQ-GNN: A Universal Framework to Scale-up Graph Neural Networks using Vector
    Quantization'
  date_iso: '2021-10-27'
  venue: NeurIPS 2021
- arxiv_id: '2010.16103'
  title: 'Labeling Trick: A Theory of Using Graph Neural Networks for Multi-Node Representation
    Learning'
  date_iso: '2020-10-30'
  venue: NeurIPS 2020
- arxiv_id: '2006.07846'
  title: Formatting Instructions for ICLR 2021 Conference Submissions
  date_iso: '2020-06-14'
  venue: ''
- arxiv_id: '2005.00687'
  title: OGB
  date_iso: '2020-05-02'
  venue: NeurIPS 2020
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Hits@50
  default_metric: Hits@50
  higher_is_better: true
  stats:
    num_graphs: 235868
    avg_nodes: 1285465.0
    avg_edges: null
    num_classes: null
  metrics:
  - Hits@50
  - MRR
  metric_display_names:
  - Hits@50
  - MRR
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: PROXI
    model_plain: PROXI
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2410.01802'
    title: 'PROXI: Challenging the GNNs for Link Prediction'
    date: Oct 2, 2024
    date_iso: '2024-10-02'
    date_display: Oct 2024
    codebase_url: https://github.com/workrep20232/PROXI
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.765
    - null
    metric_stds:
    - 0.0027
    - null
  - model: OGB Leader
    model_plain: OGB Leader
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2410.01802'
    title: 'PROXI: Challenging the GNNs for Link Prediction'
    date: Oct 2, 2024
    date_iso: '2024-10-02'
    date_display: Oct 2024
    codebase_url: https://github.com/workrep20232/PROXI
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7129
    - null
    metric_stds:
    - 0.0018
    - null
  - model: GIDN
    model_plain: GIDN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.01301'
    title: 'GIDN: A Lightweight Graph Inception Diffusion Network for High-efficient
      Link Prediction'
    date: Oct 4, 2022
    date_iso: '2022-10-04'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7096
    - null
    metric_stds:
    - 0.0055
    - null
  - model: PLNLP
    model_plain: PLNLP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.02936'
    title: Pairwise Learning for Neural Link Prediction
    date: Dec 6, 2021
    date_iso: '2021-12-06'
    date_display: Dec 2021
    codebase_url: https://github.com/zhitao-wang/PLNLP
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7059
    - null
    metric_stds:
    - 0.0029
    - null
  - model: HOP-Rec
    model_plain: HOP-Rec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2112.02936'
    title: Pairwise Learning for Neural Link Prediction
    date: Dec 6, 2021
    date_iso: '2021-12-06'
    date_display: Dec 2021
    codebase_url: https://github.com/zhitao-wang/PLNLP
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7012
    - null
    metric_stds:
    - 0.0016
    - null
  - model: LPFormer
    model_plain: LPFormer
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.11009'
    title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    date: Oct 17, 2023
    date_iso: '2023-10-17'
    date_display: Oct 2023
    codebase_url: https://github.com/HarryShomer/LPFormer
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6814
    - null
    metric_stds:
    - 0.0051
    - null
  - model: MPLP
    model_plain: MPLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.03845'
    title: Reconsidering the Performance of GAE in Link Prediction
    date: Nov 6, 2024
    date_iso: '2024-11-06'
    date_display: Nov 2024
    codebase_url: https://github.com/GraphPKU/Refined-GAE
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6699
    - null
    metric_stds:
    - 0.004
    - null
  - model: SIGN
    model_plain: SIGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2409.17475'
    title: On the Impact of Feature Heterophily on Link Prediction with Graph Neural
      Networks
    date: Sep 26, 2024
    date_iso: '2024-09-26'
    date_display: Sep 2024
    codebase_url: https://github.com/tensor-gales/HeteLinkPred
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6664
    - null
    metric_stds:
    - 0.0064
    - null
  - model: NCNC
    model_plain: NCNC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11009'
    title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    date: Oct 17, 2023
    date_iso: '2023-10-17'
    date_display: Oct 2023
    codebase_url: https://github.com/HarryShomer/LPFormer
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6661
    - null
    metric_stds:
    - 0.0071
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
    arxiv_id: '2409.17475'
    title: On the Impact of Feature Heterophily on Link Prediction with Graph Neural
      Networks
    date: Sep 26, 2024
    date_iso: '2024-09-26'
    date_display: Sep 2024
    codebase_url: https://github.com/tensor-gales/HeteLinkPred
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6621
    - null
    metric_stds:
    - 0.0033
    - null
  - model: Neo-GNN
    model_plain: Neo-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.01802'
    title: 'PROXI: Challenging the GNNs for Link Prediction'
    date: Oct 2, 2024
    date_iso: '2024-10-02'
    date_display: Oct 2024
    codebase_url: https://github.com/workrep20232/PROXI
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6613
    - null
    metric_stds:
    - 0.0061
    - null
  - model: Optimized GAE
    model_plain: Optimized GAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.03845'
    title: Reconsidering the Performance of GAE in Link Prediction
    date: Nov 6, 2024
    date_iso: '2024-11-06'
    date_display: Nov 2024
    codebase_url: https://github.com/GraphPKU/Refined-GAE
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6611
    - null
    metric_stds:
    - 0.0035
    - null
  - model: YinYanGNN
    model_plain: YinYanGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.09516'
    title: Efficient Link Prediction via GNN Layers Induced by Negative Sampling
    date: Oct 14, 2023
    date_iso: '2023-10-14'
    date_display: Oct 2023
    codebase_url: https://github.com/yxzwang/SubmissionverOfYinYanGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.661
    - null
    metric_stds:
    - 0.002
    - null
  - model: NoFeat
    model_plain: NoFeat
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2409.17475'
    title: On the Impact of Feature Heterophily on Link Prediction with Graph Neural
      Networks
    date: Sep 26, 2024
    date_iso: '2024-09-26'
    date_display: Sep 2024
    codebase_url: https://github.com/tensor-gales/HeteLinkPred
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6606
    - null
    metric_stds:
    - 0.0022
    - null
  - model: BUDDY
    model_plain: BUDDY
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.09516'
    title: Efficient Link Prediction via GNN Layers Induced by Negative Sampling
    date: Oct 14, 2023
    date_iso: '2023-10-14'
    date_display: Oct 2023
    codebase_url: https://github.com/yxzwang/SubmissionverOfYinYanGNN
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
    metric_stds:
    - 0.0058
    - null
  - model: NCNC (GIN)
    model_plain: NCNC (GIN)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.16687'
    title: Link Prediction with Untrained Message Passing Layers
    date: Jun 24, 2024
    date_iso: '2024-06-24'
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
    - 0.6587
    - null
    metric_stds:
    - 0.0074
    - null
  - model: AA+Proposal Set
    model_plain: AA+Proposal Set
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2112.02936'
    title: Pairwise Learning for Neural Link Prediction
    date: Dec 6, 2021
    date_iso: '2021-12-06'
    date_display: Dec 2021
    codebase_url: https://github.com/zhitao-wang/PLNLP
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6548
    - null
    metric_stds:
    - 0.0
    - null
  - model: SNCNC (SGCN)
    model_plain: SNCNC (SGCN)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.16687'
    title: Link Prediction with Untrained Message Passing Layers
    date: Jun 24, 2024
    date_iso: '2024-06-24'
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
    - 0.654
    - null
    metric_stds:
    - 0.0046
    - null
  - model: SEAL-PS2
    model_plain: SEAL-PS2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.12488'
    title: 'Bring Your Own View: Graph Neural Networks for Link Prediction with Personalized
      Subgraph Selection'
    date: Dec 23, 2022
    date_iso: '2022-12-23'
    date_display: Dec 2022
    codebase_url: https://github.com/qiaoyu-tan/PS2
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6483
    - null
    metric_stds:
    - 0.0054
    - null
  - model: NCN
    model_plain: NCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11009'
    title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
    date: Oct 17, 2023
    date_iso: '2023-10-17'
    date_display: Oct 2023
    codebase_url: https://github.com/HarryShomer/LPFormer
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6476
    - null
    metric_stds:
    - 0.0087
    - null
  - model: SEAL
    model_plain: SEAL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2010.16103'
    title: 'Labeling Trick: A Theory of Using Graph Neural Networks for Multi-Node
      Representation Learning'
    date: Oct 30, 2020
    date_iso: '2020-10-30'
    date_display: Oct 2020
    codebase_url: https://github.com/facebookresearch/SEAL_OGB
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6474
    - null
    metric_stds:
    - 0.0043
    - null
  - model: BUDDY
    model_plain: BUDDY
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2410.01802'
    title: 'PROXI: Challenging the GNNs for Link Prediction'
    date: Oct 2, 2024
    date_iso: '2024-10-02'
    date_display: Oct 2024
    codebase_url: https://github.com/workrep20232/PROXI
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6459
    - null
    metric_stds:
    - 0.0046
    - null
  - model: GCN+DE
    model_plain: GCN+DE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2010.16103'
    title: 'Labeling Trick: A Theory of Using Graph Neural Networks for Multi-Node
      Representation Learning'
    date: Oct 30, 2020
    date_iso: '2020-10-30'
    date_display: Oct 2020
    codebase_url: https://github.com/facebookresearch/SEAL_OGB
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6444
    - null
    metric_stds:
    - 0.0029
    - null
  - model: GCN+DRNL
    model_plain: GCN+DRNL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2010.16103'
    title: 'Labeling Trick: A Theory of Using Graph Neural Networks for Multi-Node
      Representation Learning'
    date: Oct 30, 2020
    date_iso: '2020-10-30'
    date_display: Oct 2020
    codebase_url: https://github.com/facebookresearch/SEAL_OGB
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.644
    - null
    metric_stds:
    - 0.0045
    - null
  - model: AA
    model_plain: AA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.09516'
    title: Efficient Link Prediction via GNN Layers Induced by Negative Sampling
    date: Oct 14, 2023
    date_iso: '2023-10-14'
    date_display: Oct 2023
    codebase_url: https://github.com/yxzwang/SubmissionverOfYinYanGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6435
    - null
    metric_stds:
    - 0.0
    - null
  - model: AA
    model_plain: AA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2010.16103'
    title: 'Labeling Trick: A Theory of Using Graph Neural Networks for Multi-Node
      Representation Learning'
    date: Oct 30, 2020
    date_iso: '2020-10-30'
    date_display: Oct 2020
    codebase_url: https://github.com/facebookresearch/SEAL_OGB
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6417
    - null
    metric_stds:
    - 0.0
    - null
  - model: RA
    model_plain: RA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.09516'
    title: Efficient Link Prediction via GNN Layers Induced by Negative Sampling
    date: Oct 14, 2023
    date_iso: '2023-10-14'
    date_display: Oct 2023
    codebase_url: https://github.com/yxzwang/SubmissionverOfYinYanGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.64
    - null
    metric_stds:
    - 0.0
    - null
  - model: RA
    model_plain: RA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2504.06193'
    title: 'Weak Models Can be Good Teachers: A Case Study on Link Prediction with
      MLPs'
    date: Apr 8, 2025
    date_iso: '2025-04-08'
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
    - 0.6381
    - null
    metric_stds:
    - 0.0
    - null
  - model: SEAL
    model_plain: SEAL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2410.01802'
    title: 'PROXI: Challenging the GNNs for Link Prediction'
    date: Oct 2, 2024
    date_iso: '2024-10-02'
    date_display: Oct 2024
    codebase_url: https://github.com/workrep20232/PROXI
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6337
    - null
    metric_stds:
    - 0.0069
    - null
  - model: SUREL
    model_plain: SUREL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.13538'
    title: Algorithm and System Co-design for Efficient Subgraph-based Graph Representation
      Learning
    date: Feb 28, 2022
    date_iso: '2022-02-28'
    date_display: Feb 2022
    codebase_url: https://github.com/Graph-COM/SUREL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6334
    - null
    metric_stds:
    - 0.0052
    - null
  - model: CN
    model_plain: CN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2010.16103'
    title: 'Labeling Trick: A Theory of Using Graph Neural Networks for Multi-Node
      Representation Learning'
    date: Oct 30, 2020
    date_iso: '2020-10-30'
    date_display: Oct 2020
    codebase_url: https://github.com/facebookresearch/SEAL_OGB
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6137
    - null
    metric_stds:
    - 0.0
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
    arxiv_id: '2410.01802'
    title: 'PROXI: Challenging the GNNs for Link Prediction'
    date: Oct 2, 2024
    date_iso: '2024-10-02'
    date_display: Oct 2024
    codebase_url: https://github.com/workrep20232/PROXI
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5944
    - null
    metric_stds:
    - 0.0137
    - null
  - model: Best GNN
    model_plain: Best GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.06193'
    title: 'Weak Models Can be Good Teachers: A Case Study on Link Prediction with
      MLPs'
    date: Apr 8, 2025
    date_iso: '2025-04-08'
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
    - 0.5914
    - null
    metric_stds:
    - 0.0164
    - null
  - model: DE-GNN
    model_plain: DE-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2303.00170'
    title: Asymmetric Learning for Graph Neural Network based Link Prediction
    date: Mar 1, 2023
    date_iso: '2023-03-01'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5787
    - null
    metric_stds:
    - 0.0079
    - null
  - model: AML
    model_plain: AML
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2303.00170'
    title: Asymmetric Learning for Graph Neural Network based Link Prediction
    date: Mar 1, 2023
    date_iso: '2023-03-01'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.576
    - null
    metric_stds:
    - 0.0071
    - null
  - model: SEAL
    model_plain: SEAL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2303.00170'
    title: Asymmetric Learning for Graph Neural Network based Link Prediction
    date: Mar 1, 2023
    date_iso: '2023-03-01'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5755
    - null
    metric_stds:
    - 0.0072
    - null
  - model: Neo-GNN
    model_plain: Neo-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.04216'
    title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks for Link Prediction'
    date: Jun 9, 2022
    date_iso: '2022-06-09'
    date_display: Jun 2022
    codebase_url: https://github.com/seongjunyun/Neo_GNNs
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5752
    - null
    metric_stds:
    - 0.0037
    - null
  - model: AA
    model_plain: AA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2303.00170'
    title: Asymmetric Learning for Graph Neural Network based Link Prediction
    date: Mar 1, 2023
    date_iso: '2023-03-01'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5649
    - null
    metric_stds:
    - 0.0
    - null
  - model: CN
    model_plain: CN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.09516'
    title: Efficient Link Prediction via GNN Layers Induced by Negative Sampling
    date: Oct 14, 2023
    date_iso: '2023-10-14'
    date_display: Oct 2023
    codebase_url: https://github.com/yxzwang/SubmissionverOfYinYanGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5644
    - null
    metric_stds:
    - 0.0
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
    arxiv_id: '2303.00170'
    title: Asymmetric Learning for Graph Neural Network based Link Prediction
    date: Mar 1, 2023
    date_iso: '2023-03-01'
    date_display: Mar 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5643
    - null
    metric_stds:
    - 0.0086
    - null
  - model: GraphSage-PS2
    model_plain: GraphSage-PS2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.12488'
    title: 'Bring Your Own View: Graph Neural Networks for Link Prediction with Personalized
      Subgraph Selection'
    date: Dec 23, 2022
    date_iso: '2022-12-23'
    date_display: Dec 2022
    codebase_url: https://github.com/qiaoyu-tan/PS2
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5571
    - null
    metric_stds:
    - 0.0093
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
    arxiv_id: '2406.16687'
    title: Link Prediction with Untrained Message Passing Layers
    date: Jun 24, 2024
    date_iso: '2024-06-24'
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
    - 0.5558
    - null
    metric_stds:
    - 0.0384
    - null
  - model: shaDow-SAGE
    model_plain: shaDow-SAGE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2201.07858'
    title: Decoupling the Depth and Scope of Graph Neural Networks
    date: Jan 19, 2022
    date_iso: '2022-01-19'
    date_display: Jan 2022
    codebase_url: https://github.com/facebookresearch/shaDow_GNN
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5492
    - null
    metric_stds:
    - 0.0022
    - null
  - model: GDGNN
    model_plain: GDGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.09516'
    title: Efficient Link Prediction via GNN Layers Induced by Negative Sampling
    date: Oct 14, 2023
    date_iso: '2023-10-14'
    date_display: Oct 2023
    codebase_url: https://github.com/yxzwang/SubmissionverOfYinYanGNN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5474
    - null
    metric_stds:
    - 0.0048
    - null
  - model: GDGNN-Vert
    model_plain: GDGNN-Vert
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.02636'
    title: Geodesic Graph Neural Network for Efficient Graph Representation Learning
    date: Oct 6, 2022
    date_iso: '2022-10-06'
    date_display: Oct 2022
    codebase_url: https://github.com/woodcutter1998/gdgnn
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5474
    - null
    metric_stds:
    - 0.0048
    - null
  - model: MGAE-GCN
    model_plain: MGAE-GCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2201.02534'
    title: 'MGAE: Masked Autoencoders for Self-Supervised Learning on Graphs'
    date: Jan 7, 2022
    date_iso: '2022-01-07'
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
    - 0.5474
    - null
    metric_stds:
    - 0.0106
    - null
  - model: SEAL
    model_plain: SEAL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2203.00199'
    title: Equivariant and Stable Positional Encoding for More Powerful Graph Neural
      Networks
    date: Mar 1, 2022
    date_iso: '2022-03-01'
    date_display: Mar 2022
    codebase_url: https://github.com/Graph-COM/PEG
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5471
    - null
    metric_stds:
    - 0.0001
    - null
  - model: GAE(SAGE)
    model_plain: GAE(SAGE)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.03845'
    title: Reconsidering the Performance of GAE in Link Prediction
    date: Nov 6, 2024
    date_iso: '2024-11-06'
    date_display: Nov 2024
    codebase_url: https://github.com/GraphPKU/Refined-GAE
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5463
    - null
    metric_stds:
    - 0.0112
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
    arxiv_id: '2112.02936'
    title: Pairwise Learning for Neural Link Prediction
    date: Dec 6, 2021
    date_iso: '2021-12-06'
    date_display: Dec 2021
    codebase_url: https://github.com/zhitao-wang/PLNLP
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5463
    - null
    metric_stds:
    - 0.0112
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
    arxiv_id: '2005.00687'
    title: OGB
    date: May 2, 2020
    date_iso: '2020-05-02'
    date_display: May 2020
    codebase_url: https://github.com/snap-stanford/ogb
    published_conference: NeurIPS 2020
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2020
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5463
    - null
    metric_stds:
    - 0.0112
    - null
  row_count: 163
  rows_json: /data/datasets/ogbl-collab/standard-split-rows.json
  chart_json: /data/datasets/ogbl-collab/standard-split-chart.json
  arch_counts:
    gnn: 86
    hybrid: 18
    graph_transformer: 4
    llm: 0
    walk: 8
    traditional: 45
  metric_counts:
  - 155
  - 8
  milestones: &id001
  - value: 0.522
    std: 0.007
    model: LRGA+GCN
    arxiv_id: '2006.07846'
    title: Formatting Instructions for ICLR 2021 Conference Submissions
    date: '2020-06-14'
  - value: 0.6474
    std: 0.0043
    model: SEAL
    arxiv_id: '2010.16103'
    title: 'Labeling Trick: A Theory of Using Graph Neural Networks for Multi-Node
      Representation Learning'
    date: '2020-10-30'
  - value: 0.7059
    std: 0.0029
    model: PLNLP
    arxiv_id: '2112.02936'
    title: Pairwise Learning for Neural Link Prediction
    date: '2021-12-06'
  - value: 0.7096
    std: 0.0055
    model: GIDN
    arxiv_id: '2210.01301'
    title: 'GIDN: A Lightweight Graph Inception Diffusion Network for High-efficient
      Link Prediction'
    date: '2022-10-04'
  - value: 0.765
    std: 0.0027
    model: PROXI
    arxiv_id: '2410.01802'
    title: 'PROXI: Challenging the GNNs for Link Prediction'
    date: '2024-10-02'
  milestones_by_metric:
    Hits@50: *id001
    MRR:
    - value: 0.0643
      std: null
      model: SEAL
      arxiv_id: '2506.24018'
      title: Bridging Theory and Practice in Link Representation with Graph Neural
        Networks
      date: '2025-06-30'
---

