---
title: Graph is a Substrate Across Data Modalities
arxiv_id: '2601.22384'
source_url: ''
authors:
- name: Ziming Li
  orcid: null
  s2_author_id: '2258698077'
  s2_url: null
- name: Xiao-Ming Wu
  orcid: null
  s2_author_id: '2306079575'
  s2_url: null
- name: Zehong Wang
  orcid: null
  s2_author_id: '2284578810'
  s2_url: null
- name: Jiazheng Li
  orcid: null
  s2_author_id: '2260817933'
  s2_url: null
- name: Yijun Tian
  orcid: null
  s2_author_id: '2355580074'
  s2_url: null
- name: Jinhe Bi
  orcid: null
  s2_author_id: '2267727908'
  s2_url: null
- name: Yunpu Ma
  orcid: null
  s2_author_id: '2375151391'
  s2_url: null
- name: Yanfang Ye
  orcid: null
  s2_author_id: '2347872280'
  s2_url: null
- name: Chuxu Zhang
  orcid: null
  s2_author_id: '2117879943'
  s2_url: null
published_date: Jan 29, 2026
published_date_iso: '2026-01-29'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graphs provide a natural representation of relational structure that arises
  across diverse domains. Despite this ubiquity, graph structure is typically learned
  in a modality- and task-isolated manner, where graph representations are constructed
  within individual task contexts and discarded thereafter. As a result, structural
  regularities across modalities and tasks are repeatedly reconstructed rather than
  accumulated at the level of intermediate graph representations. This motivates a
  representation-learning question: how should graph structure be organized so that
  it can persist and accumulate across heterogeneous modalities and tasks? We adopt
  a representation-centric perspective in which graph structure is treated as a structural
  substrate that persists across learning contexts. To instantiate this perspective,
  we propose G-Substrate, a graph substrate framework that organizes learning around
  shared graph structures. G-Substrate comprises two complementary mechanisms: a unified
  structural schema that ensures compatibility among graph representations across
  heterogeneous modalities and tasks, and an interleaved role-based training strategy
  that exposes the same graph structure to multiple functional roles during learning.
  Experiments across multiple domains, modalities, and tasks show that G-Substrate
  outperforms task-isolated and naive multi-task learning methods. The codebase, model,
  and datasets are available at https://github.com/zmli6/G-Substrate.'
codebase_url: https://github.com/zmli6/G-Substrate
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- G-Substrate
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- GraphBench
benchmark_coverage:
- benchmark: GraphBench
  benchmark_slug: graphbench
  evaluated: 1
  total: 5
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: Algorithmic Reasoning
  rows:
  - model: Naive multi-task
    model_key: naive multi-task
    model_plain: Naive multi-task
    value: 0.9971
    std: null
    paper_value: 0.9971
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Connectivity task
    date: Jan 29, 2026
    date_display: Jan 2026
    date_iso: '2026-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-29'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9971
    true_std: null
    value_gap_source_arxiv: '2601.22384'
    value_gap_source_title: Graph is a Substrate Across Data Modalities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9971
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
  - model: Naive single-task
    model_key: naive single-task
    model_plain: Naive single-task
    value: 0.9944
    std: null
    paper_value: 0.9944
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Connectivity task
    date: Jan 29, 2026
    date_display: Jan 2026
    date_iso: '2026-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-29'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9944
    true_std: null
    value_gap_source_arxiv: '2601.22384'
    value_gap_source_title: Graph is a Substrate Across Data Modalities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9944
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
  - model: G-Substrate
    model_key: g-substrate
    model_plain: G-Substrate
    value: 0.9841
    std: null
    paper_value: 0.9841
    paper_std: null
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Connectivity task
    date: Jan 29, 2026
    date_display: Jan 2026
    date_iso: '2026-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-29'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9841
    true_std: null
    value_gap_source_arxiv: '2601.22384'
    value_gap_source_title: Graph is a Substrate Across Data Modalities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9841
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
  - model: Naive multi-task + interleave
    model_key: naive multi-task + interleave
    model_plain: Naive multi-task + interleave
    value: 0.9827
    std: null
    paper_value: 0.9827
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Connectivity task
    date: Jan 29, 2026
    date_display: Jan 2026
    date_iso: '2026-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-29'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9827
    true_std: null
    value_gap_source_arxiv: '2601.22384'
    value_gap_source_title: Graph is a Substrate Across Data Modalities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9827
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
  - model: GITA
    model_key: gita
    model_plain: GITA
    value: 0.9817
    std: null
    paper_value: 0.9817
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Wei et al. 2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Connectivity task
    date: Jan 29, 2026
    date_display: Jan 2026
    date_iso: '2026-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-29'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9817
    true_std: null
    value_gap_source_arxiv: '2601.22384'
    value_gap_source_title: Graph is a Substrate Across Data Modalities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9817
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
  - model: Unified multi-task
    model_key: unified multi-task
    model_plain: Unified multi-task
    value: 0.9809
    std: null
    paper_value: 0.9809
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Connectivity task
    date: Jan 29, 2026
    date_display: Jan 2026
    date_iso: '2026-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-29'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9809
    true_std: null
    value_gap_source_arxiv: '2601.22384'
    value_gap_source_title: Graph is a Substrate Across Data Modalities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9809
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
  - model: Unified single-task
    model_key: unified single-task
    model_plain: Unified single-task
    value: 0.978
    std: null
    paper_value: 0.978
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Connectivity task
    date: Jan 29, 2026
    date_display: Jan 2026
    date_iso: '2026-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-29'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.978
    true_std: null
    value_gap_source_arxiv: '2601.22384'
    value_gap_source_title: Graph is a Substrate Across Data Modalities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.978
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
  - model: G-Wiz
    model_key: g-wiz
    model_plain: G-Wiz
    value: 0.9774
    std: null
    paper_value: 0.9774
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: KDD 2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Connectivity task
    date: Jan 29, 2026
    date_display: Jan 2026
    date_iso: '2026-01-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-29'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9774
    true_std: null
    value_gap_source_arxiv: '2601.22384'
    value_gap_source_title: Graph is a Substrate Across Data Modalities
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9774
    sort_std: null
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: GraphBench
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: GraphBench
    benchmark_slug: graphbench
    datasets:
    - dataset: Algorithmic Reasoning
      dataset_slug: algorithmic-reasoning
single_proposed_model: G-Substrate
---

