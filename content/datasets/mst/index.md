---
title: MST
slug: mst
benchmark: GraphBench
task_type: graph_classification
description: Minimum Spanning Tree edge prediction (GraphBench / CLRS-style algorithmic
  reasoning).
primary_metric: F1
higher_is_better: true
pyg_url: https://graphbench.github.io/website/datasets.html
stats:
  num_graphs: 21000000
  avg_nodes: 264.0
  avg_edges: 3667.0
  num_classes: null
result_count: 5
best_model:
  model: RRWP
  value: 0.9604
  metric: F1
  arxiv_id: '2511.08028'
  paper_title: Generalizable Insights for Graph Transformers in Theory and Practice
papers:
- arxiv_id: '2511.08028'
  title: Generalizable Insights for Graph Transformers in Theory and Practice
  date_iso: '2025-11-11'
  venue: NeurIPS 2025
variants:
- slug: standard-split
  name: Standard split
  notes: ''
  is_standard: true
  primary_metric: F1
  default_metric: F1
  higher_is_better: true
  stats:
    num_graphs: 21000000
    avg_nodes: 264.0
    avg_edges: 3667.0
    num_classes: null
  metrics:
  - F1
  metric_display_names:
  - F1
  show_all_metrics_desktop: false
  chart_default_log_scale: false
  chart_hidden_models: []
  rows:
  - model: RRWP
    model_plain: RRWP
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.9604
    metric_stds:
    - 0.0091
  - model: RWSE
    model_plain: RWSE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 90.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: true
    is_std_outlier: false
    metric_values:
    - 0.958
    metric_stds:
    - 0.0018
  - model: NoPE
    model_plain: NoPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9329
    metric_stds:
    - 0.0088
  - model: LPE
    model_plain: LPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 90.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9311
    metric_stds:
    - 0.0101
  - model: SPE
    model_plain: SPE
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 16.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: Nov 11, 2025
    date_iso: '2025-11-11'
    date_display: Nov 2025
    codebase_url: https://github.com/GraphPKU/BREC
    published_conference: NeurIPS 2025
    published_conference_short: NeurIPS
    published_conference_slug: neurips
    published_venue: NeurIPS 2025
    uses_external_data: false
    is_best: false
    is_std_outlier: false
    metric_values:
    - 0.9252
    metric_stds:
    - 0.0012
  row_count: 5
  rows_json: ''
  chart_json: /data/datasets/mst/standard-split-chart.json
  arch_counts:
    gnn: 0
    hybrid: 0
    graph_transformer: 5
    llm: 0
    walk: 0
    traditional: 0
  metric_counts:
  - 5
  milestones: &id001
  - value: 0.9604
    std: 0.0091
    model: RRWP
    arxiv_id: '2511.08028'
    title: Generalizable Insights for Graph Transformers in Theory and Practice
    date: '2025-11-11'
  milestones_by_metric:
    F1: *id001
---

