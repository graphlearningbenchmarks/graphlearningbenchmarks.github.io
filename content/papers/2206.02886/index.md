---
title: Graph Rationalization with Environment-based Augmentations
arxiv_id: '2206.02886'
source_url: ''
authors:
- name: Gang Liu
  orcid: null
  s2_author_id: '2146562364'
  s2_url: null
- name: Tong Zhao
  orcid: null
  s2_author_id: '1742573'
  s2_url: null
- name: Jiaxin Xu
  orcid: null
  s2_author_id: '2281299888'
  s2_url: null
- name: Tengfei Luo
  orcid: null
  s2_author_id: '2068287187'
  s2_url: null
- name: Meng Jiang
  orcid: null
  s2_author_id: '144812586'
  s2_url: null
published_date: Jun 6, 2022
published_date_iso: '2022-06-06'
published_venue: KDD 2022
published_conference: KDD 2022
published_conference_short: KDD
published_conference_slug: kdd
abstract: Rationale is defined as a subset of input features that best explains or
  supports the prediction by machine learning models. Rationale identification has
  improved the generalizability and interpretability of neural networks on vision
  and language data. In graph applications such as molecule and polymer property prediction,
  identifying representative subgraph structures named as graph rationales plays an
  essential role in the performance of graph neural networks. Existing graph pooling
  and/or distribution intervention methods suffer from the lack of examples to learn
  to identify optimal graph rationales. In this work, we introduce a new augmentation
  operation called environment replacement that automatically creates virtual data
  examples to improve rationale identification. We propose an efficient framework
  that performs rationale-environment separation and representation learning on the
  real and augmented examples in latent spaces to avoid the high complexity of explicit
  graph decoding and encoding. Comparing against recent techniques, experiments on
  seven molecular and four polymer datasets demonstrate the effectiveness and efficiency
  of the proposed augmentation-based graph rationalization framework. Data and the
  implementation of the proposed framework are publicly available.
codebase_url: https://github.com/liugangcode/GREA
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- two augmentation methods based on environment subgraphs
mrr: 0.1667
adjusted_mrr: 0.0556
mrr_dataset_count: 1
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ogbg-molhiv
  is_multi_metric: true
  rows:
  - model: Multi-RF Fusion with Multi-GNN Blending
    model_key: multi-rf fusion with multi-gnn blending
    model_plain: Multi-RF Fusion with Multi-GNN Blending
    metric_values:
    - 0.8476
    - null
    metric_stds:
    - 0.0002
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    published_venue: ''
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.8476
    sort_std: 0.0002
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: HyperFusion
    model_key: hyperfusion
    model_plain: HyperFusion
    metric_values:
    - 0.8475
    - null
    metric_stds:
    - 0.0003
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    published_venue: ''
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.8475
    sort_std: 0.0003
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: PAS+FPs
    model_key: pas+fps
    model_plain: PAS+FPs
    metric_values:
    - 0.842
    - null
    metric_stds:
    - 0.0015
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2603.20724'
    title: Multi-RF Fusion with Multi-GNN Blending for Molecular Property Prediction
    published_venue: ''
    date: Mar 21, 2026
    date_display: Mar 2026
    date_iso: '2026-03-21'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.842
    sort_std: 0.0015
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: two augmentation methods based on environment subgraphs
    model_key: two augmentation methods based on environment subgraphs
    model_plain: two augmentation methods based on environment subgraphs
    metric_values:
    - 0.8191
    - null
    metric_stds:
    - 0.024
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.8191
    sort_std: 0.024
    true_value: 0.8191
    true_std: 0.024
    paper_value: 0.8191
    paper_std: 0.024
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: KDD 2022
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: OOD-GNN
    model_key: ood-gnn
    model_plain: OOD-GNN
    metric_values:
    - 0.8096
    - 0.7799
    metric_stds:
    - 0.0132
    - 0.0078
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8096
    sort_std: 0.0132
    true_value: 0.8096
    true_std: 0.0132
    paper_value: 0.8096
    paper_std: 0.0132
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: KDD 2022
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    metric_values:
    - 0.809
    - null
    metric_stds:
    - 0.016
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 2.8
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.10131'
    title: Deep Prompt Tuning for Graph Transformers
    published_venue: ''
    date: Sep 18, 2023
    date_display: Sep 2023
    date_iso: '2023-09-18'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 12
    is_best: false
    sort_value: 0.809
    sort_std: 0.016
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: IRM
    model_key: irm
    model_plain: IRM
    metric_values:
    - 0.7947
    - 0.7817
    metric_stds:
    - 0.0186
    - 0.012
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7947
    sort_std: 0.0186
    true_value: 0.7947
    true_std: 0.0186
    paper_value: 0.7947
    paper_std: 0.0186
    has_value_gap: true
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_note: ''
    at_pub_value: 0.7446
    at_pub_std: 0.0274
    at_pub_source_arxiv: '2201.12872'
    at_pub_source_title: Discovering Invariant Rationales for Graph Neural Networks
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.05009999999999992
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: KDD 2022
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 50
  - model: GREA
    model_key: grea
    model_plain: GREA
    metric_values:
    - null
    - 0.7794
    metric_stds:
    - null
    - 0.0065
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7794
    sort_std: 0.0065
    true_value: 0.7794
    true_std: 0.0065
    paper_value: 0.7794
    paper_std: 0.0065
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: KDD 2022
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 115
  - model: GIN
    model_key: gin
    model_plain: GIN
    metric_values:
    - 0.778
    - null
    metric_stds:
    - 0.0182
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 510.0
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    published_venue: ''
    date: Jan 30, 2022
    date_display: Jan 2022
    date_iso: '2022-01-30'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 120
    is_best: false
    sort_value: 0.778
    sort_std: 0.0182
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: U-NetsPool
    model_key: u-netspool
    model_plain: U-NetsPool
    metric_values:
    - 0.7757
    - 0.7527
    metric_stds:
    - 0.0173
    - 0.0104
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7757
    sort_std: 0.0173
    true_value: 0.7757
    true_std: 0.0173
    paper_value: 0.7757
    paper_std: 0.0173
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: KDD 2022
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 128
  - model: DIR
    model_key: dir
    model_plain: DIR
    metric_values:
    - 0.6751
    - 0.7533
    metric_stds:
    - 0.0323
    - 0.0117
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7705
    sort_std: null
    true_value: 0.7705
    true_std: null
    paper_value: 0.6751
    paper_std: 0.0323
    has_value_gap: true
    has_value_note: false
    value_gap: 0.09539999999999993
    value_gap_source_arxiv: '2502.07968'
    value_gap_source_title: Generative Risk Minimization for Out-of-Distribution Generalization
      on Graphs
    value_note: ''
    at_pub_value: 0.7705
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2201.12872'
    at_pub_source_title: Discovering Invariant Rationales for Graph Neural Networks
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2025-02-11'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.09539999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: KDD 2022
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 165
  - model: DIR+RepAug
    model_key: dir+repaug
    model_plain: DIR+RepAug
    metric_values:
    - 0.7677
    - 0.7494
    metric_stds:
    - 0.0226
    - 0.0225
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7677
    sort_std: 0.0226
    true_value: 0.7677
    true_std: 0.0226
    paper_value: 0.7677
    paper_std: 0.0226
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: KDD 2022
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 181
  - model: GREA-RepAug
    model_key: grea-repaug
    model_plain: GREA-RepAug
    metric_values:
    - 0.7655
    - 0.7377
    metric_stds:
    - 0.0529
    - 0.021
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.7655
    sort_std: 0.0529
    true_value: 0.7655
    true_std: 0.0529
    paper_value: 0.7655
    paper_std: 0.0529
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: KDD 2022
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 191
  - model: SelfAttnPool
    model_key: selfattnpool
    model_plain: SelfAttnPool
    metric_values:
    - 0.7383
    - 0.7733
    metric_stds:
    - 0.0541
    - 0.0187
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7383
    sort_std: 0.0541
    true_value: 0.7383
    true_std: 0.0541
    paper_value: 0.7383
    paper_std: 0.0541
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: KDD 2022
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 279
  - model: StableGNN
    model_key: stablegnn
    model_plain: StableGNN
    metric_values:
    - 0.6607
    - 0.7218
    metric_stds:
    - 0.05
    - 0.0099
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6607
    sort_std: 0.05
    true_value: 0.6607
    true_std: 0.05
    paper_value: 0.6607
    paper_std: 0.05
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: KDD 2022
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 320
  metrics:
  - ROC-AUC
  - AUC
  primary_metric: ROC-AUC
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  - AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
single_proposed_model: two augmentation methods based on environment subgraphs
main_figure: /figures/2206.02886/main_figure.jpegoptim.jpg
---

