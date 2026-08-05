---
title: Label Deconvolution for Node Representation Learning on Large-scale Attributed
  Graphs against Learning Bias
arxiv_id: '2309.14907'
source_url: ''
authors:
- name: Zhihao Shi
  orcid: null
  s2_author_id: '2049467751'
  s2_url: null
- name: Jie Wang
  orcid: null
  s2_author_id: '2238243162'
  s2_url: null
- name: Fanghua Lu
  orcid: null
  s2_author_id: '120212140'
  s2_url: null
- name: Hanzhu Chen
  orcid: null
  s2_author_id: '2216099839'
  s2_url: null
- name: Defu Lian
  orcid: null
  s2_author_id: '1862782'
  s2_url: null
- name: Zheng Wang
  orcid: null
  s2_author_id: '2311493194'
  s2_url: null
- name: Jieping Ye
  orcid: null
  s2_author_id: '144030870'
  s2_url: null
- name: Feng Wu
  orcid: null
  s2_author_id: '2257430155'
  s2_url: null
published_date: Sep 26, 2023
published_date_iso: '2023-09-26'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Node representation learning on attributed graphs---whose nodes are associated
  with rich attributes (e.g., texts and protein sequences)---plays a crucial role
  in many important downstream tasks. To encode the attributes and graph structures
  simultaneously, recent studies integrate pre-trained models with graph neural networks
  (GNNs), where pre-trained models serve as node encoders (NEs) to encode the attributes.
  As jointly training large NEs and GNNs on large-scale graphs suffers from severe
  scalability issues, many methods propose to train NEs and GNNs separately. Consequently,
  they do not take feature convolutions in GNNs into consideration in the training
  phase of NEs, leading to a significant learning bias relative to the joint training.
  To address this challenge, we propose an efficient label regularization technique,
  namely Label Deconvolution (LD), to alleviate the learning bias by a novel and highly
  scalable approximation to the inverse mapping of GNNs. The inverse mapping leads
  to an objective function that is equivalent to that by the joint training, while
  it can effectively incorporate GNNs in the training phase of NEs against the learning
  bias. More importantly, we show that LD converges to the optimal objective function
  values by the joint training under mild assumptions. Experiments demonstrate LD
  significantly outperforms state-of-the-art methods on Open Graph Benchmark datasets.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- LD
mrr: 0.5312
adjusted_mrr: 0.3542
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
- &id002
  dataset: ogbn-arxiv
  rows:
  - model: EGP (GCN)
    model_key: ofa
    model_plain: EGP (GCN)
    value: 0.7764
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2407.19941'
    title: Boosting Cross-Domain and Cross-Task Generalization for Text-Attributed
      Graphs from Structural Perspective
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: null
    codebase_url: https://github.com/cy623/BooG
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7764
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EGP (GCN)
    model_key: giant-xrt
    model_plain: EGP (GCN)
    value: 0.7612
    std: 0.0016
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2111.00064'
    title: Node Feature Extraction by Self-Supervised Multi-scale Neighborhood Prediction
    date: Oct 29, 2021
    date_display: Oct 2021
    date_iso: '2021-10-29'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amzn/pecos
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7612
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EGP (GCN)
    model_key: gegcn
    model_plain: EGP (GCN)
    value: 0.7576
    std: 0.0064
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.26178'
    title: 'Geometric Evolution Graph Convolutional Networks: Enhancing Graph Representation
      Learning via Ricci Flow'
    date: Mar 27, 2026
    date_display: Mar 2026
    date_iso: '2026-03-27'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: integrates Ricci flow with deep graph models... multi-scale
      structural information is then incorporated into a GCN
    is_global_top: true
    global_rank: 3
    sort_value: 0.7576
    sort_std: 0.0064
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: X_OGB
    model_key: x_ogb
    model_plain: X_OGB
    value: 0.7174
    std: 0.0029
    paper_value: 0.7174
    paper_std: 0.0029
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
    feature_source_evidence: the features provided by OGB, denoted as X_OGB
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-arxiv using official OGB features.
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-26'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7174
    true_std: 0.0029
    value_gap_source_arxiv: '2309.14907'
    value_gap_source_title: Label Deconvolution for Node Representation Learning on
      Large-scale Attributed Graphs against Learning Bias
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7174
    sort_std: 0.0029
    global_rank: 65
    paper_rank: 65
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
  - model: SAGN
    model_key: sagn
    model_plain: SAGN
    value: 0.8718
    std: 0.0004
    paper_value: 0.8718
    paper_std: 0.0004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test split, Accuracy
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8736
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2210.14709'
    at_pub_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    at_pub_source_date_iso: 2022-10
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: 2022-10
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.0018000000000000238
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8736
    true_std: 0.0007
    value_gap_source_arxiv: '2210.14709'
    value_gap_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    value_gap_source_is_current_paper: false
    value_gap: 0.0018000000000000238
    has_value_note: false
    value_note: ''
    sort_value: 0.8736
    sort_std: 0.0007
    global_rank: 5
    paper_rank: 9
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning on Large-scale Text-attributed Graphs via Variational
      Inference
    comparison_source_arxiv: '2210.14709'
    is_best: false
    is_std_outlier: false
  - model: LD
    model_key: ld
    model_plain: LD
    value: 0.8645
    std: 0.0012
    paper_value: 0.8645
    paper_std: 0.0012
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
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test split, Accuracy
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-26'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8645
    true_std: 0.0012
    value_gap_source_arxiv: '2309.14907'
    value_gap_source_title: Label Deconvolution for Node Representation Learning on
      Large-scale Attributed Graphs against Learning Bias
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8645
    sort_std: 0.0012
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
  - model: X_GLEM
    model_key: x_glem
    model_plain: X_GLEM
    value: 0.8509
    std: 0.0021
    paper_value: 0.8509
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test split, Accuracy
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-26'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8509
    true_std: 0.0021
    value_gap_source_arxiv: '2309.14907'
    value_gap_source_title: Label Deconvolution for Node Representation Learning on
      Large-scale Attributed Graphs against Learning Bias
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8509
    sort_std: 0.0021
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
  - model: X_PNE
    model_key: x_pne
    model_plain: X_PNE
    value: 0.8451
    std: 0.0005
    paper_value: 0.8451
    paper_std: 0.0005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test split, Accuracy
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-26'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8451
    true_std: 0.0005
    value_gap_source_arxiv: '2309.14907'
    value_gap_source_title: Label Deconvolution for Node Representation Learning on
      Large-scale Attributed Graphs against Learning Bias
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8451
    sort_std: 0.0005
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
  - model: GAMLP
    model_key: gamlp
    model_plain: GAMLP
    value: 0.8354
    std: 0.0009
    paper_value: 0.8354
    paper_std: 0.0009
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test split, Accuracy
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8376
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2210.07494'
    at_pub_source_title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking
      and Rethinking'
    at_pub_source_date_iso: '2022-10-14'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0021999999999999797
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
  - model: X_GIANT
    model_key: x_giant
    model_plain: X_GIANT
    value: 0.8316
    std: 0.0007
    paper_value: 0.8316
    paper_std: 0.0007
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test split, Accuracy
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-26'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8316
    true_std: 0.0007
    value_gap_source_arxiv: '2309.14907'
    value_gap_source_title: Label Deconvolution for Node Representation Learning on
      Large-scale Attributed Graphs against Learning Bias
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8316
    sort_std: 0.0007
    global_rank: 65
    paper_rank: 65
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: X_FNE
    model_key: x_fne
    model_plain: X_FNE
    value: 0.8288
    std: 0.0005
    paper_value: 0.8288
    paper_std: 0.0005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-products (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: test split, Accuracy
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-26'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8288
    true_std: 0.0005
    value_gap_source_arxiv: '2309.14907'
    value_gap_source_title: Label Deconvolution for Node Representation Learning on
      Large-scale Attributed Graphs against Learning Bias
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8288
    sort_std: 0.0005
    global_rank: 73
    paper_rank: 73
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
- &id003
  dataset: ogbn-proteins
  rows:
  - model: LD
    model_key: ld
    model_plain: LD
    value: 0.8942
    std: 0.0007
    paper_value: 0.8942
    paper_std: 0.0007
    metric: ROC-AUC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-proteins (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test split, ROC-AUC metric
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-26'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8942
    true_std: 0.0007
    value_gap_source_arxiv: '2309.14907'
    value_gap_source_title: Label Deconvolution for Node Representation Learning on
      Large-scale Attributed Graphs against Learning Bias
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8942
    sort_std: 0.0007
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
  - model: X_WO/LD
    model_key: x_wo/ld
    model_plain: X_WO/LD
    value: 0.8915
    std: 0.0012
    paper_value: 0.8915
    paper_std: 0.0012
    metric: ROC-AUC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-proteins (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test split, ROC-AUC metric
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-26'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8915
    true_std: 0.0012
    value_gap_source_arxiv: '2309.14907'
    value_gap_source_title: Label Deconvolution for Node Representation Learning on
      Large-scale Attributed Graphs against Learning Bias
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8915
    sort_std: 0.0012
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
  - model: RevGNN
    model_key: mog
    model_plain: RevGNN
    value: 0.8904
    std: 0.0072
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.14260'
    title: Graph Sparsification via Mixture of Graphs
    date: May 23, 2024
    date_display: May 2024
    date_iso: '2024-05-23'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/yanweiyue/MoG
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8904
    sort_std: 0.0072
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: X_PNE
    model_key: x_pne
    model_plain: X_PNE
    value: 0.8894
    std: 0.0014
    paper_value: 0.8894
    paper_std: 0.0014
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-proteins (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test split, ROC-AUC metric
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-26'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8894
    true_std: 0.0014
    value_gap_source_arxiv: '2309.14907'
    value_gap_source_title: Label Deconvolution for Node Representation Learning on
      Large-scale Attributed Graphs against Learning Bias
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8894
    sort_std: 0.0014
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
  - model: X_GLEM
    model_key: x_glem
    model_plain: X_GLEM
    value: 0.8872
    std: null
    paper_value: 0.8872
    paper_std: null
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: GLEM and GIANT mainly focus on the text-attributed graph
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-proteins (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test split, ROC-AUC metric
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-26'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8872
    true_std: null
    value_gap_source_arxiv: '2309.14907'
    value_gap_source_title: Label Deconvolution for Node Representation Learning on
      Large-scale Attributed Graphs against Learning Bias
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8872
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
  - model: X_FNE
    model_key: x_fne
    model_plain: X_FNE
    value: 0.8866
    std: 0.0008
    paper_value: 0.8866
    paper_std: 0.0008
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-proteins (score=96)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test split, ROC-AUC metric
    date: Sep 26, 2023
    date_display: Sep 2023
    date_iso: '2023-09-26'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-26'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8866
    true_std: 0.0008
    value_gap_source_arxiv: '2309.14907'
    value_gap_source_title: Label Deconvolution for Node Representation Learning on
      Large-scale Attributed Graphs against Learning Bias
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8866
    sort_std: 0.0008
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
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
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
    - dataset: ogbn-arxiv
      dataset_slug: ogbn-arxiv
    - dataset: ogbn-proteins
      dataset_slug: ogbn-proteins
single_proposed_model: LD
main_figure: /figures/2309.14907/main_figure.jpegoptim.jpg
---

