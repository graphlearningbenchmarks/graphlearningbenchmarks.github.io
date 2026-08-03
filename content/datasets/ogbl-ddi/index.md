---
title: ogbl-ddi
slug: ogbl-ddi
benchmark: OGB
task_type: link_prediction
description: Drug-drug interaction link prediction (binary, homogeneous graph).
primary_metric: Hits@20
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.OGBLinkPropPredDataset.html
stats:
  num_graphs: 4267
  avg_nodes: 1334889.0
  avg_edges: null
  num_classes: null
result_count: 138
best_model:
  model: ELGNN
  value: 0.9777
  metric: Hits@20
  arxiv_id: '2310.14166'
  paper_title: Ensemble Learning for Graph Neural Networks
papers:
- arxiv_id: '2506.24018'
  title: Bridging Theory and Practice in Link Representation with Graph Neural Networks
  date_iso: '2025-06-30'
  venue: NeurIPS 2025
- arxiv_id: '2502.02479'
  title: Using Random Noise Equivariantly to Boost Graph Neural Networks Universally
  date_iso: '2025-02-04'
  venue: ''
- arxiv_id: '2411.03845'
  title: Reconsidering the Performance of GAE in Link Prediction
  date_iso: '2024-11-06'
  venue: ''
- arxiv_id: '2411.01410'
  title: PageRank Bandits for Link Prediction
  date_iso: '2024-11-03'
  venue: NeurIPS 2024
- arxiv_id: '2406.16687'
  title: Link Prediction with Untrained Message Passing Layers
  date_iso: '2024-06-24'
  venue: ''
- arxiv_id: '2403.01121'
  title: 'OpenGraph: Towards Open Graph Foundation Models'
  date_iso: '2024-03-02'
  venue: ''
- arxiv_id: '2310.14166'
  title: Ensemble Learning for Graph Neural Networks
  date_iso: '2023-10-22'
  venue: ''
- arxiv_id: '2310.09516'
  title: Efficient Link Prediction via GNN Layers Induced by Negative Sampling
  date_iso: '2023-10-14'
  venue: ''
- arxiv_id: '2310.00793'
  title: 'Revisiting Link Prediction: a data perspective'
  date_iso: '2023-10-01'
  venue: ICLR 2023
- arxiv_id: '2304.10074'
  title: Improving Graph Neural Networks on Multi-node Tasks with the Labeling Trick
  date_iso: '2023-04-20'
  venue: JMLR 2023
- arxiv_id: '2304.02806'
  title: 'Graph Mixture of Experts: Learning on Large-Scale Graphs with Explicit Diversity
    Modeling'
  date_iso: '2023-04-06'
  venue: NeurIPS 2023
- arxiv_id: '2301.12562'
  title: Simplifying Subgraph Representation Learning for Scalable Link Prediction
  date_iso: '2023-01-29'
  venue: ''
- arxiv_id: '2212.12488'
  title: 'Bring Your Own View: Graph Neural Networks for Link Prediction with Personalized
    Subgraph Selection'
  date_iso: '2022-12-23'
  venue: ''
- arxiv_id: '2209.15486'
  title: Graph Neural Networks for Link Prediction with Subgraph Sketching
  date_iso: '2022-09-30'
  venue: ICLR 2022
- arxiv_id: '2206.04216'
  title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks for Link Prediction'
  date_iso: '2022-06-09'
  venue: NeurIPS 2022
- arxiv_id: '2203.00199'
  title: Equivariant and Stable Positional Encoding for More Powerful Graph Neural
    Networks
  date_iso: '2022-03-01'
  venue: ICLR 2022
- arxiv_id: '2201.02534'
  title: 'MGAE: Masked Autoencoders for Self-Supervised Learning on Graphs'
  date_iso: '2022-01-07'
  venue: ''
- arxiv_id: '2112.02936'
  title: Pairwise Learning for Neural Link Prediction
  date_iso: '2021-12-06'
  venue: ''
- arxiv_id: '2106.02172'
  title: Learning from Counterfactual Links for Link Prediction
  date_iso: '2021-06-03'
  venue: ICML 2021
- arxiv_id: '2012.15024'
  title: Adaptive Graph Diffusion Networks
  date_iso: '2020-12-30'
  venue: ''
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
  primary_metric: Hits@20
  default_metric: Hits@20
  higher_is_better: true
  stats:
    num_graphs: 4267
    avg_nodes: 1334889.0
    avg_edges: null
    num_classes: null
  metrics:
  - Hits@20
  - MRR
  - Recall@20
  metric_display_names:
  - Hits@20
  - MRR
  - Recall@20
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: ELGNN
    model_plain: ELGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.14166'
    title: Ensemble Learning for Graph Neural Networks
    date: Oct 22, 2023
    date_iso: '2023-10-22'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9777
    - null
    - null
    metric_stds:
    - 0.0037
    - null
    - null
  - model: GIDN
    model_plain: GIDN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.14166'
    title: Ensemble Learning for Graph Neural Networks
    date: Oct 22, 2023
    date_iso: '2023-10-22'
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
    - 0.9542
    - null
    - null
    metric_stds:
    - 0.0
    - null
    - null
  - model: AGDN
    model_plain: AGDN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.14166'
    title: Ensemble Learning for Graph Neural Networks
    date: Oct 22, 2023
    date_iso: '2023-10-22'
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
    - 0.9538
    - null
    - null
    metric_stds:
    - 0.0094
    - null
    - null
  - model: MPNNs
    model_plain: MPNNs
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.15024'
    title: Adaptive Graph Diffusion Networks
    date: Dec 30, 2020
    date_iso: '2020-12-30'
    date_display: Dec 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9538
    - null
    - null
    metric_stds:
    - 0.0094
    - null
    - null
  - model: MPNN
    model_plain: MPNN
    is_baseline: false
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
    - 0.9443
    - null
    - null
    metric_stds:
    - 0.0057
    - null
    - null
  - model: PSG
    model_plain: PSG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.14166'
    title: Ensemble Learning for Graph Neural Networks
    date: Oct 22, 2023
    date_iso: '2023-10-22'
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
    - 0.9284
    - null
    - null
    metric_stds:
    - 0.0047
    - null
    - null
  - model: PLNLP
    model_plain: PLNLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2012.15024'
    title: Adaptive Graph Diffusion Networks
    date: Dec 30, 2020
    date_iso: '2020-12-30'
    date_display: Dec 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9088
    - null
    - null
    metric_stds:
    - 0.0313
    - null
    - null
  - model: SUREL
    model_plain: SUREL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.8974
    - null
    - null
    metric_stds:
    - 0.0018
    - null
    - null
  - model: PRB
    model_plain: PRB
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.01410'
    title: PageRank Bandits for Link Prediction
    date: Nov 3, 2024
    date_iso: '2024-11-03'
    date_display: Nov 2024
    codebase_url: https://github.com/jiaruzouu/PRB
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8831
    - null
    - null
    metric_stds:
    - 0.0436
    - null
    - null
  - model: SAGE+Edge Attr
    model_plain: SAGE+Edge Attr
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
    - 0.8781
    - null
    - null
    metric_stds:
    - 0.0447
    - null
    - null
  - model: GraphSAGE + Edge Attr
    model_plain: GraphSAGE + Edge Attr
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.14166'
    title: Ensemble Learning for Graph Neural Networks
    date: Oct 22, 2023
    date_iso: '2023-10-22'
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
    - 0.8781
    - null
    - null
    metric_stds:
    - 0.0474
    - null
    - null
  - model: CFLP (w/ JKNet)
    model_plain: CFLP (w/ JKNet)
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
    - 0.8608
    - null
    - null
    metric_stds:
    - 0.0198
    - null
    - null
  - model: CFLP w/ JKNet
    model_plain: CFLP w/ JKNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2106.02172'
    title: Learning from Counterfactual Links for Link Prediction
    date: Jun 3, 2021
    date_iso: '2021-06-03'
    date_display: Jun 2021
    codebase_url: https://github.com/DM2-ND/CFLP
    published_conference: ICML 2021
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2021
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8608
    - null
    - null
    metric_stds:
    - 0.0198
    - null
    - null
  - model: ELPH
    model_plain: ELPH
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2209.15486'
    title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    date: Sep 30, 2022
    date_iso: '2022-09-30'
    date_display: Sep 2022
    codebase_url: https://github.com/melifluos/subgraph-sketching
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8319
    - null
    - null
    metric_stds:
    - 0.0212
    - null
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
    arxiv_id: '2411.01410'
    title: PageRank Bandits for Link Prediction
    date: Nov 3, 2024
    date_iso: '2024-11-03'
    date_display: Nov 2024
    codebase_url: https://github.com/jiaruzouu/PRB
    published_conference: NeurIPS 2024
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8232
    - null
    - null
    metric_stds:
    - 0.061
    - null
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
    - 0.8092
    - null
    - null
    metric_stds:
    - 0.0335
    - null
    - null
  - model: BUDDY
    model_plain: BUDDY
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2209.15486'
    title: Graph Neural Networks for Link Prediction with Subgraph Sketching
    date: Sep 30, 2022
    date_iso: '2022-09-30'
    date_display: Sep 2022
    codebase_url: https://github.com/melifluos/subgraph-sketching
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7851
    - null
    - null
    metric_stds:
    - 0.0136
    - null
    - null
  - model: ENGNN
    model_plain: ENGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.02479'
    title: Using Random Noise Equivariantly to Boost Graph Neural Networks Universally
    date: Feb 4, 2025
    date_iso: '2025-02-04'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7761
    - null
    - null
    metric_stds:
    - 0.045
    - null
    - null
  - model: CFLP w/ GSAGE
    model_plain: CFLP w/ GSAGE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2106.02172'
    title: Learning from Counterfactual Links for Link Prediction
    date: Jun 3, 2021
    date_iso: '2021-06-03'
    date_display: Jun 2021
    codebase_url: https://github.com/DM2-ND/CFLP
    published_conference: ICML 2021
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2021
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7549
    - null
    - null
    metric_stds:
    - 0.0433
    - null
    - null
  - model: SAGE+Proposal Set
    model_plain: SAGE+Proposal Set
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
    - 0.7495
    - null
    - null
    metric_stds:
    - 0.0317
    - null
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
    arxiv_id: '2310.00793'
    title: 'Revisiting Link Prediction: a data perspective'
    date: Oct 1, 2023
    date_iso: '2023-10-01'
    date_display: Oct 2023
    codebase_url: https://github.com/Juanhui28/HeaRT
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7023
    - null
    - null
    metric_stds:
    - 0.1211
    - null
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
    - 0.6719
    - null
    - null
    metric_stds:
    - 0.0118
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
    - 0.6683
    - null
    - null
    metric_stds:
    - 0.0223
    - null
    - null
  - model: MGAE-SAGE
    model_plain: MGAE-SAGE
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
    - 0.66
    - null
    - null
    metric_stds:
    - 0.0949
    - null
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
    - 0.6591
    - null
    - null
    metric_stds:
    - 0.035
    - null
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
    - 0.6582
    - null
    - null
    metric_stds:
    - 0.0266
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
    - 0.6476
    - null
    - null
    metric_stds:
    - 0.0145
    - null
    - null
  - model: Node2Vec
    model_plain: Node2Vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
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
    - 0.6363
    - null
    - null
    metric_stds:
    - 0.0205
    - null
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
    - 0.6357
    - null
    - null
    metric_stds:
    - 0.0352
    - null
    - null
  - model: GCN+LRGA
    model_plain: GCN+LRGA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.623
    - null
    - null
    metric_stds:
    - 0.0912
    - null
    - null
  - model: LRGA+GCN
    model_plain: LRGA+GCN
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
    - 0.623
    - null
    - null
    metric_stds:
    - 0.091
    - null
    - null
  - model: GCN+JKNet
    model_plain: GCN+JKNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.14166'
    title: Ensemble Learning for Graph Neural Networks
    date: Oct 22, 2023
    date_iso: '2023-10-22'
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
    - 0.6056
    - null
    - null
    metric_stds:
    - 0.0869
    - null
    - null
  - model: JKNet
    model_plain: JKNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.02172'
    title: Learning from Counterfactual Links for Link Prediction
    date: Jun 3, 2021
    date_iso: '2021-06-03'
    date_display: Jun 2021
    codebase_url: https://github.com/DM2-ND/CFLP
    published_conference: ICML 2021
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6056
    - null
    - null
    metric_stds:
    - 0.0869
    - null
    - null
  - model: MF
    model_plain: MF
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
    - 0.595
    - null
    - null
    metric_stds:
    - 0.0168
    - null
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
    - 0.5871
    - null
    - null
    metric_stds:
    - 0.0163
    - null
    - null
  - model: JK-Net
    model_plain: JK-Net
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
    - 0.5798
    - null
    - null
    metric_stds:
    - 0.0688
    - null
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
    - 0.569
    - null
    - null
    metric_stds:
    - 0.0532
    - null
    - null
  - model: GraphConv + GAE
    model_plain: GraphConv + GAE
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
    - 0.5636
    - null
    - null
    metric_stds:
    - 0.0045
    - null
    - null
  - model: PE-SAGE-DW
    model_plain: PE-SAGE-DW
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.5616
    - null
    - null
    metric_stds:
    - 0.055
    - null
    - null
  - model: SNCNC (SGIN)
    model_plain: SNCNC (SGIN)
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
    - 0.5453
    - null
    - null
    metric_stds:
    - 0.1102
    - null
    - null
  - model: GIN + GAE
    model_plain: GIN + GAE
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
    - 0.5421
    - null
    - null
    metric_stds:
    - 0.0095
    - null
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
    - 0.539
    - null
    - null
    metric_stds:
    - 0.0474
    - null
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
    - 0.539
    - null
    - null
    metric_stds:
    - 0.0474
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
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.539
    - null
    - null
    metric_stds:
    - 0.0474
    - null
    - null
  - model: GSAGE
    model_plain: GSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.02172'
    title: Learning from Counterfactual Links for Link Prediction
    date: Jun 3, 2021
    date_iso: '2021-06-03'
    date_display: Jun 2021
    codebase_url: https://github.com/DM2-ND/CFLP
    published_conference: ICML 2021
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2021
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.539
    - null
    - null
    metric_stds:
    - 0.0474
    - null
    - null
  - model: CFLP w/ GCN
    model_plain: CFLP w/ GCN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2106.02172'
    title: Learning from Counterfactual Links for Link Prediction
    date: Jun 3, 2021
    date_iso: '2021-06-03'
    date_display: Jun 2021
    codebase_url: https://github.com/DM2-ND/CFLP
    published_conference: ICML 2021
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2021
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5251
    - null
    - null
    metric_stds:
    - 0.0109
    - null
    - null
  - model: PE-SAGE-LE
    model_plain: PE-SAGE-LE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.5149
    - null
    - null
    metric_stds:
    - 0.0971
    - null
    - null
  - model: PEG
    model_plain: PEG
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
    - 0.5012
    - null
    - null
    metric_stds:
    - 0.0655
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
    arxiv_id: '2310.00793'
    title: 'Revisiting Link Prediction: a data perspective'
    date: Oct 1, 2023
    date_iso: '2023-10-01'
    date_display: Oct 2023
    codebase_url: https://github.com/Juanhui28/HeaRT
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.499
    - null
    - null
    metric_stds:
    - 0.0723
    - null
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
    - 0.4974
    - null
    - null
    metric_stds:
    - 0.0239
    - null
    - null
  row_count: 138
  rows_json: /data/datasets/ogbl-ddi/standard-split-rows.json
  chart_json: /data/datasets/ogbl-ddi/standard-split-chart.json
  arch_counts:
    gnn: 87
    hybrid: 14
    graph_transformer: 1
    llm: 1
    walk: 4
    traditional: 27
  metric_counts:
  - 120
  - 8
  - 10
  milestones: &id001
  - value: 0.623
    std: 0.091
    model: LRGA+GCN
    arxiv_id: '2006.07846'
    title: Formatting Instructions for ICLR 2021 Conference Submissions
    date: '2020-06-14'
  - value: 0.9538
    std: 0.0094
    model: MPNNs
    arxiv_id: '2012.15024'
    title: Adaptive Graph Diffusion Networks
    date: '2020-12-30'
  - value: 0.9777
    std: 0.0037
    model: ELGNN
    arxiv_id: '2310.14166'
    title: Ensemble Learning for Graph Neural Networks
    date: '2023-10-22'
  milestones_by_metric:
    Hits@20: *id001
    MRR:
    - value: 0.1346
      std: null
      model: GCN
      arxiv_id: '2506.24018'
      title: Bridging Theory and Practice in Link Representation with Graph Neural
        Networks
      date: '2025-06-30'
    Recall@20:
    - value: 0.0921
      std: null
      model: OpenGraph
      arxiv_id: '2403.01121'
      title: 'OpenGraph: Towards Open Graph Foundation Models'
      date: '2024-03-02'
---

