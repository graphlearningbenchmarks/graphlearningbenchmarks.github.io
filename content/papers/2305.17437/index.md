---
title: 'GIMM: InfoMin-Max for Automated Graph Contrastive Learning'
arxiv_id: '2305.17437'
source_url: ''
authors:
- name: Xin Xiong
  orcid: null
  s2_author_id: '2180558296'
  s2_url: null
- name: F. Shen
  orcid: null
  s2_author_id: '71883949'
  s2_url: null
- name: Xiangyu Wang
  orcid: null
  s2_author_id: '2202725612'
  s2_url: null
- name: Jian Zhao School of Artificial Intelligence
  orcid: null
  s2_author_id: '2219044941'
  s2_url: null
- name: Nanjing University
  orcid: null
  s2_author_id: '2220099454'
  s2_url: null
- name: School of Materials Science
  orcid: null
  s2_author_id: '102700312'
  s2_url: null
- name: Engineering
  orcid: null
  s2_author_id: '2285034464'
  s2_url: null
published_date: May 27, 2023
published_date_iso: '2023-05-27'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph contrastive learning (GCL) shows great potential in unsupervised
  graph representation learning. Data augmentation plays a vital role in GCL, and
  its optimal choice heavily depends on the downstream task. Many GCL methods with
  automated data augmentation face the risk of insufficient information as they fail
  to preserve the essential information necessary for the downstream task. To solve
  this problem, we propose nfo in- ax for automated raph contrastive learning (GIMM),
  which prevents GCL from encoding redundant information and losing essential information.
  GIMM consists of two major modules: (1) automated graph view generator, which acquires
  the approximation of InfoMin’s optimal views through adversarial training without
  requiring task-relevant information; (2) view comparison, which learns an excellent
  encoder by applying InfoMax to view representations. To the best of our knowledge,
  GIMM is the first method that combines the InfoMin and InfoMax principles in GCL.
  Besides, GIMM introduces randomness to augmentation, thus stabilizing the model
  against perturbations. Extensive experiments on unsupervised and semi-supervised
  learning for node and graph classification demonstrate the superiority of our GIMM
  over state-of-the-art GCL methods with automated and manual data augmentation.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GIMM
- GIMM-Fit
- GIMM-Un-Fit-A
- GIMM-Un-Fit
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
- TU Dortmund
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 4
  total: 11
task_categories:
- graph_classification
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id001
  dataset: Amazon-Photo
  rows:
  - model: C (orthogonal)
    model_key: msh-gnn
    model_plain: C (orthogonal)
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
  - model: C (orthogonal)
    model_key: geomancer
    model_plain: C (orthogonal)
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
  - model: C (orthogonal)
    model_key: graphtarif
    model_plain: C (orthogonal)
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
  - model: GIMM
    model_key: gimm
    model_plain: GIMM
    value: 0.9352
    std: 0.0033
    paper_value: 0.9352
    paper_std: 0.0033
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.9352
    sort_std: 0.0033
    global_rank: 165
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
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.9253
    std: 0.0016
    paper_value: 0.9253
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Zhu 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.932
    at_pub_std: 0.003
    at_pub_source_arxiv: '2210.08792'
    at_pub_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    at_pub_source_date_iso: '2022-10-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-03-03'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.006700000000000039
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.932
    true_std: 0.006
    value_gap_source_arxiv: '2403.01400'
    value_gap_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    value_gap_source_is_current_paper: false
    value_gap: 0.006700000000000039
    has_value_note: false
    value_note: ''
    sort_value: 0.932
    sort_std: 0.006
    global_rank: 196
    paper_rank: 275
    rank_delta: 79
    rank_delta_abs: 79
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    comparison_source_arxiv: '2210.08792'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.9174
    std: 0.0007
    paper_value: 0.9174
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Hassani 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9249
    at_pub_std: 0.004
    at_pub_source_arxiv: '2106.05470'
    at_pub_source_title: Automated Self-Supervised Learning for Graphs
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2024-03-03'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.007500000000000062
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.931
    true_std: 0.004
    value_gap_source_arxiv: '2403.01400'
    value_gap_source_title: Decoupling Weighing and Selecting for Integrating Multiple
      Graph Pre-training Tasks
    value_gap_source_is_current_paper: false
    value_gap: 0.013600000000000056
    has_value_note: false
    value_note: ''
    sort_value: 0.931
    sort_std: 0.004
    global_rank: 207
    paper_rank: 348
    rank_delta: 141
    rank_delta_abs: 141
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Automated Self-Supervised Learning for Graphs
    comparison_source_arxiv: '2106.05470'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.9161
    std: 0.0022
    paper_value: 0.9161
    paper_std: 0.0022
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
    source_ref: Velickovic 2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9161
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9309
    true_std: 0.0008
    value_gap_source_arxiv: '2407.19944'
    value_gap_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    value_gap_source_is_current_paper: false
    value_gap: 0.014799999999999924
    has_value_note: false
    value_note: ''
    sort_value: 0.9309
    sort_std: 0.0008
    global_rank: 211
    paper_rank: 353
    rank_delta: 142
    rank_delta_abs: 142
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AutoGCL
    model_key: autogcl
    model_plain: AutoGCL
    value: 0.9198
    std: 0.0058
    paper_value: 0.9198
    paper_std: 0.0058
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
    source_ref: Yin 2022
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9225
    true_std: 0.003
    value_gap_source_arxiv: '2410.15355'
    value_gap_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    value_gap_source_is_current_paper: false
    value_gap: 0.0027000000000000357
    has_value_note: false
    value_note: ''
    sort_value: 0.9225
    sort_std: 0.003
    global_rank: 312
    paper_rank: 332
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JOAO-v2
    model_key: joao-v2
    model_plain: JOAO-v2
    value: 0.9115
    std: 0.0055
    paper_value: 0.9115
    paper_std: 0.0055
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
    source_ref: Joao 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9139
    true_std: 0.0025
    value_gap_source_arxiv: '2410.15355'
    value_gap_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    value_gap_source_is_current_paper: false
    value_gap: 0.0024000000000000687
    has_value_note: false
    value_note: ''
    sort_value: 0.9139
    sort_std: 0.0025
    global_rank: 372
    paper_rank: 386
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.9068
    std: 0.0017
    paper_value: 0.9068
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Peng 2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9073
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2212.04604'
    at_pub_source_title: Localized Graph Contrastive Learning
    at_pub_source_date_iso: '2022-12-08'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-12-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0004999999999999449
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9081
    true_std: 0.0015
    value_gap_source_arxiv: '2512.24062'
    value_gap_source_title: Energy-Balanced Hyperspherical Graph Representation Learning
      via Structural Binding and Entropic Dispersion
    value_gap_source_is_current_paper: false
    value_gap: 0.0012999999999999678
    has_value_note: false
    value_note: ''
    sort_value: 0.9081
    sort_std: 0.0015
    global_rank: 394
    paper_rank: 400
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AD-GCL
    model_key: ad-gcl
    model_plain: AD-GCL
    value: 0.8875
    std: 0.0092
    paper_value: 0.8875
    paper_std: 0.0092
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
    source_ref: Suresh 2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.8875
    sort_std: 0.0092
    global_rank: 459
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id005
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
    table_ref: Table 1
    source_ref: you2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    table_ref: Table 1
    source_ref: you2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
  - model: GIMM-Un-Fit-A
    model_key: gimm-un-fit-a
    model_plain: GIMM-Un-Fit-A
    value: 0.785
    std: 0.0048
    paper_value: 0.785
    paper_std: 0.0048
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.785
    sort_std: 0.0048
    global_rank: 194
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
  - model: GIMM-Un-Fit
    model_key: gimm-un-fit
    model_plain: GIMM-Un-Fit
    value: 0.7721
    std: 0.0047
    paper_value: 0.7721
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.7721
    sort_std: 0.0047
    global_rank: 229
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
    table_ref: Table 1
    source_ref: suresh2021adversarial
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
  - model: GIMM-Fit
    model_key: gimm-fit
    model_plain: GIMM-Fit
    value: 0.7556
    std: 0.003
    paper_value: 0.7556
    paper_std: 0.003
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.7556
    sort_std: 0.003
    global_rank: 267
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
    table_ref: Table 1
    source_ref: yin2022autogcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.745
    at_pub_std: 0.002
    at_pub_source_arxiv: '2202.13248'
    at_pub_source_title: Automated Data Augmentations for Graph Classification
    at_pub_source_date_iso: '2022-02-26'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-02-26'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.026599999999999957
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
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
    comparison_type: improved
    comparison_source_title: Automated Data Augmentations for Graph Classification
    comparison_source_arxiv: '2202.13248'
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
    table_ref: Table 1
    source_ref: zhu2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
- &id002
  dataset: Coauthor-Physics
  rows:
  - model: SelfGNN LDP
    model_key: geomancer
    model_plain: SelfGNN LDP
    value: 0.9878
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
    global_rank: 1
    sort_value: 0.9878
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SelfGNN LDP
    model_key: lgd
    model_plain: SelfGNN LDP
    value: 0.9855
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    sort_value: 0.9855
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SelfGNN LDP
    model_key: msh-gnn
    model_plain: SelfGNN LDP
    value: 0.9837
    std: 0.0008
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
    global_rank: 3
    sort_value: 0.9837
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIMM
    model_key: gimm
    model_plain: GIMM
    value: 0.9591
    std: 0.001
    paper_value: 0.9591
    paper_std: 0.001
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.9591
    sort_std: 0.001
    global_rank: 83
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
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.9573
    std: 0.0003
    paper_value: 0.9573
    paper_std: 0.0003
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
    source_ref: zhu2021graph
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.959
    at_pub_std: 0.002
    at_pub_source_arxiv: '2210.08792'
    at_pub_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    at_pub_source_date_iso: '2022-10-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0016999999999999238
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.959
    true_std: 0.002
    value_gap_source_arxiv: '2210.08792'
    value_gap_source_title: Unifying Graph Contrastive Learning with Flexible Contextual
      Scopes
    value_gap_source_is_current_paper: false
    value_gap: 0.0016999999999999238
    has_value_note: false
    value_note: ''
    sort_value: 0.959
    sort_std: 0.002
    global_rank: 83
    paper_rank: 94
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.9533
    std: 0.0003
    paper_value: 0.9533
    paper_std: 0.0003
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
    source_ref: hassani2020contrastive
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9544
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2301.12063'
    at_pub_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    at_pub_source_date_iso: '2023-01-28'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-01-28'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0010999999999999899
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9544
    true_std: 0.0027
    value_gap_source_arxiv: '2301.12063'
    value_gap_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    value_gap_source_is_current_paper: false
    value_gap: 0.0010999999999999899
    has_value_note: false
    value_note: ''
    sort_value: 0.9544
    sort_std: 0.0027
    global_rank: 123
    paper_rank: 130
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.9451
    std: 0.0052
    paper_value: 0.9451
    paper_std: 0.0052
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
    source_ref: velickovic2019deep
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9457
    at_pub_std: 0.0038
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-04-16'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.0005999999999999339
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9489
    true_std: 0.0009
    value_gap_source_arxiv: '2504.12011'
    value_gap_source_title: Balancing Graph Embedding Smoothness in Self-Supervised
      Learning via Information-Theoretic Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.0037999999999999146
    has_value_note: false
    value_note: ''
    sort_value: 0.9489
    sort_std: 0.0009
    global_rank: 151
    paper_rank: 156
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AD-GCL
    model_key: ad-gcl
    model_plain: AD-GCL
    value: 0.9457
    std: 0.0009
    paper_value: 0.9457
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: suresh2021adversarial
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.9457
    sort_std: 0.0009
    global_rank: 156
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
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
  - model: GIMM
    model_key: gimm
    model_plain: GIMM
    value: 0.9157
    std: 0.0057
    paper_value: 0.9157
    paper_std: 0.0057
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.9157
    sort_std: 0.0057
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
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.906
    std: 0.0076
    paper_value: 0.906
    paper_std: 0.0076
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
    source_ref: zhu2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.906
    sort_std: 0.0076
    global_rank: 126
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.897
    std: 0.011
    paper_value: 0.897
    paper_std: 0.011
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
    source_ref: hassani2020contrastive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2103.00111'
    at_pub_source_title: 'Graph Self-Supervised Learning: A Survey'
    at_pub_source_date_iso: '2021-02-27'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8993
    true_std: 0.0616
    value_gap_source_arxiv: '2305.19903'
    value_gap_source_title: Improving Expressivity of GNNs with Subgraph-specific
      Factor Embedded Normalization
    value_gap_source_is_current_paper: false
    value_gap: 0.0022999999999999687
    has_value_note: false
    value_note: ''
    sort_value: 0.8993
    sort_std: 0.0616
    global_rank: 180
    paper_rank: 194
    rank_delta: 14
    rank_delta_abs: 14
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
    table_ref: Table 3
    source_ref: sun2019infograph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8901
    at_pub_std: 0.0113
    at_pub_source_arxiv: '2106.07594'
    at_pub_source_title: Graph Contrastive Learning Automated
    at_pub_source_date_iso: '2021-06-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: null
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
    table_ref: Table 3
    source_ref: yin2022autogcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.783
    at_pub_std: 0.022
    at_pub_source_arxiv: '2202.13248'
    at_pub_source_title: Automated Data Augmentations for Graph Classification
    at_pub_source_date_iso: '2022-02-26'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-10-02'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.10339999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
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
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Automated Data Augmentations for Graph Classification
    comparison_source_arxiv: '2202.13248'
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
    table_ref: Table 3
    source_ref: you2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8766
    at_pub_std: 0.0103
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-09-27'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.008600000000000052
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
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.7316
    std: 0.029
    paper_value: 0.7316
    paper_std: 0.029
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
    source_ref: you2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    gap_vs_at_pub: 0.09339999999999993
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
    value_gap: 0.09339999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.825
    sort_std: 0.0013
    global_rank: 104
    paper_rank: 470
    rank_delta: 366
    rank_delta_abs: 366
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
    value: 0.7375
    std: 0.0225
    paper_value: 0.7375
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yin2022autogcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.737
    at_pub_std: 0.002
    at_pub_source_arxiv: '2202.13248'
    at_pub_source_title: Automated Data Augmentations for Graph Classification
    at_pub_source_date_iso: '2022-02-26'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.000500000000000056
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.82
    true_std: 0.0029
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0824999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.82
    sort_std: 0.0029
    global_rank: 133
    paper_rank: 460
    rank_delta: 327
    rank_delta_abs: 327
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
    value: 0.7486
    std: 0.0039
    paper_value: 0.7486
    paper_std: 0.0039
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
    source_ref: you2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.817
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2205.09802'
    at_pub_source_title: Label-invariant Augmentation for Semi-Supervised Graph Classification
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.0683999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.817
    true_std: 0.0026
    value_gap_source_arxiv: '2205.09802'
    value_gap_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.0683999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.817
    sort_std: 0.0026
    global_rank: 144
    paper_rank: 439
    rank_delta: 295
    rank_delta_abs: 295
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Label-invariant Augmentation for Semi-Supervised Graph
      Classification
    comparison_source_arxiv: '2205.09802'
    is_best: false
    is_std_outlier: false
  - model: GIMM-Fit
    model_key: gimm-fit
    model_plain: GIMM-Fit
    value: 0.7643
    std: 0.005
    paper_value: 0.7643
    paper_std: 0.005
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.7643
    sort_std: 0.005
    global_rank: 396
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
  - model: GIMM-Un-Fit-A
    model_key: gimm-un-fit-a
    model_plain: GIMM-Un-Fit-A
    value: 0.7613
    std: 0.0059
    paper_value: 0.7613
    paper_std: 0.0059
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.7613
    sort_std: 0.0059
    global_rank: 410
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
    value: 0.7518
    std: 0.0031
    paper_value: 0.7518
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
    table_ref: Table 1
    source_ref: suresh2021adversarial
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7518
    at_pub_std: 0.0031
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
    true_value: 0.7518
    true_std: 0.0031
    value_gap_source_arxiv: '2209.06560'
    value_gap_source_title: Graph Contrastive Learning with Personalized Augmentation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7518
    sort_std: 0.0031
    global_rank: 431
    paper_rank: 431
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIMM-Un-Fit
    model_key: gimm-un-fit
    model_plain: GIMM-Un-Fit
    value: 0.7432
    std: 0.0019
    paper_value: 0.7432
    paper_std: 0.0019
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_std: 0.0019
    global_rank: 450
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
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.6873
    std: 0.0236
    paper_value: 0.6873
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: zhu2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.6873
    sort_std: 0.0236
    global_rank: 523
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
- &id006
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
  - model: AutoGCL
    model_key: autogcl
    model_plain: AutoGCL
    value: 0.4991
    std: 0.027
    paper_value: 0.4991
    paper_std: 0.027
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
    source_ref: yin2022autogcl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5675
    true_std: 0.0018
    value_gap_source_arxiv: '2410.10365'
    value_gap_source_title: 'SpeGCL: Self-supervised Graph Spectrum Contrastive Learning
      without Positive Samples'
    value_gap_source_is_current_paper: false
    value_gap: 0.06840000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.5675
    sort_std: 0.0018
    global_rank: 6
    paper_rank: 17
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCL
    model_key: graphcl
    model_plain: GraphCL
    value: 0.4809
    std: 0.0174
    paper_value: 0.4809
    paper_std: 0.0174
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
    source_ref: you2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.56
    true_std: 0.003
    value_gap_source_arxiv: '2401.16011'
    value_gap_source_title: 'GPS: graph contrastive learning via multi-scale augmented
      views from adversarial pooling'
    value_gap_source_is_current_paper: false
    value_gap: 0.07910000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.56
    sort_std: 0.003
    global_rank: 9
    paper_rank: 20
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
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
    table_ref: Table 1
    source_ref: suresh2021adversarial
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
  - model: GIMM-Un-Fit
    model_key: gimm-un-fit
    model_plain: GIMM-Un-Fit
    value: 0.5396
    std: 0.0051
    paper_value: 0.5396
    paper_std: 0.0051
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    sort_value: 0.5396
    sort_std: 0.0051
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
    table_ref: Table 1
    source_ref: you2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
    table_ref: Table 1
    source_ref: zhu2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 27, 2023
    date_display: May 2023
    date_iso: '2023-05-27'
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
- benchmark: Classic
  datasets:
  - *id001
  - *id002
- benchmark: TU Dortmund
  datasets:
  - *id003
  - *id004
  - *id005
  - *id006
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Coauthor-Physics
      dataset_slug: coauthor-physics
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
    - dataset: REDDIT-MULTI-5K
      dataset_slug: reddit-multi-5k
main_figure: /figures/2305.17437/main_figure.jpegoptim.jpg
---

