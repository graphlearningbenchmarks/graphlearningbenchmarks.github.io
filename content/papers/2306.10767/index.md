---
title: 'P-tensors: a General Framework for Higher Order Message Passing in Subgraph
  Neural Networks'
arxiv_id: '2306.10767'
source_url: ''
authors:
- name: Andrew R. Hands
  orcid: null
  s2_author_id: '2220292114'
  s2_url: null
- name: Tianyi Sun
  orcid: null
  s2_author_id: '2392217579'
  s2_url: null
- name: R. Kondor
  orcid: null
  s2_author_id: '2834541'
  s2_url: null
published_date: Jun 19, 2023
published_date_iso: '2023-06-19'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Several recent papers have proposed increasing the expressive power of graph
  neural networks by exploiting subgraphs or other topological structures. In parallel,
  researchers have investigated higher order permutation equivariant networks. In
  this paper we tie these two threads together by providing a general framework for
  higher order permutation equivariant message passing in subgraph neural networks.
  In this paper we introduce a new type of mathematical object called $P$-tensors,
  which provide a simple way to define the most general form of permutation equivariant
  message passing in both the above two categories of networks. We show that the P-Tensors
  paradigm can achieve state-of-the-art performance on benchmark molecular datasets.
codebase_url: https://github.com/arhands/ptensors
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MPNNs
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
- MoleculeNet
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: MoleculeNet
  benchmark_slug: moleculenet
  evaluated: 1
  total: 9
task_categories:
- graph_classification
- graph_regression
experiment_scopes:
- graph-level
results:
- &id002
  dataset: Tox21
  rows:
  - model: HIMP
    model_key: himp
    model_plain: HIMP
    value: 0.8736
    std: 0.005
    paper_value: 0.8736
    paper_std: 0.005
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: fey2020hierarchical
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.874
    at_pub_std: 0.005
    at_pub_source_arxiv: '2011.15069'
    at_pub_source_title: Graph convolutions that can finally model local structure
    at_pub_source_date_iso: '2020-11-30'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-11-30'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.874
    true_std: 0.005
    value_gap_source_arxiv: '2011.15069'
    value_gap_source_title: Graph convolutions that can finally model local structure
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.874
    sort_std: 0.005
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HOD-GNN
    model_key: gine w/ vn
    model_plain: HOD-GNN
    value: 0.872
    std: 0.003
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_display: Nov 2020
    date_iso: '2020-11-30'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.872
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HOD-GNN
    model_key: naivegine+ k=3 w/ vn
    model_plain: HOD-GNN
    value: 0.87
    std: 0.004
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2011.15069'
    title: Graph convolutions that can finally model local structure
    date: Nov 30, 2020
    date_display: Nov 2020
    date_iso: '2020-11-30'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.87
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GINE
    model_key: gine
    model_plain: GINE
    value: 0.8668
    std: 0.0077
    paper_value: 0.8668
    paper_std: 0.0077
    metric: ROC-AUC
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
    source_ref: hu2019strategies
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.85
    at_pub_std: 0.009
    at_pub_source_arxiv: '2011.15069'
    at_pub_source_title: Graph convolutions that can finally model local structure
    at_pub_source_date_iso: '2020-11-30'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-11-30'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.016800000000000037
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.85
    true_std: 0.009
    value_gap_source_arxiv: '2011.15069'
    value_gap_source_title: Graph convolutions that can finally model local structure
    value_gap_source_is_current_paper: false
    value_gap: 0.016800000000000037
    has_value_note: false
    value_note: ''
    sort_value: 0.85
    sort_std: 0.009
    global_rank: 7
    paper_rank: 5
    rank_delta: -2
    rank_delta_abs: 2
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph convolutions that can finally model local structure
    comparison_source_arxiv: '2011.15069'
    is_best: false
    is_std_outlier: false
  - model: MPNNs
    model_key: mpnns
    model_plain: MPNNs
    value: 0.8495
    std: 0.0058
    paper_value: 0.8495
    paper_std: 0.0058
    metric: ROC-AUC
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
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
    sort_value: 0.8495
    sort_std: 0.0058
    global_rank: 9
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
    is_best: false
    is_std_outlier: false
  - model: RP-NGF
    model_key: rp-ngf
    model_plain: RP-NGF
    value: 0.794
    std: 0.01
    paper_value: 0.794
    paper_std: 0.01
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: murphy2019relational
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
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
    sort_value: 0.794
    sort_std: 0.01
    global_rank: 84
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
    is_best: false
    is_std_outlier: false
  - model: DSS-GNN (EGO+)
    model_key: dss-gnn (ego+)
    model_plain: DSS-GNN (EGO+)
    value: 0.7795
    std: 0.004
    paper_value: 0.7795
    paper_std: 0.004
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: bevilacqua2022equivariant
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
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
    sort_value: 0.7795
    sort_std: 0.004
    global_rank: 127
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
    is_best: false
    is_std_outlier: false
  - model: DS-GNN (EGO+)
    model_key: ds-gnn (ego+)
    model_plain: DS-GNN (EGO+)
    value: 0.7639
    std: 0.0118
    paper_value: 0.7639
    paper_std: 0.0118
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: null
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: bevilacqua2022equivariant
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
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
    sort_value: 0.7639
    sort_std: 0.0118
    global_rank: 176
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
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: ZINC
  rows:
  - model: GPS
    model_key: tigt
    model_plain: GPS
    value: 0.014
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: Feb 3, 2024
    date_display: Feb 2024
    date_iso: '2024-02-03'
    venue: GRaM
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.014
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS
    model_key: ppgn++
    model_plain: GPS
    value: 0.02
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2302.11556'
    title: Equivariant Polynomials for Graph Neural Networks
    date: Feb 22, 2023
    date_display: Feb 2023
    date_iso: '2023-02-22'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.02
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS
    model_key: subgraphormer
    model_plain: GPS
    value: 0.02
    std: 0.002
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2406.09291'
    title: A Flexible, Equivariant Framework for Subgraph GNNs via Graph Products
      and Graph Coarsening
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/BarSGuy/Efficient-Subgraph-GNNs
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.02
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CIN
    model_key: cin
    model_plain: CIN
    value: 0.022
    std: 0.002
    paper_value: 0.022
    paper_std: 0.002
    metric: MAE
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
    table_ref: Table 1
    source_ref: bodnar2021weisfeiler
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.021
    at_pub_std: 0.001
    at_pub_source_arxiv: '2306.03561'
    at_pub_source_title: 'CIN++: Enhancing Topological Message Passing'
    at_pub_source_date_iso: '2023-06-06'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0009999999999999974
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.021
    true_std: 0.001
    value_gap_source_arxiv: '2306.03561'
    value_gap_source_title: 'CIN++: Enhancing Topological Message Passing'
    value_gap_source_is_current_paper: false
    value_gap: 0.0009999999999999974
    has_value_note: false
    value_note: ''
    sort_value: 0.021
    sort_std: 0.001
    global_rank: 4
    paper_rank: 6
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPNNs
    model_key: mpnns
    model_plain: MPNNs
    value: 0.024
    std: 0.001
    paper_value: 0.024
    paper_std: 0.001
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
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
    sort_value: 0.024
    sort_std: 0.001
    global_rank: 12
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
    is_best: false
    is_std_outlier: false
  - model: First order P-tensors
    model_key: first order p-tensors
    model_plain: First order P-tensors
    value: 0.024
    std: 0.001
    paper_value: 0.024
    paper_std: 0.001
    metric: MAE
    higher_is_better: false
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
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
    sort_value: 0.024
    sort_std: 0.001
    global_rank: 12
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
    is_best: false
    is_std_outlier: false
  - model: HIMP
    model_key: himp
    model_plain: HIMP
    value: 0.036
    std: 0.002
    paper_value: 0.036
    paper_std: 0.002
    metric: MAE
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
    table_ref: Table 1
    source_ref: fey2020hierarchical
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.036
    at_pub_std: 0.002
    at_pub_source_arxiv: '2210.13978'
    at_pub_source_title: Boosting the Cycle Counting Power of Graph Neural Networks
      with I$^2$-GNNs
    at_pub_source_date_iso: '2022-10-22'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2023-02-22'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.036
    true_std: 0.002
    value_gap_source_arxiv: '2302.11556'
    value_gap_source_title: Equivariant Polynomials for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.036
    sort_std: 0.002
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
  - model: PNA
    model_key: pna
    model_plain: PNA
    value: 0.32
    std: 0.032
    paper_value: 0.32
    paper_std: 0.032
    metric: MAE
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
    table_ref: Table 1
    source_ref: corso2020principal
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.142
    at_pub_std: 0.01
    at_pub_source_arxiv: '2201.09332'
    at_pub_source_title: How Expressive are Transformers in Spectral Domain for Graphs?
    at_pub_source_date_iso: '2022-01-23'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2025-01-30'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.17800000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.067
    true_std: 0.009
    value_gap_source_arxiv: '2501.18739'
    value_gap_source_title: 'Beyond Message Passing: Neural Graph Pattern Machine'
    value_gap_source_is_current_paper: false
    value_gap: 0.253
    has_value_note: false
    value_note: ''
    sort_value: 0.067
    sort_std: 0.009
    global_rank: 35
    paper_rank: 63
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: How Expressive are Transformers in Spectral Domain for
      Graphs?
    comparison_source_arxiv: '2201.09332'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.088
    std: 0.002
    paper_value: 0.088
    paper_std: 0.002
    metric: MAE
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
    table_ref: Table 1
    source_ref: xu2018powerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.088
    at_pub_std: 0.002
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-02-22'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.088
    true_std: 0.002
    value_gap_source_arxiv: '2302.11556'
    value_gap_source_title: Equivariant Polynomials for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.088
    sort_std: 0.002
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
  - model: GINE
    model_key: gine
    model_plain: GINE
    value: 0.088
    std: 0.002
    paper_value: 0.088
    paper_std: 0.002
    metric: MAE
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
    table_ref: Table 1
    source_ref: hu2019strategies
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jun 19, 2023
    date_display: Jun 2023
    date_iso: '2023-06-19'
    published_venue: ''
    published_conference: ''
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
    sort_value: 0.088
    sort_std: 0.002
    global_rank: 42
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
    is_best: false
    is_std_outlier: false
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
- benchmark: MoleculeNet
  datasets:
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: ZINC
      dataset_slug: zinc
  - benchmark: MoleculeNet
    benchmark_slug: moleculenet
    datasets:
    - dataset: Tox21
      dataset_slug: tox21
single_proposed_model: MPNNs
main_figure: /figures/2306.10767/main_figure.jpegoptim.jpg
---

