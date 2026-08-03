---
title: Invariant Graph Learning Meets Information Bottleneck for Out-of-Distribution
  Generalization
arxiv_id: '2408.01697'
source_url: ''
authors:
- name: Wenyu Mao
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Jiancan Wu
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Haoyang Liu
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Yongduo Sui
  orcid: null
  s2_author_id: null
  s2_url: null
- name: Xiang Wang
  orcid: null
  s2_author_id: null
  s2_url: null
published_date: Aug 3, 2024
published_date_iso: '2024-08-03'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph out-of-distribution (OOD) generalization remains a major challenge
  in graph learning since graph neural networks (GNNs) often suffer from severe performance
  degradation under distribution shifts. Invariant learning, aiming to extract invariant
  features across varied distributions, has recently emerged as a promising approach
  for OOD generalization. Despite the great success of invariant learning in OOD problems
  for Euclidean data (images), the exploration within graph data remains constrained
  by the complex nature of graphs. The invariant features at both the attribute and
  structural levels, combined with the absence of prior knowledge regarding environmental
  factors, make the invariance and sufficiency conditions of invariant learning hard
  to satisfy on graph data. Existing studies, such as data augmentation or causal
  intervention, either suffer from disruptions to invariance during the graph manipulation
  process or face reliability issues due to a lack of supervised signals for causal
  parts. In this work, we propose a novel framework, called Invariant Graph Learning
  based on Information bottleneck theory (InfoIGL), to extract the invariant features
  of graphs and enhance models' generalization ability to unseen distributions. Specifically,
  InfoIGL introduces a redundancy filter to compress task-irrelevant information related
  to environmental factors. Cooperating with our designed multi-level contrastive
  learning, we maximize the mutual information among graphs of the same class in the
  downstream classification tasks, preserving invariant features for prediction to
  a great extent. An appealing feature of InfoIGL is its strong generalization ability
  without depending on supervised signal of invariance. Experiments on both synthetic
  and real-world datasets demonstrate that our method achieves state-of-the-art performance
  under OOD generalization for graph classification tasks. The source code is available
  at.
codebase_url: https://github.com/maowenyu-11/InfoIGL
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- InfoIGL
mrr: 0.0029
adjusted_mrr: 0.001
mrr_dataset_count: 1
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
  dataset: Amazon-Photo
  rows:
  - model: SGT
    model_key: msh-gnn
    model_plain: SGT
    value: 0.9766
    std: 0.005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9766
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGT
    model_key: geomancer
    model_plain: SGT
    value: 0.9705
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
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9705
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGT
    model_key: graphtarif
    model_plain: SGT
    value: 0.9703
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9703
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EERM
    model_key: eerm
    model_plain: EERM
    value: 0.9079
    std: 0.0218
    paper_value: 0.9079
    paper_std: 0.0218
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
    source_ref: wu2022handling
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Covariate shift split with distinct environment IDs as per EERM
      setting
    date: Aug 3, 2024
    date_display: Aug 2024
    date_iso: '2024-08-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.918
    true_std: 0.009
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: false
    value_gap: 0.010099999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.918
    sort_std: 0.009
    global_rank: 338
    paper_rank: 390
    rank_delta: 52
    rank_delta_abs: 52
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoIGL
    model_key: infoigl
    model_plain: InfoIGL
    value: 0.9173
    std: 0.0047
    paper_value: 0.9173
    paper_std: 0.0047
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Covariate shift split with distinct environment IDs as per EERM
      setting
    date: Aug 3, 2024
    date_display: Aug 2024
    date_iso: '2024-08-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9173
    true_std: 0.0047
    value_gap_source_arxiv: '2408.01697'
    value_gap_source_title: Invariant Graph Learning Meets Information Bottleneck
      for Out-of-Distribution Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9173
    sort_std: 0.0047
    global_rank: 343
    paper_rank: 343
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ERM
    model_key: erm
    model_plain: ERM
    value: 0.8806
    std: 0.0065
    paper_value: 0.8806
    paper_std: 0.0065
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Covariate shift split with distinct environment IDs as per EERM
      setting
    date: Aug 3, 2024
    date_display: Aug 2024
    date_iso: '2024-08-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-05'
    value_gap_source_date_label: TMLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.886
    true_std: 0.013
    value_gap_source_arxiv: '2602.05571'
    value_gap_source_title: 'EdgeMask-DG*: Learning Domain-Invariant Graph Structures
      via Adversarial Edge Masking'
    value_gap_source_is_current_paper: false
    value_gap: 0.00539999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.886
    sort_std: 0.013
    global_rank: 457
    paper_rank: 463
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
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
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
single_proposed_model: InfoIGL
---

