---
title: On Graph Neural Networks versus Graph-Augmented MLPs
arxiv_id: '2010.15116'
source_url: ''
authors:
- name: Lei Chen
  orcid: null
  s2_author_id: '143891665'
  s2_url: null
- name: Zhengdao Chen
  orcid: null
  s2_author_id: '8157979'
  s2_url: null
- name: Joan Bruna
  orcid: null
  s2_author_id: '1589786778'
  s2_url: null
published_date: Oct 28, 2020
published_date_iso: '2020-10-28'
published_venue: ICLR 2020
published_conference: ICLR 2020
published_conference_short: ICLR
published_conference_slug: iclr
abstract: From the perspective of expressive power, this work compares multi-layer
  Graph Neural Networks (GNNs) with a simplified alternative that we call Graph-Augmented
  Multi-Layer Perceptrons (GA-MLPs), which first augments node features with certain
  multi-hop operators on the graph and then applies an MLP in a node-wise fashion.
  From the perspective of graph isomorphism testing, we show both theoretically and
  numerically that GA-MLPs with suitable operators can distinguish almost all non-isomorphic
  graphs, just like the Weifeiler-Lehman (WL) test. However, by viewing them as node-level
  functions and examining the equivalence classes they induce on rooted graphs, we
  prove a separation in expressive power between GA-MLPs and GNNs that grows exponentially
  in depth. In particular, unlike GNNs, GA-MLPs are unable to count the number of
  attributed walks. We also demonstrate via community detection experiments that GA-MLPs
  can be limited by their choice of operator family, as compared to GNNs with higher
  flexibility in learning.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MLP
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 2
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: COLLAB
  rows:
  - model: GNN
    model_key: gnn
    model_plain: GNN
    value: 294.0
    std: null
    paper_value: 294.0
    paper_std: null
    metric: equivalence classes
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2020
    date_display: Oct 2020
    date_iso: '2020-10-28'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 294.0
    sort_std: null
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GA-MLP
    model_key: ga-mlp
    model_plain: GA-MLP
    value: 294.0
    std: null
    paper_value: 294.0
    paper_std: null
    metric: equivalence classes
    higher_is_better: false
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2020
    date_display: Oct 2020
    date_iso: '2020-10-28'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 294.0
    sort_std: null
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  rank_metric: equivalence classes
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - equivalence classes
  metric: equivalence classes
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: IMDB-MULTI
  rows:
  - model: GNN
    model_key: gnn
    model_plain: GNN
    value: 387.0
    std: null
    paper_value: 387.0
    paper_std: null
    metric: equivalence classes
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
    variant_inference_reason: 'dataset: fuzzy match to imdb-multi (score=95)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2020
    date_display: Oct 2020
    date_iso: '2020-10-28'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 387.0
    sort_std: null
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GA-MLP
    model_key: ga-mlp
    model_plain: GA-MLP
    value: 387.0
    std: null
    paper_value: 387.0
    paper_std: null
    metric: equivalence classes
    higher_is_better: false
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to imdb-multi (score=95)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Oct 28, 2020
    date_display: Oct 2020
    date_iso: '2020-10-28'
    published_venue: ICLR 2020
    published_conference: ICLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 387.0
    sort_std: null
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  rank_metric: equivalence classes
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - equivalence classes
  metric: equivalence classes
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: COLLAB
      dataset_slug: collab
    - dataset: IMDB-MULTI
      dataset_slug: imdb-multi
single_proposed_model: MLP
---

