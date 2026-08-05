---
title: ogbl-citation2
slug: ogbl-citation2
benchmark: OGB
task_type: link_prediction
description: Citation link prediction on arXiv/PubMed papers (directed).
primary_metric: MRR
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.OGBLinkPropPredDataset.html
stats:
  num_graphs: 2927963
  avg_nodes: 30561187.0
  avg_edges: null
  num_classes: null
result_count: 112
best_model:
  model: MPLP
  value: 0.9072
  metric: MRR
  arxiv_id: '2309.00976'
  paper_title: Pure Message Passing Can Estimate Common Neighbor for Link Prediction
papers:
- arxiv_id: '2508.17630'
  title: 'Quantum Graph Attention Network: A Novel Quantum Multi-Head Attention Mechanism
    for Graph Learning'
  date_iso: '2025-08-25'
  venue: ''
- arxiv_id: '2504.06193'
  title: 'Weak Models Can be Good Teachers: A Case Study on Link Prediction with MLPs'
  date_iso: '2025-04-08'
  venue: ''
- arxiv_id: '2411.03845'
  title: Reconsidering the Performance of GAE in Link Prediction
  date_iso: '2024-11-06'
  venue: ''
- arxiv_id: '2409.17475'
  title: On the Impact of Feature Heterophily on Link Prediction with Graph Neural
    Networks
  date_iso: '2024-09-26'
  venue: NeurIPS 2024
- arxiv_id: '2406.16687'
  title: Link Prediction with Untrained Message Passing Layers
  date_iso: '2024-06-24'
  venue: ''
- arxiv_id: '2312.04737'
  title: Efficient End-to-end Language Model Fine-tuning on Graphs
  date_iso: '2023-12-07'
  venue: KDD 2023
- arxiv_id: '2310.11009'
  title: 'LPFormer: An Adaptive Graph Transformer for Link Prediction'
  date_iso: '2023-10-17'
  venue: KDD 2023
- arxiv_id: '2310.09516'
  title: Efficient Link Prediction via GNN Layers Induced by Negative Sampling
  date_iso: '2023-10-14'
  venue: ''
- arxiv_id: '2309.06574'
  title: 'Circle Feature Graphormer: Can Circle Features Stimulate Graph Transformer?'
  date_iso: '2023-09-11'
  venue: ''
- arxiv_id: '2309.00976'
  title: Pure Message Passing Can Estimate Common Neighbor for Link Prediction
  date_iso: '2023-09-02'
  venue: NeurIPS 2023
- arxiv_id: '2305.09887'
  title: 'Simplifying Distributed Neural Network Training on Massive Graphs: Randomized
    Partitions Improve Model Aggregation'
  date_iso: '2023-05-17'
  venue: ''
- arxiv_id: '2304.10074'
  title: Improving Graph Neural Networks on Multi-node Tasks with the Labeling Trick
  date_iso: '2023-04-20'
  venue: JMLR 2023
- arxiv_id: '2303.03379'
  title: 'SUREL+: Moving from Walks to Sets for Scalable Subgraph-based Graph Representation
    Learning'
  date_iso: '2023-03-06'
  venue: ''
- arxiv_id: '2303.00170'
  title: Asymmetric Learning for Graph Neural Network based Link Prediction
  date_iso: '2023-03-01'
  venue: ''
- arxiv_id: '2301.12562'
  title: Simplifying Subgraph Representation Learning for Scalable Link Prediction
  date_iso: '2023-01-29'
  venue: ''
- arxiv_id: '2210.05801'
  title: Linkless Link Prediction via Relational Distillation
  date_iso: '2022-10-11'
  venue: ICML 2022
- arxiv_id: '2209.15486'
  title: Graph Neural Networks for Link Prediction with Subgraph Sketching
  date_iso: '2022-09-30'
  venue: ICLR 2022
- arxiv_id: '2206.04216'
  title: 'Neo-GNNs: Neighborhood Overlap-aware Graph Neural Networks for Link Prediction'
  date_iso: '2022-06-09'
  venue: NeurIPS 2022
- arxiv_id: '2202.13538'
  title: Algorithm and System Co-design for Efficient Subgraph-based Graph Representation
    Learning
  date_iso: '2022-02-28'
  venue: ''
- arxiv_id: '2112.02936'
  title: Pairwise Learning for Neural Link Prediction
  date_iso: '2021-12-06'
  venue: ''
- arxiv_id: '2012.15024'
  title: Adaptive Graph Diffusion Networks
  date_iso: '2020-12-30'
  venue: ''
- arxiv_id: '2010.16103'
  title: 'Labeling Trick: A Theory of Using Graph Neural Networks for Multi-Node Representation
    Learning'
  date_iso: '2020-10-30'
  venue: NeurIPS 2020
- arxiv_id: '2005.00687'
  title: OGB
  date_iso: '2020-05-02'
  venue: NeurIPS 2020
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: MRR
  default_metric: MRR
  higher_is_better: true
  stats:
    num_graphs: 2927963
    avg_nodes: 30561187.0
    avg_edges: null
    num_classes: null
  metrics:
  - MRR
  - Hits@200
  metric_display_names:
  - MRR
  - Hits@200
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: MPLP
    model_plain: MPLP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.00976'
    title: Pure Message Passing Can Estimate Common Neighbor for Link Prediction
    date: Sep 2, 2023
    date_iso: '2023-09-02'
    date_display: Sep 2023
    codebase_url: https://github.com/Barcavin/efficient-node-labelling
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9072
    - null
    metric_stds:
    - 0.0012
    - null
  - model: CFG
    model_plain: CFG
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.06574'
    title: 'Circle Feature Graphormer: Can Circle Features Stimulate Graph Transformer?'
    date: Sep 11, 2023
    date_iso: '2023-09-11'
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
    - 0.8997
    - null
    metric_stds:
    - 0.0015
    - null
  - model: SIEG
    model_plain: SIEG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2309.06574'
    title: 'Circle Feature Graphormer: Can Circle Features Stimulate Graph Transformer?'
    date: Sep 11, 2023
    date_iso: '2023-09-11'
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
    - 0.8987
    - null
    metric_stds:
    - 0.0018
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
    - 0.8981
    - null
    metric_stds:
    - 0.0013
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
    - 0.8974
    - null
    metric_stds:
    - 0.0018
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
    arxiv_id: '2309.00976'
    title: Pure Message Passing Can Estimate Common Neighbor for Link Prediction
    date: Sep 2, 2023
    date_iso: '2023-09-02'
    date_display: Sep 2023
    codebase_url: https://github.com/Barcavin/efficient-node-labelling
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8912
    - null
    metric_stds:
    - 0.004
    - null
  - model: NGNN + SEAL
    model_plain: NGNN + SEAL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.06574'
    title: 'Circle Feature Graphormer: Can Circle Features Stimulate Graph Transformer?'
    date: Sep 11, 2023
    date_iso: '2023-09-11'
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
    - 0.8891
    - null
    metric_stds:
    - 0.0022
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
    arxiv_id: '2309.06574'
    title: 'Circle Feature Graphormer: Can Circle Features Stimulate Graph Transformer?'
    date: Sep 11, 2023
    date_iso: '2023-09-11'
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
    - 0.8883
    - null
    metric_stds:
    - 0.0018
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
    - 0.8874
    - null
    metric_stds:
    - 0.0006
    - null
  - model: PoS+
    model_plain: PoS+
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2301.12562'
    title: Simplifying Subgraph Representation Learning for Scalable Link Prediction
    date: Jan 29, 2023
    date_iso: '2023-01-29'
    date_display: Jan 2023
    codebase_url: https://github.com/venomouscyanide/S3GRL
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8814
    - null
    metric_stds:
    - 0.0008
    - null
  - model: S3GRL (PoS Plus)
    model_plain: S3GRL (PoS Plus)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.06574'
    title: 'Circle Feature Graphormer: Can Circle Features Stimulate Graph Transformer?'
    date: Sep 11, 2023
    date_iso: '2023-09-11'
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
    - 0.8814
    - null
    metric_stds:
    - 0.0008
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
    - 0.8809
    - null
    metric_stds:
    - 0.0006
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
    - 0.8767
    - null
    metric_stds:
    - 0.0032
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
    - 0.8756
    - null
    metric_stds:
    - 0.0011
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
    arxiv_id: '2309.00976'
    title: Pure Message Passing Can Estimate Common Neighbor for Link Prediction
    date: Sep 2, 2023
    date_iso: '2023-09-02'
    date_display: Sep 2023
    codebase_url: https://github.com/Barcavin/efficient-node-labelling
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8756
    - null
    metric_stds:
    - 0.0011
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
    - 0.8753
    - null
    metric_stds:
    - 0.0012
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
    - 0.8726
    - null
    metric_stds:
    - 0.0084
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
    - 0.8705
    - null
    metric_stds:
    - 0.0004
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
    arxiv_id: '2303.03379'
    title: 'SUREL+: Moving from Walks to Sets for Scalable Subgraph-based Graph Representation
      Learning'
    date: Mar 6, 2023
    date_iso: '2023-03-06'
    date_display: Mar 2023
    codebase_url: 'https://github.com/Graph-COM/SUREL_Plus{https:'
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8696
    - null
    metric_stds:
    - 0.0028
    - null
  - model: AML (G)
    model_plain: AML (G)
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
    - 0.867
    - null
    metric_stds:
    - 0.0005
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
    - 0.8632
    - null
    metric_stds:
    - 0.0052
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
    - 0.8621
    - null
    metric_stds:
    - 0.0009
    - null
  - model: AML-R (G)
    model_plain: AML-R (G)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    - 0.8591
    - null
    metric_stds:
    - 0.0004
    - null
  - model: AGDN w/GraphSAINT
    model_plain: AGDN w/GraphSAINT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.06574'
    title: 'Circle Feature Graphormer: Can Circle Features Stimulate Graph Transformer?'
    date: Sep 11, 2023
    date_iso: '2023-09-11'
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
    - 0.8549
    - null
    metric_stds:
    - 0.0029
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
    - 0.8549
    - null
    metric_stds:
    - 0.0029
    - null
  - model: LEADING
    model_plain: LEADING
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.04737'
    title: Efficient End-to-end Language Model Fine-tuning on Graphs
    date: Dec 7, 2023
    date_iso: '2023-12-07'
    date_display: Dec 2023
    codebase_url: ''
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.852
    - null
    metric_stds:
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
    - 0.8492
    - null
    metric_stds:
    - 0.0029
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
    - 0.849
    - null
    metric_stds:
    - 0.0006
    - null
  - model: 'NO'
    model_plain: 'NO'
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2304.10074'
    title: Improving Graph Neural Networks on Multi-node Tasks with the Labeling Trick
    date: Apr 20, 2023
    date_iso: '2023-04-20'
    date_display: Apr 2023
    codebase_url: https://github.com/GraphPKU/LabelingTrick
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8474
    - null
    metric_stds:
    - 0.0021
    - null
  - model: GAE(GCN)
    model_plain: GAE(GCN)
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
    - 0.8474
    - null
    metric_stds:
    - 0.0021
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
    - 0.8474
    - null
    metric_stds:
    - 0.0021
    - null
  - model: Classification
    model_plain: Classification
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
    - 0.8464
    - null
    metric_stds:
    - null
    - null
  - model: GPRGNN
    model_plain: GPRGNN
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
    is_std_outlier: true
    metric_values:
    - 0.8455
    - null
    metric_stds:
    - 0.0355
    - null
  - model: DeepWalk
    model_plain: DeepWalk
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
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
    - 0.8447
    - null
    metric_stds:
    - 0.0004
    - null
  - model: SuperTMA
    model_plain: SuperTMA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.09887'
    title: 'Simplifying Distributed Neural Network Training on Massive Graphs: Randomized
      Partitions Improve Model Aggregation'
    date: May 17, 2023
    date_iso: '2023-05-17'
    date_display: May 2023
    codebase_url: https://github.com/amazon-science/random-tma
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8375
    - null
    metric_stds:
    - 0.0043
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
    - 0.8367
    - null
    metric_stds:
    - 0.0007
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
    - 0.8336
    - null
    metric_stds:
    - 0.0014
    - null
  - model: RandomTMA
    model_plain: RandomTMA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.09887'
    title: 'Simplifying Distributed Neural Network Training on Massive Graphs: Randomized
      Partitions Improve Model Aggregation'
    date: May 17, 2023
    date_iso: '2023-05-17'
    date_display: May 2023
    codebase_url: https://github.com/amazon-science/random-tma
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8328
    - null
    metric_stds:
    - 0.0024
    - null
  - model: Supervised-FT
    model_plain: Supervised-FT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2312.04737'
    title: Efficient End-to-end Language Model Fine-tuning on Graphs
    date: Dec 7, 2023
    date_iso: '2023-12-07'
    date_display: Dec 2023
    codebase_url: ''
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.831
    - null
    metric_stds:
    - null
    - null
  - model: ZO-OS
    model_plain: ZO-OS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.10074'
    title: Improving Graph Neural Networks on Multi-node Tasks with the Labeling Trick
    date: Apr 20, 2023
    date_iso: '2023-04-20'
    date_display: Apr 2023
    codebase_url: https://github.com/GraphPKU/LabelingTrick
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8285
    - null
    metric_stds:
    - 0.0043
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
    - 0.826
    - null
    metric_stds:
    - 0.0036
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
    - 0.826
    - null
    metric_stds:
    - 0.0036
    - null
  - model: ZO-S
    model_plain: ZO-S
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2304.10074'
    title: Improving Graph Neural Networks on Multi-node Tasks with the Labeling Trick
    date: Apr 20, 2023
    date_iso: '2023-04-20'
    date_display: Apr 2023
    codebase_url: https://github.com/GraphPKU/LabelingTrick
    published_conference: JMLR 2023
    published_conference_short: JMLR
    published_conference_slug: jmlr
    published_venue: JMLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8245
    - null
    metric_stds:
    - 0.0062
    - null
  - model: PSGD-PA
    model_plain: PSGD-PA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.09887'
    title: 'Simplifying Distributed Neural Network Training on Massive Graphs: Randomized
      Partitions Improve Model Aggregation'
    date: May 17, 2023
    date_iso: '2023-05-17'
    date_display: May 2023
    codebase_url: https://github.com/amazon-science/random-tma
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.824
    - null
    metric_stds:
    - 0.0028
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
    - 0.822
    - null
    metric_stds:
    - 0.0127
    - null
  - model: GGS
    model_plain: GGS
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.09887'
    title: 'Simplifying Distributed Neural Network Training on Massive Graphs: Randomized
      Partitions Improve Model Aggregation'
    date: May 17, 2023
    date_iso: '2023-05-17'
    date_display: May 2023
    codebase_url: https://github.com/amazon-science/random-tma
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8195
    - null
    metric_stds:
    - 0.002
    - null
  - model: LLCG
    model_plain: LLCG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.09887'
    title: 'Simplifying Distributed Neural Network Training on Massive Graphs: Randomized
      Partitions Improve Model Aggregation'
    date: May 17, 2023
    date_iso: '2023-05-17'
    date_display: May 2023
    codebase_url: https://github.com/amazon-science/random-tma
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8188
    - null
    metric_stds:
    - 0.0002
    - null
  - model: Pre-trained
    model_plain: Pre-trained
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2312.04737'
    title: Efficient End-to-end Language Model Fine-tuning on Graphs
    date: Dec 7, 2023
    date_iso: '2023-12-07'
    date_display: Dec 2023
    codebase_url: ''
    published_conference: KDD 2023
    published_conference_short: KDD
    published_conference_slug: kdd
    published_venue: KDD 2023
    uses_external_data: true
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.818
    - null
    metric_stds:
    - null
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
    - 0.8127
    - null
    metric_stds:
    - 0.0031
    - null
  - model: NeighborSampling
    model_plain: NeighborSampling
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
    - 0.8044
    - null
    metric_stds:
    - 0.001
    - null
  row_count: 112
  rows_json: /data/datasets/ogbl-citation2/standard-split-rows.json
  chart_json: /data/datasets/ogbl-citation2/standard-split-chart.json
  arch_counts:
    gnn: 53
    hybrid: 13
    graph_transformer: 1
    llm: 3
    walk: 4
    traditional: 36
  metric_counts:
  - 109
  - 3
  milestones: &id001
  - value: 0.8767
    std: 0.0032
    model: SEAL
    arxiv_id: '2010.16103'
    title: 'Labeling Trick: A Theory of Using Graph Neural Networks for Multi-Node
      Representation Learning'
    date: '2020-10-30'
  - value: 0.8974
    std: 0.0018
    model: SUREL
    arxiv_id: '2202.13538'
    title: Algorithm and System Co-design for Efficient Subgraph-based Graph Representation
      Learning
    date: '2022-02-28'
  - value: 0.9072
    std: 0.0012
    model: MPLP
    arxiv_id: '2309.00976'
    title: Pure Message Passing Can Estimate Common Neighbor for Link Prediction
    date: '2023-09-02'
  milestones_by_metric:
    MRR: *id001
    Hits@200:
    - value: 0.8256
      std: null
      model: GNN
      arxiv_id: '2210.05801'
      title: Linkless Link Prediction via Relational Distillation
      date: '2022-10-11'
---

