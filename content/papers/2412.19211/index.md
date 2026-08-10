---
title: 'Large Language Models Meet Graph Neural Networks: A Perspective of Graph Mining'
arxiv_id: '2412.19211'
source_url: ''
authors:
- name: Yuxin You
  orcid: null
  s2_author_id: '2338253947'
  s2_url: null
- name: Zhen Liu
  orcid: null
  s2_author_id: '2265977268'
  s2_url: null
- name: Xiangchao Wen
  orcid: null
  s2_author_id: '2338051900'
  s2_url: null
- name: Yongtao Zhang
  orcid: null
  s2_author_id: '2337763948'
  s2_url: null
- name: Wei Ai
  orcid: null
  s2_author_id: '2364679286'
  s2_url: null
published_date: Dec 26, 2024
published_date_iso: '2024-12-26'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph mining is an important area in data mining and machine learning that
  involves extracting valuable information from graph-structured data. In recent years,
  significant progress has been made in this field through the development of graph
  neural networks (GNNs). However, GNNs are still deficient in generalizing to diverse
  graph data. Aiming to this issue, Large Language Models (LLMs) could provide new
  solutions for graph mining tasks with their superior semantic understanding. In
  this review, we systematically review the combination and application techniques
  of LLMs and GNNs and present a novel taxonomy for research in this interdisciplinary
  field, which involves three main categories: GNN-driving-LLM, LLM-driving-GNN, and
  GNN-LLM-co-driving. Within this framework, we reveal the capabilities of LLMs in
  enhancing graph feature extraction as well as improving the effectiveness of downstream
  tasks such as node classification, link prediction, and community detection. Although
  LLMs have demonstrated their great potential in handling graph-structured data,
  their high computational requirements and complexity remain challenges. Future research
  needs to continue to explore how to efficiently fuse LLMs and GNNs to achieve more
  powerful graph learning and reasoning capabilities and provide new impetus for the
  development of graph mining techniques.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Amazon-Photo
  is_multi_metric: true
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    metric_values:
    - 0.9703
    - null
    metric_stds:
    - 0.0019
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    published_venue: ''
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.9703
    sort_std: 0.0019
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.9669
    - null
    metric_stds:
    - 0.0014
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    published_venue: ''
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.9669
    sort_std: 0.0014
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DAM-GT
    model_key: dam-gt
    model_plain: DAM-GT
    metric_values:
    - 0.9666
    - null
    metric_stds:
    - 0.0013
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    published_venue: ''
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.9666
    sort_std: 0.0013
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - 0.9643
    - null
    metric_stds:
    - 0.0027
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    published_venue: ''
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    is_global_top: true
    global_rank: 8
    is_best: false
    sort_value: 0.9643
    sort_std: 0.0027
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.9128
    - null
    metric_stds:
    - 0.0063
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    published_venue: ''
    date: Jun 4, 2023
    date_display: Jun 2023
    date_iso: '2023-06-04'
    codebase_url: https://github.com/GISec-Team/NCGNN
    uses_external_data: false
    is_global_top: true
    global_rank: 426
    is_best: false
    sort_value: 0.9128
    sort_std: 0.0063
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: PATTON
    model_key: patton
    model_plain: PATTON
    metric_values:
    - 0.786
    - 0.786
    metric_stds:
    - 0.0015
    - 0.0015
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    sort_value: 0.786
    sort_std: 0.0015
    true_value: 0.786
    true_std: 0.0015
    paper_value: 0.786
    paper_std: 0.0015
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2412.19211'
    value_gap_source_title: 'Large Language Models Meet Graph Neural Networks: A Perspective
      of Graph Mining'
    value_note: ''
    at_pub_value: 0.7598
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2406.12052'
    at_pub_source_title: 'UniGLM: Training One Unified Language Model for Text-Attributed
      Graph Embedding'
    at_pub_source_date_iso: '2024-06-17'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-12-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0262
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Dec 26, 2024
    date_display: Dec 2024
    date_iso: '2024-12-26'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: improved
    comparison_source_title: 'UniGLM: Training One Unified Language Model for Text-Attributed
      Graph Embedding'
    comparison_source_arxiv: '2406.12052'
    is_best: false
    is_std_outlier: false
    global_rank: 587
  metrics:
  - Accuracy
  - Recall
  primary_metric: Accuracy
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  - Recall
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
main_figure: /figures/2412.19211/main_figure.jpegoptim.jpg
---

