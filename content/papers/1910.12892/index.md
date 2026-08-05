---
title: Hyperbolic Graph Neural Networks
arxiv_id: '1910.12892'
source_url: ''
authors:
- name: Qi Liu
  orcid: null
  s2_author_id: '2144831836'
  s2_url: null
- name: Maximilian Nickel
  orcid: null
  s2_author_id: '1729762'
  s2_url: null
- name: Douwe Kiela
  orcid: null
  s2_author_id: '1743722'
  s2_url: null
published_date: Oct 28, 2019
published_date_iso: '2019-10-28'
published_venue: NeurIPS 2019
published_conference: NeurIPS 2019
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Learning from graph-structured data is an important task in machine learning
  and artificial intelligence, for which Graph Neural Networks (GNNs) have shown great
  promise. Motivated by recent advances in geometric representation learning, we propose
  a novel GNN architecture for learning representations on Riemannian manifolds with
  differentiable exponential and logarithmic maps. We develop a scalable algorithm
  for modeling the structural properties of graphs, comparing Euclidean and hyperbolic
  geometry. In our experiments, we show that hyperbolic GNNs can lead to substantial
  improvements on various benchmark datasets.
codebase_url: https://github.com/facebookresearch/hgnn
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
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ZINC
  rows:
  - model: TIGT
    model_key: tigt
    model_plain: TIGT
    value: 0.014
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: Feb 3, 2024
    date_display: Feb 2024
    date_iso: '2024-02-03'
    venue: GRaM
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.014
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FloydNet
    model_key: floydnet
    model_plain: FloydNet
    value: 0.016
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_display: Jan 2026
    date_iso: '2026-01-27'
    venue: arXiv.org
    codebase_url: https://github.com/ocx-lab/FloydNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.016
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PST
    model_key: pst
    model_plain: PST
    value: 0.018
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2405.02795'
    title: Graph as Point Set
    date: May 5, 2024
    date_display: May 2024
    date_iso: '2024-05-05'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.018
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Lorentz
    model_key: lorentz
    model_plain: Lorentz
    value: 0.024
    std: 0.0002
    paper_value: 0.024
    paper_std: 0.0002
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'zinc: mae fallback <= 0.06'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-10-28'
    value_gap_source_date_label: NeurIPS 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.024
    true_std: 0.0002
    value_gap_source_arxiv: '1910.12892'
    value_gap_source_title: Hyperbolic Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.024
    sort_std: 0.0002
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    value: 0.041
    std: 0.0002
    paper_value: 0.041
    paper_std: 0.0002
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: gilmer2017neural
    variant_inference_reason: 'zinc: mae fallback <= 0.06'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-27'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.03
    true_std: null
    value_gap_source_arxiv: '2601.19094'
    value_gap_source_title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    value_gap_source_is_current_paper: false
    value_gap: 0.011000000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.03
    sort_std: null
    global_rank: 41
    paper_rank: 52
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Poincare
    model_key: poincare
    model_plain: Poincare
    value: 0.031
    std: 0.0001
    paper_value: 0.031
    paper_std: 0.0001
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'zinc: mae fallback <= 0.06'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-10-28'
    value_gap_source_date_label: NeurIPS 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.031
    true_std: 0.0001
    value_gap_source_arxiv: '1910.12892'
    value_gap_source_title: Hyperbolic Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.031
    sort_std: 0.0001
    global_rank: 43
    paper_rank: 43
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GGNN
    model_key: ggnn
    model_plain: GGNN
    value: 0.032
    std: 0.002
    paper_value: 0.032
    paper_std: 0.002
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: li2016ggnn
    variant_inference_reason: 'zinc: mae fallback <= 0.06'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-10-28'
    value_gap_source_date_label: NeurIPS 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.032
    true_std: 0.002
    value_gap_source_arxiv: '1910.12892'
    value_gap_source_title: Hyperbolic Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.032
    sort_std: 0.002
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Euclidean
    model_key: euclidean
    model_plain: Euclidean
    value: 0.033
    std: 0.0
    paper_value: 0.033
    paper_std: 0.0
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'zinc: mae fallback <= 0.06'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-10-28'
    value_gap_source_date_label: NeurIPS 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.033
    true_std: 0.0
    value_gap_source_arxiv: '1910.12892'
    value_gap_source_title: Hyperbolic Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.033
    sort_std: 0.0
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DTNN
    model_key: dtnn
    model_plain: DTNN
    value: 0.04
    std: 0.0003
    paper_value: 0.04
    paper_std: 0.0003
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: schutt2017quantum
    variant_inference_reason: 'zinc: mae fallback <= 0.06'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2019
    date_display: Oct 2019
    date_iso: '2019-10-28'
    published_venue: NeurIPS 2019
    published_conference: NeurIPS 2019
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-10-28'
    value_gap_source_date_label: NeurIPS 2019
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.04
    true_std: 0.0003
    value_gap_source_arxiv: '1910.12892'
    value_gap_source_title: Hyperbolic Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.04
    sort_std: 0.0003
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.088
    std: 0.002
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.02479'
    title: Using Random Noise Equivariantly to Boost Graph Neural Networks Universally
    date: Feb 4, 2025
    date_display: Feb 2025
    date_iso: '2025-02-04'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 74
    sort_value: 0.088
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: ZINC
      dataset_slug: zinc
main_figure: /figures/1910.12892/main_figure.jpegoptim.jpg
---

