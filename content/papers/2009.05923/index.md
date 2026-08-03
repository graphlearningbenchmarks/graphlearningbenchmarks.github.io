---
title: Contrastive Self-supervised Learning for Graph Classification
arxiv_id: '2009.05923'
source_url: ''
authors:
- name: Jiaqi Zeng, Pengtao Xie
  orcid: null
  s2_author_id: '2072984384'
  s2_url: null
published_date: Sep 13, 2020
published_date_iso: '2020-09-13'
published_venue: AAAI 2020
published_conference: AAAI 2020
published_conference_short: AAAI
published_conference_slug: aaai
abstract: Graph classification is a widely studied problem and has broad applications.
  In many real-world problems, the number of labeled graphs available for training
  classification models is limited, which renders these models prone to overfitting.
  To address this problem, we propose two approaches based on contrastive self-supervised
  learning (CSSL) to alleviate overfitting. In the first approach, we use CSSL to
  pretrain graph encoders on widely-available unlabeled graphs without relying on
  human-provided labels, then finetune the pretrained encoders on labeled graphs.
  In the second approach, we develop a regularizer based on CSSL, and solve the supervised
  classification task and the unsupervised CSSL task simultaneously. To perform CSSL
  on graphs, given a collection of original graphs, we perform data augmentation to
  create augmented graphs out of the original graphs. An augmented graph is created
  by consecutively applying a sequence of graph alteration operations. A contrastive
  loss is defined to learn graph encoders by judging whether two augmented graphs
  are from the same original graph. Experiments on various graph classification datasets
  demonstrate the effectiveness of our proposed methods.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CSSL-Freeze A1-specific
- CSSL-Freeze A1-all
- CSSL-Freeze A3-specific
- CSSL-Freeze A3-all
- CSSL-Pretrain A1-specific
- CSSL-Pretrain A1-all
- CSSL-Pretrain A3-specific
- CSSL-Pretrain A3-all
- CSSL-Reg A1-specific
- CSSL-Reg A1-all
- CSSL-Reg A3-specific
- CSSL-Reg A3-all
mrr: 0.0097
adjusted_mrr: 0.0065
mrr_dataset_count: 2
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
- &id002
  dataset: D&D
  rows:
  - model: DiffPool-det +Both (GAT)
    model_key: gc-gnn (graphsage)
    model_plain: DiffPool-det +Both (GAT)
    value: 0.921
    std: 0.081
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2309.00738'
    title: Rethinking the Power of Graph Canonization in Graph Representation Learning
      with Stability
    date: Sep 1, 2023
    date_display: Sep 2023
    date_iso: '2023-09-01'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.921
    sort_std: 0.081
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DiffPool-det +Both (GAT)
    model_key: sugar
    model_plain: DiffPool-det +Both (GAT)
    value: 0.8403
    std: 0.0133
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2101.08170'
    title: 'SUGAR: Subgraph Neural Network with Reinforcement Pooling and Self-Supervised
      Mutual Information Mechanism'
    date: Jan 20, 2021
    date_display: Jan 2021
    date_iso: '2021-01-20'
    venue: The Web Conference
    codebase_url: https://github.com/RingBDStack/SUGAR
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8403
    sort_std: 0.0133
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DiffPool-det +Both (GAT)
    model_key: ortho-g-u-nets
    model_plain: DiffPool-det +Both (GAT)
    value: 0.8387
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2109.11338'
    title: Orthogonal Graph Neural Networks
    date: Sep 23, 2021
    date_display: Sep 2021
    date_iso: '2021-09-23'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8387
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: gPool
    model_key: gpool
    model_plain: gPool
    value: 0.7702
    std: 0.0132
    paper_value: 0.7702
    paper_std: 0.0132
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-01-20'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8243
    true_std: null
    value_gap_source_arxiv: '2101.08170'
    value_gap_source_title: 'SUGAR: Subgraph Neural Network with Reinforcement Pooling
      and Self-Supervised Mutual Information Mechanism'
    value_gap_source_is_current_paper: false
    value_gap: 0.05410000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.8243
    sort_std: null
    global_rank: 7
    paper_rank: 106
    rank_delta: 99
    rank_delta_abs: 99
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Reg A1-specific
    model_key: cssl-reg a1-specific
    model_plain: CSSL-Reg A1-specific
    value: 0.8218
    std: 0.0134
    paper_value: 0.8218
    paper_std: 0.0134
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
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8218
    true_std: 0.0134
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8218
    sort_std: 0.0134
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Pretrain A1-specific
    model_key: cssl-pretrain a1-specific
    model_plain: CSSL-Pretrain A1-specific
    value: 0.8202
    std: 0.0142
    paper_value: 0.8202
    paper_std: 0.0142
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV; Pretrain uses unlabeled graphs
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8202
    true_std: 0.0142
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8202
    sort_std: 0.0142
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGP-SL
    model_key: hgp-sl
    model_plain: HGP-SL
    value: 0.8096
    std: 0.0126
    paper_value: 0.8096
    paper_std: 0.0126
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8096
    true_std: 0.0126
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8096
    sort_std: 0.0126
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Pretrain A1-all
    model_key: cssl-pretrain a1-all
    model_plain: CSSL-Pretrain A1-all
    value: 0.8084
    std: 0.0124
    paper_value: 0.8084
    paper_std: 0.0124
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV; Pretrain uses all 5 datasets
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8084
    true_std: 0.0124
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8084
    sort_std: 0.0124
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Pretrain A3-specific
    model_key: cssl-pretrain a3-specific
    model_plain: CSSL-Pretrain A3-specific
    value: 0.8084
    std: 0.0154
    paper_value: 0.8084
    paper_std: 0.0154
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV; Pretrain uses unlabeled graphs
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8084
    true_std: 0.0154
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8084
    sort_std: 0.0154
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
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.7861
    std: 0.0132
    paper_value: 0.7861
    paper_std: 0.0132
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.8064
    at_pub_std: null
    at_pub_source_arxiv: '2007.11202'
    at_pub_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for
      Graph Representation and Learning'
    at_pub_source_date_iso: '2020-07-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-07-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.020299999999999985
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8064
    true_std: null
    value_gap_source_arxiv: '2007.11202'
    value_gap_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for
      Graph Representation and Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.020299999999999985
    has_value_note: false
    value_note: ''
    sort_value: 0.8064
    sort_std: null
    global_rank: 21
    paper_rank: 62
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis
      for Graph Representation and Learning'
    comparison_source_arxiv: '2007.11202'
    is_best: false
    is_std_outlier: false
  - model: CSSL-Reg A1-all
    model_key: cssl-reg a1-all
    model_plain: CSSL-Reg A1-all
    value: 0.805
    std: 0.0134
    paper_value: 0.805
    paper_std: 0.0134
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV; 'all' uses all 5 datasets
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.805
    true_std: 0.0134
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.805
    sort_std: 0.0134
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
  - model: CSSL-Pretrain A3-all
    model_key: cssl-pretrain a3-all
    model_plain: CSSL-Pretrain A3-all
    value: 0.8025
    std: 0.0141
    paper_value: 0.8025
    paper_std: 0.0141
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV; Pretrain uses all 5 datasets
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8025
    true_std: 0.0141
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8025
    sort_std: 0.0141
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
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.7644
    std: 0.0235
    paper_value: 0.7644
    paper_std: 0.0235
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.7978
    at_pub_std: null
    at_pub_source_arxiv: '1704.02901'
    at_pub_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    at_pub_source_date_iso: '2017-04-10'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2017-04-10'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: 0.033399999999999985
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7978
    true_std: null
    value_gap_source_arxiv: '1704.02901'
    value_gap_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.033399999999999985
    has_value_note: false
    value_note: ''
    sort_value: 0.7978
    sort_std: null
    global_rank: 28
    paper_rank: 110
    rank_delta: 82
    rank_delta_abs: 82
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    comparison_source_arxiv: '1704.02901'
    is_best: false
    is_std_outlier: false
  - model: CSSL-Reg A3-specific
    model_key: cssl-reg a3-specific
    model_plain: CSSL-Reg A3-specific
    value: 0.7966
    std: 0.0171
    paper_value: 0.7966
    paper_std: 0.0171
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
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7966
    true_std: 0.0171
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7966
    sort_std: 0.0171
    global_rank: 32
    paper_rank: 32
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Reg A3-all
    model_key: cssl-reg a3-all
    model_plain: CSSL-Reg A3-all
    value: 0.7958
    std: 0.0141
    paper_value: 0.7958
    paper_std: 0.0141
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV; 'all' uses all 5 datasets
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7958
    true_std: 0.0141
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7958
    sort_std: 0.0141
    global_rank: 34
    paper_rank: 34
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.7006
    std: 0.0121
    paper_value: 0.7006
    paper_std: 0.0121
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.7937
    at_pub_std: 0.0094
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2020-07-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.09309999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7937
    true_std: null
    value_gap_source_arxiv: '2007.11202'
    value_gap_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for
      Graph Representation and Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.09309999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.7937
    sort_std: null
    global_rank: 40
    paper_rank: 178
    rank_delta: 138
    rank_delta_abs: 138
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Capsule Convolutional Neural Networks
    comparison_source_arxiv: '1805.08090'
    is_best: false
    is_std_outlier: false
  - model: EdgePool
    model_key: edgepool
    model_plain: EdgePool
    value: 0.792
    std: 0.0261
    paper_value: 0.792
    paper_std: 0.0261
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.792
    true_std: 0.0261
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.792
    sort_std: 0.0261
    global_rank: 44
    paper_rank: 44
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
    value: 0.7326
    std: 0.0446
    paper_value: 0.7326
    paper_std: 0.0446
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.759
    at_pub_std: null
    at_pub_source_arxiv: '1904.13107'
    at_pub_source_title: Graph Convolutional Networks with EigenPooling
    at_pub_source_date_iso: '2019-04-30'
    at_pub_source_date_label: KDD 2019
    value_gap_source_date_iso: '2020-12-16'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.02639999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7912
    true_std: 0.0307
    value_gap_source_arxiv: '2012.08734'
    value_gap_source_title: Hierarchical Graph Capsule Network
    value_gap_source_is_current_paper: false
    value_gap: 0.058599999999999985
    has_value_note: false
    value_note: ''
    sort_value: 0.7912
    sort_std: 0.0307
    global_rank: 46
    paper_rank: 156
    rank_delta: 110
    rank_delta_abs: 110
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SP
    model_key: sp
    model_plain: SP
    value: 0.7872
    std: 0.0389
    paper_value: 0.7872
    paper_std: 0.0389
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.79
    at_pub_std: 0.006
    at_pub_source_arxiv: '1606.01141'
    at_pub_source_title: On Valid Optimal Assignment Kernels and Applications to Graph
      Classification
    at_pub_source_date_iso: '2016-06-03'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2016-06-03'
    value_gap_source_date_label: NeurIPS 2016
    gap_vs_at_pub: 0.0028000000000000247
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.79
    true_std: 0.006
    value_gap_source_arxiv: '1606.01141'
    value_gap_source_title: On Valid Optimal Assignment Kernels and Applications to
      Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.0028000000000000247
    has_value_note: false
    value_note: ''
    sort_value: 0.79
    sort_std: 0.006
    global_rank: 48
    paper_rank: 58
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Freeze A1-specific
    model_key: cssl-freeze a1-specific
    model_plain: CSSL-Freeze A1-specific
    value: 0.7874
    std: 0.0092
    paper_value: 0.7874
    paper_std: 0.0092
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
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7874
    true_std: 0.0092
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7874
    sort_std: 0.0092
    global_rank: 58
    paper_rank: 58
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGPool
    model_key: sagpool
    model_plain: SAGPool
    value: 0.787
    std: 0.0229
    paper_value: 0.787
    paper_std: 0.0229
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.7707
    at_pub_std: null
    at_pub_source_arxiv: '2007.11202'
    at_pub_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for
      Graph Representation and Learning'
    at_pub_source_date_iso: '2020-07-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.01629999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.787
    true_std: 0.0229
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.787
    sort_std: 0.0229
    global_rank: 60
    paper_rank: 60
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EigenPool
    model_key: eigenpool
    model_plain: EigenPool
    value: 0.7863
    std: 0.0136
    paper_value: 0.7863
    paper_std: 0.0136
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.786
    at_pub_std: null
    at_pub_source_arxiv: '2007.11202'
    at_pub_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for
      Graph Representation and Learning'
    at_pub_source_date_iso: '2020-07-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7863
    true_std: 0.0136
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7863
    sort_std: 0.0136
    global_rank: 61
    paper_rank: 61
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Freeze A3-specific
    model_key: cssl-freeze a3-specific
    model_plain: CSSL-Freeze A3-specific
    value: 0.7849
    std: 0.0094
    paper_value: 0.7849
    paper_std: 0.0094
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
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7849
    true_std: 0.0094
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7849
    sort_std: 0.0094
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphlet
    model_key: graphlet
    model_plain: Graphlet
    value: 0.7254
    std: 0.0383
    paper_value: 0.7254
    paper_std: 0.0383
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.7845
    at_pub_std: null
    at_pub_source_arxiv: '2007.11202'
    at_pub_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for
      Graph Representation and Learning'
    at_pub_source_date_iso: '2020-07-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-07-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.05909999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7845
    true_std: null
    value_gap_source_arxiv: '2007.11202'
    value_gap_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for
      Graph Representation and Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.05909999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7845
    sort_std: null
    global_rank: 65
    paper_rank: 162
    rank_delta: 97
    rank_delta_abs: 97
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis
      for Graph Representation and Learning'
    comparison_source_arxiv: '2007.11202'
    is_best: false
    is_std_outlier: false
  - model: CSSL-Freeze A3-all
    model_key: cssl-freeze a3-all
    model_plain: CSSL-Freeze A3-all
    value: 0.7773
    std: 0.0173
    paper_value: 0.7773
    paper_std: 0.0173
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV; 'all' uses all 5 datasets
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7773
    true_std: 0.0173
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7773
    sort_std: 0.0173
    global_rank: 86
    paper_rank: 86
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.773
    std: 0.0368
    paper_value: 0.773
    paper_std: 0.0368
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.709
    at_pub_std: 0.04
    at_pub_source_arxiv: '1901.01343'
    at_pub_source_title: Graph Neural Networks With Convolutional ARMA Filters
    at_pub_source_date_iso: '2019-01-05'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.06400000000000006
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.773
    true_std: 0.0368
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.773
    sort_std: 0.0368
    global_rank: 101
    paper_rank: 101
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Freeze A1-all
    model_key: cssl-freeze a1-all
    model_plain: CSSL-Freeze A1-all
    value: 0.7596
    std: 0.016
    paper_value: 0.7596
    paper_std: 0.016
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV; 'all' uses all 5 datasets
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7596
    true_std: 0.016
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7596
    sort_std: 0.016
    global_rank: 121
    paper_rank: 121
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7578
    std: 0.0391
    paper_value: 0.7578
    paper_std: 0.0391
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.766
    at_pub_std: null
    at_pub_source_arxiv: '1904.13107'
    at_pub_source_title: Graph Convolutional Networks with EigenPooling
    at_pub_source_date_iso: '2019-04-30'
    at_pub_source_date_label: KDD 2019
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.008199999999999985
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7578
    true_std: 0.0391
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7578
    sort_std: 0.0391
    global_rank: 126
    paper_rank: 126
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCC-freezing
    model_key: gcc-freezing
    model_plain: GCC-freezing
    value: 0.7563
    std: 0.0322
    paper_value: 0.7563
    paper_std: 0.0322
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7563
    true_std: 0.0322
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7563
    sort_std: 0.0322
    global_rank: 129
    paper_rank: 129
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCC-finetuning
    model_key: gcc-finetuning
    model_plain: GCC-finetuning
    value: 0.7546
    std: 0.0244
    paper_value: 0.7546
    paper_std: 0.0244
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7546
    true_std: 0.0244
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7546
    sort_std: 0.0244
    global_rank: 132
    paper_rank: 132
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.7424
    std: 0.0086
    paper_value: 0.7424
    paper_std: 0.0086
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7424
    true_std: 0.0086
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7424
    sort_std: 0.0086
    global_rank: 149
    paper_rank: 149
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Set2Set
    model_key: set2set
    model_plain: Set2Set
    value: 0.7083
    std: 0.0084
    paper_value: 0.7083
    paper_std: 0.0084
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.745
    at_pub_std: null
    at_pub_source_arxiv: '1904.13107'
    at_pub_source_title: Graph Convolutional Networks with EigenPooling
    at_pub_source_date_iso: '2019-04-30'
    at_pub_source_date_label: KDD 2019
    value_gap_source_date_iso: '2023-06-22'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.036699999999999955
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7265
    true_std: 0.0047
    value_gap_source_arxiv: '2306.12726'
    value_gap_source_title: On Exploring Node-feature and Graph-structure Diversities
      for Node Drop Graph Pooling
    value_gap_source_is_current_paper: false
    value_gap: 0.018199999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.7265
    sort_std: 0.0047
    global_rank: 162
    paper_rank: 173
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Convolutional Networks with EigenPooling
    comparison_source_arxiv: '1904.13107'
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
- &id001
  dataset: NCI1
  rows:
  - model: Diverse B12C3
    model_key: msa-aud
    model_plain: Diverse B12C3
    value: 0.969
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2312.10943'
    title: Model Stealing Attack against Graph Classification with Authenticity, Uncertainty
      and Diversity
    date: Dec 18, 2023
    date_display: Dec 2023
    date_iso: '2023-12-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.969
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Diverse B12C3
    model_key: msa-au
    model_plain: Diverse B12C3
    value: 0.966
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.10943'
    title: Model Stealing Attack against Graph Classification with Authenticity, Uncertainty
      and Diversity
    date: Dec 18, 2023
    date_display: Dec 2023
    date_iso: '2023-12-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Diverse B12C3
    model_key: msa-ad
    model_plain: Diverse B12C3
    value: 0.963
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.10943'
    title: Model Stealing Attack against Graph Classification with Authenticity, Uncertainty
      and Diversity
    date: Dec 18, 2023
    date_display: Dec 2023
    date_iso: '2023-12-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.963
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.7773
    std: 0.0083
    paper_value: 0.7773
    paper_std: 0.0083
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.711
    at_pub_std: 0.03
    at_pub_source_arxiv: '2006.12138'
    at_pub_source_title: Graph Neural Networks in TensorFlow and Keras with Spektral
    at_pub_source_date_iso: '2020-06-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-04-24'
    value_gap_source_date_label: IJCAI 2024
    gap_vs_at_pub: 0.06630000000000003
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.921
    true_std: 0.026
    value_gap_source_arxiv: '2404.15806'
    value_gap_source_title: 'Where to Mask: Structure-Guided Masking for Graph Masked
      Autoencoders'
    value_gap_source_is_current_paper: false
    value_gap: 0.14370000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.921
    sort_std: 0.026
    global_rank: 7
    paper_rank: 332
    rank_delta: 325
    rank_delta_abs: 325
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Neural Networks in TensorFlow and Keras with Spektral
    comparison_source_arxiv: '2006.12138'
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.7665
    std: 0.0199
    paper_value: 0.7665
    paper_std: 0.0199
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.859
    at_pub_std: 0.001
    at_pub_source_arxiv: '1410.3314'
    at_pub_source_title: Propagation Kernels
    at_pub_source_date_iso: '2014-10-13'
    at_pub_source_date_label: '2014'
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.09250000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.86
    true_std: 0.018
    value_gap_source_arxiv: '2205.14368'
    value_gap_source_title: Going Deeper into Permutation-Sensitive Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.09350000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.018
    global_rank: 13
    paper_rank: 375
    rank_delta: 362
    rank_delta_abs: 362
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Propagation Kernels
    comparison_source_arxiv: '1410.3314'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7629
    std: 0.0179
    paper_value: 0.7629
    paper_std: 0.0179
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.802
    at_pub_std: 0.02
    at_pub_source_arxiv: '1905.13192'
    at_pub_source_title: 'Graph Neural Tangent Kernel: Fusing Graph Neural Networks
      with Graph Kernels'
    at_pub_source_date_iso: '2019-05-30'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2021-07-08'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.039100000000000024
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.84
    true_std: null
    value_gap_source_arxiv: '2107.04086'
    value_gap_source_title: Robust Counterfactual Explanations on Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07709999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.84
    sort_std: null
    global_rank: 39
    paper_rank: 386
    rank_delta: 347
    rank_delta_abs: 347
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Neural Tangent Kernel: Fusing Graph Neural Networks
      with Graph Kernels'
    comparison_source_arxiv: '1905.13192'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7473
    std: 0.0134
    paper_value: 0.7473
    paper_std: 0.0134
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.777
    at_pub_std: 0.015
    at_pub_source_arxiv: '1905.13192'
    at_pub_source_title: 'Graph Neural Tangent Kernel: Fusing Graph Neural Networks
      with Graph Kernels'
    at_pub_source_date_iso: '2019-05-30'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2023-10-03'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.02970000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8303
    true_std: 0.0137
    value_gap_source_arxiv: '2310.01794'
    value_gap_source_title: 'GnnX-Bench: Unravelling the Utility of Perturbation-based
      Gnn Explainers through In-depth Benchmarking'
    value_gap_source_is_current_paper: false
    value_gap: 0.08300000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.8303
    sort_std: 0.0137
    global_rank: 75
    paper_rank: 421
    rank_delta: 346
    rank_delta_abs: 346
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Neural Tangent Kernel: Fusing Graph Neural Networks
      with Graph Kernels'
    comparison_source_arxiv: '1905.13192'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.749
    std: 0.0172
    paper_value: 0.749
    paper_std: 0.0172
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-31'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.81
    true_std: 0.01
    value_gap_source_arxiv: '2201.13410'
    value_gap_source_title: 'Weisfeiler and Leman Go Infinite: Spectral and Combinatorial
      Pre-Colorings'
    value_gap_source_is_current_paper: false
    value_gap: 0.061000000000000054
    has_value_note: false
    value_note: ''
    sort_value: 0.81
    sort_std: 0.01
    global_rank: 172
    paper_rank: 419
    rank_delta: 247
    rank_delta_abs: 247
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Reg A3-specific
    model_key: cssl-reg a3-specific
    model_plain: CSSL-Reg A3-specific
    value: 0.8009
    std: 0.0107
    paper_value: 0.8009
    paper_std: 0.0107
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
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8009
    true_std: 0.0107
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8009
    sort_std: 0.0107
    global_rank: 221
    paper_rank: 221
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Reg A1-specific
    model_key: cssl-reg a1-specific
    model_plain: CSSL-Reg A1-specific
    value: 0.8007
    std: 0.006
    paper_value: 0.8007
    paper_std: 0.006
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
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8007
    true_std: 0.006
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8007
    sort_std: 0.006
    global_rank: 222
    paper_rank: 222
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Pretrain A3-specific
    model_key: cssl-pretrain a3-specific
    model_plain: CSSL-Pretrain A3-specific
    value: 0.7944
    std: 0.0067
    paper_value: 0.7944
    paper_std: 0.0067
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
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7944
    true_std: 0.0067
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7944
    sort_std: 0.0067
    global_rank: 250
    paper_rank: 250
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGPool
    model_key: sagpool
    model_plain: SAGPool
    value: 0.7788
    std: 0.0159
    paper_value: 0.7788
    paper_std: 0.0159
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.694
    at_pub_std: 0.084
    at_pub_source_arxiv: '2006.12138'
    at_pub_source_title: Graph Neural Networks in TensorFlow and Keras with Spektral
    at_pub_source_date_iso: '2020-06-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-04-04'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.0848000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.791
    true_std: 0.03
    value_gap_source_arxiv: '2304.01575'
    value_gap_source_title: The expressive power of pooling in Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.012199999999999989
    has_value_note: false
    value_note: ''
    sort_value: 0.791
    sort_std: 0.03
    global_rank: 260
    paper_rank: 326
    rank_delta: 66
    rank_delta_abs: 66
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePool
    model_key: edgepool
    model_plain: EdgePool
    value: 0.7656
    std: 0.0101
    paper_value: 0.7656
    paper_std: 0.0101
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-22'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7893
    true_std: 0.0222
    value_gap_source_arxiv: '2402.14393'
    value_gap_source_title: Graph Parsing Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.023700000000000054
    has_value_note: false
    value_note: ''
    sort_value: 0.7893
    sort_std: 0.0222
    global_rank: 270
    paper_rank: 376
    rank_delta: 106
    rank_delta_abs: 106
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EigenPool
    model_key: eigenpool
    model_plain: EigenPool
    value: 0.7724
    std: 0.0096
    paper_value: 0.7724
    paper_std: 0.0096
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.787
    true_std: 0.019
    value_gap_source_arxiv: '2009.10564'
    value_gap_source_title: 'GraphCrop: Subgraph Cropping for Graph Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.014600000000000057
    has_value_note: false
    value_note: ''
    sort_value: 0.787
    sort_std: 0.019
    global_rank: 279
    paper_rank: 354
    rank_delta: 75
    rank_delta_abs: 75
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Pretrain A1-specific
    model_key: cssl-pretrain a1-specific
    model_plain: CSSL-Pretrain A1-specific
    value: 0.7862
    std: 0.0063
    paper_value: 0.7862
    paper_std: 0.0063
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
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7862
    true_std: 0.0063
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7862
    sort_std: 0.0063
    global_rank: 287
    paper_rank: 287
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGP-SL
    model_key: hgp-sl
    model_plain: HGP-SL
    value: 0.7845
    std: 0.0077
    paper_value: 0.7845
    paper_std: 0.0077
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7845
    true_std: 0.0077
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7845
    sort_std: 0.0077
    global_rank: 300
    paper_rank: 300
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.7093
    std: 0.0178
    paper_value: 0.7093
    paper_std: 0.0178
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.775
    true_std: 0.0074
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.06569999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.775
    sort_std: 0.0074
    global_rank: 343
    paper_rank: 475
    rank_delta: 132
    rank_delta_abs: 132
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.7408
    std: 0.0219
    paper_value: 0.7408
    paper_std: 0.0219
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.7444
    at_pub_std: 0.0047
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2020-09-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.0035999999999999366
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.765
    true_std: 0.019
    value_gap_source_arxiv: '2009.10564'
    value_gap_source_title: 'GraphCrop: Subgraph Cropping for Graph Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.0242
    has_value_note: false
    value_note: ''
    sort_value: 0.765
    sort_std: 0.019
    global_rank: 377
    paper_rank: 435
    rank_delta: 58
    rank_delta_abs: 58
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: gPool
    model_key: gpool
    model_plain: gPool
    value: 0.7625
    std: 0.0139
    paper_value: 0.7625
    paper_std: 0.0139
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7625
    true_std: 0.0139
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7625
    sort_std: 0.0139
    global_rank: 389
    paper_rank: 389
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SP
    model_key: sp
    model_plain: SP
    value: 0.6744
    std: 0.0276
    paper_value: 0.6744
    paper_std: 0.0276
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.745
    at_pub_std: 0.003
    at_pub_source_arxiv: '1606.01141'
    at_pub_source_title: On Valid Optimal Assignment Kernels and Applications to Graph
      Classification
    at_pub_source_date_iso: '2016-06-03'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2016-06-03'
    value_gap_source_date_label: NeurIPS 2016
    gap_vs_at_pub: 0.0706
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.745
    true_std: 0.003
    value_gap_source_arxiv: '1606.01141'
    value_gap_source_title: On Valid Optimal Assignment Kernels and Applications to
      Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.0706
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.003
    global_rank: 424
    paper_rank: 508
    rank_delta: 84
    rank_delta_abs: 84
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Valid Optimal Assignment Kernels and Applications
      to Graph Classification
    comparison_source_arxiv: '1606.01141'
    is_best: false
    is_std_outlier: false
  - model: CSSL-Freeze A3-specific
    model_key: cssl-freeze a3-specific
    model_plain: CSSL-Freeze A3-specific
    value: 0.727
    std: 0.0194
    paper_value: 0.727
    paper_std: 0.0194
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
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.727
    true_std: 0.0194
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.727
    sort_std: 0.0194
    global_rank: 460
    paper_rank: 460
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CSSL-Freeze A1-specific
    model_key: cssl-freeze a1-specific
    model_plain: CSSL-Freeze A1-specific
    value: 0.726
    std: 0.0143
    paper_value: 0.726
    paper_std: 0.0143
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
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.726
    true_std: 0.0143
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.726
    sort_std: 0.0143
    global_rank: 463
    paper_rank: 463
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Set2Set
    model_key: set2set
    model_plain: Set2Set
    value: 0.6962
    std: 0.0132
    paper_value: 0.6962
    paper_std: 0.0132
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.715
    at_pub_std: null
    at_pub_source_arxiv: '1904.13107'
    at_pub_source_title: Graph Convolutional Networks with EigenPooling
    at_pub_source_date_iso: '2019-04-30'
    at_pub_source_date_label: KDD 2019
    value_gap_source_date_iso: '2023-06-22'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.018799999999999928
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.717
    true_std: 0.0073
    value_gap_source_arxiv: '2306.12726'
    value_gap_source_title: On Exploring Node-feature and Graph-structure Diversities
      for Node Drop Graph Pooling
    value_gap_source_is_current_paper: false
    value_gap: 0.02079999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.717
    sort_std: 0.0073
    global_rank: 466
    paper_rank: 491
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Convolutional Networks with EigenPooling
    comparison_source_arxiv: '1904.13107'
    is_best: false
    is_std_outlier: false
  - model: GCC-finetuning
    model_key: gcc-finetuning
    model_plain: GCC-finetuning
    value: 0.71
    std: 0.0178
    paper_value: 0.71
    paper_std: 0.0178
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.71
    true_std: 0.0178
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.71
    sort_std: 0.0178
    global_rank: 474
    paper_rank: 474
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCC-freezing
    model_key: gcc-freezing
    model_plain: GCC-freezing
    value: 0.6633
    std: 0.0265
    paper_value: 0.6633
    paper_std: 0.0265
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6633
    true_std: 0.0265
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6633
    sort_std: 0.0265
    global_rank: 515
    paper_rank: 515
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphlet
    model_key: graphlet
    model_plain: Graphlet
    value: 0.6248
    std: 0.0211
    paper_value: 0.6248
    paper_std: 0.0211
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Sep 13, 2020
    date_display: Sep 2020
    date_iso: '2020-09-13'
    published_venue: AAAI 2020
    published_conference: AAAI 2020
    at_pub_value: 0.624
    at_pub_std: 0.0027
    at_pub_source_arxiv: '1603.06186'
    at_pub_source_title: The Multiscale Laplacian Graph Kernel
    at_pub_source_date_iso: '2016-03-01'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2020-09-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.0008000000000000229
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.643
    true_std: 0.022
    value_gap_source_arxiv: '2009.10564'
    value_gap_source_title: 'GraphCrop: Subgraph Cropping for Graph Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.018199999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.643
    sort_std: 0.022
    global_rank: 530
    paper_rank: 539
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
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
    - dataset: NCI1
      dataset_slug: nci1
    - dataset: D&D
      dataset_slug: d-d
---

