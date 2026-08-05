---
title: 'DeepGCNs: Making GCNs Go as Deep as CNNs'
arxiv_id: '1910.06849'
source_url: ''
authors:
- name: G. Li
  orcid: null
  s2_author_id: '49461641'
  s2_url: null
- name: Matthias Müller
  orcid: null
  s2_author_id: '1391027880'
  s2_url: null
- name: Guocheng Qian
  orcid: null
  s2_author_id: '113143344'
  s2_url: null
- name: Itzel C. Delgadillo
  orcid: null
  s2_author_id: '1379921764'
  s2_url: null
- name: Abdulellah Abualshour
  orcid: null
  s2_author_id: '1379921717'
  s2_url: null
- name: Ali K. Thabet
  orcid: null
  s2_author_id: '1872964'
  s2_url: null
- name: Bernard Ghanem
  orcid: null
  s2_author_id: '2931652'
  s2_url: null
published_date: Oct 15, 2019
published_date_iso: '2019-10-15'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Convolutional Neural Networks (CNNs) have been very successful at solving
  a variety of computer vision tasks such as object classification and detection,
  semantic segmentation, activity understanding, to name just a few. One key enabling
  factor for their great performance has been the ability to train very deep networks.
  Despite their huge success in many tasks, CNNs do not work well with non-Euclidean
  data, which is prevalent in many real-world applications. Graph Convolutional Networks
  (GCNs) offer an alternative that allows for non-Eucledian data input to a neural
  network. While GCNs already achieve encouraging results, they are currently limited
  to architectures with a relatively small number of layers, primarily due to vanishing
  gradients during training. This work transfers concepts such as residual/dense connections
  and dilated convolutions from CNNs to GCNs in order to successfully train very deep
  GCNs. We show the benefit of using deep GCNs (with as many as $112$ layers) experimentally
  across various datasets and tasks. We believe that the insights in this work will
  open avenues for future research on GCNs and their application to further tasks
  not explored in this paper. The source code for this work is available at https://github.com/lightaime/deep_gcns_torch
  and https://github.com/lightaime/deep_gcns for PyTorch and TensorFlow implementation
  respectively.
codebase_url: https://github.com/lightaime/deep_gcns_torch
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
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
  dataset: PPI
  rows:
  - model: GAMLP(JK)
    model_key: gamlp(jk)
    model_plain: GAMLP(JK)
    value: 0.9982
    std: 0.01
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2206.04355'
    title: Graph Attention Multi-Layer Perceptron
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/PKU-DAIR/GAMLP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9982
    sort_std: 0.01
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphCON-GCN
    model_key: graphcon-gcn
    model_plain: GraphCON-GCN
    value: 0.996
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_display: Feb 2022
    date_iso: '2022-02-04'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/tk-rusch/GraphCON
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.996
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.9956
    std: 0.02
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2007.02133'
    title: Simple and Deep Graph Convolutional Networks
    date: Jul 4, 2020
    date_display: Jul 2020
    date_iso: '2020-07-04'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/DropEdge/DropEdge
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9956
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DenseMRGCN-14
    model_key: densemrgcn-14
    model_plain: DenseMRGCN-14
    value: 0.9943
    std: null
    paper_value: 0.9943
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: m-F1 score for node classification on PPI
    date: Oct 15, 2019
    date_display: Oct 2019
    date_iso: '2019-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-10-15'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9943
    true_std: null
    value_gap_source_arxiv: '1910.06849'
    value_gap_source_title: 'DeepGCNs: Making GCNs Go as Deep as CNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9943
    sort_std: null
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
  - model: ResMRGCN-28
    model_key: resmrgcn-28
    model_plain: ResMRGCN-28
    value: 0.9941
    std: null
    paper_value: 0.9941
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: m-F1 score for node classification on PPI
    date: Oct 15, 2019
    date_display: Oct 2019
    date_iso: '2019-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-10-15'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9941
    true_std: null
    value_gap_source_arxiv: '1910.06849'
    value_gap_source_title: 'DeepGCNs: Making GCNs Go as Deep as CNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9941
    sort_std: null
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Cluster-GCN
    model_key: cluster-gcn
    model_plain: Cluster-GCN
    value: 0.9936
    std: null
    paper_value: 0.9936
    paper_std: null
    metric: F1
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
    source_ref: chiang2019cluster
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: m-F1 score for node classification on PPI
    date: Oct 15, 2019
    date_display: Oct 2019
    date_iso: '2019-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9936
    at_pub_std: null
    at_pub_source_arxiv: '1901.00596'
    at_pub_source_title: A Comprehensive Survey on Graph Neural Networks
    at_pub_source_date_iso: '2019-01-01'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2022-02-04'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.994
    true_std: null
    value_gap_source_arxiv: '2202.02296'
    value_gap_source_title: Graph-Coupled Oscillator Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.994
    sort_std: null
    global_rank: 10
    paper_rank: 11
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GaAN
    model_key: gaan
    model_plain: GaAN
    value: 0.9871
    std: null
    paper_value: 0.9871
    paper_std: null
    metric: F1
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
    source_ref: zhang2018gaan
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: m-F1 score for node classification on PPI
    date: Oct 15, 2019
    date_display: Oct 2019
    date_iso: '2019-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9871
    at_pub_std: 0.0002
    at_pub_source_arxiv: '1803.07294'
    at_pub_source_title: 'GaAN: Gated Attention Networks for Learning on Large and
      Spatiotemporal Graphs'
    at_pub_source_date_iso: '2018-03-20'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2026-03-17'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9871
    true_std: null
    value_gap_source_arxiv: '2603.16849'
    value_gap_source_title: 'GIST: Gauge-Invariant Spectral Transformers for Scalable
      Graph Neural Operators'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9871
    sort_std: null
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GeniePath
    model_key: geniepath
    model_plain: GeniePath
    value: 0.985
    std: null
    paper_value: 0.985
    paper_std: null
    metric: F1
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
    source_ref: liu2019geniepath
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: m-F1 score for node classification on PPI
    date: Oct 15, 2019
    date_display: Oct 2019
    date_iso: '2019-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.985
    at_pub_std: null
    at_pub_source_arxiv: '1905.07953'
    at_pub_source_title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and
      Large Graph Convolutional Networks'
    at_pub_source_date_iso: '2019-05-20'
    at_pub_source_date_label: KDD 2019
    value_gap_source_date_iso: '2022-02-04'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.985
    true_std: null
    value_gap_source_arxiv: '2202.02296'
    value_gap_source_title: Graph-Coupled Oscillator Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.985
    sort_std: null
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.985
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.02296'
    title: Graph-Coupled Oscillator Networks
    date: Feb 4, 2022
    date_display: Feb 2022
    date_iso: '2022-02-04'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/tk-rusch/GraphCON
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 21
    sort_value: 0.985
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VR-GCN
    model_key: vr-gcn
    model_plain: VR-GCN
    value: 0.978
    std: null
    paper_value: 0.978
    paper_std: null
    metric: F1
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
    source_ref: chen2017vrgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: m-F1 score for node classification on PPI
    date: Oct 15, 2019
    date_display: Oct 2019
    date_iso: '2019-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.978
    at_pub_std: null
    at_pub_source_arxiv: '1905.07953'
    at_pub_source_title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and
      Large Graph Convolutional Networks'
    at_pub_source_date_iso: '2019-05-20'
    at_pub_source_date_label: KDD 2019
    value_gap_source_date_iso: '2025-05-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.978
    true_std: null
    value_gap_source_arxiv: '2505.02020'
    value_gap_source_title: Wide & Deep Learning for Node Classification
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.978
    sort_std: null
    global_rank: 42
    paper_rank: 42
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATConv
    model_key: gatconv
    model_plain: GATConv
    value: 0.973
    std: null
    paper_value: 0.973
    paper_std: null
    metric: F1
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
    source_ref: velivckovic2017graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: m-F1 score for node classification on PPI
    date: Oct 15, 2019
    date_display: Oct 2019
    date_iso: '2019-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2019-10-15'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.973
    true_std: null
    value_gap_source_arxiv: '1910.06849'
    value_gap_source_title: 'DeepGCNs: Making GCNs Go as Deep as CNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.973
    sort_std: null
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.612
    std: null
    paper_value: 0.612
    paper_std: null
    metric: F1
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
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: m-F1 score for node classification on PPI
    date: Oct 15, 2019
    date_display: Oct 2019
    date_iso: '2019-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.637
    at_pub_std: 0.006
    at_pub_source_arxiv: '1907.04931'
    at_pub_source_title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    at_pub_source_date_iso: '2019-07-10'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2022-01-31'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: 0.025000000000000022
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.958
    true_std: 0.001
    value_gap_source_arxiv: '2201.13410'
    value_gap_source_title: 'Weisfeiler and Leman Go Infinite: Spectral and Combinatorial
      Pre-Colorings'
    value_gap_source_is_current_paper: false
    value_gap: 0.346
    has_value_note: false
    value_note: ''
    sort_value: 0.958
    sort_std: 0.001
    global_rank: 78
    paper_rank: 155
    rank_delta: 77
    rank_delta_abs: 77
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    comparison_source_arxiv: '1907.04931'
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
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
    - dataset: PPI
      dataset_slug: ppi
main_figure: /figures/1910.06849/main_figure.jpegoptim.jpg
---

