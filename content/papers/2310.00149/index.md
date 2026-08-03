---
title: 'One for All: Towards Training One Graph Model for All Classification Tasks'
arxiv_id: '2310.00149'
source_url: ''
authors:
- name: Hao Liu
  orcid: null
  s2_author_id: '2264134998'
  s2_url: null
- name: Jiarui Feng
  orcid: null
  s2_author_id: '48441034'
  s2_url: null
- name: Lecheng Kong
  orcid: null
  s2_author_id: '2164063663'
  s2_url: null
- name: Ningyue Liang
  orcid: null
  s2_author_id: '2345368821'
  s2_url: null
- name: Dacheng Tao
  orcid: null
  s2_author_id: '2244621611'
  s2_url: null
- name: Yixin Chen
  orcid: null
  s2_author_id: '2223152252'
  s2_url: null
- name: Muhan Zhang
  orcid: null
  s2_author_id: '2239188141'
  s2_url: null
published_date: Sep 29, 2023
published_date_iso: '2023-09-29'
published_venue: ICLR 2023
published_conference: ICLR 2023
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Designing a single model to address multiple tasks has been a long-standing
  objective in artificial intelligence. Recently, large language models have demonstrated
  exceptional capability in solving different tasks within the language domain. However,
  a unified model for various graph tasks remains underexplored, primarily due to
  the challenges unique to the graph learning domain. First, graph data from different
  areas carry distinct attributes and follow different distributions. Such discrepancy
  makes it hard to represent graphs in a single representation space. Second, tasks
  on graphs diversify into node, link, and graph tasks, requiring distinct embedding
  strategies. Finally, an appropriate graph prompting paradigm for in-context learning
  is unclear. We propose One for All (OFA), the first general framework that can use
  a single graph model to address the above challenges. Specifically, OFA proposes
  text-attributed graphs to unify different graph data by describing nodes and edges
  with natural language and uses language models to encode the diverse and possibly
  cross-domain text attributes to feature vectors in the same embedding space. Furthermore,
  OFA introduces the concept of nodes-of-interest to standardize different tasks with
  a single task representation. For in-context learning on graphs, OFA introduces
  a novel graph prompting paradigm that appends prompting substructures to the input
  graph, which enables it to address varied tasks without fine-tuning. We train the
  OFA model using graph data from multiple domains (including citation networks, molecular
  graphs, knowledge graphs, etc.) simultaneously and evaluate its ability in supervised,
  few-shot, and zero-shot learning scenarios. OFA performs well across different tasks,
  making it the first general-purpose across-domains classification model on graphs.
codebase_url: https://github.com/LechengKong/OneForAll
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Knowledge Graphs
benchmark_coverage:
- benchmark: Knowledge Graphs
  benchmark_slug: knowledge-graphs
  evaluated: 1
  total: 3
task_categories:
- link_prediction
experiment_scopes:
- edge-level
results:
- &id001
  dataset: WN18RR
  rows:
  - model: OFA-llama2-13b
    model_key: ofa-llama2-13b
    model_plain: OFA-llama2-13b
    value: 0.9814
    std: 0.0025
    paper_value: 0.9814
    paper_std: 0.0025
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Supervised learning on WN18RR link prediction task; reported as
      mean of 10 runs.
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9814
    true_std: 0.0025
    value_gap_source_arxiv: '2310.00149'
    value_gap_source_title: 'One for All: Towards Training One Graph Model for All
      Classification Tasks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9814
    sort_std: 0.0025
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
  - model: OFA-llama2-7b
    model_key: ofa-llama2-7b
    model_plain: OFA-llama2-7b
    value: 0.9808
    std: 0.0016
    paper_value: 0.9808
    paper_std: 0.0016
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Supervised learning on WN18RR link prediction task; reported as
      mean of 10 runs.
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9808
    true_std: 0.0016
    value_gap_source_arxiv: '2310.00149'
    value_gap_source_title: 'One for All: Towards Training One Graph Model for All
      Classification Tasks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9808
    sort_std: 0.0016
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
  - model: OFA-e5
    model_key: ofa-e5
    model_plain: OFA-e5
    value: 0.9784
    std: 0.0035
    paper_value: 0.9784
    paper_std: 0.0035
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Supervised learning on WN18RR link prediction task; reported as
      mean of 10 runs.
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9784
    true_std: 0.0035
    value_gap_source_arxiv: '2310.00149'
    value_gap_source_title: 'One for All: Towards Training One Graph Model for All
      Classification Tasks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9784
    sort_std: 0.0035
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
  - model: OFA-ind-st
    model_key: ofa-ind-st
    model_plain: OFA-ind-st
    value: 0.9722
    std: 0.0018
    paper_value: 0.9722
    paper_std: 0.0018
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Supervised learning on WN18RR link prediction task; reported as
      mean of 10 runs.
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9722
    true_std: 0.0018
    value_gap_source_arxiv: '2310.00149'
    value_gap_source_title: 'One for All: Towards Training One Graph Model for All
      Classification Tasks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9722
    sort_std: 0.0018
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
  - model: OFA-st
    model_key: ofa-st
    model_plain: OFA-st
    value: 0.9691
    std: 0.0011
    paper_value: 0.9691
    paper_std: 0.0011
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Supervised learning on WN18RR link prediction task; reported as
      mean of 10 runs.
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9691
    true_std: 0.0011
    value_gap_source_arxiv: '2310.00149'
    value_gap_source_title: 'One for All: Towards Training One Graph Model for All
      Classification Tasks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9691
    sort_std: 0.0011
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
    value: 0.674
    std: 0.024
    paper_value: 0.674
    paper_std: 0.024
    metric: Accuracy
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Supervised learning on WN18RR link prediction task; reported as
      mean of 10 runs.
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8677
    true_std: 0.003
    value_gap_source_arxiv: '2412.16441'
    value_gap_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    value_gap_source_is_current_paper: false
    value_gap: 0.19369999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.8677
    sort_std: 0.003
    global_rank: 18
    paper_rank: 28
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.573
    std: 0.034
    paper_value: 0.573
    paper_std: 0.034
    metric: Accuracy
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Supervised learning on WN18RR link prediction task; reported as
      mean of 10 runs.
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    published_venue: ICLR 2023
    published_conference: ICLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-09'
    value_gap_source_date_label: KDD 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7402
    true_std: 0.0055
    value_gap_source_arxiv: '2602.09258'
    value_gap_source_title: Generalizing GNNs with Tokenized Mixture of Experts
    value_gap_source_is_current_paper: false
    value_gap: 0.16720000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7402
    sort_std: 0.0055
    global_rank: 25
    paper_rank: 28
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: MRR
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Knowledge Graphs
  datasets:
  - *id001
datasets_by_scope:
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: Knowledge Graphs
    benchmark_slug: knowledge-graphs
    datasets:
    - dataset: WN18RR
      dataset_slug: wn18rr
---

