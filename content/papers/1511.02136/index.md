---
title: Diffusion-Convolutional Neural Networks
arxiv_id: '1511.02136'
source_url: ''
authors:
- name: James Atwood
  orcid: null
  s2_author_id: '144585309'
  s2_url: null
- name: D. Towsley
  orcid: null
  s2_author_id: '1705427'
  s2_url: null
published_date: Nov 6, 2015
published_date_iso: '2015-11-06'
published_venue: NeurIPS 2015
published_conference: NeurIPS 2015
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: We present diffusion-convolutional neural networks (DCNNs), a new model
  for graph-structured data. Through the introduction of a diffusion-convolution operation,
  we show how diffusion-based representations can be learned from graph-structured
  data and used as an effective basis for node classification. DCNNs have several
  attractive qualities, including a latent representation for graphical data that
  is invariant under isomorphism, as well as polynomial-time prediction and learning
  that can be represented as tensor operations and efficiently implemented on the
  GPU. Through several experiments with real structured datasets, we demonstrate that
  DCNNs are able to outperform probabilistic relational models and kernel-on-graph
  methods at relational node classification tasks.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- 5-hop DCNN
- DCNNs
mrr: 0.0031
adjusted_mrr: 0.001
mrr_dataset_count: 1
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ENZYMES
  is_multi_metric: true
  rows:
  - model: WL
    model_key: bgnn(m)-cs
    model_plain: WL
    metric_values:
    - 0.8068
    - null
    - null
    metric_stds:
    - 0.0149
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    published_venue: ''
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.8068
    sort_std: 0.0149
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
  - model: WL
    model_key: bgnn
    model_plain: WL
    metric_values:
    - 0.7936
    - null
    - null
    metric_stds:
    - 0.0281
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    published_venue: ''
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.7936
    sort_std: 0.0281
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
  - model: WL
    model_key: bgnn(m)-sc
    model_plain: WL
    metric_values:
    - 0.7889
    - null
    - null
    metric_stds:
    - 0.0079
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    published_venue: ''
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: true
    sort_value: 0.7889
    sort_std: 0.0079
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
  - model: deepwl
    model_key: deepwl
    model_plain: deepwl
    metric_values:
    - 0.2155
    - 0.2155
    - 0.1431
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5343
    sort_std: null
    true_value: 0.5343
    true_std: null
    paper_value: 0.2155
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.3188
    value_gap_source_arxiv: '1704.02901'
    value_gap_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-04-10'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2015
    date: Nov 6, 2015
    date_display: Nov 2015
    date_iso: '2015-11-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 167
  - model: l2logistic
    model_key: l2logistic
    model_plain: l2logistic
    metric_values:
    - 0.203
    - 0.203
    - 0.111
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.203
    sort_std: null
    true_value: 0.203
    true_std: null
    paper_value: 0.203
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '1511.02136'
    value_gap_source_title: Diffusion-Convolutional Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2015-11-06'
    value_gap_source_date_label: NeurIPS 2015
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2015
    date: Nov 6, 2015
    date_display: Nov 2015
    date_iso: '2015-11-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The inputs to the logistic regression models are the
      node features alone
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 319
  - model: 5-hop DCNN
    model_key: 5-hop dcnn
    model_plain: 5-hop DCNN
    metric_values:
    - 0.181
    - 0.181
    - 0.0991
    metric_stds:
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.181
    sort_std: null
    true_value: 0.181
    true_std: null
    paper_value: 0.181
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '1511.02136'
    value_gap_source_title: Diffusion-Convolutional Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2015-11-06'
    value_gap_source_date_label: NeurIPS 2015
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2015
    date: Nov 6, 2015
    date_display: Nov 2015
    date_iso: '2015-11-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 322
  - model: l1logistic
    model_key: l1logistic
    model_plain: l1logistic
    metric_values:
    - 0.164
    - 0.164
    - 0.0904
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.164
    sort_std: null
    true_value: 0.164
    true_std: null
    paper_value: 0.164
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '1511.02136'
    value_gap_source_title: Diffusion-Convolutional Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2015-11-06'
    value_gap_source_date_label: NeurIPS 2015
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2015
    date: Nov 6, 2015
    date_display: Nov 2015
    date_iso: '2015-11-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The inputs to the logistic regression models are the
      node features alone
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 324
  - model: DCNNs
    model_key: dcnns
    model_plain: DCNNs
    metric_values:
    - 0.159
    - 0.159
    - 0.0809
    metric_stds:
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.159
    sort_std: null
    true_value: 0.159
    true_std: null
    paper_value: 0.159
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '1511.02136'
    value_gap_source_title: Diffusion-Convolutional Neural Networks
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2015-11-06'
    value_gap_source_date_label: NeurIPS 2015
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2015
    date: Nov 6, 2015
    date_display: Nov 2015
    date_iso: '2015-11-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: unknown
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 325
  metrics:
  - Accuracy
  - F (micro)
  - F (macro)
  primary_metric: Accuracy
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  - F (micro)
  - F (macro)
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: ENZYMES
      dataset_slug: enzymes
main_figure: /figures/1511.02136/main_figure.jpegoptim.jpg
---

