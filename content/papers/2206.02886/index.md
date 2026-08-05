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
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 2
  total: 16
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: Code
  rows:
  - model: two augmentation methods based on environment subgraphs
    model_key: two augmentation methods based on environment subgraphs
    model_plain: two augmentation methods based on environment subgraphs
    value: 0.8191
    std: 0.024
    paper_value: 0.8191
    paper_std: 0.024
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbg-code (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB-BACE classification task
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.8191
    true_std: 0.024
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8191
    sort_std: 0.024
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
  - model: OOD-GNN
    model_key: ood-gnn
    model_plain: OOD-GNN
    value: 0.8096
    std: 0.0132
    paper_value: 0.8096
    paper_std: 0.0132
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
    table_ref: Table 3
    source_ref: li2021ood
    variant_inference_reason: 'dataset: fuzzy match to ogbg-code (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB-BACE classification task
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.8096
    true_std: 0.0132
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8096
    sort_std: 0.0132
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: IRM
    model_key: irm
    model_plain: IRM
    value: 0.7947
    std: 0.0186
    paper_value: 0.7947
    paper_std: 0.0186
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
    table_ref: Table 3
    source_ref: arjovsky2019invariant
    variant_inference_reason: 'dataset: fuzzy match to ogbg-code (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB-BACE classification task
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7947
    true_std: 0.0186
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7947
    sort_std: 0.0186
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: U-NetsPool
    model_key: u-netspool
    model_plain: U-NetsPool
    value: 0.7757
    std: 0.0173
    paper_value: 0.7757
    paper_std: 0.0173
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
    table_ref: Table 3
    source_ref: gao2021graph
    variant_inference_reason: 'dataset: fuzzy match to ogbg-code (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB-BACE classification task
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7757
    true_std: 0.0173
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7757
    sort_std: 0.0173
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
  - model: DIR+RepAug
    model_key: dir+repaug
    model_plain: DIR+RepAug
    value: 0.7677
    std: 0.0226
    paper_value: 0.7677
    paper_std: 0.0226
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbg-code (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB-BACE classification task
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7677
    true_std: 0.0226
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7677
    sort_std: 0.0226
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
  - model: GREA-RepAug
    model_key: grea-repaug
    model_plain: GREA-RepAug
    value: 0.7655
    std: 0.0529
    paper_value: 0.7655
    paper_std: 0.0529
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbg-code (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB-BACE classification task
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7655
    true_std: 0.0529
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7655
    sort_std: 0.0529
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SelfAttnPool
    model_key: selfattnpool
    model_plain: SelfAttnPool
    value: 0.7383
    std: 0.0541
    paper_value: 0.7383
    paper_std: 0.0541
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
    table_ref: Table 3
    source_ref: lee2019self
    variant_inference_reason: 'dataset: fuzzy match to ogbg-code (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB-BACE classification task
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7383
    true_std: 0.0541
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7383
    sort_std: 0.0541
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DIR
    model_key: dir
    model_plain: DIR
    value: 0.6751
    std: 0.0323
    paper_value: 0.6751
    paper_std: 0.0323
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
    table_ref: Table 3
    source_ref: wu2022discovering
    variant_inference_reason: 'dataset: fuzzy match to ogbg-code (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB-BACE classification task
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.6751
    true_std: 0.0323
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6751
    sort_std: 0.0323
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
  - model: StableGNN
    model_key: stablegnn
    model_plain: StableGNN
    value: 0.6607
    std: 0.05
    paper_value: 0.6607
    paper_std: 0.05
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
    table_ref: Table 3
    source_ref: fan2021generalizing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-code (score=78)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB-BACE classification task
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.6607
    true_std: 0.05
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6607
    sort_std: 0.05
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
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: F1
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: ogbg-molhiv
  rows:
  - model: IRM
    model_key: irm
    model_plain: IRM
    value: 0.7817
    std: 0.012
    paper_value: 0.7817
    paper_std: 0.012
    metric: AUC
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
    source_ref: arjovsky2019invariant
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=84)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB benchmark task and split for molecule classification.
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7817
    true_std: 0.012
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7817
    sort_std: 0.012
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
  - model: OOD-GNN
    model_key: ood-gnn
    model_plain: OOD-GNN
    value: 0.7799
    std: 0.0078
    paper_value: 0.7799
    paper_std: 0.0078
    metric: AUC
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
    source_ref: li2021ood
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=84)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB benchmark task and split for molecule classification.
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7799
    true_std: 0.0078
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7799
    sort_std: 0.0078
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GREA
    model_key: grea
    model_plain: GREA
    value: 0.7794
    std: 0.0065
    paper_value: 0.7794
    paper_std: 0.0065
    metric: AUC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=84)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB benchmark task and split for molecule classification.
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7794
    true_std: 0.0065
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7794
    sort_std: 0.0065
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SelfAttnPool
    model_key: selfattnpool
    model_plain: SelfAttnPool
    value: 0.7733
    std: 0.0187
    paper_value: 0.7733
    paper_std: 0.0187
    metric: AUC
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
    source_ref: lee2019self
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=84)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB benchmark task and split for molecule classification.
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7733
    true_std: 0.0187
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7733
    sort_std: 0.0187
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DIR
    model_key: dir
    model_plain: DIR
    value: 0.7533
    std: 0.0117
    paper_value: 0.7533
    paper_std: 0.0117
    metric: AUC
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
    source_ref: wu2022discovering
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=84)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB benchmark task and split for molecule classification.
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7533
    true_std: 0.0117
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7533
    sort_std: 0.0117
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
  - model: U-NetsPool
    model_key: u-netspool
    model_plain: U-NetsPool
    value: 0.7527
    std: 0.0104
    paper_value: 0.7527
    paper_std: 0.0104
    metric: AUC
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
    source_ref: gao2021graph
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=84)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB benchmark task and split for molecule classification.
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7527
    true_std: 0.0104
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7527
    sort_std: 0.0104
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
  - model: DIR+RepAug
    model_key: dir+repaug
    model_plain: DIR+RepAug
    value: 0.7494
    std: 0.0225
    paper_value: 0.7494
    paper_std: 0.0225
    metric: AUC
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
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=84)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB benchmark task and split for molecule classification.
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7494
    true_std: 0.0225
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7494
    sort_std: 0.0225
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GREA-RepAug
    model_key: grea-repaug
    model_plain: GREA-RepAug
    value: 0.7377
    std: 0.021
    paper_value: 0.7377
    paper_std: 0.021
    metric: AUC
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=84)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB benchmark task and split for molecule classification.
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7377
    true_std: 0.021
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7377
    sort_std: 0.021
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
  - model: StableGNN
    model_key: stablegnn
    model_plain: StableGNN
    value: 0.7218
    std: 0.0099
    paper_value: 0.7218
    paper_std: 0.0099
    metric: AUC
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
    source_ref: fan2021generalizing
    variant_inference_reason: 'dataset: fuzzy match to ogbg-molhiv (score=84)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB benchmark task and split for molecule classification.
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    published_venue: KDD 2022
    published_conference: KDD 2022
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
    true_value: 0.7218
    true_std: 0.0099
    value_gap_source_arxiv: '2206.02886'
    value_gap_source_title: Graph Rationalization with Environment-based Augmentations
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7218
    sort_std: 0.0099
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
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - AUC
  metric: AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
    - dataset: Code
      dataset_slug: code
single_proposed_model: two augmentation methods based on environment subgraphs
main_figure: /figures/2206.02886/main_figure.jpegoptim.jpg
---

