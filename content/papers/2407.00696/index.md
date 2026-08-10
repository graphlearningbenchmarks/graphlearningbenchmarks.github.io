---
title: Graph in Graph Neural Network
arxiv_id: '2407.00696'
source_url: ''
authors:
- name: Jiongshu Wang
  orcid: null
  s2_author_id: '2360838051'
  s2_url: null
- name: Jing Yang
  orcid: null
  s2_author_id: '2339357845'
  s2_url: null
- name: Jiankang Deng
  orcid: null
  s2_author_id: '2271553319'
  s2_url: null
- name: Hatice Gunes
  orcid: null
  s2_author_id: '2256439823'
  s2_url: null
- name: Siyang Song
  orcid: null
  s2_author_id: '2309215377'
  s2_url: null
published_date: Jun 30, 2024
published_date_iso: '2024-06-30'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Existing Graph Neural Networks (GNNs) are limited to process graphs each
  of whose vertices is represented by a vector or a single value, limited their representing
  capability to describe complex objects. In this paper, we propose a novel GNN (called
  Graph in Graph Neural (GIG) Network) which can process graph-style data (called
  GIG sample) whose vertices are further represented by graphs. Given a set of graphs
  or a data sample whose components can be represented by a set of graphs (called
  multi-graph data sample), our GIG network starts with a GIG sample generation (GSG)
  module which encodes the input as a GIG sample, where each GIG vertex includes a
  graph. Then, a set of GIG hidden layers are stacked, with each consisting of: (1)
  a GIG vertex-level updating (GVU) module that individually updates the graph in
  every GIG vertex based on its internal information; and (2) a global-level GIG sample
  updating (GGU) module that updates graphs in all GIG vertices based on their relationships,
  making the updated GIG vertices become global context-aware. This way, both internal
  cues within the graph contained in each GIG vertex and the relationships among GIG
  vertices could be utilized for down-stream tasks. Experimental results demonstrate
  that our GIG network generalizes well for not only various generic graph analysis
  tasks but also real-world multi-graph data analysis (e.g., human skeleton video-based
  action recognition), which achieved the new state-of-the-art results on 15 out of
  16 evaluated datasets. Our code is publicly available at https://github.com/wangjs96/Graph-in-Graph-Neural-Network.'
codebase_url: https://github.com/wangjs96/Graph-in-Graph-Neural-Network
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CNNs
mrr: 0.1385
adjusted_mrr: 0.0923
mrr_dataset_count: 2
benchmark_categories:
- Classic
- OGB
- GNNBenchmark
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 3
  total: 6
task_categories:
- graph_classification
- graph_regression
- link_prediction
- node_classification
experiment_scopes:
- edge-level
- graph-level
- node-level
results:
- &id003
  dataset: MNIST
  rows:
  - model: Schrödinger
    model_key: schrödinger
    model_plain: Schrödinger
    value: 0.9913
    std: 0.0004
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9913
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CNN
    model_key: cnn
    model_plain: CNN
    value: 0.9907
    std: 0.0007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9907
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    value: 0.9895
    std: 0.0006
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9895
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIG-GatedGCN
    model_key: gig-gatedgcn
    model_plain: GIG-GatedGCN
    value: 0.988
    std: 0.0003
    paper_value: 0.988
    paper_std: 0.0003
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MNIST
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.988
    true_std: 0.0003
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.988
    sort_std: 0.0003
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
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.9734
    std: 0.0014
    paper_value: 0.9734
    paper_std: 0.0014
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
    source_ref: 2017arXiv171107553B
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MNIST
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.98552
    at_pub_std: 0.00023
    at_pub_source_arxiv: '2404.09774'
    at_pub_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    at_pub_source_date_iso: '2024-04-15'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-15'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.012119999999999909
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.98552
    true_std: 0.00023
    value_gap_source_arxiv: '2404.09774'
    value_gap_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.012119999999999909
    has_value_note: false
    value_note: ''
    sort_value: 0.98552
    sort_std: 0.00023
    global_rank: 11
    paper_rank: 91
    rank_delta: 80
    rank_delta_abs: 80
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'RandAlign: A Parameter-Free Method for Regularizing
      Graph Convolutional Networks'
    comparison_source_arxiv: '2404.09774'
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.9855
    std: 0.0004
    paper_value: 0.9855
    paper_std: 0.0004
    metric: Accuracy
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
    source_ref: shirzad2023exphormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MNIST
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9855
    at_pub_std: 0.0003
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-07-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9855
    true_std: 0.00039
    value_gap_source_arxiv: '2407.02758'
    value_gap_source_title: Differential Encoding for Improved Representation Learning
      Over Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9855
    sort_std: 0.00039
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.9649
    std: 0.0025
    paper_value: 0.9649
    paper_std: 0.0025
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
    source_ref: xupowerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MNIST
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9723
    at_pub_std: null
    at_pub_source_arxiv: '2202.02296'
    at_pub_source_title: Graph-Coupled Oscillator Networks
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.007400000000000073
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9833
    true_std: 0.0011
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: 0.018399999999999972
    has_value_note: false
    value_note: ''
    sort_value: 0.9833
    sort_std: 0.0011
    global_rank: 32
    paper_rank: 112
    rank_delta: 80
    rank_delta_abs: 80
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph-Coupled Oscillator Networks
    comparison_source_arxiv: '2202.02296'
    is_best: false
    is_std_outlier: false
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.9817
    std: 0.0009
    paper_value: 0.9817
    paper_std: 0.0009
    metric: Accuracy
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
    source_ref: hussain2022global
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MNIST
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.98173
    at_pub_std: 0.00087
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 2.999999999997449e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.98173
    true_std: 0.00087
    value_gap_source_arxiv: '2605.05689'
    value_gap_source_title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive
      Consistency Model'
    value_gap_source_is_current_paper: false
    value_gap: 2.999999999997449e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.98173
    sort_std: 0.00087
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNAS-MP
    model_key: gnas-mp
    model_plain: GNAS-MP
    value: 0.9801
    std: 0.001
    paper_value: 0.9801
    paper_std: 0.001
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
    source_ref: cai2021rethinking
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MNIST
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9801
    true_std: 0.001
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9801
    sort_std: 0.001
    global_rank: 69
    paper_rank: 69
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PNA
    model_key: pna
    model_plain: PNA
    value: 0.9794
    std: 0.0012
    paper_value: 0.9794
    paper_std: 0.0012
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
    source_ref: corso2020principal
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MNIST
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9794
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-05-07'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9794
    true_std: 0.0012
    value_gap_source_arxiv: '2605.05689'
    value_gap_source_title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive
      Consistency Model'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9794
    sort_std: 0.0012
    global_rank: 75
    paper_rank: 75
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9554
    std: 0.0021
    paper_value: 0.9554
    paper_std: 0.0021
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
    source_ref: velivckovicgraph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MNIST
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.97553
    at_pub_std: 0.00034
    at_pub_source_arxiv: '2404.09774'
    at_pub_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    at_pub_source_date_iso: '2024-04-15'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-15'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.02012999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.97553
    true_std: 0.00034
    value_gap_source_arxiv: '2404.09774'
    value_gap_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.02012999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.97553
    sort_std: 0.00034
    global_rank: 87
    paper_rank: 123
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'RandAlign: A Parameter-Free Method for Regularizing
      Graph Convolutional Networks'
    comparison_source_arxiv: '2404.09774'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.97312
    std: 0.00097
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.02758'
    title: Differential Encoding for Improved Representation Learning Over Graphs
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    venue: IEEE Transactions on Big Data
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 97
    sort_value: 0.97312
    sort_std: 0.00097
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9534
    std: 0.00138
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: nodes in these graphs already have features describing
      their positions in R^2
    is_global_top: true
    global_rank: 128
    sort_value: 0.9534
    sort_std: 0.00138
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9012
    std: 0.0015
    paper_value: 0.9012
    paper_std: 0.0015
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
    source_ref: kipfsemi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard graph classification task on MNIST
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.94051
    at_pub_std: 0.00052
    at_pub_source_arxiv: '2404.09774'
    at_pub_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    at_pub_source_date_iso: '2024-04-15'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-15'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.039309999999999956
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.94051
    true_std: 0.00052
    value_gap_source_arxiv: '2404.09774'
    value_gap_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.039309999999999956
    has_value_note: false
    value_note: ''
    sort_value: 0.94051
    sort_std: 0.00052
    global_rank: 138
    paper_rank: 145
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'RandAlign: A Parameter-Free Method for Regularizing
      Graph Convolutional Networks'
    comparison_source_arxiv: '2404.09774'
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
  dataset: PATTERN
  rows:
  - model: DeepGraph (48)
    model_key: deepgraph (48)
    model_plain: DeepGraph (48)
    value: 0.90657
    std: 0.00062
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2303.00579'
    title: Are More Layers Beneficial to Graph Transformers?
    date: Mar 1, 2023
    date_display: Mar 2023
    date_iso: '2023-03-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/zhao-ht/DeepGraph
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.90657
    sort_std: 0.00062
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GRIT (our run)
    model_key: grit (our run)
    model_plain: GRIT (our run)
    value: 0.90405
    std: 0.00232
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.90405
    sort_std: 0.00232
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GRIT 2-QiQRW
    model_key: grit 2-qiqrw
    model_plain: GRIT 2-QiQRW
    value: 0.90165
    std: 0.00446
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2310.20519'
    title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    date: Oct 31, 2023
    date_display: Oct 2023
    date_iso: '2023-10-31'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.90165
    sort_std: 0.00446
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIG-GatedGCN
    model_key: gig-gatedgcn
    model_plain: GIG-GatedGCN
    value: 0.8687
    std: 0.0001
    paper_value: 0.8687
    paper_std: 0.0001
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on PATTERN dataset
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8687
    true_std: 0.0001
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8687
    sort_std: 0.0001
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.8557
    std: 0.0009
    paper_value: 0.8557
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
    source_ref: 2017arXiv171107553B
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification task on PATTERN dataset
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86508
    at_pub_std: 0.00085
    at_pub_source_arxiv: '2305.11424'
    at_pub_source_title: IJCAI--23 Formatting Instructions
    at_pub_source_date_iso: '2023-05-19'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2023-05-19'
    value_gap_source_date_label: IJCAI 2023
    gap_vs_at_pub: 0.009379999999999944
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.86508
    true_std: 0.00085
    value_gap_source_arxiv: '2305.11424'
    value_gap_source_title: IJCAI--23 Formatting Instructions
    value_gap_source_is_current_paper: false
    value_gap: 0.009379999999999944
    has_value_note: false
    value_note: ''
    sort_value: 0.86508
    sort_std: 0.00085
    global_rank: 66
    paper_rank: 91
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: IJCAI--23 Formatting Instructions
    comparison_source_arxiv: '2305.11424'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.85614
    std: 0.00032
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.01538'
    title: Recurrent Distance Filtering for Graph Representation Learning
    date: Dec 3, 2023
    date_display: Dec 2023
    date_iso: '2023-12-03'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/skeletondyh/GRED
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 88
    sort_value: 0.85614
    sort_std: 0.00032
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.50519
    std: 0.0
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 127
    sort_value: 0.50519
    sort_std: 0.0
    comparison_type: global_top
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
  dataset: TSP
  rows:
  - model: TGT-Agx4
    model_key: tgt-agx4
    model_plain: TGT-Agx4
    value: 0.871
    std: 0.001
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/shamim-hussain/tgt
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.871
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TGT-Agx3
    model_key: tgt-agx3
    model_plain: TGT-Agx3
    value: 0.866
    std: 0.001
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/shamim-hussain/tgt
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.866
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIG-GatedGCN
    model_key: gig-gatedgcn
    model_plain: GIG-GatedGCN
    value: 0.863
    std: 0.001
    paper_value: 0.863
    paper_std: 0.001
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
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Edge classification task on TSP dataset
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.863
    true_std: 0.001
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.863
    sort_std: 0.001
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.838
    std: 0.002
    paper_value: 0.838
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: 2017arXiv171107553B
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Edge classification task on TSP dataset
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.838
    at_pub_std: 0.002
    at_pub_source_arxiv: '2402.04538'
    at_pub_source_title: 'Triplet Interaction Improves Graph Transformers: Accurate
      Molecular Graph Learning with Triplet Graph Transformers'
    at_pub_source_date_iso: '2024-02-07'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.838
    true_std: 0.002
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.838
    sort_std: 0.002
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.671
    std: 0.002
    paper_value: 0.671
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: velivckovicgraph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Edge classification task on TSP dataset
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.671
    at_pub_std: 0.002
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.671
    true_std: 0.002
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.671
    sort_std: 0.002
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.665
    std: 0.003
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: nodes in these graphs already have features describing
      their positions in R^2
    is_global_top: true
    global_rank: 19
    sort_value: 0.665
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.656
    std: 0.003
    paper_value: 0.656
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: xupowerful
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Edge classification task on TSP dataset
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.656
    at_pub_std: 0.003
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.656
    true_std: 0.003
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.656
    sort_std: 0.003
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.643
    std: 0.001
    paper_value: 0.643
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: kipfsemi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: link_prediction
    protocol_decision: standard
    protocol_note: Edge classification task on TSP dataset
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.643
    at_pub_std: 0.001
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.643
    true_std: 0.001
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.643
    sort_std: 0.001
    global_rank: 21
    paper_rank: 21
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
    value: 0.544
    std: 0.001
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2003.00982'
    title: GNNBenchmark
    date: Jan 1, 2023
    date_display: Jan 2023
    date_iso: '2023-01-01'
    venue: Journal of machine learning research
    codebase_url: https://github.com/graphdeeplearning/benchmarking-gnns
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: nodes in these graphs already have features describing
      their positions in R^2
    is_global_top: true
    global_rank: 24
    sort_value: 0.544
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: edge-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
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
  - model: CNNs
    model_key: cnns
    model_plain: CNNs
    value: 0.029
    std: 0.001
    paper_value: 0.029
    paper_std: 0.001
    metric: MAE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Evaluates on the full ZINC dataset as described in the text.
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.029
    true_std: 0.001
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.029
    sort_std: 0.001
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.088
    std: 0.002
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.02479'
    title: Using Random Noise Equivariantly to Boost Graph Neural Networks Universally
    date: Feb 4, 2025
    date_display: Feb 2025
    date_iso: '2025-02-04'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 71
    sort_value: 0.088
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: ogbg-ppa
  rows:
  - model: A-NLSF
    model_key: a-nlsf
    model_plain: A-NLSF
    value: 0.8149
    std: 0.0067
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: Sep 29, 2025
    date_display: Sep 2025
    date_iso: '2025-09-29'
    venue: arXiv.org
    codebase_url: https://github.com/ywelld/_ac
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8149
    sort_std: 0.0067
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: differential encoding
    model_key: differential encoding
    model_plain: differential encoding
    value: 0.8096
    std: 0.0029
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.02758'
    title: Differential Encoding for Improved Representation Learning Over Graphs
    date: Jul 3, 2024
    date_display: Jul 2024
    date_iso: '2024-07-03'
    venue: IEEE Transactions on Big Data
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8096
    sort_std: 0.0029
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MPNN + VN + NoPE
    model_key: mpnn + vn + nope
    model_plain: MPNN + VN + NoPE
    value: 0.8055
    std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2301.11956'
    title: On the Connection Between MPNN and Graph Transformer
    date: Jan 27, 2023
    date_display: Jan 2023
    date_iso: '2023-01-27'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/Chen-Cai-OSU/MPNN-GT-Connection
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8055
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CNNs
    model_key: cnns
    model_plain: CNNs
    value: 0.8017
    std: null
    paper_value: 0.8017
    paper_std: null
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB species split for ogbg-ppa
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8017
    true_std: null
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8017
    sort_std: null
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
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.8015
    std: null
    paper_value: 0.8015
    paper_std: null
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
    source_ref: rampavsek2022recipe
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB species split for ogbg-ppa
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8015
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2301.11956'
    at_pub_source_title: On the Connection Between MPNN and Graph Transformer
    at_pub_source_date_iso: '2023-01-27'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-09-29'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8015
    true_std: 0.0033
    value_gap_source_arxiv: '2509.24886'
    value_gap_source_title: Adaptive Canonicalization with Application to Invariant
      Anisotropic Geometric Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8015
    sort_std: 0.0033
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
  - model: ExpC
    model_key: expc
    model_plain: ExpC
    value: 0.7976
    std: null
    paper_value: 0.7976
    paper_std: null
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
    source_ref: yang2020breaking
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB species split for ogbg-ppa
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7976
    at_pub_std: 0.0072
    at_pub_source_arxiv: '2305.06102'
    at_pub_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-07-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7976
    true_std: 0.0072
    value_gap_source_arxiv: '2407.02758'
    value_gap_source_title: Differential Encoding for Improved Representation Learning
      Over Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7976
    sort_std: 0.0072
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
  - model: DeeperGCN+FLAG
    model_key: deepergcn+flag
    model_plain: DeeperGCN+FLAG
    value: 0.7752
    std: null
    paper_value: 0.7752
    paper_std: null
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
    source_ref: kong2022robust
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB species split for ogbg-ppa
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7752
    at_pub_std: 0.0069
    at_pub_source_arxiv: '2103.16584'
    at_pub_source_title: Parameterized Hypercomplex Graph Neural Networks for Graph
      Classification
    at_pub_source_date_iso: '2021-03-30'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7752
    true_std: null
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7752
    sort_std: null
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeeperGCN
    model_key: deepergcn
    model_plain: DeeperGCN
    value: 0.7712
    std: null
    paper_value: 0.7712
    paper_std: null
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
    source_ref: li2020deepergcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard OGB species split for ogbg-ppa
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7712
    at_pub_std: 0.0071
    at_pub_source_arxiv: '2103.16584'
    at_pub_source_title: Parameterized Hypercomplex Graph Neural Networks for Graph
      Classification
    at_pub_source_date_iso: '2021-03-30'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-07-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7712
    true_std: 0.0071
    value_gap_source_arxiv: '2407.02758'
    value_gap_source_title: Differential Encoding for Improved Representation Learning
      Over Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7712
    sort_std: 0.0071
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.7531
    std: 0.0083
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: Sep 29, 2025
    date_display: Sep 2025
    date_iso: '2025-09-29'
    venue: arXiv.org
    codebase_url: https://github.com/ywelld/_ac
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 16
    sort_value: 0.7531
    sort_std: 0.0083
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.7037
    std: 0.0107
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: Sep 29, 2025
    date_display: Sep 2025
    date_iso: '2025-09-29'
    venue: arXiv.org
    codebase_url: https://github.com/ywelld/_ac
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 33
    sort_value: 0.7037
    sort_std: 0.0107
    comparison_type: global_top
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
- benchmark: Classic
  datasets:
  - *id001
- benchmark: OGB
  datasets:
  - *id002
- benchmark: GNNBenchmark
  datasets:
  - *id003
  - *id004
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: PATTERN
      dataset_slug: pattern
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: ZINC
      dataset_slug: zinc
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-ppa
      dataset_slug: ogbg-ppa
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: MNIST
      dataset_slug: mnist
- scope: edge-level
  label: Edge-level
  benchmarks:
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: TSP
      dataset_slug: tsp
single_proposed_model: CNNs
main_figure: /figures/2407.00696/main_figure.jpegoptim.jpg
---

