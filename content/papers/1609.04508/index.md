---
title: Column Networks for Collective Classification
arxiv_id: '1609.04508'
source_url: ''
authors:
- name: Trang Pham
  orcid: null
  s2_author_id: '145227897'
  s2_url: null
- name: T. Tran
  orcid: null
  s2_author_id: '6254479'
  s2_url: null
- name: Dinh Q. Phung
  orcid: null
  s2_author_id: '1749657'
  s2_url: null
- name: S. Venkatesh
  orcid: null
  s2_author_id: '143761093'
  s2_url: null
published_date: Sep 15, 2016
published_date_iso: '2016-09-15'
published_venue: AAAI 2016
published_conference: AAAI 2016
published_conference_short: AAAI
published_conference_slug: aaai
abstract: 'Relational learning deals with data that are characterized by relational
  structures. An important task is collective classification, which is to jointly
  classify networked objects. While it holds a great promise to produce a better accuracy
  than non-collective classifiers, collective classification is computationally challenging
  and has not leveraged on the recent breakthroughs of deep learning. We present Column
  Network ($CLN$), a novel deep learning model for collective classification in multi-relational
  domains. $CLN$ has many desirable theoretical properties: (i) it encodes multi-relations
  between any two instances; (ii) it is deep and compact, allowing complex functions
  to be approximated at the network level with a small set of free parameters; (iii)
  local and relational features are learned simultaneously; (iv) long-range, higher-order
  dependencies between instances are supported naturally; and (v) crucially, learning
  and inference are efficient with linear complexity in the size of the network and
  the number of relations. We evaluate $CLN$ on multiple real-world applications:
  (a) delay prediction in software projects, (b) PubMed Diabetes publication classification
  and (c) film genre classification. In all of these applications, $CLN$ demonstrates
  a higher accuracy than state-of-the-art rivals.'
codebase_url: https://github.com/trangptm/Column_networks
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CLN-HWN-full
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: MovieLens Film
  rows:
  - model: CLN-HWN-mini
    model_key: cln-hwn-mini
    model_plain: CLN-HWN-mini
    value: 0.575
    std: null
    paper_value: 0.575
    paper_std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Movie genre classification using Micro-F1 and Macro-F1 metrics.
    date: Sep 15, 2016
    date_display: Sep 2016
    date_iso: '2016-09-15'
    published_venue: AAAI 2016
    published_conference: AAAI 2016
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2016-09-15'
    value_gap_source_date_label: AAAI 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.575
    true_std: null
    value_gap_source_arxiv: '1609.04508'
    value_gap_source_title: Column Networks for Collective Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.575
    sort_std: null
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
  - model: CLN-HWN-full
    model_key: cln-hwn-full
    model_plain: CLN-HWN-full
    value: 0.574
    std: null
    paper_value: 0.574
    paper_std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Movie genre classification using Micro-F1 and Macro-F1 metrics.
    date: Sep 15, 2016
    date_display: Sep 2016
    date_iso: '2016-09-15'
    published_venue: AAAI 2016
    published_conference: AAAI 2016
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2016-09-15'
    value_gap_source_date_label: AAAI 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.574
    true_std: null
    value_gap_source_arxiv: '1609.04508'
    value_gap_source_title: Column Networks for Collective Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.574
    sort_std: null
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CLN-FNN
    model_key: cln-fnn
    model_plain: CLN-FNN
    value: 0.543
    std: null
    paper_value: 0.543
    paper_std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Movie genre classification using Micro-F1 and Macro-F1 metrics.
    date: Sep 15, 2016
    date_display: Sep 2016
    date_iso: '2016-09-15'
    published_venue: AAAI 2016
    published_conference: AAAI 2016
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2016-09-15'
    value_gap_source_date_label: AAAI 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.543
    true_std: null
    value_gap_source_arxiv: '1609.04508'
    value_gap_source_title: Column Networks for Collective Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.543
    sort_std: null
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SL-LR
    model_key: sl-lr
    model_plain: SL-LR
    value: 0.534
    std: null
    paper_value: 0.534
    paper_std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Movie genre classification using Micro-F1 and Macro-F1 metrics.
    date: Sep 15, 2016
    date_display: Sep 2016
    date_iso: '2016-09-15'
    published_venue: AAAI 2016
    published_conference: AAAI 2016
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2016-09-15'
    value_gap_source_date_label: AAAI 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.534
    true_std: null
    value_gap_source_arxiv: '1609.04508'
    value_gap_source_title: Column Networks for Collective Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.534
    sort_std: null
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HWN-noRel
    model_key: hwn-norel
    model_plain: HWN-noRel
    value: 0.508
    std: null
    paper_value: 0.508
    paper_std: null
    metric: Micro-F1
    higher_is_better: true
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Movie genre classification using Micro-F1 and Macro-F1 metrics.
    date: Sep 15, 2016
    date_display: Sep 2016
    date_iso: '2016-09-15'
    published_venue: AAAI 2016
    published_conference: AAAI 2016
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2016-09-15'
    value_gap_source_date_label: AAAI 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.508
    true_std: null
    value_gap_source_arxiv: '1609.04508'
    value_gap_source_title: Column Networks for Collective Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.508
    sort_std: null
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
  - model: nbC-IC
    model_key: nbc-ic
    model_plain: nbC-IC
    value: 0.466
    std: null
    paper_value: 0.466
    paper_std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Movie genre classification using Micro-F1 and Macro-F1 metrics.
    date: Sep 15, 2016
    date_display: Sep 2016
    date_iso: '2016-09-15'
    published_venue: AAAI 2016
    published_conference: AAAI 2016
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2016-09-15'
    value_gap_source_date_label: AAAI 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.466
    true_std: null
    value_gap_source_arxiv: '1609.04508'
    value_gap_source_title: Column Networks for Collective Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.466
    sort_std: null
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
  - model: nbC-RL
    model_key: nbc-rl
    model_plain: nbC-RL
    value: 0.435
    std: null
    paper_value: 0.435
    paper_std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Movie genre classification using Micro-F1 and Macro-F1 metrics.
    date: Sep 15, 2016
    date_display: Sep 2016
    date_iso: '2016-09-15'
    published_venue: AAAI 2016
    published_conference: AAAI 2016
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2016-09-15'
    value_gap_source_date_label: AAAI 2016
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.435
    true_std: null
    value_gap_source_arxiv: '1609.04508'
    value_gap_source_title: Column Networks for Collective Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.435
    sort_std: null
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
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Other Graph Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: MovieLens Film
      dataset_slug: movielens-film
single_proposed_model: CLN-HWN-full
main_figure: /figures/1609.04508/main_figure.jpegoptim.jpg
---

