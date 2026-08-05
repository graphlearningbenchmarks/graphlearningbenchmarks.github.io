---
title: Comparing Graph Transformers via Positional Encodings
arxiv_id: '2402.14202'
source_url: ''
authors:
- name: Mitchell Black
  orcid: null
  s2_author_id: '2057793151'
  s2_url: null
- name: Zhengchao Wan
  orcid: null
  s2_author_id: '2284993817'
  s2_url: null
- name: Gal Mishne
  orcid: null
  s2_author_id: '24394460'
  s2_url: null
- name: A. Nayyeri
  orcid: null
  s2_author_id: '1747558'
  s2_url: null
- name: Yusu Wang
  orcid: null
  s2_author_id: '2285184471'
  s2_url: null
published_date: Feb 22, 2024
published_date_iso: '2024-02-22'
published_venue: ICML 2024
published_conference: ICML 2024
published_conference_short: ICML
published_conference_slug: icml
abstract: 'The distinguishing power of graph transformers is closely tied to the choice
  of positional encoding: features used to augment the base transformer with information
  about the graph. There are two primary types of positional encoding: absolute positional
  encodings (APEs) and relative positional encodings (RPEs). APEs assign features
  to each node and are given as input to the transformer. RPEs instead assign a feature
  to each pair of nodes, e.g., graph distance, and are used to augment the attention
  block. A priori, it is unclear which method is better for maximizing the power of
  the resulting graph transformer. In this paper, we aim to understand the relationship
  between these different types of positional encodings. Interestingly, we show that
  graph transformers using APEs and RPEs are equivalent in terms of distinguishing
  power. In particular, we demonstrate how to interchange APEs and RPEs while maintaining
  their distinguishing power in terms of graph transformers. Based on our theoretical
  results, we provide a study on several APEs and RPEs (including the resistance distance
  and the recently introduced stable and expressive positional encoding (SPE)) and
  compare their distinguishing power in terms of transformers. We believe our work
  will help navigate the huge number of choices of positional encoding and will provide
  guidance on the future design of positional encodings for graph transformers.'
codebase_url: https://github.com/blackmit/comparing_graph_transformers_via_positional_encodings
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- RPE-augWL
mrr: 0.04
adjusted_mrr: 0.0133
mrr_dataset_count: 1
benchmark_categories:
- GNNBenchmark
benchmark_coverage:
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 1
  total: 6
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: CSL
  rows:
  - model: RPE-augWL
    model_key: rpe-augwl
    model_plain: RPE-augWL
    value: 1.0
    std: 0.0
    paper_value: 1.0
    paper_std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CSL dataset using RSPE RPE
    date: Feb 22, 2024
    date_display: Feb 2024
    date_iso: '2024-02-22'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-22'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0
    true_std: 0.0
    value_gap_source_arxiv: '2402.14202'
    value_gap_source_title: Comparing Graph Transformers via Positional Encodings
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0
    sort_std: 0.0
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: APE-GT
    model_key: ape-gt
    model_plain: APE-GT
    value: 1.0
    std: 0.0
    paper_value: 1.0
    paper_std: 0.0
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CSL dataset using HKdiagSE APE
    date: Feb 22, 2024
    date_display: Feb 2024
    date_iso: '2024-02-22'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-22'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0
    true_std: 0.0
    value_gap_source_arxiv: '2402.14202'
    value_gap_source_title: Comparing Graph Transformers via Positional Encodings
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0
    sort_std: 0.0
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DeepSet RPE-GT
    model_key: deepset rpe-gt
    model_plain: DeepSet RPE-GT
    value: 1.0
    std: 0.0
    paper_value: 1.0
    paper_std: 0.0
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CSL dataset using HKdiagSE RPE
    date: Feb 22, 2024
    date_display: Feb 2024
    date_iso: '2024-02-22'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-22'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0
    true_std: 0.0
    value_gap_source_arxiv: '2402.14202'
    value_gap_source_title: Comparing Graph Transformers via Positional Encodings
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0
    sort_std: 0.0
    global_rank: 24
    paper_rank: 24
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EGN APE-GT
    model_key: egn ape-gt
    model_plain: EGN APE-GT
    value: 1.0
    std: 0.0
    paper_value: 1.0
    paper_std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CSL dataset using RSPE APE
    date: Feb 22, 2024
    date_display: Feb 2024
    date_iso: '2024-02-22'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-22'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.0
    true_std: 0.0
    value_gap_source_arxiv: '2402.14202'
    value_gap_source_title: Comparing Graph Transformers via Positional Encodings
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.0
    sort_std: 0.0
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: ppgn
    model_plain: GPM
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: rw-agentnet
    model_plain: GPM
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: agentnet
    model_plain: GPM
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.1
    std: 0.0
    paper_value: 0.1
    paper_std: 0.0
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: muller2023attending
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CSL dataset
    date: Feb 22, 2024
    date_display: Feb 2024
    date_iso: '2024-02-22'
    published_venue: ICML 2024
    published_conference: ICML 2024
    at_pub_value: 0.99333
    at_pub_std: 0.01333
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2023-01-01'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: 0.8933300000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.99333
    true_std: 0.01333
    value_gap_source_arxiv: '2003.00982'
    value_gap_source_title: GNNBenchmark
    value_gap_source_is_current_paper: false
    value_gap: 0.8933300000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.99333
    sort_std: 0.01333
    global_rank: 42
    paper_rank: 79
    rank_delta: 37
    rank_delta_abs: 37
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: GNNBenchmark
    comparison_source_arxiv: '2003.00982'
    is_best: true
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
- benchmark: GNNBenchmark
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: CSL
      dataset_slug: csl
single_proposed_model: RPE-augWL
main_figure: /figures/2402.14202/main_figure.jpegoptim.jpg
---

