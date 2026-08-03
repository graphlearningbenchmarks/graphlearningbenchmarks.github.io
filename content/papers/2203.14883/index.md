---
title: 'TGL: A General Framework for Temporal GNN Training on Billion-Scale Graphs'
arxiv_id: '2203.14883'
source_url: ''
authors:
- name: Hongkuan Zhou
  orcid: null
  s2_author_id: '1443735039'
  s2_url: null
- name: Da Zheng
  orcid: null
  s2_author_id: '122579067'
  s2_url: null
- name: Israt Nisa
  orcid: null
  s2_author_id: '2365882761'
  s2_url: null
- name: Vasileios Ioannidis
  orcid: null
  s2_author_id: '28310338'
  s2_url: null
- name: Xiang Song
  orcid: null
  s2_author_id: '2118943843'
  s2_url: null
- name: George Karypis
  orcid: null
  s2_author_id: '50877490'
  s2_url: null
published_date: Mar 28, 2022
published_date_iso: '2022-03-28'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Many real world graphs contain time domain information. Temporal Graph Neural
  Networks capture temporal information as well as structural and contextual information
  in the generated dynamic node embeddings. Researchers have shown that these embeddings
  achieve state-of-the-art performance in many different tasks. In this work, we propose
  TGL, a unified framework rebfor large-scale offline Temporal Graph Neural Network
  training where users can compose various Temporal Graph Neural Networks with simple
  configuration files. TGL comprises five main components, a temporal sampler, a mailbox,
  a node memory module, a memory updater, and a message passing engine. rebWe design
  a Temporal-CSR data structure and a parallel sampler to efficiently sample temporal
  neighbors to form training mini-batches. We propose a novel random chunk scheduling
  technique that mitigates the problem of obsolete node memory rebwhen training with
  a large batch size. rebTo address the limitations of current TGNNs only being evaluated
  on small-scale datasets, we introduce two large-scale real-world datasets with 0.2
  and 1.3 billion temporal edges. We evaluate the performance of TGL on rebfour small-scale
  datasets with a single GPU and the two large datasets with multiple GPUs for both
  link prediction and node classification tasks. We compare TGL with the open-sourced
  code of five methods and show that TGL achieves similar or better accuracy with
  an average of $13 $ speedup. Our temporal parallel sampler achieves an average of
  $173 $ speedup on a multi-core CPU compared with the baselines. On a 4-GPU machine,
  TGL can train one epoch of more than one billion temporal edges within reb1-10 hours.
  To the best of our knowledge, this is the first work rebthat proposes a general
  framework for large-scale Temporal Graph Neural Networks training on multiple GPUs.
codebase_url: 'https://github.com/amazon-research/tgl{https:'
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- TGL
mrr: 0.0
adjusted_mrr: 0.0
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
  dataset: Reddit
  rows:
  - model: JODIE
    model_key: jodie
    model_plain: JODIE
    value: 0.7091
    std: null
    paper_value: 0.7091
    paper_std: null
    metric: F1-Micro
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic node classification task
    date: Mar 28, 2022
    date_display: Mar 2022
    date_iso: '2022-03-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-03-28'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7091
    true_std: null
    value_gap_source_arxiv: '2203.14883'
    value_gap_source_title: 'TGL: A General Framework for Temporal GNN Training on
      Billion-Scale Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7091
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
  - model: TGL
    model_key: tgl
    model_plain: TGL
    value: 0.6378
    std: null
    paper_value: 0.6378
    paper_std: null
    metric: F1-Micro
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic node classification task
    date: Mar 28, 2022
    date_display: Mar 2022
    date_iso: '2022-03-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-03-28'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6378
    true_std: null
    value_gap_source_arxiv: '2203.14883'
    value_gap_source_title: 'TGL: A General Framework for Temporal GNN Training on
      Billion-Scale Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6378
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
  - model: TGN
    model_key: tgn
    model_plain: TGN
    value: 0.6378
    std: null
    paper_value: 0.6378
    paper_std: null
    metric: F1-Micro
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic node classification task
    date: Mar 28, 2022
    date_display: Mar 2022
    date_iso: '2022-03-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-03-28'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6378
    true_std: null
    value_gap_source_arxiv: '2203.14883'
    value_gap_source_title: 'TGL: A General Framework for Temporal GNN Training on
      Billion-Scale Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6378
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
  - model: APAN
    model_key: apan
    model_plain: APAN
    value: 0.62
    std: null
    paper_value: 0.62
    paper_std: null
    metric: F1-Micro
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic node classification task
    date: Mar 28, 2022
    date_display: Mar 2022
    date_iso: '2022-03-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-03-28'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.62
    true_std: null
    value_gap_source_arxiv: '2203.14883'
    value_gap_source_title: 'TGL: A General Framework for Temporal GNN Training on
      Billion-Scale Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.62
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
  - model: DySAT
    model_key: dysat
    model_plain: DySAT
    value: 0.617
    std: null
    paper_value: 0.617
    paper_std: null
    metric: F1-Micro
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic node classification task
    date: Mar 28, 2022
    date_display: Mar 2022
    date_iso: '2022-03-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-03-28'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.617
    true_std: null
    value_gap_source_arxiv: '2203.14883'
    value_gap_source_title: 'TGL: A General Framework for Temporal GNN Training on
      Billion-Scale Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.617
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
  - model: TGAT
    model_key: tgat
    model_plain: TGAT
    value: 0.6061
    std: null
    paper_value: 0.6061
    paper_std: null
    metric: F1-Micro
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Dynamic node classification task
    date: Mar 28, 2022
    date_display: Mar 2022
    date_iso: '2022-03-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-03-28'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6061
    true_std: null
    value_gap_source_arxiv: '2203.14883'
    value_gap_source_title: 'TGL: A General Framework for Temporal GNN Training on
      Billion-Scale Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6061
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
  rank_metric: F1-Micro
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1-Micro
  metric: F1-Micro
  uses_non_primary_metric: true
  paper_has_primary_metric: false
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
    - dataset: Reddit
      dataset_slug: reddit
single_proposed_model: TGL
---

