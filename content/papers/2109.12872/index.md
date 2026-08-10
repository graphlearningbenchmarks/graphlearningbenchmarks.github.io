---
title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph Neural Networks'
arxiv_id: '2109.12872'
source_url: ''
authors:
- name: Yongcheng Jing
  orcid: null
  s2_author_id: '9633703'
  s2_url: null
- name: Yiding Yang
  orcid: null
  s2_author_id: '3148439'
  s2_url: null
- name: Xinchao Wang
  orcid: null
  s2_author_id: '48631088'
  s2_url: null
- name: Mingli Song
  orcid: null
  s2_author_id: '144646841'
  s2_url: null
- name: D. Tao
  orcid: null
  s2_author_id: '143719920'
  s2_url: null
published_date: Sep 27, 2021
published_date_iso: '2021-09-27'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: In this paper, we study a novel meta aggregation scheme towards binarizing
  graph neural networks (GNNs). We begin by developing a vanilla 1-bit GNN framework
  that binarizes both the GNN parameters and the graph features. Despite the lightweight
  architecture, we observed that this vanilla framework suffered from insufficient
  discriminative power in distinguishing graph topologies, leading to a dramatic drop
  in performance. This discovery motivates us to devise meta aggregators to improve
  the expressive power of vanilla binarized GNNs, of which the aggregation schemes
  can be adaptively changed in a learnable manner based on the binarized features.
  Towards this end, we propose two dedicated forms of meta neighborhood aggregators,
  an exclusive meta aggregator termed as Greedy Gumbel Neighborhood Aggregator (GNA),
  and a diffused meta aggregator termed as Adaptable Hybrid Neighborhood Aggregator
  (ANA). GNA learns to exclusively pick one single optimal aggregator from a pool
  of candidates, while ANA learns a hybrid aggregation behavior to simultaneously
  retain the benefits of several individual aggregators. Furthermore, the proposed
  meta aggregators may readily serve as a generic plugin module into existing full-precision
  GNNs. Experiments across various domains demonstrate that the proposed method yields
  results superior to the state of the art.
codebase_url: ''
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
- graph_regression
- node_classification
experiment_scopes:
- graph-level
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
  - model: Full Prec.
    model_key: full prec.
    model_plain: Full Prec.
    value: 0.987
    std: null
    paper_value: 0.987
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
    source_ref: velivckovic2018graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: micro-averaged F1 score on PPI node classification task
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-09-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.987
    true_std: null
    value_gap_source_arxiv: '2109.12872'
    value_gap_source_title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.987
    sort_std: null
    global_rank: 18
    paper_rank: 18
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
  - model: ANA
    model_key: ana
    model_plain: ANA
    value: 0.9771
    std: null
    paper_value: 0.9771
    paper_std: null
    metric: F1
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: micro-averaged F1 score on PPI node classification task
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-09-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9771
    true_std: null
    value_gap_source_arxiv: '2109.12872'
    value_gap_source_title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9771
    sort_std: null
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNA
    model_key: gna
    model_plain: GNA
    value: 0.9752
    std: null
    paper_value: 0.9752
    paper_std: null
    metric: F1
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: micro-averaged F1 score on PPI node classification task
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-09-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9752
    true_std: null
    value_gap_source_arxiv: '2109.12872'
    value_gap_source_title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9752
    sort_std: null
    global_rank: 53
    paper_rank: 53
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Vanilla
    model_key: vanilla
    model_plain: Vanilla
    value: 0.9268
    std: null
    paper_value: 0.9268
    paper_std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: hubara2016binarized
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: micro-averaged F1 score on PPI node classification task
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-09-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9268
    true_std: null
    value_gap_source_arxiv: '2109.12872'
    value_gap_source_title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9268
    sort_std: null
    global_rank: 90
    paper_rank: 90
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
- &id002
  dataset: ZINC
  rows:
  - model: TIGT
    model_key: tigt
    model_plain: TIGT
    value: 0.014
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: Feb 3, 2024
    date_display: Feb 2024
    date_iso: '2024-02-03'
    venue: GRaM
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.014
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FloydNet
    model_key: floydnet
    model_plain: FloydNet
    value: 0.016
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_display: Jan 2026
    date_iso: '2026-01-27'
    venue: arXiv.org
    codebase_url: https://github.com/ocx-lab/FloydNet
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.016
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PST
    model_key: pst
    model_plain: PST
    value: 0.018
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2405.02795'
    title: Graph as Point Set
    date: May 5, 2024
    date_display: May 2024
    date_iso: '2024-05-05'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.018
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.387
    std: 0.019
    paper_value: 0.387
    paper_std: 0.019
    metric: MAE
    higher_is_better: false
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
    source_ref: xu2018powerful
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for ZINC regression
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.088
    at_pub_std: 0.002
    at_pub_source_arxiv: '2106.12575'
    at_pub_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    at_pub_source_date_iso: '2021-06-23'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.29900000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.088
    true_std: 0.002
    value_gap_source_arxiv: '2502.02479'
    value_gap_source_title: Using Random Noise Equivariantly to Boost Graph Neural
      Networks Universally
    value_gap_source_is_current_paper: false
    value_gap: 0.29900000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.088
    sort_std: 0.002
    global_rank: 71
    paper_rank: 102
    rank_delta: 31
    rank_delta_abs: 31
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Weisfeiler and Lehman Go Cellular: CW Networks'
    comparison_source_arxiv: '2106.12575'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.476
    std: 0.006
    paper_value: 0.476
    paper_std: 0.006
    metric: MAE
    higher_is_better: false
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
    source_ref: velivckovic2018graph
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for ZINC regression
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.111
    true_std: 0.002
    value_gap_source_arxiv: '2406.05815'
    value_gap_source_title: What Can We Learn from State Space Models for Machine
      Learning on Graphs?
    value_gap_source_is_current_paper: false
    value_gap: 0.365
    has_value_note: false
    value_note: ''
    sort_value: 0.111
    sort_std: 0.002
    global_rank: 79
    paper_rank: 104
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.407
    std: 0.018
    paper_value: 0.407
    paper_std: 0.018
    metric: MAE
    higher_is_better: false
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
    source_ref: kipf2017semi
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for ZINC regression
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.113
    true_std: 0.002
    value_gap_source_arxiv: '2406.05815'
    value_gap_source_title: What Can We Learn from State Space Models for Machine
      Learning on Graphs?
    value_gap_source_is_current_paper: false
    value_gap: 0.294
    has_value_note: false
    value_note: ''
    sort_value: 0.113
    sort_std: 0.002
    global_rank: 80
    paper_rank: 102
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.475
    std: 0.007
    paper_value: 0.475
    paper_std: 0.007
    metric: MAE
    higher_is_better: false
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
    source_ref: hamilton2017inductive
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for ZINC regression
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-31'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.126
    true_std: 0.003
    value_gap_source_arxiv: '2310.20519'
    value_gap_source_title: Enhancing Graph Neural Networks with Quantum Computed
      Encodings
    value_gap_source_is_current_paper: false
    value_gap: 0.349
    has_value_note: false
    value_note: ''
    sort_value: 0.126
    sort_std: 0.003
    global_rank: 81
    paper_rank: 104
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.426
    std: 0.012
    paper_value: 0.426
    paper_std: 0.012
    metric: MAE
    higher_is_better: false
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
    source_ref: bresson2017residual
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for ZINC regression
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.282
    true_std: 0.015
    value_gap_source_arxiv: '2402.02005'
    value_gap_source_title: Topology-Informed Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: 0.14400000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.282
    sort_std: 0.015
    global_rank: 98
    paper_rank: 104
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ANA
    model_key: ana
    model_plain: ANA
    value: 0.325
    std: 0.015
    paper_value: 0.325
    paper_std: 0.015
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for ZINC regression
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-09-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.325
    true_std: 0.015
    value_gap_source_arxiv: '2109.12872'
    value_gap_source_title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.325
    sort_std: 0.015
    global_rank: 100
    paper_rank: 100
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNA
    model_key: gna
    model_plain: GNA
    value: 0.337
    std: 0.021
    paper_value: 0.337
    paper_std: 0.021
    metric: MAE
    higher_is_better: false
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
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for ZINC regression
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-09-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.337
    true_std: 0.021
    value_gap_source_arxiv: '2109.12872'
    value_gap_source_title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.337
    sort_std: 0.021
    global_rank: 101
    paper_rank: 101
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MoNet
    model_key: monet
    model_plain: MoNet
    value: 0.386
    std: 0.009
    paper_value: 0.386
    paper_std: 0.009
    metric: MAE
    higher_is_better: false
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
    source_ref: monti2017geometric
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for ZINC regression
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-09-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.386
    true_std: 0.009
    value_gap_source_arxiv: '2109.12872'
    value_gap_source_title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.386
    sort_std: 0.009
    global_rank: 102
    paper_rank: 102
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Full (GCN)
    model_key: full (gcn)
    model_plain: Full (GCN)
    value: 0.407
    std: 0.018
    paper_value: 0.407
    paper_std: 0.018
    metric: MAE
    higher_is_better: false
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
    source_ref: kipf2017semi
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for ZINC regression
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-09-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.407
    true_std: 0.018
    value_gap_source_arxiv: '2109.12872'
    value_gap_source_title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.407
    sort_std: 0.018
    global_rank: 103
    paper_rank: 103
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Vanilla (GCN)
    model_key: vanilla (gcn)
    model_plain: Vanilla (GCN)
    value: 0.669
    std: 0.07
    paper_value: 0.669
    paper_std: 0.07
    metric: MAE
    higher_is_better: false
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
    source_ref: hubara2016binarized
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for ZINC regression
    date: Sep 27, 2021
    date_display: Sep 2021
    date_iso: '2021-09-27'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-09-27'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.669
    true_std: 0.07
    value_gap_source_arxiv: '2109.12872'
    value_gap_source_title: 'Meta-Aggregator: Learning to Aggregate for 1-bit Graph
      Neural Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.669
    sort_std: 0.07
    global_rank: 107
    paper_rank: 107
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
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
    - dataset: PPI
      dataset_slug: ppi
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: ZINC
      dataset_slug: zinc
main_figure: /figures/2109.12872/main_figure.jpegoptim.jpg
---

