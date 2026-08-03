---
title: arxiv-year
slug: arxiv-year
benchmark: LINKX Benchmarks
task_type: node_classification
description: OGB-arXiv node classification by publication year (5 classes, heterophilic
  variant).
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.LINKXDataset.html
stats:
  num_graphs: 1
  avg_nodes: 169343.0
  avg_edges: 1166243.0
  num_classes: 40
result_count: 62
best_model:
  model: LargeScaleNet
  value: 0.6582
  metric: Accuracy
  arxiv_id: '2411.19392'
  paper_title: Scale-aware Message Passing For Graph Node Classification
papers:
- arxiv_id: '2604.15699'
  title: Frequency-Corrupt Based Graph Self-Supervised Learning
  date_iso: '2026-04-17'
  venue: WWW 2026
- arxiv_id: '2504.18273'
  title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
  date_iso: '2025-04-25'
  venue: ''
- arxiv_id: '2411.19392'
  title: Scale-aware Message Passing For Graph Node Classification
  date_iso: '2024-11-28'
  venue: ''
- arxiv_id: '2406.10871'
  title: Graph Neural Reaction Diffusion Models Submitted to the editors June 2023.
    Accepted in March 2024.
  date_iso: '2024-06-16'
  venue: ''
- arxiv_id: '2401.09125'
  title: Understanding Heterophily for Graph Neural Networks
  date_iso: '2024-01-17'
  venue: ICML 2024
- arxiv_id: '2310.18884'
  title: Simple and Asymmetric Graph Contrastive Learning without Augmentations
  date_iso: '2023-10-29'
  venue: NeurIPS 2023
- arxiv_id: '2310.02232'
  title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
  date_iso: '2023-10-03'
  venue: ICLR 2023
- arxiv_id: '2307.16092'
  title: Feature Transportation Improves Graph Neural Networks
  date_iso: '2023-07-29'
  venue: AAAI 2023
- arxiv_id: '2210.00513'
  title: Gradient Gating for Deep Multi-Rate Learning on Graphs
  date_iso: '2022-10-02'
  venue: ICLR 2022
- arxiv_id: '2202.03580'
  title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
  date_iso: '2022-02-04'
  venue: NeurIPS 2022
- arxiv_id: '2110.08128'
  title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
  date_iso: '2021-10-15'
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
    num_graphs: 1
    avg_nodes: 169343.0
    avg_edges: 1166243.0
    num_classes: 40
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: LargeScaleNet
    model_plain: LargeScaleNet
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: Nov 28, 2024
    date_iso: '2024-11-28'
    date_display: Nov 2024
    codebase_url: https://github.com/Qin87/ScaleNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.6582
    metric_stds:
    - 0.0036
  - model: FaberNet
    model_plain: FaberNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_iso: '2023-10-03'
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
    - 0.6462
    metric_stds:
    - 0.0101
  - model: DirGNN
    model_plain: DirGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_iso: '2023-10-03'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6397
    metric_stds:
    - 0.003
  - model: G^2
    model_plain: G^2
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.16092'
    title: Feature Transportation Improves Graph Neural Networks
    date: Jul 29, 2023
    date_iso: '2023-07-29'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.633
    metric_stds:
    - 0.0184
  - model: G^2-GraphSAGE
    model_plain: G^2-GraphSAGE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.633
    metric_stds:
    - 0.0184
  - model: Grad. Gating
    model_plain: Grad. Gating
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_iso: '2023-10-03'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.633
    metric_stds:
    - 0.0184
  - model: ADR-GNN_S
    model_plain: ADR-GNN_S
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.16092'
    title: Feature Transportation Improves Graph Neural Networks
    date: Jul 29, 2023
    date_iso: '2023-07-29'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6117
    metric_stds:
    - 0.0154
  - model: MagNet
    model_plain: MagNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_iso: '2023-10-03'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6029
    metric_stds:
    - 0.0027
  - model: IBG-NN
    model_plain: IBG-NN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: Apr 25, 2025
    date_iso: '2025-04-25'
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
    - 0.6014
    metric_stds:
    - null
  - model: RDGNN-I
    model_plain: RDGNN-I
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.10871'
    title: Graph Neural Reaction Diffusion Models Submitted to the editors June 2023.
      Accepted in March 2024.
    date: Jun 16, 2024
    date_iso: '2024-06-16'
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
    - 0.5846
    metric_stds:
    - 0.0059
  - model: LINKX
    model_plain: LINKX
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.08128'
    title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/ChandlerBang/SimP-GCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.56
    metric_stds:
    - 0.013
  - model: GCNs
    model_plain: GCNs
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.08128'
    title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/ChandlerBang/SimP-GCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.558
    metric_stds:
    - 0.002
  - model: RDGNN-S
    model_plain: RDGNN-S
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.10871'
    title: Graph Neural Reaction Diffusion Models Submitted to the editors June 2023.
      Accepted in March 2024.
    date: Jun 16, 2024
    date_iso: '2024-06-16'
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
    - 0.5516
    metric_stds:
    - 0.0046
  - model: GloGNN
    model_plain: GloGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.08128'
    title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/ChandlerBang/SimP-GCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.548
    metric_stds:
    - 0.003
  - model: LINK
    model_plain: LINK
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5397
    metric_stds:
    - 0.0018
  - model: Polynormer
    model_plain: Polynormer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: Nov 28, 2024
    date_iso: '2024-11-28'
    date_display: Nov 2024
    codebase_url: https://github.com/Qin87/ScaleNet
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.525
    metric_stds:
    - 0.0077
  - model: MixHop
    model_plain: MixHop
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5181
    metric_stds:
    - 0.0017
  - model: FSGNN
    model_plain: FSGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_iso: '2023-10-03'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5047
    metric_stds:
    - 0.0021
  - model: H2GCN
    model_plain: H2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.08128'
    title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/ChandlerBang/SimP-GCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.491
    metric_stds:
    - 0.001
  - model: H_2GCN
    model_plain: H_2GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: Oct 3, 2023
    date_iso: '2023-10-03'
    date_display: Oct 2023
    codebase_url: ''
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4909
    metric_stds:
    - 0.001
  - model: ChebNetII
    model_plain: ChebNetII
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4853
    metric_stds:
    - 0.0031
  - model: ACM-GCN
    model_plain: ACM-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4737
    metric_stds:
    - 0.0059
  - model: GraphACL
    model_plain: GraphACL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.18884'
    title: Simple and Asymmetric Graph Contrastive Learning without Augmentations
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/tengxiao1/GraphACL
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4721
    metric_stds:
    - 0.0039
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.08128'
    title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/ChandlerBang/SimP-GCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.472
    metric_stds:
    - 0.003
  - model: ChebNet
    model_plain: ChebNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4676
    metric_stds:
    - 0.0024
  - model: BernNet
    model_plain: BernNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.0921
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4634
    metric_stds:
    - 0.0032
  - model: MixHop
    model_plain: MixHop
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.08128'
    title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/ChandlerBang/SimP-GCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.461
    metric_stds:
    - 0.005
  - model: L Prop (2 hop)
    model_plain: L Prop (2 hop)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.16092'
    title: Feature Transportation Improves Graph Neural Networks
    date: Jul 29, 2023
    date_iso: '2023-07-29'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4607
    metric_stds:
    - 0.0015
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4605
    metric_stds:
    - 0.0051
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.08128'
    title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/ChandlerBang/SimP-GCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.46
    metric_stds:
    - 0.003
  - model: GPR-GNN
    model_plain: GPR-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.0921
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.03580'
    title: Convolutional Neural Networks on Graphs with Chebyshev Approximation, Revisited
    date: Feb 4, 2022
    date_iso: '2022-02-04'
    date_display: Feb 2022
    codebase_url: https://github.com/ivam-he/ChebNetII
    published_conference: NeurIPS 2022
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4597
    metric_stds:
    - 0.0026
  - model: SP-GCL
    model_plain: SP-GCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.18884'
    title: Simple and Asymmetric Graph Contrastive Learning without Augmentations
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/tengxiao1/GraphACL
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.458
    metric_stds:
    - 0.0057
  - model: GPRGNN
    model_plain: GPRGNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.08128'
    title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/ChandlerBang/SimP-GCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.451
    metric_stds:
    - 0.002
  - model: GPR-GNN
    model_plain: GPR-GNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4507
    metric_stds:
    - 0.0021
  - model: HGRL
    model_plain: HGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.18884'
    title: Simple and Asymmetric Graph Contrastive Learning without Augmentations
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/tengxiao1/GraphACL
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4392
    metric_stds:
    - 0.0052
  - model: DSSL
    model_plain: DSSL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.18884'
    title: Simple and Asymmetric Graph Contrastive Learning without Augmentations
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/tengxiao1/GraphACL
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4371
    metric_stds:
    - 0.0054
  - model: BGRL
    model_plain: BGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.18884'
    title: Simple and Asymmetric Graph Contrastive Learning without Augmentations
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/tengxiao1/GraphACL
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4302
    metric_stds:
    - 0.0062
  - model: GCA
    model_plain: GCA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.18884'
    title: Simple and Asymmetric Graph Contrastive Learning without Augmentations
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/tengxiao1/GraphACL
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4296
    metric_stds:
    - 0.0039
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_iso: '2024-01-17'
    date_display: Jan 2024
    codebase_url: ''
    published_conference: ICML 2024
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4244
    metric_stds:
    - null
  - model: C&S (2 hop)
    model_plain: C&S (2 hop)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.16092'
    title: Feature Transportation Improves Graph Neural Networks
    date: Jul 29, 2023
    date_iso: '2023-07-29'
    date_display: Jul 2023
    codebase_url: ''
    published_conference: AAAI 2023
    published_conference_short: AAAI
    published_conference_slug: aaai
    published_venue: AAAI 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4217
    metric_stds:
    - 0.0027
  - model: FC-GSSL
    model_plain: FC-GSSL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.42
    metric_stds:
    - 0.0011
  - model: GraphPAE
    model_plain: GraphPAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4185
    metric_stds:
    - 0.0004
  - model: BGRL
    model_plain: BGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4143
    metric_stds:
    - 0.0004
  - model: CCA-SSG
    model_plain: CCA-SSG
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4078
    metric_stds:
    - 0.0001
  - model: FAGCN
    model_plain: FAGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.08128'
    title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/ChandlerBang/SimP-GCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.406
    metric_stds:
    - 0.004
  - model: MaskGAE
    model_plain: MaskGAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4059
    metric_stds:
    - 0.0004
  - model: S2GAE
    model_plain: S2GAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4032
    metric_stds:
    - 0.0012
  - model: GraphMAE
    model_plain: GraphMAE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.15699'
    title: Frequency-Corrupt Based Graph Self-Supervised Learning
    date: Apr 17, 2026
    date_iso: '2026-04-17'
    date_display: Apr 2026
    codebase_url: https://github.com/rookitkitlee/FC-GSSL
    published_conference: WWW 2026
    published_conference_short: WWW
    published_conference_slug: www
    published_venue: WWW 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.403
    metric_stds:
    - 0.0004
  - model: DGI
    model_plain: DGI
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.18884'
    title: Simple and Asymmetric Graph Contrastive Learning without Augmentations
    date: Oct 29, 2023
    date_iso: '2023-10-29'
    date_display: Oct 2023
    codebase_url: https://github.com/tengxiao1/GraphACL
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3926
    metric_stds:
    - 0.0072
  - model: ASGC
    model_plain: ASGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.08128'
    title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    date: Oct 15, 2021
    date_iso: '2021-10-15'
    date_display: Oct 2021
    codebase_url: https://github.com/ChandlerBang/SimP-GCN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.392
    metric_stds:
    - 0.001
  row_count: 62
  rows_json: /data/datasets/arxiv-year/standard-split-rows.json
  chart_json: /data/datasets/arxiv-year/standard-split-chart.json
  arch_counts:
    gnn: 51
    hybrid: 6
    graph_transformer: 2
    llm: 0
    walk: 1
    traditional: 2
  metric_counts:
  - 62
  milestones: &id001
  - value: 0.56
    std: 0.013
    model: LINKX
    arxiv_id: '2110.08128'
    title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    date: '2021-10-15'
  - value: 0.633
    std: 0.0184
    model: G^2-GraphSAGE
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: '2022-10-02'
  - value: 0.6462
    std: 0.0101
    model: FaberNet
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: '2023-10-03'
  - value: 0.6582
    std: 0.0036
    model: LargeScaleNet
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: '2024-11-28'
  milestones_by_metric:
    Accuracy: *id001
---

