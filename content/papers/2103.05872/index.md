---
title: 'Sampling methods for efficient training of graph convolutional networks: A
  survey'
arxiv_id: '2103.05872'
source_url: ''
authors:
- name: Xin Liu
  orcid: null
  s2_author_id: '2146076015'
  s2_url: null
- name: Mingyu Yan
  orcid: null
  s2_author_id: '152206233'
  s2_url: null
- name: Lei Deng
  orcid: null
  s2_author_id: '143895326'
  s2_url: null
- name: Guoqi Li
  orcid: null
  s2_author_id: '1730243'
  s2_url: null
- name: Xiaochun Ye
  orcid: null
  s2_author_id: '144530359'
  s2_url: null
- name: Dongrui Fan
  orcid: null
  s2_author_id: '3276641'
  s2_url: null
published_date: Mar 10, 2021
published_date_iso: '2021-03-10'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Convolutional Networks (GCNs) have received significant attention
  from various research fields due to the excellent performance in learning graph
  representations. Although GCN performs well compared with other methods, it still
  faces challenges. Training a GCN model for large-scale graphs in a conventional
  way requires high computation and storage costs. Therefore, motivated by an urgent
  need in terms of efficiency and scalability in training GCN, sampling methods have
  been proposed and achieved a significant effect. In this paper, we categorize sampling
  methods based on the sampling mechanisms and provide a comprehensive survey of sampling
  methods for efficient training of GCN. To highlight the characteristics and differences
  of sampling methods, we present a detailed comparison within each category and further
  give an overall comparative analysis for the sampling methods in all categories.
  Finally, we discuss some challenges and future research directions of the sampling
  methods.
codebase_url: https://github.com/tkipf/gcn
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
  evaluated: 2
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
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
  - model: Cluster-GCN
    model_key: cluster-gcn
    model_plain: Cluster-GCN
    value: 0.875
    std: 0.004
    paper_value: 0.875
    paper_std: 0.004
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: chiang2019cluster
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing micro F1 score on PPI dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
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
    gap_vs_at_pub: 0.11860000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.119
    has_value_note: false
    value_note: ''
    sort_value: 0.994
    sort_std: null
    global_rank: 10
    paper_rank: 96
    rank_delta: 86
    rank_delta_abs: 86
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Comprehensive Survey on Graph Neural Networks
    comparison_source_arxiv: '1901.00596'
    is_best: true
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
  - model: GraphSAINT-EDGE
    model_key: graphsaint-edge
    model_plain: GraphSAINT-EDGE
    value: 0.981
    std: 0.007
    paper_value: 0.981
    paper_std: 0.007
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: graphsaint-iclr20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing micro F1 score on PPI dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.981
    at_pub_std: 0.007
    at_pub_source_arxiv: '1907.04931'
    at_pub_source_title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    at_pub_source_date_iso: '2019-07-10'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2021-03-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.981
    true_std: 0.007
    value_gap_source_arxiv: '2103.05872'
    value_gap_source_title: 'Sampling methods for efficient training of graph convolutional
      networks: A survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.981
    sort_std: 0.007
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAINT-RW
    model_key: graphsaint-rw
    model_plain: GraphSAINT-RW
    value: 0.981
    std: 0.004
    paper_value: 0.981
    paper_std: 0.004
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: graphsaint-iclr20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing micro F1 score on PPI dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.981
    at_pub_std: 0.004
    at_pub_source_arxiv: '1907.04931'
    at_pub_source_title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    at_pub_source_date_iso: '2019-07-10'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2021-03-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.981
    true_std: 0.004
    value_gap_source_arxiv: '2103.05872'
    value_gap_source_title: 'Sampling methods for efficient training of graph convolutional
      networks: A survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.981
    sort_std: 0.004
    global_rank: 31
    paper_rank: 31
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Parallelized Graph Sampling
    model_key: parallelized graph sampling
    model_plain: Parallelized Graph Sampling
    value: 0.696
    std: 0.004
    paper_value: 0.696
    paper_std: 0.004
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: zeng2019accurate
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing micro F1 score on PPI dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-03-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.696
    true_std: 0.004
    value_gap_source_arxiv: '2103.05872'
    value_gap_source_title: 'Sampling methods for efficient training of graph convolutional
      networks: A survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.696
    sort_std: 0.004
    global_rank: 136
    paper_rank: 136
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AS-GCN
    model_key: as-gcn
    model_plain: AS-GCN
    value: 0.599
    std: 0.004
    paper_value: 0.599
    paper_std: 0.004
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: huang2018adaptive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing Micro F1 score on PPI dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.687
    at_pub_std: 0.012
    at_pub_source_arxiv: '1907.04931'
    at_pub_source_title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    at_pub_source_date_iso: '2019-07-10'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2021-04-19'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.08800000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.687
    true_std: 0.012
    value_gap_source_arxiv: '2104.09376'
    value_gap_source_title: Scalable and Adaptive Graph Neural Networks with Self-Label-Enhanced
      Training
    value_gap_source_is_current_paper: false
    value_gap: 0.08800000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.687
    sort_std: 0.012
    global_rank: 142
    paper_rank: 168
    rank_delta: 26
    rank_delta_abs: 26
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    comparison_source_arxiv: '1907.04931'
    is_best: false
    is_std_outlier: false
  - model: FastGCN
    model_key: fastgcn
    model_plain: FastGCN
    value: 0.502
    std: 0.003
    paper_value: 0.502
    paper_std: 0.003
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: chen2018fastgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing Micro F1 score on PPI dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.637
    at_pub_std: 0.006
    at_pub_source_arxiv: '2009.10273'
    at_pub_source_title: Sub-graph Contrast for Scalable Self-Supervised Graph Representation
      Learning
    at_pub_source_date_iso: '2020-09-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-09-22'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.135
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.637
    true_std: 0.006
    value_gap_source_arxiv: '2009.10273'
    value_gap_source_title: Sub-graph Contrast for Scalable Self-Supervised Graph
      Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.135
    has_value_note: false
    value_note: ''
    sort_value: 0.637
    sort_std: 0.006
    global_rank: 157
    paper_rank: 177
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Sub-graph Contrast for Scalable Self-Supervised Graph
      Representation Learning
    comparison_source_arxiv: '2009.10273'
    is_best: false
    is_std_outlier: false
  - model: LADIES
    model_key: ladies
    model_plain: LADIES
    value: 0.574
    std: 0.003
    paper_value: 0.574
    paper_std: 0.003
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: zou2019layer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing Micro F1 score on PPI dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-03-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.574
    true_std: 0.003
    value_gap_source_arxiv: '2103.05872'
    value_gap_source_title: 'Sampling methods for efficient training of graph convolutional
      networks: A survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.574
    sort_std: 0.003
    global_rank: 172
    paper_rank: 172
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.462
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.00494'
    title: Graph Neural Networks Gone Hogwild
    date: Jun 29, 2024
    date_display: Jun 2024
    date_iso: '2024-06-29'
    venue: International Conference on Learning Representations
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 183
    sort_value: 0.462
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
- &id001
  dataset: Reddit
  rows:
  - model: Node Sampled Soup
    model_key: node sampled soup
    model_plain: Node Sampled Soup
    value: 0.9728
    std: 0.0008
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.10466'
    title: 'Graph Ladling: Shockingly Simple Parallel GNN Training without Intermediate
      Communication'
    date: Jun 18, 2023
    date_display: Jun 2023
    date_iso: '2023-06-18'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/VITA-Group/graph_ladling
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9728
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EnGCN
    model_key: engcn
    model_plain: EnGCN
    value: 0.9714
    std: 0.0003
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2210.07494'
    title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking and
      Rethinking'
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/VITA-Group/Large_Scale_GCN_Benchmarking
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9714
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGN+SLE
    model_key: sagn+sle
    model_plain: SAGN+SLE
    value: 0.971
    std: 0.0
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.07494'
    title: 'A Comprehensive Study on Large-Scale Graph Training: Benchmarking and
      Rethinking'
    date: Oct 14, 2022
    date_display: Oct 2022
    date_iso: '2022-10-14'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/VITA-Group/Large_Scale_GCN_Benchmarking
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.971
    sort_std: 0.0
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Cluster-GCN
    model_key: cluster-gcn
    model_plain: Cluster-GCN
    value: 0.954
    std: 0.001
    paper_value: 0.954
    paper_std: 0.001
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: chiang2019cluster
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing micro F1 score on Reddit dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.966
    at_pub_std: null
    at_pub_source_arxiv: '1905.07953'
    at_pub_source_title: 'Cluster-GCN: An Efficient Algorithm for Training Deep and
      Large Graph Convolutional Networks'
    at_pub_source_date_iso: '2019-05-20'
    at_pub_source_date_label: KDD 2019
    value_gap_source_date_iso: '2023-02-02'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.01200000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.966
    true_std: null
    value_gap_source_arxiv: '2302.00924'
    value_gap_source_title: 'LMC: Fast Training of GNNs via subgraph-wise sampling
      with Provable Convergence'
    value_gap_source_is_current_paper: false
    value_gap: 0.01200000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: null
    global_rank: 21
    paper_rank: 61
    rank_delta: 40
    rank_delta_abs: 40
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Cluster-GCN: An Efficient Algorithm for Training Deep
      and Large Graph Convolutional Networks'
    comparison_source_arxiv: '1905.07953'
    is_best: false
    is_std_outlier: false
  - model: GraphSAINT-EDGE
    model_key: graphsaint-edge
    model_plain: GraphSAINT-EDGE
    value: 0.966
    std: 0.001
    paper_value: 0.966
    paper_std: 0.001
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: graphsaint-iclr20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing micro F1 score on Reddit dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.966
    at_pub_std: 0.001
    at_pub_source_arxiv: '1907.04931'
    at_pub_source_title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    at_pub_source_date_iso: '2019-07-10'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2021-03-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.966
    true_std: 0.001
    value_gap_source_arxiv: '2103.05872'
    value_gap_source_title: 'Sampling methods for efficient training of graph convolutional
      networks: A survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: 0.001
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAINT-RW
    model_key: graphsaint-rw
    model_plain: GraphSAINT-RW
    value: 0.966
    std: 0.001
    paper_value: 0.966
    paper_std: 0.001
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: graphsaint-iclr20
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing micro F1 score on Reddit dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.966
    at_pub_std: 0.001
    at_pub_source_arxiv: '1907.04931'
    at_pub_source_title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    at_pub_source_date_iso: '2019-07-10'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2021-03-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.966
    true_std: 0.001
    value_gap_source_arxiv: '2103.05872'
    value_gap_source_title: 'Sampling methods for efficient training of graph convolutional
      networks: A survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: 0.001
    global_rank: 20
    paper_rank: 20
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
    value: 0.966
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
    arxiv_id: '2105.04528'
    title: Accelerating Large Scale Real-Time GNN Inference using Channel Pruning
    date: May 10, 2021
    date_display: May 2021
    date_iso: '2021-05-10'
    venue: Proceedings of the VLDB Endowment
    codebase_url: https://github.com/tedzhouhk/GCNP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 18
    sort_value: 0.966
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AS-GCN
    model_key: as-gcn
    model_plain: AS-GCN
    value: 0.89
    std: 0.013
    paper_value: 0.89
    paper_std: 0.013
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: huang2018adaptive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing Micro F1 score on Reddit dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.958
    at_pub_std: 0.001
    at_pub_source_arxiv: '1907.04931'
    at_pub_source_title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    at_pub_source_date_iso: '2019-07-10'
    at_pub_source_date_label: ICLR 2019
    value_gap_source_date_iso: '2022-11-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.06799999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.964
    true_std: 0.001
    value_gap_source_arxiv: '2211.11761'
    value_gap_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.07399999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.964
    sort_std: 0.001
    global_rank: 28
    paper_rank: 152
    rank_delta: 124
    rank_delta_abs: 124
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GraphSAINT: mpling Based ductive Learning Me hod'
    comparison_source_arxiv: '1907.04931'
    is_best: false
    is_std_outlier: false
  - model: Parallelized Graph Sampling
    model_key: parallelized graph sampling
    model_plain: Parallelized Graph Sampling
    value: 0.96
    std: 0.002
    paper_value: 0.96
    paper_std: 0.002
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: zeng2019accurate
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing micro F1 score on Reddit dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-03-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.96
    true_std: 0.002
    value_gap_source_arxiv: '2103.05872'
    value_gap_source_title: 'Sampling methods for efficient training of graph convolutional
      networks: A survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.96
    sort_std: 0.002
    global_rank: 48
    paper_rank: 48
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FastGCN
    model_key: fastgcn
    model_plain: FastGCN
    value: 0.825
    std: 0.006
    paper_value: 0.825
    paper_std: 0.006
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: chen2018fastgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing Micro F1 score on Reddit dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.937
    at_pub_std: null
    at_pub_source_arxiv: '1801.10247'
    at_pub_source_title: 'FastGCN: Fast Learning with Graph Convolutional Networks
      via Importance Sampling'
    at_pub_source_date_iso: '2018-01-30'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2023-02-02'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.1120000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.937
    true_std: null
    value_gap_source_arxiv: '2302.00924'
    value_gap_source_title: 'LMC: Fast Training of GNNs via subgraph-wise sampling
      with Provable Convergence'
    value_gap_source_is_current_paper: false
    value_gap: 0.1120000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.937
    sort_std: null
    global_rank: 112
    paper_rank: 155
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'FastGCN: Fast Learning with Graph Convolutional Networks
      via Importance Sampling'
    comparison_source_arxiv: '1801.10247'
    is_best: false
    is_std_outlier: false
  - model: LADIES
    model_key: ladies
    model_plain: LADIES
    value: 0.932
    std: 0.001
    paper_value: 0.932
    paper_std: 0.001
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: zou2019layer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Testing Micro F1 score on Reddit dataset
    date: Mar 10, 2021
    date_display: Mar 2021
    date_iso: '2021-03-10'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-03-10'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.932
    true_std: 0.001
    value_gap_source_arxiv: '2103.05872'
    value_gap_source_title: 'Sampling methods for efficient training of graph convolutional
      networks: A survey'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.932
    sort_std: 0.001
    global_rank: 126
    paper_rank: 126
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7216
    std: 0.0015
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2405.20445'
    title: Fully-inductive Node Classification on Arbitrary Graphs
    date: May 30, 2024
    date_display: May 2024
    date_iso: '2024-05-30'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/DeepGraphLearning/GraphAny
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 162
    sort_value: 0.7216
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Reddit
      dataset_slug: reddit
    - dataset: PPI
      dataset_slug: ppi
main_figure: /figures/2103.05872/main_figure.jpegoptim.jpg
---

