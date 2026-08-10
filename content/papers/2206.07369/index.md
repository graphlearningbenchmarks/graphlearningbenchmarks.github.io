---
title: 'DiffWire: Inductive Graph Rewiring via the Lovász Bound'
arxiv_id: '2206.07369'
source_url: ''
authors:
- name: Adrián Arnaiz-Rodríguez
  orcid: null
  s2_author_id: '2148391192'
  s2_url: null
- name: Ahmed Begga
  orcid: null
  s2_author_id: '2170361105'
  s2_url: null
- name: Francisco Escolano
  orcid: null
  s2_author_id: '1704343'
  s2_url: null
- name: Nuria Oliver
  orcid: null
  s2_author_id: '145709776'
  s2_url: null
published_date: Jun 15, 2022
published_date_iso: '2022-06-15'
published_venue: LoG 2022
published_conference: LoG 2022
published_conference_short: LoG
published_conference_slug: log
abstract: 'Graph Neural Networks (GNNs) have been shown to achieve competitive results
  to tackle graph-related tasks, such as node and graph classification, link prediction
  and node and graph clustering in a variety of domains. Most GNNs use a message passing
  framework and hence are called MPNNs. Despite their promising results, MPNNs have
  been reported to suffer from over-smoothing, over-squashing and under-reaching.
  Graph rewiring and graph pooling have been proposed in the literature as solutions
  to address these limitations. However, most state-of-the-art graph rewiring methods
  fail to preserve the global topology of the graph, are neither differentiable nor
  inductive, and require the tuning of hyper-parameters. In this paper, we propose
  DiffWire, a novel framework for graph rewiring in MPNNs that is principled, fully
  differentiable and parameter-free by leveraging the Lov\''asz bound. The proposed
  approach provides a unified theory for graph rewiring by proposing two new, complementary
  layers in MPNNs: CT-Layer, a layer that learns the commute times and uses them as
  a relevance function for edge re-weighting; and GAP-Layer, a layer to optimize the
  spectral gap, depending on the nature of the network and the task at hand. We empirically
  validate the value of each of these layers separately with benchmark datasets for
  graph classification. We also perform preliminary studies on the use of CT-Layer
  for homophilic and heterophilic node classification tasks. DiffWire brings together
  the learnability of commute times to related definitions of curvature, opening the
  door to creating more expressive MPNNs.'
codebase_url: https://github.com/AdrianArnaiz/DiffWire
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
    value: 0.826
    std: 0.022
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.11714'
    title: Scalable Expressiveness through Preprocessed Graph Perturbations
    date: Jun 17, 2024
    date_display: Jun 2024
    date_iso: '2024-06-17'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/Danial-sb/SE2P
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 23
    sort_value: 0.826
    sort_std: 0.022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MINCUTPOOL
    model_key: mincutpool
    model_plain: MINCUTPOOL
    value: 0.58
    std: 0.062
    paper_value: 0.58
    paper_std: 0.062
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
    date: Jun 15, 2022
    date_display: Jun 2022
    date_iso: '2022-06-15'
    published_venue: LoG 2022
    published_conference: LoG 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-08-21'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.809
    true_std: 0.003
    value_gap_source_arxiv: '2408.11370'
    value_gap_source_title: 'Graph Classification via Reference Distribution Learning:
      Theory and Practice'
    value_gap_source_is_current_paper: false
    value_gap: 0.2290000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.809
    sort_std: 0.003
    global_rank: 87
    paper_rank: 360
    rank_delta: 273
    rank_delta_abs: 273
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
    value: 0.792
    std: 0.024
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 157
    sort_value: 0.792
    sort_std: 0.024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SDRF
    model_key: sdrf
    model_plain: SDRF
    value: 0.566
    std: 0.1
    paper_value: 0.566
    paper_std: 0.1
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
    date: Jun 15, 2022
    date_display: Jun 2022
    date_iso: '2022-06-15'
    published_venue: LoG 2022
    published_conference: LoG 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-21'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7648
    true_std: 0.00388
    value_gap_source_arxiv: '2210.11790'
    value_gap_source_title: 'FoSR: First-order Spectral Rewiring for addressing Oversquashing
      in GNNs'
    value_gap_source_is_current_paper: false
    value_gap: 0.1988000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7648
    sort_std: 0.00388
    global_rank: 237
    paper_rank: 363
    rank_delta: 126
    rank_delta_abs: 126
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CT-Layer
    model_key: ct-layer
    model_plain: CT-Layer
    value: 0.6987
    std: 0.024
    paper_value: 0.6987
    paper_std: 0.024
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
    date: Jun 15, 2022
    date_display: Jun 2022
    date_iso: '2022-06-15'
    published_venue: LoG 2022
    published_conference: LoG 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-15'
    value_gap_source_date_label: LoG 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6987
    true_std: 0.024
    value_gap_source_arxiv: '2206.07369'
    value_gap_source_title: 'DiffWire: Inductive Graph Rewiring via the Lovász Bound'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6987
    sort_std: 0.024
    global_rank: 328
    paper_rank: 328
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAP-Layer(N)
    model_key: gap-layer(n)
    model_plain: GAP-Layer(N)
    value: 0.6589
    std: 0.049
    paper_value: 0.6589
    paper_std: 0.049
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
    date: Jun 15, 2022
    date_display: Jun 2022
    date_iso: '2022-06-15'
    published_venue: LoG 2022
    published_conference: LoG 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-15'
    value_gap_source_date_label: LoG 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6589
    true_std: 0.049
    value_gap_source_arxiv: '2206.07369'
    value_gap_source_title: 'DiffWire: Inductive Graph Rewiring via the Lovász Bound'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6589
    sort_std: 0.049
    global_rank: 342
    paper_rank: 342
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: K-NN
    model_key: k-nn
    model_plain: K-NN
    value: 0.5833
    std: 0.11
    paper_value: 0.5833
    paper_std: 0.11
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
    date: Jun 15, 2022
    date_display: Jun 2022
    date_iso: '2022-06-15'
    published_venue: LoG 2022
    published_conference: LoG 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-15'
    value_gap_source_date_label: LoG 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5833
    true_std: 0.11
    value_gap_source_arxiv: '2206.07369'
    value_gap_source_title: 'DiffWire: Inductive Graph Rewiring via the Lovász Bound'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5833
    sort_std: 0.11
    global_rank: 359
    paper_rank: 359
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DIGL
    model_key: digl
    model_plain: DIGL
    value: 0.5751
    std: 0.059
    paper_value: 0.5751
    paper_std: 0.059
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
    date: Jun 15, 2022
    date_display: Jun 2022
    date_iso: '2022-06-15'
    published_venue: LoG 2022
    published_conference: LoG 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-15'
    value_gap_source_date_label: LoG 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5751
    true_std: 0.059
    value_gap_source_arxiv: '2206.07369'
    value_gap_source_title: 'DiffWire: Inductive Graph Rewiring via the Lovász Bound'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5751
    sort_std: 0.059
    global_rank: 363
    paper_rank: 363
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
main_figure: /figures/2206.07369/main_figure.jpegoptim.jpg
---

