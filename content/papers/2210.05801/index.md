---
title: Linkless Link Prediction via Relational Distillation
arxiv_id: '2210.05801'
source_url: ''
authors:
- name: Zhichun Guo
  orcid: null
  s2_author_id: '2109411071'
  s2_url: null
- name: William Shiao
  orcid: null
  s2_author_id: '2094369655'
  s2_url: null
- name: Shichang Zhang
  orcid: null
  s2_author_id: '2145408511'
  s2_url: null
- name: Yozen Liu
  orcid: null
  s2_author_id: '152891495'
  s2_url: null
- name: N. Chawla
  orcid: null
  s2_author_id: '144539424'
  s2_url: null
- name: Neil Shah
  orcid: null
  s2_author_id: '145474474'
  s2_url: null
- name: Tong Zhao
  orcid: null
  s2_author_id: '1742573'
  s2_url: null
published_date: Oct 11, 2022
published_date_iso: '2022-10-11'
published_venue: ICML 2022
published_conference: ICML 2022
published_conference_short: ICML
published_conference_slug: icml
abstract: Graph Neural Networks (GNNs) have shown exceptional performance in the task
  of link prediction. Despite their effectiveness, the high latency brought by non-trivial
  neighborhood data dependency limits GNNs in practical deployments. Conversely, the
  known efficient MLPs are much less effective than GNNs due to the lack of relational
  knowledge. In this work, to combine the advantages of GNNs and MLPs, we start with
  exploring direct knowledge distillation (KD) methods for link prediction, i.e.,
  predicted logit-based matching and node representation-based matching. Upon observing
  direct KD analogs do not perform well for link prediction, we propose a relational
  KD framework, Linkless Link Prediction (LLP), to distill knowledge for link prediction
  with MLPs. Unlike simple KD methods that match independent link logits or node representations,
  LLP distills relational knowledge that is centered around each (anchor) node to
  the student MLP. Specifically, we propose rank-based matching and distribution-based
  matching strategies that complement each other. Extensive experiments demonstrate
  that LLP boosts the link prediction performance of MLPs with significant margins,
  and even outperforms the teacher GNNs on 7 out of 8 benchmarks. LLP also achieves
  a 70.68x speedup in link prediction inference compared to GNNs on the large-scale
  OGB dataset.
codebase_url: https://github.com/snap-research/linkless-link-prediction
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- LLP
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id001
  dataset: ogbl-citation2
  rows:
  - model: GNN
    model_key: gnn
    model_plain: GNN
    value: 0.8256
    std: null
    paper_value: 0.8256
    paper_std: null
    metric: Hits@200
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbl-citation2 (score=78)'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction performance reported as Hits@200
    date: Oct 11, 2022
    date_display: Oct 2022
    date_iso: '2022-10-11'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-11'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8256
    true_std: null
    value_gap_source_arxiv: '2210.05801'
    value_gap_source_title: Linkless Link Prediction via Relational Distillation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8256
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
  - model: LLP
    model_key: llp
    model_plain: LLP
    value: 0.532
    std: null
    paper_value: 0.532
    paper_std: null
    metric: Hits@200
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbl-citation2 (score=78)'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction performance reported as Hits@200
    date: Oct 11, 2022
    date_display: Oct 2022
    date_iso: '2022-10-11'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-11'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.532
    true_std: null
    value_gap_source_arxiv: '2210.05801'
    value_gap_source_title: Linkless Link Prediction via Relational Distillation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.532
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.4056
    std: null
    paper_value: 0.4056
    paper_std: null
    metric: Hits@200
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbl-citation2 (score=78)'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Link prediction performance reported as Hits@200
    date: Oct 11, 2022
    date_display: Oct 2022
    date_iso: '2022-10-11'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-11'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4056
    true_std: null
    value_gap_source_arxiv: '2210.05801'
    value_gap_source_title: Linkless Link Prediction via Relational Distillation
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4056
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
  rank_metric: Hits@200
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - Hits@200
  metric: Hits@200
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbl-citation2
      dataset_slug: ogbl-citation2
single_proposed_model: LLP
---

