---
title: Case 1
slug: case-1
benchmark: Power Flow Benchmarks
task_type: graph_regression
description: Power flow analysis on IEEE test case 1 (small power grid, node-level
  regression).
primary_metric: Accuracy
higher_is_better: true
pyg_url: ''
stats:
  num_graphs: 1000000
  avg_nodes: null
  avg_edges: null
  num_classes: null
result_count: 17
best_model:
  model: RMGL
  value: 0.9987
  metric: Accuracy
  arxiv_id: '2601.01387'
  paper_title: Power Flow Benchmarks
papers:
- arxiv_id: '2601.01387'
  title: Power Flow Benchmarks
  date_iso: '2026-01-04'
  venue: ''
- arxiv_id: '2009.01411'
  title: Learning from Protein Structure with Geometric Vector Perceptrons
  date_iso: '2020-09-03'
  venue: ICLR 2020
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: Accuracy
  default_metric: Accuracy
  higher_is_better: true
  stats:
    num_graphs: 1000000
    avg_nodes: null
    avg_edges: null
    num_classes: null
  metrics:
  - Accuracy
  - Pearson correlation
  metric_display_names:
  - Accuracy
  - Pearson correlation
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: RMGL
    model_plain: RMGL
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9987
    - null
    metric_stds:
    - null
    - null
  - model: MGL
    model_plain: MGL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9964
    - null
    metric_stds:
    - null
    - null
  - model: GLR
    model_plain: GLR
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9963
    - null
    metric_stds:
    - null
    - null
  - model: GLP
    model_plain: GLP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: Jan 4, 2026
    date_iso: '2026-01-04'
    date_display: Jan 2026
    codebase_url: ''
    published_conference: ''
    published_conference_short: ''
    published_conference_slug: ''
    published_venue: ''
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9954
    - null
    metric_stds:
    - null
    - null
  - model: GVP-GNN
    model_plain: GVP-GNN
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.888
    metric_stds:
    - null
    - null
  - model: ProQ3D
    model_plain: ProQ3D
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.847
    metric_stds:
    - null
    - null
  - model: SASHAN
    model_plain: SASHAN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.84
    metric_stds:
    - null
    - null
  - model: FaeNNz
    model_plain: FaeNNz
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.81
    metric_stds:
    - null
    - null
  - model: VoroMQA-A
    model_plain: VoroMQA-A
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.744
    metric_stds:
    - null
    - null
  - model: VoroMQA-B
    model_plain: VoroMQA-B
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.726
    metric_stds:
    - null
    - null
  - model: MULTICOM-NOVEL
    model_plain: MULTICOM-NOVEL
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.652
    metric_stds:
    - null
    - null
  - model: ProQ4
    model_plain: ProQ4
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.691
    metric_stds:
    - null
    - null
  - model: 3DCNN
    model_plain: 3DCNN
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.61
    metric_stds:
    - null
    - null
  - model: Ornate
    model_plain: Ornate
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.67
    metric_stds:
    - null
    - null
  - model: GraphQA
    model_plain: GraphQA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.81
    metric_stds:
    - null
    - null
  - model: VoroMQA
    model_plain: VoroMQA
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.61
    metric_stds:
    - null
    - null
  - model: SBROD
    model_plain: SBROD
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2009.01411'
    title: Learning from Protein Structure with Geometric Vector Perceptrons
    date: Sep 3, 2020
    date_iso: '2020-09-03'
    date_display: Sep 2020
    codebase_url: https://github.com/drorlab/gvp
    published_conference: ICLR 2020
    published_conference_short: ICLR
    published_conference_slug: iclr
    published_venue: ICLR 2020
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - null
    - 0.64
    metric_stds:
    - null
    - null
  row_count: 17
  rows_json: ''
  chart_json: /data/datasets/case-1/standard-split-chart.json
  arch_counts:
    gnn: 5
    hybrid: 1
    graph_transformer: 0
    llm: 0
    walk: 0
    traditional: 11
  metric_counts:
  - 4
  - 13
  milestones: &id001
  - value: 0.9987
    std: null
    model: RMGL
    arxiv_id: '2601.01387'
    title: Power Flow Benchmarks
    date: '2026-01-04'
  milestones_by_metric:
    Accuracy: *id001
    Pearson correlation:
    - value: 0.888
      std: null
      model: GVP-GNN
      arxiv_id: '2009.01411'
      title: Learning from Protein Structure with Geometric Vector Perceptrons
      date: '2020-09-03'
---

