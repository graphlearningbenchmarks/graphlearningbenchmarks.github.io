---
title: Graph Prototypical Networks for Few-shot Learning on Attributed Networks
arxiv_id: '2006.12739'
source_url: ''
authors:
- name: Kaize Ding
  orcid: null
  s2_author_id: '66807781'
  s2_url: null
- name: Jianling Wang
  orcid: null
  s2_author_id: '46584367'
  s2_url: null
- name: Jundong Li
  orcid: null
  s2_author_id: '2040455'
  s2_url: null
- name: Kai Shu
  orcid: null
  s2_author_id: '145800151'
  s2_url: null
- name: Chenghao Liu
  orcid: null
  s2_author_id: '2039481'
  s2_url: null
- name: Huan Liu
  orcid: null
  s2_author_id: '145896397'
  s2_url: null
published_date: Jun 23, 2020
published_date_iso: '2020-06-23'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Attributed networks nowadays are ubiquitous in a myriad of high-impact
  applications, such as social network analysis, financial fraud detection, and drug
  discovery. As a central analytical task on attributed networks, node classification
  has received much attention in the research community. In real-world attributed
  networks, a large portion of node classes only contains limited labeled instances,
  rendering a long-tail node class distribution. Existing node classification algorithms
  are unequipped to handle the few-shot node classes. As a remedy, few-shot learning
  has attracted a surge of attention in the research community. Yet, few-shot node
  classification remains a challenging problem as we need to address the following
  questions: (i) How to extract meta-knowledge from an attributed network for few-shot
  node classification? (ii) How to identify the informativeness of each labeled instance
  for building a robust and effective model? To answer these questions, in this paper,
  we propose a graph meta-learning framework -- Graph Prototypical Networks (GPN).
  By constructing a pool of semi-supervised node classification tasks to mimic the
  real test environment, GPN is able to perform meta-learning on an attributed network
  and derive a highly generalizable model for handling the target classification task.
  Extensive experiments demonstrate the superior capability of GPN in few-shot node
  classification.'
codebase_url: https://github.com/kaize0409/GPN_Graph-Few-shot
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GPN
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 13
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Amazon-ratings
  rows:
  - model: GPN
    model_key: gpn
    model_plain: GPN
    value: 0.786
    std: null
    paper_value: 0.786
    paper_std: null
    metric: ACC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-ratings (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 5-way 5-shot meta-test task
    date: Jun 23, 2020
    date_display: Jun 2020
    date_iso: '2020-06-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-23'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.786
    true_std: null
    value_gap_source_arxiv: '2006.12739'
    value_gap_source_title: Graph Prototypical Networks for Few-shot Learning on Attributed
      Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.786
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
  - model: Meta-GNN
    model_key: meta-gnn
    model_plain: Meta-GNN
    value: 0.773
    std: null
    paper_value: 0.773
    paper_std: null
    metric: ACC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-ratings (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 5-way 5-shot meta-test task
    date: Jun 23, 2020
    date_display: Jun 2020
    date_iso: '2020-06-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-23'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.773
    true_std: null
    value_gap_source_arxiv: '2006.12739'
    value_gap_source_title: Graph Prototypical Networks for Few-shot Learning on Attributed
      Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.773
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
  - model: MAML
    model_key: maml
    model_plain: MAML
    value: 0.661
    std: null
    paper_value: 0.661
    paper_std: null
    metric: ACC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-ratings (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 5-way 5-shot meta-test task
    date: Jun 23, 2020
    date_display: Jun 2020
    date_iso: '2020-06-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-23'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.661
    true_std: null
    value_gap_source_arxiv: '2006.12739'
    value_gap_source_title: Graph Prototypical Networks for Few-shot Learning on Attributed
      Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.661
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
  - model: PN
    model_key: pn
    model_plain: PN
    value: 0.635
    std: null
    paper_value: 0.635
    paper_std: null
    metric: ACC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-ratings (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 5-way 5-shot meta-test task
    date: Jun 23, 2020
    date_display: Jun 2020
    date_iso: '2020-06-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-23'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.635
    true_std: null
    value_gap_source_arxiv: '2006.12739'
    value_gap_source_title: Graph Prototypical Networks for Few-shot Learning on Attributed
      Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.635
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
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.622
    std: null
    paper_value: 0.622
    paper_std: null
    metric: ACC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-ratings (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 5-way 5-shot meta-test task
    date: Jun 23, 2020
    date_display: Jun 2020
    date_iso: '2020-06-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-23'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.622
    true_std: null
    value_gap_source_arxiv: '2006.12739'
    value_gap_source_title: Graph Prototypical Networks for Few-shot Learning on Attributed
      Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.622
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.593
    std: null
    paper_value: 0.593
    paper_std: null
    metric: ACC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-ratings (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 5-way 5-shot meta-test task
    date: Jun 23, 2020
    date_display: Jun 2020
    date_iso: '2020-06-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-23'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.593
    true_std: null
    value_gap_source_arxiv: '2006.12739'
    value_gap_source_title: Graph Prototypical Networks for Few-shot Learning on Attributed
      Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.593
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
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.465
    std: null
    paper_value: 0.465
    paper_std: null
    metric: ACC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-ratings (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 5-way 5-shot meta-test task
    date: Jun 23, 2020
    date_display: Jun 2020
    date_iso: '2020-06-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-23'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.465
    true_std: null
    value_gap_source_arxiv: '2006.12739'
    value_gap_source_title: Graph Prototypical Networks for Few-shot Learning on Attributed
      Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.465
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
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.419
    std: null
    paper_value: 0.419
    paper_std: null
    metric: ACC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-ratings (score=76)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 5-way 5-shot meta-test task
    date: Jun 23, 2020
    date_display: Jun 2020
    date_iso: '2020-06-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-06-23'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.419
    true_std: null
    value_gap_source_arxiv: '2006.12739'
    value_gap_source_title: Graph Prototypical Networks for Few-shot Learning on Attributed
      Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.419
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
  rank_metric: ACC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - ACC
  metric: ACC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Amazon-ratings
      dataset_slug: amazon-ratings
single_proposed_model: GPN
---

