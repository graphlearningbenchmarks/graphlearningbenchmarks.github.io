---
title: 'Propagate & Distill: Towards Effective Graph Learners Using Propagation-Embracing
  MLPs'
arxiv_id: '2311.17781'
source_url: ''
authors:
- name: Yong-Min Shin
  orcid: null
  s2_author_id: '2087244325'
  s2_url: null
- name: Won-Yong Shin
  orcid: null
  s2_author_id: '2267336556'
  s2_url: null
published_date: Nov 29, 2023
published_date_iso: '2023-11-29'
published_venue: LoG 2023
published_conference: LoG 2023
published_conference_short: LoG
published_conference_slug: log
abstract: Recent studies attempted to utilize multilayer perceptrons (MLPs) to solve
  semi-supervised node classification on graphs, by training a student MLP by knowledge
  distillation from a teacher graph neural network (GNN). While previous studies have
  focused mostly on training the student MLP by matching the output probability distributions
  between the teacher and student models during distillation, it has not been systematically
  studied how to inject the structural information in an explicit and interpretable
  manner. Inspired by GNNs that separate feature transformation $T$ and propagation
  $ $, we re-frame the distillation process as making the student MLP learn both $T$
  and $ $. Although this can be achieved by applying the inverse propagation $ ^-1$
  before distillation from the teacher, it still comes with a high computational cost
  from large matrix multiplications during training. To solve this problem, we propose
  Propagate & Distill (P&D), which propagates the output of the teacher before distillation,
  which can be interpreted as an approximate process of the inverse propagation. We
  demonstrate that P&D can readily improve the performance of the student MLP.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- P&D
mrr: 0.005
adjusted_mrr: 0.0033
mrr_dataset_count: 2
benchmark_categories:
- Classic
- OGB
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Cora
  rows:
  - model: SGC+TSC
    model_key: exphormer
    model_plain: SGC+TSC
    value: 0.9635
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9635
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: sgformer
    model_plain: SGC+TSC
    value: 0.9629
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9629
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: coral
    model_plain: SGC+TSC
    value: 0.9574
    std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9574
    sort_std: 0.0039
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GLNN
    model_key: glnn
    model_plain: GLNN
    value: 0.8073
    std: 0.0342
    paper_value: 0.8073
    paper_std: 0.0342
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
    source_ref: zhang2022glnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting, Planetoid split (20/30 nodes per class),
      Accuracy
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: 0.836
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2307.06631'
    at_pub_source_title: Frameless Graph Knowledge Distillation
    at_pub_source_date_iso: '2023-07-13'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-07-13'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.028699999999999948
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.836
    true_std: 0.0022
    value_gap_source_arxiv: '2307.06631'
    value_gap_source_title: Frameless Graph Knowledge Distillation
    value_gap_source_is_current_paper: false
    value_gap: 0.028699999999999948
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.0022
    global_rank: 461
    paper_rank: 749
    rank_delta: 288
    rank_delta_abs: 288
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: P&D-fix
    model_key: p&d-fix
    model_plain: P&D-fix
    value: 0.8229
    std: 0.016
    paper_value: 0.8229
    paper_std: 0.016
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting, Planetoid split (20/30 nodes per class),
      Accuracy
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8229
    true_std: 0.016
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8229
    sort_std: 0.016
    global_rank: 618
    paper_rank: 618
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InvKD
    model_key: invkd
    model_plain: InvKD
    value: 0.8222
    std: 0.0145
    paper_value: 0.8222
    paper_std: 0.0145
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting, Planetoid split (20/30 nodes per class),
      Accuracy
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8222
    true_std: 0.0145
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8222
    sort_std: 0.0145
    global_rank: 625
    paper_rank: 625
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
  dataset: PubMed
  rows:
  - model: R-SoftGraphAIN
    model_key: lgtl
    model_plain: R-SoftGraphAIN
    value: 0.9518
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9518
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: sagn
    model_plain: R-SoftGraphAIN
    value: 0.9517
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
    arxiv_id: '2605.24867'
    title: 'Clustering as Reasoning: A $k$-Means Interpretation of Chain-of-Thought
      Graph Learning'
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    venue: Accepted by ICML 2026
    codebase_url: https://github.com/Uncnbb/KCoT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9517
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: mixhop (lo)
    model_plain: R-SoftGraphAIN
    value: 0.9513
    std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GLNN
    model_key: glnn
    model_plain: GLNN
    value: 0.7639
    std: 0.0236
    paper_value: 0.7639
    paper_std: 0.0236
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
    source_ref: zhang2022glnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting, Planetoid split (20/30 nodes per class),
      Accuracy
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: 0.796
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2307.06631'
    at_pub_source_title: Frameless Graph Knowledge Distillation
    at_pub_source_date_iso: '2023-07-13'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03210000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8027
    true_std: 0.0036
    value_gap_source_arxiv: '2405.03401'
    value_gap_source_title: 'E2GNN: Efficient Graph Neural Network Ensembles for Semi-Supervised
      Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.038799999999999946
    has_value_note: false
    value_note: ''
    sort_value: 0.8027
    sort_std: 0.0036
    global_rank: 451
    paper_rank: 790
    rank_delta: 339
    rank_delta_abs: 339
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Frameless Graph Knowledge Distillation
    comparison_source_arxiv: '2307.06631'
    is_best: false
    is_std_outlier: false
  - model: P&D-fix
    model_key: p&d-fix
    model_plain: P&D-fix
    value: 0.7811
    std: 0.0289
    paper_value: 0.7811
    paper_std: 0.0289
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting, Planetoid split (20/30 nodes per class),
      Accuracy
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7811
    true_std: 0.0289
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7811
    sort_std: 0.0289
    global_rank: 702
    paper_rank: 702
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: P&D
    model_key: p&d
    model_plain: P&D
    value: 0.7788
    std: 0.0289
    paper_value: 0.7788
    paper_std: 0.0289
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
    protocol_note: Transductive setting, Planetoid split (20/30 nodes per class),
      Accuracy
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7788
    true_std: 0.0289
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7788
    sort_std: 0.0289
    global_rank: 728
    paper_rank: 728
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: L_invkd
    model_key: l_invkd
    model_plain: L_invkd
    value: 0.7767
    std: 0.0073
    paper_value: 0.7767
    paper_std: 0.0073
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting, Planetoid split
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7767
    true_std: 0.0073
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7767
    sort_std: 0.0073
    global_rank: 741
    paper_rank: 741
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InvKD
    model_key: invkd
    model_plain: InvKD
    value: 0.7724
    std: null
    paper_value: 0.7724
    paper_std: null
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
    table_ref: Table 7
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Transductive setting, Teacher: APPNP, Planetoid split'
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7724
    true_std: null
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7724
    sort_std: null
    global_rank: 758
    paper_rank: 758
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: L_distill
    model_key: l_distill
    model_plain: L_distill
    value: 0.7677
    std: 0.0102
    paper_value: 0.7677
    paper_std: 0.0102
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting, Planetoid split
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7677
    true_std: 0.0102
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7677
    sort_std: 0.0102
    global_rank: 779
    paper_rank: 779
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Teacher GNN
    model_key: teacher gnn
    model_plain: Teacher GNN
    value: 0.7549
    std: 0.0225
    paper_value: 0.7549
    paper_std: 0.0225
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting, Planetoid split (20/30 nodes per class),
      Accuracy
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7549
    true_std: 0.0225
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7549
    sort_std: 0.0225
    global_rank: 816
    paper_rank: 816
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Plain MLP
    model_key: plain mlp
    model_plain: Plain MLP
    value: 0.6839
    std: 0.0309
    paper_value: 0.6839
    paper_std: 0.0309
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting, Planetoid split (20/30 nodes per class),
      Accuracy
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6839
    true_std: 0.0309
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6839
    sort_std: 0.0309
    global_rank: 885
    paper_rank: 885
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: L_conv
    model_key: l_conv
    model_plain: L_conv
    value: 0.6027
    std: 0.0964
    paper_value: 0.6027
    paper_std: 0.0964
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive setting, Planetoid split
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6027
    true_std: 0.0964
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6027
    sort_std: 0.0964
    global_rank: 902
    paper_rank: 902
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
  - model: Teacher GNN
    model_key: teacher gnn
    model_plain: Teacher GNN
    value: 0.7064
    std: 0.0041
    paper_value: 0.7064
    paper_std: 0.0041
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
    variant_inference_reason: 'dataset: fuzzy match to ogbn-arxiv (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive setting, Accuracy, OGB-arxiv
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7064
    true_std: 0.0041
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7064
    sort_std: 0.0041
    global_rank: 91
    paper_rank: 91
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: P&D
    model_key: p&d
    model_plain: P&D
    value: 0.652
    std: 0.0045
    paper_value: 0.652
    paper_std: 0.0045
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
    feature_source_evidence: fixing the input of the student MLP to the node features
      only
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-arxiv (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive setting, Accuracy, OGB-arxiv
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.652
    true_std: 0.0045
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.652
    sort_std: 0.0045
    global_rank: 116
    paper_rank: 116
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: P&D-fix
    model_key: p&d-fix
    model_plain: P&D-fix
    value: 0.6514
    std: 0.0035
    paper_value: 0.6514
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
    input_feature_source: raw_features
    feature_source_evidence: fixing the input of the student MLP to the node features
      only
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-arxiv (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive setting, Accuracy, OGB-arxiv
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6514
    true_std: 0.0035
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6514
    sort_std: 0.0035
    global_rank: 117
    paper_rank: 117
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GLNN
    model_key: glnn
    model_plain: GLNN
    value: 0.6302
    std: 0.0041
    paper_value: 0.6302
    paper_std: 0.0041
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
    source_ref: zhang2022glnn
    variant_inference_reason: 'dataset: fuzzy match to ogbn-arxiv (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive setting, Accuracy, OGB-arxiv
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6302
    true_std: 0.0041
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6302
    sort_std: 0.0041
    global_rank: 119
    paper_rank: 119
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Plain MLP
    model_key: plain mlp
    model_plain: Plain MLP
    value: 0.5533
    std: 0.0154
    paper_value: 0.5533
    paper_std: 0.0154
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbn-arxiv (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive setting, Accuracy, OGB-arxiv
    date: Nov 29, 2023
    date_display: Nov 2023
    date_iso: '2023-11-29'
    published_venue: LoG 2023
    published_conference: LoG 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-11-29'
    value_gap_source_date_label: LoG 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5533
    true_std: 0.0154
    value_gap_source_arxiv: '2311.17781'
    value_gap_source_title: 'Propagate & Distill: Towards Effective Graph Learners
      Using Propagation-Embracing MLPs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5533
    sort_std: 0.0154
    global_rank: 123
    paper_rank: 123
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
- benchmark: OGB
  datasets:
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: PubMed
      dataset_slug: pubmed
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-arxiv
      dataset_slug: ogbn-arxiv
single_proposed_model: P&D
main_figure: /figures/2311.17781/main_figure.jpegoptim.jpg
---

