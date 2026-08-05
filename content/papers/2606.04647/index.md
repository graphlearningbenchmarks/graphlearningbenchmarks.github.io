---
title: 'ALINC: Active Learning for Inductive Node Classification via Graph Sampling'
arxiv_id: '2606.04647'
source_url: ''
authors:
- name: Pascal Plettenberg
  orcid: null
  s2_author_id: '2231822885'
  s2_url: null
- name: Denis Huseljic
  orcid: null
  s2_author_id: '25891432'
  s2_url: null
- name: André Alcalde
  orcid: null
  s2_author_id: '2366559484'
  s2_url: null
- name: Bernhard Sick
  orcid: null
  s2_author_id: '2365993150'
  s2_url: null
- name: Josephine M. Thomas
  orcid: null
  s2_author_id: '2310396038'
  s2_url: null
published_date: Jun 3, 2026
published_date_iso: '2026-06-03'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Active learning (AL) for node classification typically focuses on selecting
  the most informative nodes for annotation within one or a few large graphs (e.g.,
  in social network analysis). However, in other domains, such as molecular chemistry
  or electronic design automation, datasets consist of thousands of independent graphs.
  In many of these inductive settings, annotating an individual node requires a full-graph
  analysis, which effectively yields the remaining node labels on-the-fly. Therefore,
  these scenarios require AL strategies that select entire graphs instead of single
  nodes, a problem which has not been tackled in the literature so far. Thus, we introduce
  ALINC, an AL framework for inductive node classification via graph sampling. It
  bridges the existing methodological gap by elevating node-level utility measures
  to graph-level selection criteria through various aggregation mechanisms. In an
  extensive benchmark including ten strategies, three aggregation methods, and four
  datasets, we identify CoreSet, TypiClust, and BADGE as the top-performing graph
  sampling strategies. Our detailed analysis further reveals that the choice of the
  aggregation method is pivotal, as it substantially affects model performance and
  annotation costs. Finally, we demonstrate the effectiveness of ALINC in two use
  case studies: site-of-metabolism prediction in molecules and design automation of
  printed circuit board schematics.'
codebase_url: https://github.com/pasplett/alinc
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- LRGB
- GNNBenchmark
benchmark_coverage:
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 1
  total: 5
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 2
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: CLUSTER
  rows:
  - model: Degree (Max)
    model_key: degree (max)
    model_plain: Degree (Max)
    value: 62.36
    std: 0.26
    paper_value: 62.36
    paper_std: 0.26
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 62.36
    true_std: 0.26
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 62.36
    sort_std: 0.26
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AGE (Mean)
    model_key: age (mean)
    model_plain: AGE (Mean)
    value: 62.31
    std: 0.19
    paper_value: 62.31
    paper_std: 0.19
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 62.31
    true_std: 0.19
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 62.31
    sort_std: 0.19
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CoreSet (Sum)
    model_key: coreset (sum)
    model_plain: CoreSet (Sum)
    value: 62.19
    std: 0.28
    paper_value: 62.19
    paper_std: 0.28
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 62.19
    true_std: 0.28
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 62.19
    sort_std: 0.28
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Node-Density (Sum)
    model_key: node-density (sum)
    model_plain: Node-Density (Sum)
    value: 61.98
    std: 0.28
    paper_value: 61.98
    paper_std: 0.28
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 61.98
    true_std: 0.28
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 61.98
    sort_std: 0.28
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Margin (Sum)
    model_key: margin (sum)
    model_plain: Margin (Sum)
    value: 60.91
    std: 0.16
    paper_value: 60.91
    paper_std: 0.16
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 60.91
    true_std: 0.16
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 60.91
    sort_std: 0.16
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ANRMAB (Sum)
    model_key: anrmab (sum)
    model_plain: ANRMAB (Sum)
    value: 60.74
    std: 0.27
    paper_value: 60.74
    paper_std: 0.27
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 60.74
    true_std: 0.27
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 60.74
    sort_std: 0.27
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TypiClust (Sum)
    model_key: typiclust (sum)
    model_plain: TypiClust (Sum)
    value: 60.58
    std: 0.2
    paper_value: 60.58
    paper_std: 0.2
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 60.58
    true_std: 0.2
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 60.58
    sort_std: 0.2
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Entropy (Sum)
    model_key: entropy (sum)
    model_plain: Entropy (Sum)
    value: 60.57
    std: 0.22
    paper_value: 60.57
    paper_std: 0.22
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 60.57
    true_std: 0.22
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 60.57
    sort_std: 0.22
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BADGE (Sum)
    model_key: badge (sum)
    model_plain: BADGE (Sum)
    value: 60.21
    std: 0.19
    paper_value: 60.21
    paper_std: 0.19
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 60.21
    true_std: 0.19
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 60.21
    sort_std: 0.19
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 59.97
    std: 0.2
    paper_value: 59.97
    paper_std: 0.2
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs with different random seeds
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 59.97
    true_std: 0.2
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 59.97
    sort_std: 0.2
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graph-Density (Mean)
    model_key: graph-density (mean)
    model_plain: Graph-Density (Mean)
    value: 59.48
    std: 0.28
    paper_value: 59.48
    paper_std: 0.28
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 59.48
    true_std: 0.28
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 59.48
    sort_std: 0.28
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AULC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AULC
  metric: AULC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: COCO-SP
  rows:
  - model: ANRMAB (Max)
    model_key: anrmab (max)
    model_plain: ANRMAB (Max)
    value: 6.68
    std: 0.13
    paper_value: 6.68
    paper_std: 0.13
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.68
    true_std: 0.13
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.68
    sort_std: 0.13
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BADGE (Sum)
    model_key: badge (sum)
    model_plain: BADGE (Sum)
    value: 6.68
    std: 0.18
    paper_value: 6.68
    paper_std: 0.18
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.68
    true_std: 0.18
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.68
    sort_std: 0.18
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TypiClust (Mean)
    model_key: typiclust (mean)
    model_plain: TypiClust (Mean)
    value: 6.63
    std: 0.24
    paper_value: 6.63
    paper_std: 0.24
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.63
    true_std: 0.24
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.63
    sort_std: 0.24
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Margin (Max)
    model_key: margin (max)
    model_plain: Margin (Max)
    value: 6.58
    std: 0.21
    paper_value: 6.58
    paper_std: 0.21
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.58
    true_std: 0.21
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.58
    sort_std: 0.21
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graph-Density (Max)
    model_key: graph-density (max)
    model_plain: Graph-Density (Max)
    value: 6.58
    std: 0.27
    paper_value: 6.58
    paper_std: 0.27
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.58
    true_std: 0.27
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.58
    sort_std: 0.27
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AGE (Sum)
    model_key: age (sum)
    model_plain: AGE (Sum)
    value: 6.57
    std: 0.18
    paper_value: 6.57
    paper_std: 0.18
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.57
    true_std: 0.18
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.57
    sort_std: 0.18
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Node-Density (Max)
    model_key: node-density (max)
    model_plain: Node-Density (Max)
    value: 6.55
    std: 0.18
    paper_value: 6.55
    paper_std: 0.18
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.55
    true_std: 0.18
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.55
    sort_std: 0.18
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CoreSet (Mean)
    model_key: coreset (mean)
    model_plain: CoreSet (Mean)
    value: 6.54
    std: 0.16
    paper_value: 6.54
    paper_std: 0.16
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.54
    true_std: 0.16
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.54
    sort_std: 0.16
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 6.45
    std: 0.27
    paper_value: 6.45
    paper_std: 0.27
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs with different random seeds
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.45
    true_std: 0.27
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.45
    sort_std: 0.27
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Degree (Sum)
    model_key: degree (sum)
    model_plain: Degree (Sum)
    value: 6.45
    std: 0.1
    paper_value: 6.45
    paper_std: 0.1
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.45
    true_std: 0.1
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.45
    sort_std: 0.1
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Entropy (Mean)
    model_key: entropy (mean)
    model_plain: Entropy (Mean)
    value: 6.26
    std: 0.15
    paper_value: 6.26
    paper_std: 0.15
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC averaged across 10 runs
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 6.26
    true_std: 0.15
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 6.26
    sort_std: 0.15
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AULC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - AULC
  metric: AULC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id003
  dataset: PATTERN
  rows:
  - model: TypiClust (Sum)
    model_key: typiclust (sum)
    model_plain: TypiClust (Sum)
    value: 81.62
    std: 0.49
    paper_value: 81.62
    paper_std: 0.49
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC (Area Under Learning Curve) measured in % over 10 runs.
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 81.62
    true_std: 0.49
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 81.62
    sort_std: 0.49
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BADGE (Max)
    model_key: badge (max)
    model_plain: BADGE (Max)
    value: 81.5
    std: 0.29
    paper_value: 81.5
    paper_std: 0.29
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC (Area Under Learning Curve) measured in % over 10 runs.
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 81.5
    true_std: 0.29
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 81.5
    sort_std: 0.29
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CoreSet (Mean)
    model_key: coreset (mean)
    model_plain: CoreSet (Mean)
    value: 81.34
    std: 0.69
    paper_value: 81.34
    paper_std: 0.69
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC (Area Under Learning Curve) measured in % over 10 runs.
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 81.34
    true_std: 0.69
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 81.34
    sort_std: 0.69
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graph-Density (Sum)
    model_key: graph-density (sum)
    model_plain: Graph-Density (Sum)
    value: 80.46
    std: 0.81
    paper_value: 80.46
    paper_std: 0.81
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC (Area Under Learning Curve) measured in % over 10 runs.
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 80.46
    true_std: 0.81
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 80.46
    sort_std: 0.81
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Node-Density (Max)
    model_key: node-density (max)
    model_plain: Node-Density (Max)
    value: 80.01
    std: 0.53
    paper_value: 80.01
    paper_std: 0.53
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC (Area Under Learning Curve) measured in % over 10 runs.
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 80.01
    true_std: 0.53
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 80.01
    sort_std: 0.53
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AGE (Max)
    model_key: age (max)
    model_plain: AGE (Max)
    value: 79.89
    std: 1.03
    paper_value: 79.89
    paper_std: 1.03
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC (Area Under Learning Curve) measured in % over 10 runs.
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 79.89
    true_std: 1.03
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 79.89
    sort_std: 1.03
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 79.57
    std: 0.97
    paper_value: 79.57
    paper_std: 0.97
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC (Area Under Learning Curve) measured in % over 10 runs.
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 79.57
    true_std: 0.97
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 79.57
    sort_std: 0.97
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ANRMAB (Sum)
    model_key: anrmab (sum)
    model_plain: ANRMAB (Sum)
    value: 79.53
    std: 0.65
    paper_value: 79.53
    paper_std: 0.65
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC (Area Under Learning Curve) measured in % over 10 runs.
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 79.53
    true_std: 0.65
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 79.53
    sort_std: 0.65
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Degree (Max)
    model_key: degree (max)
    model_plain: Degree (Max)
    value: 79.44
    std: 1.47
    paper_value: 79.44
    paper_std: 1.47
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC (Area Under Learning Curve) measured in % over 10 runs.
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 79.44
    true_std: 1.47
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 79.44
    sort_std: 1.47
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Entropy (Max)
    model_key: entropy (max)
    model_plain: Entropy (Max)
    value: 78.1
    std: 1.77
    paper_value: 78.1
    paper_std: 1.77
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC (Area Under Learning Curve) measured in % over 10 runs.
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 78.1
    true_std: 1.77
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 78.1
    sort_std: 1.77
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Margin (Max)
    model_key: margin (max)
    model_plain: Margin (Max)
    value: 77.7
    std: 1.91
    paper_value: 77.7
    paper_std: 1.91
    metric: AULC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table app:tab:aulc
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: AULC (Area Under Learning Curve) measured in % over 10 runs.
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 77.7
    true_std: 1.91
    value_gap_source_arxiv: '2606.04647'
    value_gap_source_title: 'ALINC: Active Learning for Inductive Node Classification
      via Graph Sampling'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 77.7
    sort_std: 1.91
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AULC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AULC
  metric: AULC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: LRGB
  datasets:
  - *id001
- benchmark: GNNBenchmark
  datasets:
  - *id002
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: COCO-SP
      dataset_slug: coco-sp
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: CLUSTER
      dataset_slug: cluster
    - dataset: PATTERN
      dataset_slug: pattern
main_figure: /figures/2606.04647/main_figure.jpegoptim.jpg
---

