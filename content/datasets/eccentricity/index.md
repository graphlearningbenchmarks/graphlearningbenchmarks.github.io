---
title: Eccentricity
slug: eccentricity
benchmark: Algorithmic Graph Tasks
task_type: graph_regression
description: Graph eccentricity prediction — node-level task predicting max distance
  to any other node.
primary_metric: MSE
higher_is_better: false
pyg_url: ''
stats:
  num_graphs: 7040
  avg_nodes: null
  avg_edges: null
  num_classes: null
result_count: 31
best_model:
  model: GCN-SSM + k-hop
  value: -4.2652
  metric: MSE
  arxiv_id: '2502.10818'
  paper_title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs:
    Bridging Recurrent and Graph Learning'
papers:
- arxiv_id: '2508.05070'
  title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
  date_iso: '2025-08-07'
  venue: ''
- arxiv_id: '2505.18728'
  title: 'Message-Passing State-Space Models: Improving Graph Learning with Modern
    Sequence Modeling'
  date_iso: '2025-05-24'
  venue: ''
- arxiv_id: '2502.10818'
  title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
    Recurrent and Graph Learning'
  date_iso: '2025-02-15'
  venue: ''
- arxiv_id: '2210.09789'
  title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
  date_iso: '2022-10-18'
  venue: ICLR 2022
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: MSE
  default_metric: MSE
  higher_is_better: false
  stats:
    num_graphs: 7040
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - MSE
  - log10(MSE)
  metric_display_names:
  - MSE
  - log10(MSE)
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GCN-SSM + k-hop
    model_plain: GCN-SSM + k-hop
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
    date_display: Feb 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - -4.2652
    - null
    metric_stds:
    - 0.1776
    - null
  - model: MP-SSM
    model_plain: MP-SSM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.18728'
    title: 'Message-Passing State-Space Models: Improving Graph Learning with Modern
      Sequence Modeling'
    date: May 24, 2025
    date_iso: '2025-05-24'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - -2.9724
    - null
    metric_stds:
    - 0.0271
    - null
  - model: GCN-SSM + eig(Lambda) approx 1
    model_plain: GCN-SSM + eig(Lambda) approx 1
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
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
    - -2.2583
    - null
    metric_stds:
    - 0.0085
    - null
  - model: GCN-SSM
    model_plain: GCN-SSM
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
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
    - -2.2446
    - null
    metric_stds:
    - 0.0027
    - null
  - model: DRew-GCN
    model_plain: DRew-GCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
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
    - -2.1004
    - null
    metric_stds:
    - 0.0256
    - null
  - model: DRew-GCN + delay
    model_plain: DRew-GCN + delay
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
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
    - -2.0291
    - null
    metric_stds:
    - 0.024
    - null
  - model: PH-DGN
    model_plain: PH-DGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
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
    - -0.9348
    - null
    metric_stds:
    - 0.2097
    - null
  - model: SWAN
    model_plain: SWAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
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
    - -0.0739
    - null
    metric_stds:
    - 0.219
    - null
  - model: A-DGN(GCN)
    model_plain: A-DGN(GCN)
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: Oct 18, 2022
    date_iso: '2022-10-18'
    date_display: Oct 2022
    codebase_url: https://github.com/gravins/Anti-SymmetricDGN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.3046
    - null
    metric_stds:
    - 0.1181
    - null
  - model: ADGN
    model_plain: ADGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
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
    - 0.4296
    - null
    metric_stds:
    - 0.1003
    - null
  - model: A-DGN
    model_plain: A-DGN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.18728'
    title: 'Message-Passing State-Space Models: Improving Graph Learning with Modern
      Sequence Modeling'
    date: May 24, 2025
    date_iso: '2025-05-24'
    date_display: May 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.4296
    - null
    metric_stds:
    - 0.1003
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
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
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
    - 0.6077
    - null
    metric_stds:
    - 0.0282
    - null
  - model: GRAND
    model_plain: GRAND
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: Oct 18, 2022
    date_iso: '2022-10-18'
    date_display: Oct 2022
    codebase_url: https://github.com/gravins/Anti-SymmetricDGN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6602
    - null
    metric_stds:
    - 0.1393
    - null
  - model: GraphCON
    model_plain: GraphCON
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: Feb 15, 2025
    date_iso: '2025-02-15'
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
    - 0.6833
    - null
    metric_stds:
    - 0.0074
    - null
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: Oct 18, 2022
    date_iso: '2022-10-18'
    date_display: Oct 2022
    codebase_url: https://github.com/gravins/Anti-SymmetricDGN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.764
    - null
    metric_stds:
    - 0.0355
    - null
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: Oct 18, 2022
    date_iso: '2022-10-18'
    date_display: Oct 2022
    codebase_url: https://github.com/gravins/Anti-SymmetricDGN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7863
    - null
    metric_stds:
    - 0.0207
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
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: Oct 18, 2022
    date_iso: '2022-10-18'
    date_display: Oct 2022
    codebase_url: https://github.com/gravins/Anti-SymmetricDGN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7909
    - null
    metric_stds:
    - 0.0222
    - null
  - model: DGC
    model_plain: DGC
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: Oct 18, 2022
    date_iso: '2022-10-18'
    date_display: Oct 2022
    codebase_url: https://github.com/gravins/Anti-SymmetricDGN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8261
    - null
    metric_stds:
    - 0.0032
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
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: Oct 18, 2022
    date_iso: '2022-10-18'
    date_display: Oct 2022
    codebase_url: https://github.com/gravins/Anti-SymmetricDGN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8468
    - null
    metric_stds:
    - 0.0028
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
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: Oct 18, 2022
    date_iso: '2022-10-18'
    date_display: Oct 2022
    codebase_url: https://github.com/gravins/Anti-SymmetricDGN
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9504
    - null
    metric_stds:
    - 0.0007
    - null
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: true
    override_reason: The source table labels Eccentricity as log10(MSE).
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - null
    - 0.6995
    metric_stds:
    - null
    - null
  - model: GCN
    model_plain: GCN
    is_baseline: true
    is_overridden: true
    override_reason: The source table labels Eccentricity as log10(MSE).
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - null
    - 0.8468
    metric_stds:
    - null
    - null
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: true
    override_reason: The source table labels Eccentricity as log10(MSE).
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - null
    - 0.7909
    metric_stds:
    - null
    - null
  - model: GraphSAGE
    model_plain: GraphSAGE
    is_baseline: true
    is_overridden: true
    override_reason: The source table labels Eccentricity as log10(MSE).
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - null
    - 0.7863
    metric_stds:
    - null
    - null
  - model: GIN
    model_plain: GIN
    is_baseline: true
    is_overridden: true
    override_reason: The source table labels Eccentricity as log10(MSE).
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - null
    - 0.9504
    metric_stds:
    - null
    - null
  - model: GCNII
    model_plain: GCNII
    is_baseline: true
    is_overridden: true
    override_reason: The source table labels Eccentricity as log10(MSE).
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - null
    - 0.764
    metric_stds:
    - null
    - null
  - model: DGC
    model_plain: DGC
    is_baseline: true
    is_overridden: true
    override_reason: The source table labels Eccentricity as log10(MSE).
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - null
    - 0.8261
    metric_stds:
    - null
    - null
  - model: GRAND
    model_plain: GRAND
    is_baseline: true
    is_overridden: true
    override_reason: The source table labels Eccentricity as log10(MSE).
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - null
    - 0.6602
    metric_stds:
    - null
    - null
  - model: GraphCON
    model_plain: GraphCON
    is_baseline: true
    is_overridden: true
    override_reason: The source table labels Eccentricity as log10(MSE).
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - null
    - 0.6833
    metric_stds:
    - null
    - null
  - model: A-DGN
    model_plain: A-DGN
    is_baseline: true
    is_overridden: true
    override_reason: The source table labels Eccentricity as log10(MSE).
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - null
    - 0.4296
    metric_stds:
    - null
    - null
  - model: GPS
    model_plain: GPS
    is_baseline: true
    is_overridden: true
    override_reason: The source table labels Eccentricity as log10(MSE).
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
    - null
    - 0.6077
    metric_stds:
    - null
    - null
  row_count: 31
  rows_json: ''
  chart_json: /data/datasets/eccentricity/standard-split-chart.json
  arch_counts:
    gnn: 25
    hybrid: 3
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 20
  - 11
  milestones: &id001
  - value: 0.3046
    std: 0.1181
    model: A-DGN(GCN)
    arxiv_id: '2210.09789'
    title: 'Anti-Symmetric DGN: a stable architecture for Deep Graph Networks'
    date: '2022-10-18'
  - value: -4.2652
    std: 0.1776
    model: GCN-SSM + k-hop
    arxiv_id: '2502.10818'
    title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing in GNNs: Bridging
      Recurrent and Graph Learning'
    date: '2025-02-15'
  milestones_by_metric:
    MSE: *id001
    log10(MSE):
    - value: 0.4296
      std: null
      model: A-DGN
      arxiv_id: '2508.05070'
      title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
      date: '2025-08-07'
---

