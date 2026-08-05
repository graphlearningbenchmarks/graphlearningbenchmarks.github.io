---
title: Graph Attention MLP with Reliable Label Utilization
arxiv_id: '2108.10097'
source_url: ''
authors:
- name: Wentao Zhang
  orcid: null
  s2_author_id: '2108232566'
  s2_url: null
- name: Ziqi Yin
  orcid: null
  s2_author_id: '27036277'
  s2_url: null
- name: Zeang Sheng
  orcid: null
  s2_author_id: '2120972284'
  s2_url: null
- name: Wenbin Ouyang
  orcid: null
  s2_author_id: '2134930026'
  s2_url: null
- name: Xiaosen Li
  orcid: null
  s2_author_id: '2108698628'
  s2_url: null
- name: Yangyu Tao
  orcid: null
  s2_author_id: '2105710451'
  s2_url: null
- name: Zhi Yang
  orcid: null
  s2_author_id: '2109540175'
  s2_url: null
- name: Bin Cui
  orcid: null
  s2_author_id: '2068228300'
  s2_url: null
published_date: Aug 23, 2021
published_date_iso: '2021-08-23'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph neural networks (GNNs) have recently achieved state-of-the-art performance
  in many graph-based applications. Despite the high performance, they typically need
  to perform expensive recursive neighborhood expansions during every training epoch
  and has the scalability issue. Moreover, most of them are inflexible since they
  are restricted to fixed-hop neighborhoods and insensitive to actual receptive field
  requirements for each node. We circumvent these limitations by introducing a scalable
  and flexible method: Graph Attention Multi-Layer Perceptron (GAMLP). Following the
  routine of decoupled GNNs, the feature propagation in GAMLP is executed during pre-computation,
  which helps it maintain high scalability. With three proposed receptive field attention,
  each node in GAMLP is flexible in leveraging the propagated features over the different
  sizes of reception field. We conduct extensive evaluations on two large open graph
  benchmarks (ogbn-products and ogbn-papers100M), demonstrating that GAMLP not only
  achieves state-of-the-art performance, but also enjoys high scalability and efficiency.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GAMLP
- GAMLP+RLU
- NARS-GAMLP
- NARS-GAMLP+RLU
mrr: 0.2593
adjusted_mrr: 0.1728
mrr_dataset_count: 2
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 3
  total: 16
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id003
  dataset: ogbn-mag
  rows:
  - model: ALS (GraphSAINT)
    model_key: lmsps+lp+ms
    model_plain: ALS (GraphSAINT)
    value: 0.5784
    std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.5784
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ALS (GraphSAINT)
    model_key: sehgnn+emb+ms
    model_plain: ALS (GraphSAINT)
    value: 0.5719
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_display: Jul 2022
    date_iso: '2022-07-06'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.5719
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ALS (GraphSAINT)
    model_key: sehgnn+ms
    model_plain: ALS (GraphSAINT)
    value: 0.5671
    std: 0.0014
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_display: Jul 2022
    date_iso: '2022-07-06'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.5671
    sort_std: 0.0014
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NARS-GAMLP+RLU
    model_key: nars-gamlp+rlu
    model_plain: NARS-GAMLP+RLU
    value: 0.559
    std: 0.0027
    paper_value: 0.559
    paper_std: 0.0027
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-mag
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-08-23'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.559
    true_std: 0.0027
    value_gap_source_arxiv: '2108.10097'
    value_gap_source_title: Graph Attention MLP with Reliable Label Utilization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.559
    sort_std: 0.0027
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
  - model: NARS-SAGN+2-SLE
    model_key: nars-sagn+2-sle
    model_plain: NARS-SAGN+2-SLE
    value: 0.544
    std: 0.0015
    paper_value: 0.544
    paper_std: 0.0015
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
    table_ref: Table 1
    source_ref: sun2021scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-mag
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-08-23'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.544
    true_std: 0.0015
    value_gap_source_arxiv: '2108.10097'
    value_gap_source_title: Graph Attention MLP with Reliable Label Utilization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.544
    sort_std: 0.0015
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
  - model: NARS-GAMLP
    model_key: nars-gamlp
    model_plain: NARS-GAMLP
    value: 0.5396
    std: 0.0018
    paper_value: 0.5396
    paper_std: 0.0018
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-mag
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.5401
    true_std: 0.0021
    value_gap_source_arxiv: '2206.04355'
    value_gap_source_title: Graph Attention Multi-Layer Perceptron
    value_gap_source_is_current_paper: false
    value_gap: 0.000500000000000056
    has_value_note: false
    value_note: ''
    sort_value: 0.5401
    sort_std: 0.0021
    global_rank: 12
    paper_rank: 14
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.4046
    std: 0.0012
    paper_value: 0.4046
    paper_std: 0.0012
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
    table_ref: Table 1
    source_ref: frasca2020sign
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-mag
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.481
    at_pub_std: 0.001
    at_pub_source_arxiv: '2011.09679'
    at_pub_source_title: Scalable Graph Neural Networks for Heterogeneous Graphs
    at_pub_source_date_iso: '2020-11-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.07639999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5289
    true_std: 0.0011
    value_gap_source_arxiv: '2305.19903'
    value_gap_source_title: Improving Expressivity of GNNs with Subgraph-specific
      Factor Embedded Normalization
    value_gap_source_is_current_paper: false
    value_gap: 0.12430000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.5289
    sort_std: 0.0011
    global_rank: 19
    paper_rank: 40
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scalable Graph Neural Networks for Heterogeneous Graphs
    comparison_source_arxiv: '2011.09679'
    is_best: false
    is_std_outlier: false
  - model: NARS
    model_key: nars
    model_plain: NARS
    value: 0.524
    std: 0.0016
    paper_value: 0.524
    paper_std: 0.0016
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
    table_ref: Table 1
    source_ref: yu2020scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-mag
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.524
    true_std: 0.0016
    value_gap_source_arxiv: '2206.04355'
    value_gap_source_title: Graph Attention Multi-Layer Perceptron
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.524
    sort_std: 0.0016
    global_rank: 20
    paper_rank: 20
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NARS-SAGN+0-SLE
    model_key: nars-sagn+0-sle
    model_plain: NARS-SAGN+0-SLE
    value: 0.5232
    std: 0.0025
    paper_value: 0.5232
    paper_std: 0.0025
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
    table_ref: Table 1
    source_ref: sun2021scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-mag
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-08-23'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5232
    true_std: 0.0025
    value_gap_source_arxiv: '2108.10097'
    value_gap_source_title: Graph Attention MLP with Reliable Label Utilization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5232
    sort_std: 0.0025
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: R-HGNN
    model_key: r-hgnn
    model_plain: R-HGNN
    value: 0.5204
    std: 0.0026
    paper_value: 0.5204
    paper_std: 0.0026
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
    table_ref: Table 1
    source_ref: yu2021heterogeneous
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-mag
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5204
    at_pub_std: null
    at_pub_source_arxiv: '2105.11122'
    at_pub_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    at_pub_source_date_iso: '2021-05-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5204
    true_std: 0.0026
    value_gap_source_arxiv: '2206.04355'
    value_gap_source_title: Graph Attention Multi-Layer Perceptron
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5204
    sort_std: 0.0026
    global_rank: 24
    paper_rank: 24
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGConv
    model_key: hgconv
    model_plain: HGConv
    value: 0.5045
    std: 0.0017
    paper_value: 0.5045
    paper_std: 0.0017
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
    table_ref: Table 1
    source_ref: yu2020hybrid
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-mag
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5045
    true_std: 0.0017
    value_gap_source_arxiv: '2205.15653'
    value_gap_source_title: Label-Enhanced Graph Neural Network for Semi-supervised
      Node Classification
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5045
    sort_std: 0.0017
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: R-GSN
    model_key: r-gsn
    model_plain: R-GSN
    value: 0.5032
    std: 0.0037
    paper_value: 0.5032
    paper_std: 0.0037
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
    table_ref: Table 1
    source_ref: wu2021r
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-mag
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5032
    true_std: 0.0037
    value_gap_source_arxiv: '2205.15653'
    value_gap_source_title: Label-Enhanced Graph Neural Network for Semi-supervised
      Node Classification
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5032
    sort_std: 0.0037
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.4927
    std: 0.0061
    paper_value: 0.4927
    paper_std: 0.0061
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
    table_ref: Table 1
    source_ref: hu2020heterogeneous
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-mag
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4921
    at_pub_std: null
    at_pub_source_arxiv: '2105.11122'
    at_pub_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    at_pub_source_date_iso: '2021-05-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0006000000000000449
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4927
    true_std: 0.0061
    value_gap_source_arxiv: '2205.15653'
    value_gap_source_title: Label-Enhanced Graph Neural Network for Semi-supervised
      Node Classification
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4927
    sort_std: 0.0061
    global_rank: 34
    paper_rank: 34
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: R-GCN
    model_key: r-gcn
    model_plain: R-GCN
    value: 0.3977
    std: 0.0046
    paper_value: 0.3977
    paper_std: 0.0046
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
    table_ref: Table 1
    source_ref: schlichtkrull2018modeling
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-mag
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3977
    true_std: 0.0046
    value_gap_source_arxiv: '2206.04355'
    value_gap_source_title: Graph Attention Multi-Layer Perceptron
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3977
    sort_std: 0.0046
    global_rank: 41
    paper_rank: 41
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: ogbn-papers100M
  rows:
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.6329
    std: 0.0019
    paper_value: 0.6329
    paper_std: 0.0019
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
    table_ref: Table 1
    source_ref: wu2019simplifying
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-papers100M standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.632
    at_pub_std: 0.002
    at_pub_source_arxiv: '2108.00955'
    at_pub_source_title: Evaluating Deep Graph Neural Networks
    at_pub_source_date_iso: '2021-08-02'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.0009000000000000119
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.791
    true_std: null
    value_gap_source_arxiv: '2403.13268'
    value_gap_source_title: 'Unifews: You Need Fewer Operations for Efficient Graph
      Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.15810000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.791
    sort_std: null
    global_rank: 1
    paper_rank: 61
    rank_delta: 60
    rank_delta_abs: 60
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAMLP
    model_key: gamlp
    model_plain: GAMLP
    value: 0.6771
    std: 0.002
    paper_value: 0.6771
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-papers100M standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7036
    true_std: 0.0002
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: false
    value_gap: 0.026499999999999968
    has_value_note: false
    value_note: ''
    sort_value: 0.7036
    sort_std: 0.0002
    global_rank: 2
    paper_rank: 10
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LargeGT-full
    model_key: glem-gnn
    model_plain: LargeGT-full
    value: 0.7036
    std: 0.0002
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.14709'
    title: Learning on Large-scale Text-attributed Graphs via Variational Inference
    date: Oct 2022
    date_display: Oct 2022
    date_iso: 2022-10
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/AndyJZhao/GLEM
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7036
    sort_std: 0.0002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAMLP+RLU
    model_key: gamlp+rlu
    model_plain: GAMLP+RLU
    value: 0.6825
    std: 0.0011
    paper_value: 0.6825
    paper_std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-papers100M standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6967
    true_std: 0.0004
    value_gap_source_arxiv: '2111.00064'
    value_gap_source_title: Node Feature Extraction by Self-Supervised Multi-scale
      Neighborhood Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.01419999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.6967
    sort_std: 0.0004
    global_rank: 5
    paper_rank: 6
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGN+SLE
    model_key: sagn+sle
    model_plain: SAGN+SLE
    value: 0.68
    std: 0.0015
    paper_value: 0.68
    paper_std: 0.0015
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
    table_ref: Table 1
    source_ref: sun2021scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-papers100M standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.68
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2104.09376'
    at_pub_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    at_pub_source_date_iso: '2021-04-19'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-04-19'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.68
    true_std: 0.0015
    value_gap_source_arxiv: '2104.09376'
    value_gap_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.68
    sort_std: 0.0015
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
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.6568
    std: 0.0006
    paper_value: 0.6568
    paper_std: 0.0006
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
    table_ref: Table 1
    source_ref: frasca2020sign
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-papers100M standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6568
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2104.09376'
    at_pub_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    at_pub_source_date_iso: '2021-04-19'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2025-04-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6636
    true_std: 0.0005
    value_gap_source_arxiv: '2504.13266'
    value_gap_source_title: 'Graph Learning at Scale: Characterizing and Optimizing
      Pre-Propagation GNNs'
    value_gap_source_is_current_paper: false
    value_gap: 0.006799999999999917
    has_value_note: false
    value_note: ''
    sort_value: 0.6636
    sort_std: 0.0005
    global_rank: 27
    paper_rank: 41
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIGN-XL
    model_key: sign-xl
    model_plain: SIGN-XL
    value: 0.6606
    std: 0.0019
    paper_value: 0.6606
    paper_std: 0.0019
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
    table_ref: Table 1
    source_ref: frasca2020sign
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-papers100M standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6606
    true_std: 0.0019
    value_gap_source_arxiv: '2206.04355'
    value_gap_source_title: Graph Attention Multi-Layer Perceptron
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6606
    sort_std: 0.0019
    global_rank: 35
    paper_rank: 35
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: ogbn-products
  rows:
  - model: LargeGT-full
    model_key: advsyngnn
    model_plain: LargeGT-full
    value: 0.8931
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.17071'
    title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial Synthesis
      and Self-Corrective Propagation'
    date: Feb 19, 2026
    date_display: Feb 2026
    date_iso: '2026-02-19'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8931
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LargeGT-full
    model_key: gofa-f
    model_plain: LargeGT-full
    value: 0.8834
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.09709'
    title: 'GOFA: A Generative One-For-All Model for Joint Graph Language Modeling'
    date: Jul 12, 2024
    date_display: Jul 2024
    date_iso: '2024-07-12'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/JiaruiFeng/GOFA
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8834
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LargeGT-full
    model_key: llms
    model_plain: LargeGT-full
    value: 0.882
    std: 0.0005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2412.16441'
    title: 'Towards Graph Foundation Models: Learning Generalities Across Graphs via
      Task-Trees'
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/Zehong-Wang/GIT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.882
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7564
    std: 0.0021
    paper_value: 0.7564
    paper_std: 0.0021
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
    table_ref: Table 1
    source_ref: kipf2016semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-products standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7564
    at_pub_std: 0.0021
    at_pub_source_arxiv: '2101.11525'
    at_pub_source_title: Calibrating and Improving Graph Contrastive Learning
    at_pub_source_date_iso: '2021-01-27'
    at_pub_source_date_label: TMLR 2021
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
    true_value: 0.8691
    true_std: 0.0005
    value_gap_source_arxiv: '2412.16441'
    value_gap_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    value_gap_source_is_current_paper: false
    value_gap: 0.11270000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8691
    sort_std: 0.0005
    global_rank: 12
    paper_rank: 251
    rank_delta: 239
    rank_delta_abs: 239
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGN+SLE
    model_key: sagn+sle
    model_plain: SAGN+SLE
    value: 0.8428
    std: 0.0014
    paper_value: 0.8428
    paper_std: 0.0014
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
    table_ref: Table 1
    source_ref: sun2021scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-products standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8428
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2104.09376'
    at_pub_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    at_pub_source_date_iso: '2021-04-19'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8501
    true_std: 0.001
    value_gap_source_arxiv: '2111.00064'
    value_gap_source_title: Node Feature Extraction by Self-Supervised Multi-scale
      Neighborhood Prediction
    value_gap_source_is_current_paper: false
    value_gap: 0.007299999999999973
    has_value_note: false
    value_note: ''
    sort_value: 0.8501
    sort_std: 0.001
    global_rank: 30
    paper_rank: 41
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAMLP+RLU
    model_key: gamlp+rlu
    model_plain: GAMLP+RLU
    value: 0.8459
    std: 0.001
    paper_value: 0.8459
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-products standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-08-23'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8459
    true_std: 0.001
    value_gap_source_arxiv: '2108.10097'
    value_gap_source_title: Graph Attention MLP with Reliable Label Utilization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8459
    sort_std: 0.001
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP+C&S
    model_key: mlp+c&s
    model_plain: MLP+C&S
    value: 0.8418
    std: 0.0007
    paper_value: 0.8418
    paper_std: 0.0007
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: huang2020combining
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-products standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8418
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2104.09376'
    at_pub_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    at_pub_source_date_iso: '2021-04-19'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-04-19'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8418
    true_std: 0.0007
    value_gap_source_arxiv: '2104.09376'
    value_gap_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8418
    sort_std: 0.0007
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
  - model: GAMLP
    model_key: gamlp
    model_plain: GAMLP
    value: 0.8354
    std: 0.0009
    paper_value: 0.8354
    paper_std: 0.0009
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-products standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8376
    true_std: 0.0019
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.0021999999999999797
    has_value_note: false
    value_note: ''
    sort_value: 0.8376
    sort_std: 0.0019
    global_rank: 54
    paper_rank: 60
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SIGN
    model_key: sign
    model_plain: SIGN
    value: 0.8052
    std: 0.0016
    paper_value: 0.8052
    paper_std: 0.0016
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
    table_ref: Table 1
    source_ref: frasca2020sign
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-products standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8052
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2104.09376'
    at_pub_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    at_pub_source_date_iso: '2021-04-19'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-03-01'
    value_gap_source_date_label: WWW 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.831
    true_std: 0.008
    value_gap_source_arxiv: '2203.00638'
    value_gap_source_title: 'PaSca: a Graph Neural Architecture Search System under
      the Scalable Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.025799999999999934
    has_value_note: false
    value_note: ''
    sort_value: 0.831
    sort_std: 0.008
    global_rank: 67
    paper_rank: 131
    rank_delta: 64
    rank_delta_abs: 64
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.785
    std: 0.0014
    paper_value: 0.785
    paper_std: 0.0014
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
    table_ref: Table 1
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-products standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.785
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2104.09376'
    at_pub_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    at_pub_source_date_iso: '2021-04-19'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2026-05-24'
    value_gap_source_date_label: ICML 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8287
    true_std: null
    value_gap_source_arxiv: '2605.24867'
    value_gap_source_title: 'Clustering as Reasoning: A $k$-Means Interpretation of
      Chain-of-Thought Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.04369999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8287
    sort_std: null
    global_rank: 74
    paper_rank: 211
    rank_delta: 137
    rank_delta_abs: 137
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniMP
    model_key: unimp
    model_plain: UniMP
    value: 0.8256
    std: 0.0031
    paper_value: 0.8256
    paper_std: 0.0031
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
    table_ref: Table 1
    source_ref: shi2020masked
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-products standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8256
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2009.03509'
    at_pub_source_title: 'Masked Label Prediction: Unified Message Passing Model for
      Semi-Supervised Classification'
    at_pub_source_date_iso: '2020-09-08'
    at_pub_source_date_label: IJCAI 2020
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8256
    true_std: 0.0031
    value_gap_source_arxiv: '2206.04355'
    value_gap_source_title: Graph Attention Multi-Layer Perceptron
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8256
    sort_std: 0.0031
    global_rank: 78
    paper_rank: 78
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeeperGCN
    model_key: deepergcn
    model_plain: DeeperGCN
    value: 0.8098
    std: 0.002
    paper_value: 0.8098
    paper_std: 0.002
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
    table_ref: Table 1
    source_ref: li2020deepergcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on ogbn-products standard split
    date: Aug 23, 2021
    date_display: Aug 2021
    date_iso: '2021-08-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.809
    at_pub_std: 0.002
    at_pub_source_arxiv: '2009.03509'
    at_pub_source_title: 'Masked Label Prediction: Unified Message Passing Model for
      Semi-Supervised Classification'
    at_pub_source_date_iso: '2020-09-08'
    at_pub_source_date_label: IJCAI 2020
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.0007999999999999119
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8098
    true_std: 0.002
    value_gap_source_arxiv: '2206.04355'
    value_gap_source_title: Graph Attention Multi-Layer Perceptron
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8098
    sort_std: 0.002
    global_rank: 122
    paper_rank: 122
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-products
      dataset_slug: ogbn-products
    - dataset: ogbn-papers100M
      dataset_slug: ogbn-papers100m
    - dataset: ogbn-mag
      dataset_slug: ogbn-mag
main_figure: /figures/2108.10097/main_figure.jpegoptim.jpg
---

