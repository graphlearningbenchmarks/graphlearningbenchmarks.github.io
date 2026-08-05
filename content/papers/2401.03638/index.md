---
title: Unifying Graph Contrastive Learning via Graph Message Augmentation
arxiv_id: '2401.03638'
source_url: ''
authors:
- name: Ziyan Zhang
  orcid: null
  s2_author_id: '152780956'
  s2_url: null
- name: Bo Jiang
  orcid: null
  s2_author_id: '152390773'
  s2_url: null
- name: Jin Tang
  orcid: null
  s2_author_id: '2260595835'
  s2_url: null
- name: Bin Luo
  orcid: null
  s2_author_id: '2213563581'
  s2_url: null
published_date: Jan 8, 2024
published_date_iso: '2024-01-08'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph contrastive learning is usually performed by first conducting Graph
  Data Augmentation (GDA) and then employing a contrastive learning pipeline to train
  GNNs. As we know that GDA is an important issue for graph contrastive learning.
  Various GDAs have been developed recently which mainly involve dropping or perturbing
  edges, nodes, node attributes and edge attributes. However, to our knowledge, it
  still lacks a universal and effective augmentor that is suitable for different types
  of graph data. To address this issue, in this paper, we first introduce the graph
  message representation of graph data. Based on it, we then propose a novel Graph
  Message Augmentation (GMA), a universal scheme for reformulating many existing GDAs.
  The proposed unified GMA not only gives a new perspective to understand many existing
  GDAs but also provides a universal and more effective graph data augmentation for
  graph self-supervised learning tasks. Moreover, GMA introduces an easy way to implement
  the mixup augmentor which is natural for images but usually challengeable for graphs.
  Based on the proposed GMA, we then propose a unified graph contrastive learning,
  termed Graph Message Contrastive Learning (GMCL), that employs attribution-guided
  universal GMA for graph contrastive learning. Experiments on many graph learning
  tasks demonstrate the effectiveness and benefits of the proposed GMA and GMCL approaches.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 5
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id003
  dataset: COLLAB
  rows:
  - model: GPM
    model_key: wl-mlp
    model_plain: GPM
    value: 0.9792
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9792
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPM
    model_key: msh-gnn
    model_plain: GPM
    value: 0.964
    std: 0.007
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
    global_rank: 2
    sort_value: 0.964
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPM
    model_key: cocn
    model_plain: GPM
    value: 0.8722
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.18480'
    title: Scalable Graph Compressed Convolutions
    date: Jul 26, 2024
    date_display: Jul 2024
    date_iso: '2024-07-26'
    venue: arXiv.org
    codebase_url: https://github.com/sunjss/CoCN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: use the one-hot encoding of node degrees as node features
    is_global_top: true
    global_rank: 3
    sort_value: 0.8722
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAOv2
    model_key: joaov2
    model_plain: JOAOv2
    value: 0.7553
    std: 0.0018
    paper_value: 0.7553
    paper_std: 0.0018
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
    table_ref: Table 2
    source_ref: JOAO
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8216
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.06630000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8216
    true_std: 0.0017
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.06630000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8216
    sort_std: 0.0017
    global_rank: 40
    paper_rank: 267
    rank_delta: 227
    rank_delta_abs: 227
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.755
    std: 0.0215
    paper_value: 0.755
    paper_std: 0.0215
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
    table_ref: Table 2
    source_ref: graphcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8108
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.05579999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8108
    true_std: 0.0017
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.05579999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8108
    sort_std: 0.0017
    global_rank: 92
    paper_rank: 268
    rank_delta: 176
    rank_delta_abs: 176
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: Infomax
    model_key: infomax
    model_plain: Infomax
    value: 0.7375
    std: 0.0029
    paper_value: 0.7375
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: DGI
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8104
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.07289999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8104
    true_std: 0.0012
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.07289999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8104
    sort_std: 0.0012
    global_rank: 93
    paper_rank: 302
    rank_delta: 209
    rank_delta_abs: 209
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.7532
    std: 0.0256
    paper_value: 0.7532
    paper_std: 0.0256
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
    table_ref: Table 2
    source_ref: zhu2020deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.796
    true_std: 0.013
    value_gap_source_arxiv: '2410.10241'
    value_gap_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    value_gap_source_is_current_paper: false
    value_gap: 0.04280000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.796
    sort_std: 0.013
    global_rank: 163
    paper_rank: 276
    rank_delta: 113
    rank_delta_abs: 113
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.7065
    std: 0.0113
    paper_value: 0.7065
    paper_std: 0.0113
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
    source_ref: infograph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.794
    at_pub_std: null
    at_pub_source_arxiv: '2103.00959'
    at_pub_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    at_pub_source_date_iso: '2021-03-01'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2021-03-01'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: 0.08750000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.794
    true_std: null
    value_gap_source_arxiv: '2103.00959'
    value_gap_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.08750000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.794
    sort_std: null
    global_rank: 165
    paper_rank: 328
    rank_delta: 163
    rank_delta_abs: 163
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    comparison_source_arxiv: '2103.00959'
    is_best: false
    is_std_outlier: false
  - model: GMCL-M
    model_key: gmcl-m
    model_plain: GMCL-M
    value: 0.767
    std: 0.018
    paper_value: 0.767
    paper_std: 0.018
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.767
    sort_std: 0.018
    global_rank: 245
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
  - model: GMCL-P
    model_key: gmcl-p
    model_plain: GMCL-P
    value: 0.7644
    std: 0.0167
    paper_value: 0.7644
    paper_std: 0.0167
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.7644
    sort_std: 0.0167
    global_rank: 249
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
  - model: GMCL-D
    model_key: gmcl-d
    model_plain: GMCL-D
    value: 0.764
    std: 0.014
    paper_value: 0.764
    paper_std: 0.014
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.764
    sort_std: 0.014
    global_rank: 251
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
  - model: AD-GCL
    model_key: ad-gcl
    model_plain: AD-GCL
    value: 0.7582
    std: 0.0026
    paper_value: 0.7582
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: ADGCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7582
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2209.06560'
    at_pub_source_title: Graph Contrastive Learning with Personalized Augmentation
    at_pub_source_date_iso: '2022-09-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-09-14'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7582
    true_std: 0.0026
    value_gap_source_arxiv: '2209.06560'
    value_gap_source_title: Graph Contrastive Learning with Personalized Augmentation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7582
    sort_std: 0.0026
    global_rank: 262
    paper_rank: 262
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AutoGCL
    model_key: autogcl
    model_plain: AutoGCL
    value: 0.7716
    std: 0.0148
    paper_value: 0.7716
    paper_std: 0.0148
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
    table_ref: Table 2
    source_ref: autoGCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7716
    at_pub_std: 0.0148
    at_pub_source_arxiv: '2305.17437'
    at_pub_source_title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-05-27'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2022-02-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.745
    true_std: 0.002
    value_gap_source_arxiv: '2202.13248'
    value_gap_source_title: Automated Data Augmentations for Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.026599999999999957
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.002
    global_rank: 289
    paper_rank: 232
    rank_delta: -57
    rank_delta_abs: 57
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.7432
    std: 0.023
    paper_value: 0.7432
    paper_std: 0.023
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
    table_ref: Table 2
    source_ref: GCA
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.7432
    sort_std: 0.023
    global_rank: 291
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: IMDB-BINARY
  rows:
  - model: DMoNPool-TIP
    model_key: gcfl
    model_plain: DMoNPool-TIP
    value: 0.8299
    std: 0.052
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2106.13423'
    title: Federated Graph Classification over Non-IID Graphs
    date: Jun 25, 2021
    date_display: Jun 2021
    date_iso: '2021-06-25'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8299
    sort_std: 0.052
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DMoNPool-TIP
    model_key: gat +del-f
    model_plain: DMoNPool-TIP
    value: 0.7863
    std: 0.0054
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_display: Feb 2024
    date_iso: '2024-02-26'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7863
    sort_std: 0.0054
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DMoNPool-TIP
    model_key: graph transformer +del-f
    model_plain: DMoNPool-TIP
    value: 0.7828
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2402.16402'
    title: Graph Learning with Distributional Edge Layouts
    date: Feb 26, 2024
    date_display: Feb 2024
    date_iso: '2024-02-26'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7828
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GMCL-P
    model_key: gmcl-p
    model_plain: GMCL-P
    value: 0.756
    std: 0.0317
    paper_value: 0.756
    paper_std: 0.0317
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.756
    sort_std: 0.0317
    global_rank: 25
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
    is_best: true
    is_std_outlier: false
  - model: GMCL-D
    model_key: gmcl-d
    model_plain: GMCL-D
    value: 0.752
    std: 0.0404
    paper_value: 0.752
    paper_std: 0.0404
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.752
    sort_std: 0.0404
    global_rank: 30
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
    is_best: true
    is_std_outlier: false
  - model: GMCL-M
    model_key: gmcl-m
    model_plain: GMCL-M
    value: 0.751
    std: 0.0416
    paper_value: 0.751
    paper_std: 0.0416
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.751
    sort_std: 0.0416
    global_rank: 33
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
    is_best: true
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.723
    std: 0.0344
    paper_value: 0.723
    paper_std: 0.0344
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
    source_ref: wlsubtree
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.723
    at_pub_std: 0.034
    at_pub_source_arxiv: '2006.05582'
    at_pub_source_title: Contrastive Multi-View Representation Learning on Graphs
    at_pub_source_date_iso: '2020-06-01'
    at_pub_source_date_label: ICML 2020
    value_gap_source_date_iso: '2024-02-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.734
    true_std: 0.0463
    value_gap_source_arxiv: '2402.16402'
    value_gap_source_title: Graph Learning with Distributional Edge Layouts
    value_gap_source_is_current_paper: false
    value_gap: 0.01100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.734
    sort_std: 0.0463
    global_rank: 72
    paper_rank: 98
    rank_delta: 26
    rank_delta_abs: 26
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.7303
    std: 0.0087
    paper_value: 0.7303
    paper_std: 0.0087
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
    source_ref: infograph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7303
    at_pub_std: 0.0087
    at_pub_source_arxiv: '2111.03220'
    at_pub_source_title: 'Augmentations in Graph Contrastive Learning: Current Methodological
      Flaws & Towards Better Practices'
    at_pub_source_date_iso: '2021-11-05'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2021-11-05'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7303
    true_std: 0.0087
    value_gap_source_arxiv: '2111.03220'
    value_gap_source_title: 'Augmentations in Graph Contrastive Learning: Current
      Methodological Flaws & Towards Better Practices'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7303
    sort_std: 0.0087
    global_rank: 82
    paper_rank: 82
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.7135
    std: 0.0046
    paper_value: 0.7135
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zhu2020deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.7135
    sort_std: 0.0046
    global_rank: 122
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
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.7114
    std: 0.0044
    paper_value: 0.7114
    paper_std: 0.0044
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
    source_ref: graphcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7114
    at_pub_std: 0.0044
    at_pub_source_arxiv: '2111.03220'
    at_pub_source_title: 'Augmentations in Graph Contrastive Learning: Current Methodological
      Flaws & Towards Better Practices'
    at_pub_source_date_iso: '2021-11-05'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2021-11-05'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7114
    true_std: 0.0044
    value_gap_source_arxiv: '2111.03220'
    value_gap_source_title: 'Augmentations in Graph Contrastive Learning: Current
      Methodological Flaws & Towards Better Practices'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7114
    sort_std: 0.0044
    global_rank: 122
    paper_rank: 122
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: graph2vec
    model_key: graph2vec
    model_plain: graph2vec
    value: 0.711
    std: 0.0054
    paper_value: 0.711
    paper_std: 0.0054
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: narayanan2017graph2vec
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.711
    sort_std: 0.0054
    global_rank: 124
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
  - model: JOAOv2
    model_key: joaov2
    model_plain: JOAOv2
    value: 0.716
    std: 0.0086
    paper_value: 0.716
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
    source_ref: JOAO
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.707
    at_pub_std: 0.008
    at_pub_source_arxiv: '2202.13248'
    at_pub_source_title: Automated Data Augmentations for Graph Classification
    at_pub_source_date_iso: '2022-02-26'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-02-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.009000000000000008
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.707
    true_std: 0.008
    value_gap_source_arxiv: '2202.13248'
    value_gap_source_title: Automated Data Augmentations for Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.009000000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.707
    sort_std: 0.008
    global_rank: 134
    paper_rank: 116
    rank_delta: -18
    rank_delta_abs: 18
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AutoGCL
    model_key: autogcl
    model_plain: AutoGCL
    value: 0.733
    std: 0.004
    paper_value: 0.733
    paper_std: 0.004
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
    source_ref: autoGCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.707
    at_pub_std: 0.007
    at_pub_source_arxiv: '2202.13248'
    at_pub_source_title: Automated Data Augmentations for Graph Classification
    at_pub_source_date_iso: '2022-02-26'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-02-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.026000000000000023
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.707
    true_std: 0.007
    value_gap_source_arxiv: '2202.13248'
    value_gap_source_title: Automated Data Augmentations for Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.026000000000000023
    has_value_note: false
    value_note: ''
    sort_value: 0.707
    sort_std: 0.007
    global_rank: 135
    paper_rank: 74
    rank_delta: -61
    rank_delta_abs: 61
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Automated Data Augmentations for Graph Classification
    comparison_source_arxiv: '2202.13248'
    is_best: false
    is_std_outlier: false
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.6696
    std: 0.0056
    paper_value: 0.6696
    paper_std: 0.0056
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: datasets
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.67
    at_pub_std: 0.006
    at_pub_source_arxiv: '2006.05582'
    at_pub_source_title: Contrastive Multi-View Representation Learning on Graphs
    at_pub_source_date_iso: '2020-06-01'
    at_pub_source_date_label: ICML 2020
    value_gap_source_date_iso: '2018-05-21'
    value_gap_source_date_label: ICML 2018
    gap_vs_at_pub: 0.00040000000000006697
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6696
    true_std: 0.0056
    value_gap_source_arxiv: '1805.08090'
    value_gap_source_title: Graph Capsule Convolutional Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6696
    sort_std: 0.0056
    global_rank: 140
    paper_rank: 140
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GL
    model_key: gl
    model_plain: GL
    value: 0.6587
    std: 0.0098
    paper_value: 0.6587
    paper_std: 0.0098
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
    source_ref: gk
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.6587
    sort_std: 0.0098
    global_rank: 142
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
  - model: Sub2Vec
    model_key: sub2vec
    model_plain: Sub2Vec
    value: 0.5526
    std: 0.0154
    paper_value: 0.5526
    paper_std: 0.0154
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: adhikari2018sub2vec
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.5526
    sort_std: 0.0154
    global_rank: 151
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
  dataset: MUTAG
  rows:
  - model: ECC
    model_key: msh-gnn
    model_plain: ECC
    value: 0.991
    std: 0.003
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
    sort_value: 0.991
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: supcosine
    model_plain: ECC
    value: 0.983
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.07691'
    title: Supervised Contrastive Learning with Structure Inference for Graph Classification
    date: Mar 15, 2022
    date_display: Mar 2022
    date_iso: '2022-03-15'
    venue: IEEE Transactions on Network Science and Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: cauemo
    model_plain: ECC
    value: 0.9692
    std: 0.0136
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.06283'
    title: 'Soft causal learning for generalized molecule property prediction: An
      environment modeling perspective'
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9692
    sort_std: 0.0136
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMCL-D
    model_key: gmcl-d
    model_plain: GMCL-D
    value: 0.9409
    std: 0.0628
    paper_value: 0.9409
    paper_std: 0.0628
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.9409
    sort_std: 0.0628
    global_rank: 25
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
    is_best: true
    is_std_outlier: false
  - model: GMCL-P
    model_key: gmcl-p
    model_plain: GMCL-P
    value: 0.931
    std: 0.0533
    paper_value: 0.931
    paper_std: 0.0533
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.931
    sort_std: 0.0533
    global_rank: 37
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
  - model: GMCL-M
    model_key: gmcl-m
    model_plain: GMCL-M
    value: 0.931
    std: 0.063
    paper_value: 0.931
    paper_std: 0.063
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.931
    sort_std: 0.063
    global_rank: 37
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
    is_best: true
    is_std_outlier: false
  - model: Message perturb
    model_key: message perturb
    model_plain: Message perturb
    value: 0.931
    std: 0.0533
    paper_value: 0.931
    paper_std: 0.0533
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.931
    sort_std: 0.0533
    global_rank: 37
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
  - model: Message mixup
    model_key: message mixup
    model_plain: Message mixup
    value: 0.9254
    std: 0.0685
    paper_value: 0.9254
    paper_std: 0.0685
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.9254
    sort_std: 0.0685
    global_rank: 51
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
    is_best: true
    is_std_outlier: false
  - model: Message drop
    model_key: message drop
    model_plain: Message drop
    value: 0.9208
    std: 0.0484
    paper_value: 0.9208
    paper_std: 0.0484
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.9208
    sort_std: 0.0484
    global_rank: 63
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
  - model: Node drop
    model_key: node drop
    model_plain: Node drop
    value: 0.9149
    std: 0.0587
    paper_value: 0.9149
    paper_std: 0.0587
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.9149
    sort_std: 0.0587
    global_rank: 86
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
  - model: Edge drop
    model_key: edge drop
    model_plain: Edge drop
    value: 0.9146
    std: 0.0612
    paper_value: 0.9146
    paper_std: 0.0612
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.9146
    sort_std: 0.0612
    global_rank: 86
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
  - model: Node attribute drop
    model_key: node attribute drop
    model_plain: Node attribute drop
    value: 0.9146
    std: 0.0428
    paper_value: 0.9146
    paper_std: 0.0428
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.9146
    sort_std: 0.0428
    global_rank: 86
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
  - model: Node perturb
    model_key: node perturb
    model_plain: Node perturb
    value: 0.9096
    std: 0.0426
    paper_value: 0.9096
    paper_std: 0.0426
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.9096
    sort_std: 0.0426
    global_rank: 110
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
  - model: Node attribute perturb
    model_key: node attribute perturb
    model_plain: Node attribute perturb
    value: 0.9096
    std: 0.0337
    paper_value: 0.9096
    paper_std: 0.0337
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.9096
    sort_std: 0.0337
    global_rank: 110
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
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.8072
    std: 0.03
    paper_value: 0.8072
    paper_std: 0.03
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.904
    at_pub_std: 0.057
    at_pub_source_arxiv: '1912.06058'
    at_pub_source_title: Coloring graph neural networks for node disambiguation
    at_pub_source_date_iso: '2019-12-12'
    at_pub_source_date_label: IJCAI 2019
    value_gap_source_date_iso: '2022-05-26'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.0968
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.904
    true_std: 0.057
    value_gap_source_arxiv: '2205.13328'
    value_gap_source_title: How Powerful are $K$-hop Message Passing Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0968
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.057
    global_rank: 141
    paper_rank: 603
    rank_delta: 462
    rank_delta_abs: 462
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Coloring graph neural networks for node disambiguation
    comparison_source_arxiv: '1912.06058'
    is_best: false
    is_std_outlier: false
  - model: Edge perturb
    model_key: edge perturb
    model_plain: Edge perturb
    value: 0.9038
    std: 0.0528
    paper_value: 0.9038
    paper_std: 0.0528
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.9038
    sort_std: 0.0528
    global_rank: 155
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
  - model: subgraph
    model_key: subgraph
    model_plain: subgraph
    value: 0.9
    std: 0.0598
    paper_value: 0.9
    paper_std: 0.0598
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.9
    sort_std: 0.0598
    global_rank: 179
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
  - model: AD-GCL
    model_key: ad-gcl
    model_plain: AD-GCL
    value: 0.9028
    std: 0.0401
    paper_value: 0.9028
    paper_std: 0.0401
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2103.00111'
    at_pub_source_title: 'Graph Self-Supervised Learning: A Survey'
    at_pub_source_date_iso: '2021-02-27'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-02-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.005800000000000027
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.897
    true_std: null
    value_gap_source_arxiv: '2103.00111'
    value_gap_source_title: 'Graph Self-Supervised Learning: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.005800000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.897
    sort_std: null
    global_rank: 196
    paper_rank: 160
    rank_delta: -36
    rank_delta_abs: 36
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.8901
    std: 0.0113
    paper_value: 0.8901
    paper_std: 0.0113
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.893
    at_pub_std: 0.0514
    at_pub_source_arxiv: '2305.19903'
    at_pub_source_title: Improving Expressivity of GNNs with Subgraph-specific Factor
      Embedded Normalization
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.0029000000000000137
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.893
    true_std: 0.0514
    value_gap_source_arxiv: '2305.19903'
    value_gap_source_title: Improving Expressivity of GNNs with Subgraph-specific
      Factor Embedded Normalization
    value_gap_source_is_current_paper: false
    value_gap: 0.0029000000000000137
    has_value_note: false
    value_note: ''
    sort_value: 0.893
    sort_std: 0.0514
    global_rank: 236
    paper_rank: 251
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.9065
    std: 0.0081
    paper_value: 0.9065
    paper_std: 0.0081
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.89
    true_std: 0.011
    value_gap_source_arxiv: '2410.10241'
    value_gap_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    value_gap_source_is_current_paper: false
    value_gap: 0.01649999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.89
    sort_std: 0.011
    global_rank: 252
    paper_rank: 122
    rank_delta: -130
    rank_delta_abs: 130
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AutoGCL
    model_key: autogcl
    model_plain: AutoGCL
    value: 0.8864
    std: 0.0108
    paper_value: 0.8864
    paper_std: 0.0108
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8864
    at_pub_std: 0.0108
    at_pub_source_arxiv: '2305.17437'
    at_pub_source_title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-05-27'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8864
    true_std: 0.0108
    value_gap_source_arxiv: '2410.01778'
    value_gap_source_title: 'TopER: Topological Embeddings in Graph Representation
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8864
    sort_std: 0.0108
    global_rank: 281
    paper_rank: 281
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.868
    std: 0.0134
    paper_value: 0.868
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8829
    at_pub_std: 0.0131
    at_pub_source_arxiv: '2309.16014'
    at_pub_source_title: Graph-level Representation Learning with Joint-Embedding
      Predictive Architectures
    at_pub_source_date_iso: '2023-09-27'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2023-09-27'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.014900000000000024
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8829
    true_std: 0.0131
    value_gap_source_arxiv: '2309.16014'
    value_gap_source_title: Graph-level Representation Learning with Joint-Embedding
      Predictive Architectures
    value_gap_source_is_current_paper: false
    value_gap: 0.014900000000000024
    has_value_note: false
    value_note: ''
    sort_value: 0.8829
    sort_std: 0.0131
    global_rank: 301
    paper_rank: 377
    rank_delta: 76
    rank_delta_abs: 76
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAOv2
    model_key: joaov2
    model_plain: JOAOv2
    value: 0.8967
    std: 0.0524
    paper_value: 0.8967
    paper_std: 0.0524
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8767
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2106.07594'
    at_pub_source_title: Graph Contrastive Learning Automated
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2021-06-10'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8767
    true_std: 0.0079
    value_gap_source_arxiv: '2106.05819'
    value_gap_source_title: Adversarial Graph Augmentation to Improve Graph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.8767
    sort_std: 0.0079
    global_rank: 331
    paper_rank: 205
    rank_delta: -126
    rank_delta_abs: 126
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.8744
    std: 0.0272
    paper_value: 0.8744
    paper_std: 0.0272
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8744
    at_pub_std: 0.027
    at_pub_source_arxiv: '1905.11136'
    at_pub_source_title: Provably Powerful Graph Networks
    at_pub_source_date_iso: '2019-05-27'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8744
    true_std: 0.0272
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8744
    sort_std: 0.0272
    global_rank: 339
    paper_rank: 339
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: graph2vec
    model_key: graph2vec
    model_plain: graph2vec
    value: 0.8315
    std: 0.0925
    paper_value: 0.8315
    paper_std: 0.0925
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8644
    at_pub_std: 0.0125
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.03289999999999993
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8644
    true_std: 0.0125
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.03289999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.8644
    sort_std: 0.0125
    global_rank: 389
    paper_rank: 518
    rank_delta: 129
    rank_delta_abs: 129
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GL
    model_key: gl
    model_plain: GL
    value: 0.8166
    std: 0.0211
    paper_value: 0.8166
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.852
    at_pub_std: 0.009
    at_pub_source_arxiv: '1606.01141'
    at_pub_source_title: On Valid Optimal Assignment Kernels and Applications to Graph
      Classification
    at_pub_source_date_iso: '2016-06-03'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2016-06-03'
    value_gap_source_date_label: NeurIPS 2016
    gap_vs_at_pub: 0.03539999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.852
    true_std: 0.009
    value_gap_source_arxiv: '1606.01141'
    value_gap_source_title: On Valid Optimal Assignment Kernels and Applications to
      Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.03539999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.852
    sort_std: 0.009
    global_rank: 434
    paper_rank: 583
    rank_delta: 149
    rank_delta_abs: 149
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On Valid Optimal Assignment Kernels and Applications
      to Graph Classification
    comparison_source_arxiv: '1606.01141'
    is_best: false
    is_std_outlier: false
  - model: Sub2Vec
    model_key: sub2vec
    model_plain: Sub2Vec
    value: 0.6105
    std: 0.158
    paper_value: 0.6105
    paper_std: 0.158
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8447
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.23419999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8447
    true_std: 0.0037
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.23419999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8447
    sort_std: 0.0037
    global_rank: 466
    paper_rank: 789
    rank_delta: 323
    rank_delta_abs: 323
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Masked Autoencoders with Transformers
    comparison_source_arxiv: '2202.08391'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.8079
    std: 0.1051
    paper_value: 0.8079
    paper_std: 0.1051
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.8079
    sort_std: 0.1051
    global_rank: 604
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
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.7263
    std: 0.102
    paper_value: 0.7263
    paper_std: 0.102
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7263
    at_pub_std: 0.102
    at_pub_source_arxiv: '2106.07594'
    at_pub_source_title: Graph Contrastive Learning Automated
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2025-06-06'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7263
    true_std: 0.102
    value_gap_source_arxiv: '2506.06212'
    value_gap_source_title: Model-Driven Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7263
    sort_std: 0.102
    global_rank: 750
    paper_rank: 750
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: NCI1
  rows:
  - model: ECC
    model_key: wl-mlp
    model_plain: ECC
    value: 0.9954
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9954
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: gin
    model_plain: ECC
    value: 0.9934
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
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: GNNs ... use node features
    is_global_top: true
    global_rank: 2
    sort_value: 0.9934
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ECC
    model_key: gcn
    model_plain: ECC
    value: 0.9727
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
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: GNNs ... use node features
    is_global_top: true
    global_rank: 3
    sort_value: 0.9727
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.8001
    std: 0.005
    paper_value: 0.8001
    paper_std: 0.005
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
    table_ref: Table unsupervised
    source_ref: wlsubtree
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86
    at_pub_std: 0.018
    at_pub_source_arxiv: '2205.14368'
    at_pub_source_title: Going Deeper into Permutation-Sensitive Graph Neural Networks
    at_pub_source_date_iso: '2022-05-28'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.05989999999999995
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
    value_gap: 0.05989999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.86
    sort_std: 0.018
    global_rank: 10
    paper_rank: 226
    rank_delta: 216
    rank_delta_abs: 216
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Going Deeper into Permutation-Sensitive Graph Neural
      Networks
    comparison_source_arxiv: '2205.14368'
    is_best: false
    is_std_outlier: false
  - model: GMCL-D
    model_key: gmcl-d
    model_plain: GMCL-D
    value: 0.8299
    std: 0.0206
    paper_value: 0.8299
    paper_std: 0.0206
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
    table_ref: Table unsupervised
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.8299
    sort_std: 0.0206
    global_rank: 80
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
  - model: GMCL-M
    model_key: gmcl-m
    model_plain: GMCL-M
    value: 0.8275
    std: 0.017
    paper_value: 0.8275
    paper_std: 0.017
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
    table_ref: Table unsupervised
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.8275
    sort_std: 0.017
    global_rank: 92
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
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.7787
    std: 0.0041
    paper_value: 0.7787
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table unsupervised
    source_ref: graphcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.825
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.04630000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.825
    true_std: 0.0013
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.04630000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.825
    sort_std: 0.0013
    global_rank: 104
    paper_rank: 342
    rank_delta: 238
    rank_delta_abs: 238
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: AutoGCL
    model_key: autogcl
    model_plain: AutoGCL
    value: 0.82
    std: 0.0029
    paper_value: 0.82
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table unsupervised
    source_ref: autoGCL
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7375
    at_pub_std: 0.0225
    at_pub_source_arxiv: '2305.17437'
    at_pub_source_title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-05-27'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0824999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.82
    true_std: 0.0029
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.82
    sort_std: 0.0029
    global_rank: 133
    paper_rank: 133
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    comparison_source_arxiv: '2305.17437'
    is_best: false
    is_std_outlier: false
  - model: GMCL-P
    model_key: gmcl-p
    model_plain: GMCL-P
    value: 0.8199
    std: 0.0218
    paper_value: 0.8199
    paper_std: 0.0218
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
    table_ref: Table unsupervised
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.8199
    sort_std: 0.0218
    global_rank: 134
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
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.8031
    std: 0.0046
    paper_value: 0.8031
    paper_std: 0.0046
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table unsupervised
    source_ref: datasets
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8031
    at_pub_std: 0.0046
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8031
    true_std: 0.0046
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8031
    sort_std: 0.0046
    global_rank: 210
    paper_rank: 210
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
    value: 0.762
    std: 0.0106
    paper_value: 0.762
    paper_std: 0.0106
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
    table_ref: Table unsupervised
    source_ref: infograph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.775
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.013000000000000012
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.775
    true_std: 0.0074
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.013000000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.775
    sort_std: 0.0074
    global_rank: 358
    paper_rank: 406
    rank_delta: 48
    rank_delta_abs: 48
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.7616
    std: 0.0042
    paper_value: 0.7616
    paper_std: 0.0042
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
    table_ref: Table unsupervised
    source_ref: zhu2020deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.772
    true_std: 0.015
    value_gap_source_arxiv: '2410.10241'
    value_gap_source_title: Revisiting Graph Autoencoders as Implicit Contrastive
      Learners
    value_gap_source_is_current_paper: false
    value_gap: 0.010399999999999965
    has_value_note: false
    value_note: ''
    sort_value: 0.772
    sort_std: 0.015
    global_rank: 372
    paper_rank: 409
    rank_delta: 37
    rank_delta_abs: 37
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: graph2vec
    model_key: graph2vec
    model_plain: graph2vec
    value: 0.7322
    std: 0.0181
    paper_value: 0.7322
    paper_std: 0.0181
    metric: Accuracy
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
    table_ref: Table unsupervised
    source_ref: narayanan2017graph2vec
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.754
    at_pub_std: 0.012
    at_pub_source_arxiv: '2110.15438'
    at_pub_source_title: 'InfoGCL: Information-Aware Graph Contrastive Learning'
    at_pub_source_date_iso: '2021-10-28'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2022-06-26'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.02180000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7322
    true_std: 0.0181
    value_gap_source_arxiv: '2206.12933'
    value_gap_source_title: Wiener Graph Deconvolutional Network Improves Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7322
    sort_std: 0.0181
    global_rank: 469
    paper_rank: 469
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Sub2Vec
    model_key: sub2vec
    model_plain: Sub2Vec
    value: 0.5284
    std: 0.0147
    paper_value: 0.5284
    paper_std: 0.0147
    metric: Accuracy
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
    table_ref: Table unsupervised
    source_ref: adhikari2018sub2vec
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5976
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.06920000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5976
    true_std: 0.0035
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.06920000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.5976
    sort_std: 0.0035
    global_rank: 573
    paper_rank: 593
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Masked Autoencoders with Transformers
    comparison_source_arxiv: '2202.08391'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.5489
    std: 0.0161
    paper_value: 0.5489
    paper_std: 0.0161
    metric: Accuracy
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
    table_ref: Table unsupervised
    source_ref: grover2016node2vec
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.549
    at_pub_std: 0.016
    at_pub_source_arxiv: '2110.15438'
    at_pub_source_title: 'InfoGCL: Information-Aware Graph Contrastive Learning'
    at_pub_source_date_iso: '2021-10-28'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.549
    true_std: 0.016
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.549
    sort_std: 0.016
    global_rank: 589
    paper_rank: 589
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id005
  dataset: REDDIT-MULTI-5K
  rows:
  - model: Coarsened
    model_key: spegcl
    model_plain: Coarsened
    value: 0.5944
    std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2410.10365'
    title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning without Positive
      Samples'
    date: Oct 14, 2024
    date_display: Oct 2024
    date_iso: '2024-10-14'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.5944
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Coarsened
    model_key: gin
    model_plain: Coarsened
    value: 0.576
    std: 0.015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.16011'
    title: 'GPS: graph contrastive learning via multi-scale augmented views from adversarial
      pooling'
    date: Jan 29, 2024
    date_display: Jan 2024
    date_iso: '2024-01-29'
    venue: Science China Information Sciences
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.576
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Coarsened
    model_key: sum--mlp (gin-0)
    model_plain: Coarsened
    value: 0.575
    std: 0.015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '1810.00826'
    title: How Powerful are Graph Neural Networks?
    date: Oct 1, 2018
    date_display: Oct 2018
    date_iso: '2018-10-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/weihua916/powerful-gnns
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.575
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMCL-M
    model_key: gmcl-m
    model_plain: GMCL-M
    value: 0.5681
    std: 0.025
    paper_value: 0.5681
    paper_std: 0.025
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
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.5681
    sort_std: 0.025
    global_rank: 6
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
    is_best: true
    is_std_outlier: false
  - model: AutoGCL
    model_key: autogcl
    model_plain: AutoGCL
    value: 0.5675
    std: 0.0018
    paper_value: 0.5675
    paper_std: 0.0018
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
    source_ref: autoGCL
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4991
    at_pub_std: 0.027
    at_pub_source_arxiv: '2305.17437'
    at_pub_source_title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-05-27'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.06840000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5675
    true_std: 0.0018
    value_gap_source_arxiv: '2410.10365'
    value_gap_source_title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning
      without Positive Samples'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5675
    sort_std: 0.0018
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    comparison_source_arxiv: '2305.17437'
    is_best: false
    is_std_outlier: false
  - model: GMCL-D
    model_key: gmcl-d
    model_plain: GMCL-D
    value: 0.5663
    std: 0.0186
    paper_value: 0.5663
    paper_std: 0.0186
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
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.5663
    sort_std: 0.0186
    global_rank: 7
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
  - model: GMCL-P
    model_key: gmcl-p
    model_plain: GMCL-P
    value: 0.5635
    std: 0.0231
    paper_value: 0.5635
    paper_std: 0.0231
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
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.5635
    sort_std: 0.0231
    global_rank: 7
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
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.5599
    std: 0.0028
    paper_value: 0.5599
    paper_std: 0.0028
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
    source_ref: graphcl
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4809
    at_pub_std: 0.0174
    at_pub_source_arxiv: '2305.17437'
    at_pub_source_title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-05-27'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-01-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.07899999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.56
    true_std: 0.003
    value_gap_source_arxiv: '2401.16011'
    value_gap_source_title: 'GPS: graph contrastive learning via multi-scale augmented
      views from adversarial pooling'
    value_gap_source_is_current_paper: false
    value_gap: 0.00010000000000010001
    has_value_note: false
    value_note: ''
    sort_value: 0.56
    sort_std: 0.003
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    comparison_source_arxiv: '2305.17437'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.5571
    std: 0.0083
    paper_value: 0.5571
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
    source_ref: zhu2020deep
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.5571
    sort_std: 0.0083
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
  - model: AD-GCL
    model_key: ad-gcl
    model_plain: AD-GCL
    value: 0.5349
    std: 0.0028
    paper_value: 0.5349
    paper_std: 0.0028
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
    table_ref: Table 2
    source_ref: ADGCL
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5349
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2305.17437'
    at_pub_source_title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-05-27'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-01-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.549
    true_std: 0.004
    value_gap_source_arxiv: '2401.16011'
    value_gap_source_title: 'GPS: graph contrastive learning via multi-scale augmented
      views from adversarial pooling'
    value_gap_source_is_current_paper: false
    value_gap: 0.014100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.549
    sort_std: 0.004
    global_rank: 14
    paper_rank: 16
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Infomax
    model_key: infomax
    model_plain: Infomax
    value: 0.5361
    std: 0.0031
    paper_value: 0.5361
    paper_std: 0.0031
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
    table_ref: Table 2
    source_ref: DGI
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.5361
    sort_std: 0.0031
    global_rank: 16
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
  - model: InfoGraph
    model_key: infograph
    model_plain: InfoGraph
    value: 0.5346
    std: 0.0103
    paper_value: 0.5346
    paper_std: 0.0103
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
    source_ref: infograph
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-01-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.535
    true_std: 0.01
    value_gap_source_arxiv: '2401.16011'
    value_gap_source_title: 'GPS: graph contrastive learning via multi-scale augmented
      views from adversarial pooling'
    value_gap_source_is_current_paper: false
    value_gap: 0.00040000000000006697
    has_value_note: false
    value_note: ''
    sort_value: 0.535
    sort_std: 0.01
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: graph2vec
    model_key: graph2vec
    model_plain: graph2vec
    value: 0.4786
    std: 0.0026
    paper_value: 0.4786
    paper_std: 0.0026
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: narayanan2017graph2vec
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-01-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.479
    true_std: 0.003
    value_gap_source_arxiv: '2401.16011'
    value_gap_source_title: 'GPS: graph contrastive learning via multi-scale augmented
      views from adversarial pooling'
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.479
    sort_std: 0.003
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.4606
    std: 0.0021
    paper_value: 0.4606
    paper_std: 0.0021
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
    source_ref: wlsubtree
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-01-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.461
    true_std: 0.002
    value_gap_source_arxiv: '2401.16011'
    value_gap_source_title: 'GPS: graph contrastive learning via multi-scale augmented
      views from adversarial pooling'
    value_gap_source_is_current_paper: false
    value_gap: 0.00040000000000001146
    has_value_note: false
    value_note: ''
    sort_value: 0.461
    sort_std: 0.002
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAOv2
    model_key: joaov2
    model_plain: JOAOv2
    value: 0.5271
    std: 0.0028
    paper_value: 0.5271
    paper_std: 0.0028
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
    table_ref: Table 2
    source_ref: JOAO
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5271
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2305.17437'
    at_pub_source_title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-05-27'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.4557
    true_std: 0.0286
    value_gap_source_arxiv: '2410.10365'
    value_gap_source_title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning
      without Positive Samples'
    value_gap_source_is_current_paper: false
    value_gap: 0.07140000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.4557
    sort_std: 0.0286
    global_rank: 24
    paper_rank: 17
    rank_delta: -7
    rank_delta_abs: 7
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGK
    model_key: dgk
    model_plain: DGK
    value: 0.4127
    std: 0.0018
    paper_value: 0.4127
    paper_std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: datasets
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4127
    true_std: 0.0018
    value_gap_source_arxiv: '2410.10365'
    value_gap_source_title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning
      without Positive Samples'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4127
    sort_std: 0.0018
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GL
    model_key: gl
    model_plain: GL
    value: 0.4101
    std: 0.0017
    paper_value: 0.4101
    paper_std: 0.0017
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
    source_ref: gk
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-14'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4101
    true_std: 0.0017
    value_gap_source_arxiv: '2410.10365'
    value_gap_source_title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning
      without Positive Samples'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4101
    sort_std: 0.0017
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Sub2Vec
    model_key: sub2vec
    model_plain: Sub2Vec
    value: 0.3668
    std: 0.0042
    paper_value: 0.3668
    paper_std: 0.0042
    metric: Accuracy
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
    table_ref: Table 1
    source_ref: adhikari2018sub2vec
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-01-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.367
    true_std: 0.004
    value_gap_source_arxiv: '2401.16011'
    value_gap_source_title: 'GPS: graph contrastive learning via multi-scale augmented
      views from adversarial pooling'
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.367
    sort_std: 0.004
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.3295
    std: 0.1089
    paper_value: 0.3295
    paper_std: 0.1089
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
    table_ref: Table 2
    source_ref: GCA
    variant_inference_reason: 'dataset: fuzzy match to reddit-multi-5k (score=85)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 8, 2024
    date_display: Jan 2024
    date_iso: '2024-01-08'
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
    sort_value: 0.3295
    sort_std: 0.1089
    global_rank: 31
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
    is_std_outlier: true
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
  - *id003
  - *id004
  - *id005
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: NCI1
      dataset_slug: nci1
    - dataset: COLLAB
      dataset_slug: collab
    - dataset: IMDB-BINARY
      dataset_slug: imdb-binary
    - dataset: REDDIT-MULTI-5K
      dataset_slug: reddit-multi-5k
main_figure: /figures/2401.03638/main_figure.jpegoptim.jpg
---

