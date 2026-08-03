---
title: REDDIT-BINARY
slug: reddit-binary
benchmark: TU Dortmund
task_type: graph_classification
description: Binary graph classification of Reddit discussion threads (question-answering
  vs. online discussion).
primary_metric: Accuracy
higher_is_better: true
pyg_url: https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.datasets.TUDataset.html
stats:
  num_graphs: 2000
  avg_nodes: 429.63
  avg_edges: 497.75
  num_classes: 2
result_count: 60
best_model:
  model: GIN-0
  value: 0.924
  metric: Accuracy
  arxiv_id: '2006.05582'
  paper_title: Contrastive Multi-View Representation Learning on Graphs
papers:
- arxiv_id: '2512.12642'
  title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural Networks'
  date_iso: '2025-12-14'
  venue: ''
- arxiv_id: '2508.20597'
  title: Local Virtual Nodes for Alleviating Over-Squashing in Graph Neural Networks
  date_iso: '2025-08-28'
  venue: ''
- arxiv_id: '2407.04236'
  title: Graph Pooling via Ricci Flow
  date_iso: '2024-07-05'
  venue: TMLR 2024
- arxiv_id: '2310.01668'
  title: Locality-Aware Graph Rewiring in GNNs
  date_iso: '2023-10-02'
  venue: ICLR 2023
- arxiv_id: '2306.03698'
  title: Fine-grained Expressivity of Graph Neural Networks
  date_iso: '2023-06-06'
  venue: NeurIPS 2023
- arxiv_id: '2210.11790'
  title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing in GNNs'
  date_iso: '2022-10-21'
  venue: ICLR 2022
- arxiv_id: '2210.00643'
  title: Spectral Augmentation for Self-Supervised Learning on Graphs
  date_iso: '2022-10-02'
  venue: ICLR 2022
- arxiv_id: '2006.05582'
  title: Contrastive Multi-View Representation Learning on Graphs
  date_iso: '2020-06-01'
  venue: ICML 2020
variants:
- slug: 10-fold-cv
  name: 10-fold CV
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 2000
    avg_nodes: 429.63
    avg_edges: 497.75
    num_classes: 2
  metrics:
  - Accuracy
  metric_display_names:
  - Accuracy
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: GIN-0
    model_plain: GIN-0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.05582'
    title: Contrastive Multi-View Representation Learning on Graphs
    date: Jun 1, 2020
    date_iso: '2020-06-01'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.924
    metric_stds:
    - 0.025
  - model: GIN-ε
    model_plain: GIN-ε
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.05582'
    title: Contrastive Multi-View Representation Learning on Graphs
    date: Jun 1, 2020
    date_iso: '2020-06-01'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.922
    metric_stds:
    - 0.023
  - model: bnpool
    model_plain: bnpool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.91
    metric_stds:
    - 0.02
  - model: DMoN
    model_plain: DMoN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.91
    metric_stds:
    - 0.01
  - model: hosc
    model_plain: hosc
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.91
    metric_stds:
    - 0.01
  - model: jbgnn
    model_plain: jbgnn
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.91
    metric_stds:
    - 0.02
  - model: kmis
    model_plain: kmis
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.91
    metric_stds:
    - 0.03
  - model: Last layer FA
    model_plain: Last layer FA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.11790'
    title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing in GNNs'
    date: Oct 21, 2022
    date_iso: '2022-10-21'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9022
    metric_stds:
    - 0.00475
  - model: acc
    model_plain: acc
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9
    metric_stds:
    - 0.03
  - model: ecpool
    model_plain: ecpool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9
    metric_stds:
    - 0.02
  - model: eigen
    model_plain: eigen
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9
    metric_stds:
    - 0.03
  - model: Graclus
    model_plain: Graclus
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9
    metric_stds:
    - 0.02
  - model: lapool
    model_plain: lapool
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9
    metric_stds:
    - 0.01
  - model: MinCut
    model_plain: MinCut
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9
    metric_stds:
    - 0.02
  - model: GIN-m (trained)
    model_plain: GIN-m (trained)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.03698'
    title: Fine-grained Expressivity of Graph Neural Networks
    date: Jun 6, 2023
    date_iso: '2023-06-06'
    date_display: Jun 2023
    codebase_url: https://github.com/nhuang37/finegrain_expressivity_GNN
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8973
    metric_stds:
    - 0.0037
  - model: FoSR
    model_plain: FoSR
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2210.11790'
    title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing in GNNs'
    date: Oct 21, 2022
    date_iso: '2022-10-21'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.89665
    metric_stds:
    - 0.00416
  - model: SEP
    model_plain: SEP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.89
    metric_stds:
    - 0.03
  - model: AD-GCL
    model_plain: AD-GCL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.00643'
    title: Spectral Augmentation for Self-Supervised Learning on Graphs
    date: Oct 2, 2022
    date_iso: '2022-10-02'
    date_display: Oct 2022
    codebase_url: ''
    published_conference: ICLR 2022
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2022
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.8872
    metric_stds:
    - 0.0153
  - model: GCL-SPAN
    model_plain: GCL-SPAN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.00643'
    title: Spectral Augmentation for Self-Supervised Learning on Graphs
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
    - 0.8841
    metric_stds:
    - 0.0112
  - model: ORC
    model_plain: ORC
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.04236'
    title: Graph Pooling via Ricci Flow
    date: Jul 5, 2024
    date_iso: '2024-07-05'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.88
    metric_stds:
    - 0.02
  - model: ASAP
    model_plain: ASAP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.88
    metric_stds:
    - 0.03
  - model: None
    model_plain: None
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.11790'
    title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing in GNNs'
    date: Oct 21, 2022
    date_iso: '2022-10-21'
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
    - 0.87965
    metric_stds:
    - 0.00564
  - model: JOAO
    model_plain: JOAO
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.00643'
    title: Spectral Augmentation for Self-Supervised Learning on Graphs
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
    - 0.8765
    metric_stds:
    - 0.0172
  - model: maxcut
    model_plain: maxcut
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.87
    metric_stds:
    - 0.03
  - model: ndp
    model_plain: ndp
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.87
    metric_stds:
    - 0.02
  - model: pan
    model_plain: pan
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.87
    metric_stds:
    - 0.05
  - model: sag
    model_plain: sag
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.87
    metric_stds:
    - 0.03
  - model: SDRF
    model_plain: SDRF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2210.11790'
    title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing in GNNs'
    date: Oct 21, 2022
    date_iso: '2022-10-21'
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
    - 0.86825
    metric_stds:
    - 0.00523
  - model: No-Pre-Train-GIN
    model_plain: No-Pre-Train-GIN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.00643'
    title: Spectral Augmentation for Self-Supervised Learning on Graphs
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
    - 0.8679
    metric_stds:
    - 0.0204
  - model: MVGRL
    model_plain: MVGRL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.00643'
    title: Spectral Augmentation for Self-Supervised Learning on Graphs
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
    - 0.8624
    metric_stds:
    - 0.0126
  - model: Diff
    model_plain: Diff
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.04236'
    title: Graph Pooling via Ricci Flow
    date: Jul 5, 2024
    date_iso: '2024-07-05'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.86
    metric_stds:
    - 0.02
  - model: topk
    model_plain: topk
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: Dec 14, 2025
    date_iso: '2025-12-14'
    date_display: Dec 2025
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.86
    metric_stds:
    - 0.03
  - model: FoSR
    model_plain: FoSR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.01668'
    title: Locality-Aware Graph Rewiring in GNNs
    date: Oct 2, 2023
    date_iso: '2023-10-02'
    date_display: Oct 2023
    codebase_url: https://github.com/Fedzbar/laser-release
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8593
    metric_stds:
    - 0.02793
  - model: GTR
    model_plain: GTR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.01668'
    title: Locality-Aware Graph Rewiring in GNNs
    date: Oct 2, 2023
    date_iso: '2023-10-02'
    date_display: Oct 2023
    codebase_url: https://github.com/Fedzbar/laser-release
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.857
    metric_stds:
    - 0.02786
  - model: LVN
    model_plain: LVN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2508.20597'
    title: Local Virtual Nodes for Alleviating Over-Squashing in Graph Neural Networks
    date: Aug 28, 2025
    date_iso: '2025-08-28'
    date_display: Aug 2025
    codebase_url: https://github.com/ALLab-Boun/LVN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8562
    metric_stds:
    - 0.0099
  - model: LASER
    model_plain: LASER
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.01668'
    title: Locality-Aware Graph Rewiring in GNNs
    date: Oct 2, 2023
    date_iso: '2023-10-02'
    date_display: Oct 2023
    codebase_url: https://github.com/Fedzbar/laser-release
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.85458
    metric_stds:
    - 0.02827
  - model: GAT
    model_plain: GAT
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.05582'
    title: Contrastive Multi-View Representation Learning on Graphs
    date: Jun 1, 2020
    date_iso: '2020-06-01'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.852
    metric_stds:
    - 0.033
  - model: MinCut
    model_plain: MinCut
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.04236'
    title: Graph Pooling via Ricci Flow
    date: Jul 5, 2024
    date_iso: '2024-07-05'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.85
    metric_stds:
    - 0.02
  - model: DMoN
    model_plain: DMoN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.04236'
    title: Graph Pooling via Ricci Flow
    date: Jul 5, 2024
    date_iso: '2024-07-05'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.85
    metric_stds:
    - 0.02
  - model: TV
    model_plain: TV
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.04236'
    title: Graph Pooling via Ricci Flow
    date: Jul 5, 2024
    date_iso: '2024-07-05'
    date_display: Jul 2024
    codebase_url: ''
    published_conference: TMLR 2024
    published_conference_short: TMLR
    published_conference_slug: tmlr
    published_venue: TMLR 2024
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.85
    metric_stds:
    - 0.03
  - model: BORF
    model_plain: BORF
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.01668'
    title: Locality-Aware Graph Rewiring in GNNs
    date: Oct 2, 2023
    date_iso: '2023-10-02'
    date_display: Oct 2023
    codebase_url: https://github.com/Fedzbar/laser-release
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8492
    metric_stds:
    - 0.02534
  - model: MI
    model_plain: MI
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2006.05582'
    title: Contrastive Multi-View Representation Learning on Graphs
    date: Jun 1, 2020
    date_iso: '2020-06-01'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.845
    metric_stds:
    - 0.006
  - model: InfoGraph
    model_plain: InfoGraph
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2006.05582'
    title: Contrastive Multi-View Representation Learning on Graphs
    date: Jun 1, 2020
    date_iso: '2020-06-01'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.825
    metric_stds:
    - 0.014
  - model: GraphConv-m (trained)
    model_plain: GraphConv-m (trained)
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.03698'
    title: Fine-grained Expressivity of Graph Neural Networks
    date: Jun 6, 2023
    date_iso: '2023-06-06'
    date_display: Jun 2023
    codebase_url: https://github.com/nhuang37/finegrain_expressivity_GNN
    published_conference: NeurIPS 2023
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.824
    metric_stds:
    - 0.0019
  - model: None
    model_plain: None
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.01668'
    title: Locality-Aware Graph Rewiring in GNNs
    date: Oct 2, 2023
    date_iso: '2023-10-02'
    date_display: Oct 2023
    codebase_url: https://github.com/Fedzbar/laser-release
    published_conference: ICLR 2023
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2023
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.81
    metric_stds:
    - 0.02717
  - model: PANDA
    model_plain: PANDA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.20597'
    title: Local Virtual Nodes for Alleviating Over-Squashing in Graph Neural Networks
    date: Aug 28, 2025
    date_iso: '2025-08-28'
    date_display: Aug 2025
    codebase_url: https://github.com/ALLab-Boun/LVN
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.8008
    metric_stds:
    - 0.01241
  - model: DGK
    model_plain: DGK
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    arxiv_id: '2006.05582'
    title: Contrastive Multi-View Representation Learning on Graphs
    date: Jun 1, 2020
    date_iso: '2020-06-01'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.78
    metric_stds:
    - 0.004
  - model: GK
    model_plain: GK
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    arxiv_id: '2006.05582'
    title: Contrastive Multi-View Representation Learning on Graphs
    date: Jun 1, 2020
    date_iso: '2020-06-01'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.773
    metric_stds:
    - 0.002
  - model: DIGL
    model_plain: DIGL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2210.11790'
    title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing in GNNs'
    date: Oct 21, 2022
    date_iso: '2022-10-21'
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
    - 0.76035
    metric_stds:
    - 0.00774
  - model: graph2vec
    model_plain: graph2vec
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2006.05582'
    title: Contrastive Multi-View Representation Learning on Graphs
    date: Jun 1, 2020
    date_iso: '2020-06-01'
    date_display: Jun 2020
    codebase_url: ''
    published_conference: ICML 2020
    published_conference_short: ICML
    published_conference_slug: icml
    published_venue: ICML 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.758
    metric_stds:
    - 0.01
  row_count: 60
  rows_json: /data/datasets/reddit-binary/10-fold-cv-rows.json
  chart_json: /data/datasets/reddit-binary/10-fold-cv-chart.json
  arch_counts:
    gnn: 35
    hybrid: 3
    graph_transformer: 0
    llm: 0
    walk: 2
    traditional: 19
  metric_counts:
  - 60
  milestones: &id001
  - value: 0.8872
    std: 0.0153
    model: AD-GCL
    arxiv_id: '2210.00643'
    title: Spectral Augmentation for Self-Supervised Learning on Graphs
    date: '2022-10-02'
  - value: 0.9022
    std: 0.00475
    model: Last layer FA
    arxiv_id: '2210.11790'
    title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing in GNNs'
    date: '2022-10-21'
  - value: 0.91
    std: 0.02
    model: bnpool
    arxiv_id: '2512.12642'
    title: 'Torch Geometric Pool: the Pytorch library for pooling in Graph Neural
      Networks'
    date: '2025-12-14'
  milestones_by_metric:
    Accuracy: *id001
---

