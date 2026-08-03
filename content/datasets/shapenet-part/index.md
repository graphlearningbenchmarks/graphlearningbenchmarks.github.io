---
title: ShapeNet-Part
slug: shapenet-part
benchmark: Other Graph Benchmarks
task_type: node_classification
description: '3D point cloud part segmentation on ShapeNet objects. Graph-based part
  label prediction on point cloud graphs (16 object categories, 50 part classes).

  '
primary_metric: F1
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: null
  avg_nodes: null
  avg_edges: null
  num_classes: 50
result_count: 40
best_model:
  model: GPS + k-MIP
  value: 0.8268
  metric: F1
  arxiv_id: '2604.03815'
  paper_title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
    Power of GraphGPS
papers:
- arxiv_id: '2604.03815'
  title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
    Power of GraphGPS
  date_iso: '2026-04-04'
  venue: ICLR 2026
- arxiv_id: '2509.24886'
  title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
    Networks
  date_iso: '2025-09-29'
  venue: ''
- arxiv_id: '2211.06489'
  title: Equivariance with Learned Canonicalization Functions
  date_iso: '2022-11-11'
  venue: ICML 2022
- arxiv_id: '2002.04999'
  title: Differentiable Graph Module (DGM) for Graph Convolutional Networks
  date_iso: '2020-02-11'
  venue: ''
- arxiv_id: '1801.07829'
  title: Dynamic Graph CNN for Learning on Point Clouds
  date_iso: '2018-01-24'
  venue: ''
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: F1
  default_metric: F1
  higher_is_better: true
  stats:
    num_graphs: null
    avg_nodes: null
    avg_edges: null
    num_classes: 50
  metrics:
  - F1
  - IoU
  - mIoU
  metric_display_names:
  - F1
  - IoU
  - mIoU
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GPS + k-MIP
    model_plain: GPS + k-MIP
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8268
    - null
    - null
    metric_stds:
    - 0.0064
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
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8262
    - null
    - null
    metric_stds:
    - 0.0031
    - null
    - null
  - model: VN-DGCNN
    model_plain: VN-DGCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.814
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: AC-DGCNN
    model_plain: AC-DGCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
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
    - 0.809
    - null
    - null
    metric_stds:
    - 0.007
    - null
    - null
  - model: GPS + BigBird
    model_plain: GPS + BigBird
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7965
    - null
    - null
    metric_stds:
    - 0.0098
    - null
    - null
  - model: DGCNN
    model_plain: DGCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.786
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: CN-DGCNN
    model_plain: CN-DGCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.785
    - null
    - null
    metric_stds:
    - 0.009
    - null
    - null
  - model: GPS + Performer
    model_plain: GPS + Performer
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.7736
    - null
    - null
    metric_stds:
    - 0.0123
    - null
    - null
  - model: GatedGCN
    model_plain: GatedGCN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.762
    - null
    - null
    metric_stds:
    - 0.0032
    - null
    - null
  - model: AC-PointNet
    model_plain: AC-PointNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    - 0.76
    - null
    - null
    metric_stds:
    - 0.006
    - null
    - null
  - model: CN-PointNet
    model_plain: CN-PointNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.736
    - null
    - null
    metric_stds:
    - 0.011
    - null
    - null
  - model: VN-PointNet
    model_plain: VN-PointNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.728
    - null
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GINE
    model_plain: GINE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6457
    - null
    - null
    metric_stds:
    - 0.0035
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
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6301
    - null
    - null
    metric_stds:
    - 0.0017
    - null
    - null
  - model: PointNet++
    model_plain: PointNet++
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    - 0.623
    - null
    - null
    metric_stds:
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
    arxiv_id: '2604.03815'
    title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
      Power of GraphGPS
    date: Apr 4, 2026
    date_iso: '2026-04-04'
    date_display: Apr 2026
    codebase_url: ''
    published_conference: ICLR 2026
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2026
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.6018
    - null
    - null
    metric_stds:
    - 0.0004
    - null
    - null
  - model: PointNet++
    model_plain: PointNet++
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.767
    - null
    metric_stds:
    - null
    - null
    - null
  - model: DGCNN
    model_plain: DGCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.786
    - null
    metric_stds:
    - null
    - null
    - null
  - model: VN-PointNet
    model_plain: VN-PointNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.728
    - null
    metric_stds:
    - null
    - null
    - null
  - model: VN-DGCNN
    model_plain: VN-DGCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.814
    - null
    metric_stds:
    - null
    - null
    - null
  - model: PointCNN
    model_plain: PointCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.714
    - null
    metric_stds:
    - null
    - null
    - null
  - model: ShellNet
    model_plain: ShellNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.771
    - null
    metric_stds:
    - null
    - null
    - null
  - model: RI-Conv
    model_plain: RI-Conv
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.753
    - null
    metric_stds:
    - null
    - null
    - null
  - model: TFN
    model_plain: TFN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.768
    - null
    metric_stds:
    - null
    - null
    - null
  - model: GC-Conv
    model_plain: GC-Conv
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.773
    - null
    metric_stds:
    - null
    - null
    - null
  - model: RI-Framework
    model_plain: RI-Framework
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.794
    - null
    metric_stds:
    - null
    - null
    - null
  - model: CN(frozen)-PointNet
    model_plain: CN(frozen)-PointNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.723
    - null
    metric_stds:
    - null
    - 0.011
    - null
  - model: CN(L)-PointNet
    model_plain: CN(L)-PointNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.734
    - null
    metric_stds:
    - null
    - 0.012
    - null
  - model: CN(NL)-PointNet
    model_plain: CN(NL)-PointNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.736
    - null
    metric_stds:
    - null
    - 0.011
    - null
  - model: CN(frozen)-DGCNN
    model_plain: CN(frozen)-DGCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.782
    - null
    metric_stds:
    - null
    - 0.012
    - null
  - model: CN(L)-DGCNN
    model_plain: CN(L)-DGCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.785
    - null
    metric_stds:
    - null
    - 0.011
    - null
  - model: CN(NL)-DGCNN
    model_plain: CN(NL)-DGCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2211.06489'
    title: Equivariance with Learned Canonicalization Functions
    date: Nov 11, 2022
    date_iso: '2022-11-11'
    date_display: Nov 2022
    codebase_url: ''
    published_conference: ICML 2022
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2022
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.785
    - null
    metric_stds:
    - null
    - 0.009
    - null
  - model: DGCNN
    model_plain: DGCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2002.04999'
    title: Differentiable Graph Module (DGM) for Graph Convolutional Networks
    date: Feb 11, 2020
    date_iso: '2020-02-11'
    date_display: Feb 2020
    codebase_url: https://github.com/lcosmo/DGM_pytorch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - null
    - 0.852
    metric_stds:
    - null
    - null
    - null
  - model: dDGM
    model_plain: dDGM
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2002.04999'
    title: Differentiable Graph Module (DGM) for Graph Convolutional Networks
    date: Feb 11, 2020
    date_iso: '2020-02-11'
    date_display: Feb 2020
    codebase_url: https://github.com/lcosmo/DGM_pytorch
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - null
    - 0.856
    metric_stds:
    - null
    - null
    - null
  - model: PointNet++
    model_plain: PointNet++
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1801.07829'
    title: Dynamic Graph CNN for Learning on Point Clouds
    date: Jan 24, 2018
    date_iso: '2018-01-24'
    date_display: Jan 2018
    codebase_url: https://github.com/WangYueFt/dgcnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - null
    - 0.851
    metric_stds:
    - null
    - null
    - null
  - model: Kd-Net
    model_plain: Kd-Net
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '1801.07829'
    title: Dynamic Graph CNN for Learning on Point Clouds
    date: Jan 24, 2018
    date_iso: '2018-01-24'
    date_display: Jan 2018
    codebase_url: https://github.com/WangYueFt/dgcnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - null
    - 0.823
    metric_stds:
    - null
    - null
    - null
  - model: LocalFeatureNet
    model_plain: LocalFeatureNet
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1801.07829'
    title: Dynamic Graph CNN for Learning on Point Clouds
    date: Jan 24, 2018
    date_iso: '2018-01-24'
    date_display: Jan 2018
    codebase_url: https://github.com/WangYueFt/dgcnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - null
    - 0.843
    metric_stds:
    - null
    - null
    - null
  - model: PCNN
    model_plain: PCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '1801.07829'
    title: Dynamic Graph CNN for Learning on Point Clouds
    date: Jan 24, 2018
    date_iso: '2018-01-24'
    date_display: Jan 2018
    codebase_url: https://github.com/WangYueFt/dgcnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - null
    - 0.851
    metric_stds:
    - null
    - null
    - null
  - model: PointCNN
    model_plain: PointCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1801.07829'
    title: Dynamic Graph CNN for Learning on Point Clouds
    date: Jan 24, 2018
    date_iso: '2018-01-24'
    date_display: Jan 2018
    codebase_url: https://github.com/WangYueFt/dgcnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - null
    - 0.861
    metric_stds:
    - null
    - null
    - null
  - model: EdgeConv
    model_plain: EdgeConv
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1801.07829'
    title: Dynamic Graph CNN for Learning on Point Clouds
    date: Jan 24, 2018
    date_iso: '2018-01-24'
    date_display: Jan 2018
    codebase_url: https://github.com/WangYueFt/dgcnn
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - null
    - 0.852
    metric_stds:
    - null
    - null
    - null
  row_count: 40
  rows_json: ''
  chart_json: /data/datasets/shapenet-part/standard-split-chart.json
  arch_counts:
    gnn: 25
    hybrid: 3
    graph_transformer: 1
    llm: 0
    walk: 0
    traditional: 1
  metric_counts:
  - 16
  - 16
  - 8
  milestones: &id001
  - value: 0.814
    std: null
    model: VN-DGCNN
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: '2025-09-29'
  milestones_by_metric:
    F1: *id001
    IoU: []
    mIoU: []
---

