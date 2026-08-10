---
title: Edge Contraction Pooling for Graph Neural Networks
arxiv_id: '1905.10990'
source_url: ''
authors:
- name: Frederik Diehl
  orcid: null
  s2_author_id: '3294622'
  s2_url: null
published_date: May 27, 2019
published_date_iso: '2019-05-27'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'research has concentrated on improving convolutional layers, with little
  attention paid to developing graph pooling layers. Yet pooling layers can enable
  to reason over abstracted groups of nodes instead of single nodes. To close this
  gap, we propose a graph pooling layer relying on the notion of edge contraction:
  EdgePool learns a localized and sparse hard pooling transform. We show that EdgePool
  outperforms alternative pooling methods, can be easily integrated into most models,
  and improves performance on both node and graph classification.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- EdgePool
mrr: 0.0064
adjusted_mrr: 0.0021
mrr_dataset_count: 1
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: COLLAB
  rows:
  - model: WL-MLP
    model_key: wl-mlp
    model_plain: WL-MLP
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
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
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
    input_feature_source: raw_features
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
  - model: CoCN
    model_key: cocn
    model_plain: CoCN
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.715
    std: 0.02
    paper_value: 0.715
    paper_std: 0.02
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: May 27, 2019
    date_display: May 2019
    date_iso: '2019-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.806
    at_pub_std: 0.021
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2024-06-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.09100000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.826
    true_std: 0.022
    value_gap_source_arxiv: '2406.11714'
    value_gap_source_title: Scalable Expressiveness through Preprocessed Graph Perturbations
    value_gap_source_is_current_paper: false
    value_gap: 0.11099999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.826
    sort_std: 0.022
    global_rank: 23
    paper_rank: 313
    rank_delta: 290
    rank_delta_abs: 290
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fast Graph Representation Learning with PyTorch Geometric
    comparison_source_arxiv: '1903.02428'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.742
    std: 0.018
    paper_value: 0.742
    paper_std: 0.018
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: May 27, 2019
    date_display: May 2019
    date_iso: '2019-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.822
    true_std: 0.021
    value_gap_source_arxiv: '2406.11714'
    value_gap_source_title: Scalable Expressiveness through Preprocessed Graph Perturbations
    value_gap_source_is_current_paper: false
    value_gap: 0.07999999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.021
    global_rank: 30
    paper_rank: 283
    rank_delta: 253
    rank_delta_abs: 253
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.701
    std: 0.015
    paper_value: 0.701
    paper_std: 0.015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: yingHierarchicalGraphRepresentation2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: May 27, 2019
    date_display: May 2019
    date_iso: '2019-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.789
    at_pub_std: 0.023
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2024-07-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.08800000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8213
    true_std: 0.0043
    value_gap_source_arxiv: '2407.18480'
    value_gap_source_title: Scalable Graph Compressed Convolutions
    value_gap_source_is_current_paper: false
    value_gap: 0.12030000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.8213
    sort_std: 0.0043
    global_rank: 34
    paper_rank: 325
    rank_delta: 291
    rank_delta_abs: 291
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fast Graph Representation Learning with PyTorch Geometric
    comparison_source_arxiv: '1903.02428'
    is_best: false
    is_std_outlier: false
  - model: SAGPool
    model_key: sagpool
    model_plain: SAGPool
    value: 0.639
    std: 0.025
    paper_value: 0.639
    paper_std: 0.025
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
    date: May 27, 2019
    date_display: May 2019
    date_iso: '2019-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8176
    true_std: 0.0157
    value_gap_source_arxiv: '2205.15068'
    value_gap_source_title: Embedding Graphs on Grassmann Manifold
    value_gap_source_is_current_paper: false
    value_gap: 0.17859999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.8176
    sort_std: 0.0157
    global_rank: 40
    paper_rank: 349
    rank_delta: 309
    rank_delta_abs: 309
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TopKPool
    model_key: topkpool
    model_plain: TopKPool
    value: 0.646
    std: 0.021
    paper_value: 0.646
    paper_std: 0.021
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
    date: May 27, 2019
    date_display: May 2019
    date_iso: '2019-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.814
    true_std: 0.0094
    value_gap_source_arxiv: '2205.15068'
    value_gap_source_title: Embedding Graphs on Grassmann Manifold
    value_gap_source_is_current_paper: false
    value_gap: 0.16799999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.814
    sort_std: 0.0094
    global_rank: 58
    paper_rank: 347
    rank_delta: 289
    rank_delta_abs: 289
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.643
    std: 0.019
    paper_value: 0.643
    paper_std: 0.019
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: May 27, 2019
    date_display: May 2019
    date_iso: '2019-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.797
    at_pub_std: 0.017
    at_pub_source_arxiv: '1903.02428'
    at_pub_source_title: Fast Graph Representation Learning with PyTorch Geometric
    at_pub_source_date_iso: '2019-03-06'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2019-03-06'
    value_gap_source_date_label: ICLR 2019
    gap_vs_at_pub: 0.15400000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.797
    true_std: 0.017
    value_gap_source_arxiv: '1903.02428'
    value_gap_source_title: Fast Graph Representation Learning with PyTorch Geometric
    value_gap_source_is_current_paper: false
    value_gap: 0.15400000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.797
    sort_std: 0.017
    global_rank: 143
    paper_rank: 347
    rank_delta: 204
    rank_delta_abs: 204
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fast Graph Representation Learning with PyTorch Geometric
    comparison_source_arxiv: '1903.02428'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.797
    std: 0.017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 142
    sort_value: 0.797
    sort_std: 0.017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePool
    model_key: edgepool
    model_plain: EdgePool
    value: 0.671
    std: 0.027
    paper_value: 0.671
    paper_std: 0.027
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: May 27, 2019
    date_display: May 2019
    date_iso: '2019-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.792
    true_std: 0.0166
    value_gap_source_arxiv: '2205.15068'
    value_gap_source_title: Embedding Graphs on Grassmann Manifold
    value_gap_source_is_current_paper: false
    value_gap: 0.121
    has_value_note: false
    value_note: ''
    sort_value: 0.792
    sort_std: 0.0166
    global_rank: 156
    paper_rank: 339
    rank_delta: 183
    rank_delta_abs: 183
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.678
    std: 0.032
    paper_value: 0.678
    paper_std: 0.032
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: May 27, 2019
    date_display: May 2019
    date_iso: '2019-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.792
    true_std: 0.024
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: false
    value_gap: 0.11399999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.792
    sort_std: 0.024
    global_rank: 157
    paper_rank: 336
    rank_delta: 179
    rank_delta_abs: 179
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN0
    model_key: gin0
    model_plain: GIN0
    value: 0.741
    std: 0.016
    paper_value: 0.741
    paper_std: 0.016
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: May 27, 2019
    date_display: May 2019
    date_iso: '2019-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-27'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.741
    true_std: 0.016
    value_gap_source_arxiv: '1905.10990'
    value_gap_source_title: Edge Contraction Pooling for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.741
    sort_std: 0.016
    global_rank: 285
    paper_rank: 285
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Base Model
    model_key: base model
    model_plain: Base Model
    value: 0.654
    std: 0.015
    paper_value: 0.654
    paper_std: 0.015
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
    date: May 27, 2019
    date_display: May 2019
    date_iso: '2019-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-27'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.654
    true_std: 0.015
    value_gap_source_arxiv: '1905.10990'
    value_gap_source_title: Edge Contraction Pooling for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.654
    sort_std: 0.015
    global_rank: 344
    paper_rank: 344
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE nacc
    model_key: sage nacc
    model_plain: SAGE nacc
    value: 0.641
    std: 0.021
    paper_value: 0.641
    paper_std: 0.021
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: May 27, 2019
    date_display: May 2019
    date_iso: '2019-05-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-05-27'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.641
    true_std: 0.021
    value_gap_source_arxiv: '1905.10990'
    value_gap_source_title: Edge Contraction Pooling for Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.641
    sort_std: 0.021
    global_rank: 349
    paper_rank: 349
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
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: COLLAB
      dataset_slug: collab
single_proposed_model: EdgePool
main_figure: /figures/1905.10990/main_figure.jpegoptim.jpg
---

