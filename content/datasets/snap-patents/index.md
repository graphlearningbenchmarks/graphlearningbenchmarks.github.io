---
title: snap-patents
slug: snap-patents
benchmark: LINKX Benchmarks
task_type: node_classification
description: USPTO patent citation graph node classification (5 time-based classes).
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.LINKXDataset.html
stats:
  num_graphs: 1
  avg_nodes: 2745480.0
  avg_edges: 12800500.0
  num_classes: 5
result_count: 34
best_model:
  model: GloGNN
  value: 0.8432
  metric: Accuracy
  arxiv_id: '2205.07308'
  paper_title: Finding Global Homophily in Graph Neural Networks When Meeting Heterophily
papers:
- arxiv_id: '2411.19392'
  title: Scale-aware Message Passing For Graph Node Classification
  date_iso: '2024-11-28'
  venue: ''
- arxiv_id: '2401.09125'
  title: Understanding Heterophily for Graph Neural Networks
  date_iso: '2024-01-17'
  venue: ICML 2024
- arxiv_id: '2310.02232'
  title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
  date_iso: '2023-10-03'
  venue: ICLR 2023
- arxiv_id: '2305.10498'
  title: Edge Directionality Improves Learning on Heterophilic Graphs
  date_iso: '2023-05-17'
  venue: ''
- arxiv_id: '2212.02483'
  title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
  date_iso: '2022-12-05'
  venue: ICML 2022
- arxiv_id: '2210.00513'
  title: Gradient Gating for Deep Multi-Rate Learning on Graphs
  date_iso: '2022-10-02'
  venue: ICLR 2022
- arxiv_id: '2205.07308'
  title: Finding Global Homophily in Graph Neural Networks When Meeting Heterophily
  date_iso: '2022-05-15'
  venue: ICML 2022
- arxiv_id: '2005.14612'
  title: Non-Local Graph Neural Networks
  date_iso: '2020-05-29'
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
    avg_nodes: 2745480.0
    avg_edges: 12800500.0
    num_classes: 5
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GloGNN
    model_plain: GloGNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07308'
    title: Finding Global Homophily in Graph Neural Networks When Meeting Heterophily
    date: May 15, 2022
    date_iso: '2022-05-15'
    date_display: May 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8432
    metric_stds:
    - null
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.751
    metric_stds:
    - 0.0003
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
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7505
    metric_stds:
    - 0.0005
  - model: FaberNet
    model_plain: FaberNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.7455
    metric_stds:
    - 0.0011
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
    - 0.7395
    metric_stds:
    - 0.0005
  - model: dir-gcn
    model_plain: dir-gcn
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.10498'
    title: Edge Directionality Improves Learning on Heterophilic Graphs
    date: May 17, 2023
    date_iso: '2023-05-17'
    date_display: May 2023
    codebase_url: https://github.com/emalgorithm/directed-graph-neural-network
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7132
    metric_stds:
    - 0.0006
  - model: dir-sage
    model_plain: dir-sage
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2305.10498'
    title: Edge Directionality Improves Learning on Heterophilic Graphs
    date: May 17, 2023
    date_iso: '2023-05-17'
    date_display: May 2023
    codebase_url: https://github.com/emalgorithm/directed-graph-neural-network
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7026
    metric_stds:
    - 0.0014
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
    - 0.695
    metric_stds:
    - 0.0039
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
    - 0.695
    metric_stds:
    - 0.0039
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
    - 0.6507
    metric_stds:
    - 0.0003
  - model: GloGNN
    model_plain: GloGNN
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
    - 0.6209
    metric_stds:
    - 0.0027
  - model: LINKX
    model_plain: LINKX
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
    - 0.6195
    metric_stds:
    - 0.0012
  - model: LINK
    model_plain: LINK
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
    - 0.6039
    metric_stds:
    - 0.0007
  - model: H_A
    model_plain: H_A
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.07308'
    title: Finding Global Homophily in Graph Neural Networks When Meeting Heterophily
    date: May 15, 2022
    date_iso: '2022-05-15'
    date_display: May 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.5622
    metric_stds:
    - null
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
    - 0.5514
    metric_stds:
    - 0.0016
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
    - 0.5216
    metric_stds:
    - 0.0009
  - model: GCN
    model_plain: GCN
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
    - 0.5102
    metric_stds:
    - 0.0006
  - model: NLGCN
    model_plain: NLGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2005.14612'
    title: Non-Local Graph Neural Networks
    date: May 29, 2020
    date_iso: '2020-05-29'
    date_display: May 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.508
    metric_stds:
    - 0.004
  - model: NLGAT
    model_plain: NLGAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2005.14612'
    title: Non-Local Graph Neural Networks
    date: May 29, 2020
    date_iso: '2020-05-29'
    date_display: May 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.483
    metric_stds:
    - 0.002
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2005.14612'
    title: Non-Local Graph Neural Networks
    date: May 29, 2020
    date_iso: '2020-05-29'
    date_display: May 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.457
    metric_stds:
    - 0.0
  - model: GCN
    model_plain: GCN
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
    - 0.4565
    metric_stds:
    - 0.0004
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2005.14612'
    title: Non-Local Graph Neural Networks
    date: May 29, 2020
    date_iso: '2020-05-29'
    date_display: May 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.454
    metric_stds:
    - 0.004
  - model: TIDE-s
    model_plain: TIDE-s
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.02483'
    title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
    date: Dec 5, 2022
    date_iso: '2022-12-05'
    date_display: Dec 2022
    codebase_url: https://github.com/maysambehmanesh/TIDE
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4075
    metric_stds:
    - 0.0058
  - model: TIDE-m
    model_plain: TIDE-m
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2212.02483'
    title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
    date: Dec 5, 2022
    date_iso: '2022-12-05'
    date_display: Dec 2022
    codebase_url: https://github.com/maysambehmanesh/TIDE
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: true
    metric_values:
    - 0.4056
    metric_stds:
    - 0.017
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
    - 0.4019
    metric_stds:
    - 0.0003
  - model: GRAND
    model_plain: GRAND
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.02483'
    title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
    date: Dec 5, 2022
    date_iso: '2022-12-05'
    date_display: Dec 2022
    codebase_url: https://github.com/maysambehmanesh/TIDE
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3889
    metric_stds:
    - 0.0042
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.02483'
    title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
    date: Dec 5, 2022
    date_iso: '2022-12-05'
    date_display: Dec 2022
    codebase_url: https://github.com/maysambehmanesh/TIDE
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3876
    metric_stds:
    - 0.0075
  - model: GCNII
    model_plain: GCNII
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
    - 0.3788
    metric_stds:
    - 0.0069
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.02483'
    title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
    date: Dec 5, 2022
    date_iso: '2022-12-05'
    date_display: Dec 2022
    codebase_url: https://github.com/maysambehmanesh/TIDE
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3684
    metric_stds:
    - 0.0037
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
    - 0.3442
    metric_stds:
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
    - 0.3219
    metric_stds:
    - 0.0007
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    - 0.315
    metric_stds:
    - null
  - model: MLP
    model_plain: MLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2005.14612'
    title: Non-Local Graph Neural Networks
    date: May 29, 2020
    date_iso: '2020-05-29'
    date_display: May 2020
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.313
    metric_stds:
    - 0.001
  - model: DiffusionNet
    model_plain: DiffusionNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2212.02483'
    title: 'TIDE: Time Derivative Diffusion for Deep Learning on Graphs'
    date: Dec 5, 2022
    date_iso: '2022-12-05'
    date_display: Dec 2022
    codebase_url: https://github.com/maysambehmanesh/TIDE
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3069
    metric_stds:
    - 0.00014
  row_count: 34
  rows_json: ''
  chart_json: /data/datasets/snap-patents/standard-split-chart.json
  arch_counts:
    gnn: 23
    hybrid: 9
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 2
  metric_counts:
  - 34
  milestones: &id001
  - value: 0.508
    std: 0.004
    model: NLGCN
    arxiv_id: '2005.14612'
    title: Non-Local Graph Neural Networks
    date: '2020-05-29'
  - value: 0.695
    std: 0.0039
    model: G^2-GraphSAGE
    arxiv_id: '2210.00513'
    title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    date: '2022-10-02'
  - value: 0.7132
    std: 0.0006
    model: dir-gcn
    arxiv_id: '2305.10498'
    title: Edge Directionality Improves Learning on Heterophilic Graphs
    date: '2023-05-17'
  - value: 0.751
    std: 0.0003
    model: FaberNet
    arxiv_id: '2310.02232'
    title: 'HoloNets: Spectral Convolutions do extend to Directed Graphs'
    date: '2023-10-03'
  milestones_by_metric:
    Accuracy: *id001
---

