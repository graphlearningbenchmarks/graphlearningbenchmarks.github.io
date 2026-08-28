---
title: Differentiable Cluster Graph Neural Network
arxiv_id: '2405.16185'
source_url: ''
authors:
- name: Yanfei Dong
  orcid: null
  s2_author_id: '2294395732'
  s2_url: null
- name: Mohammed Haroon Dupty
  orcid: null
  s2_author_id: '3469411'
  s2_url: null
- name: Lambert Deng
  orcid: null
  s2_author_id: '2215629379'
  s2_url: null
- name: Zhuanghua Liu
  orcid: null
  s2_author_id: '2282914806'
  s2_url: null
- name: Yong Liang Goh
  orcid: null
  s2_author_id: '2294358396'
  s2_url: null
- name: Wee Sun Lee
  orcid: null
  s2_author_id: '2294397274'
  s2_url: null
published_date: May 25, 2024
published_date_iso: '2024-05-25'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Neural Networks often struggle with long-range information propagation
  and in the presence of heterophilous neighborhoods. We address both challenges with
  a unified framework that incorporates a clustering inductive bias into the message
  passing mechanism, using additional cluster-nodes. Central to our approach is the
  formulation of an optimal transport based implicit clustering objective function.
  However, the algorithm for solving the implicit objective function needs to be differentiable
  to enable end-to-end learning of the GNN. To facilitate this, we adopt an entropy
  regularized objective function and propose an iterative optimization process, alternating
  between solving for the cluster assignments and updating the node/cluster-node embeddings.
  Notably, our derived closed-form optimization steps are themselves simple yet elegant
  message passing steps operating seamlessly on a bipartite graph of nodes and cluster-nodes.
  Our clustering-based approach can effectively capture both local and global information,
  demonstrated by extensive experiments on both heterophilous and homophilous datasets.
codebase_url: ''
extraction_model: google/gemma-4-26B-A4B-it
has_results: true
paper_type: method
proposed_models:
- DC-GNN
mrr: 0.2322
adjusted_mrr: 0.2322
mrr_dataset_count: 7
benchmark_categories:
- Heterophilic Graphs
- Heterophily Benchmark
- LINKX Benchmarks
benchmark_coverage:
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 1
  total: 6
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 5
  total: 5
- benchmark: LINKX Benchmarks
  benchmark_slug: linkx-benchmarks
  evaluated: 1
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id003
  dataset: Amazon-ratings
  rows:
  - model: UniGAP
    model_key: unigap
    model_plain: UniGAP
    value: 0.6375
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.6375
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN + HalfHop
    model_key: h2gcn + halfhop
    model_plain: H2GCN + HalfHop
    value: 0.5961
    std: 0.01
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.5961
    sort_std: 0.01
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE + HalfHop
    model_key: graphsage + halfhop
    model_plain: GraphSAGE + HalfHop
    value: 0.5897
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
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.5897
    sort_std: 0.015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.5363
    std: 0.0039
    paper_value: 0.5363
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5363
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5569
    true_std: 0.0023
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.02059999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.5569
    sort_std: 0.0023
    global_rank: 12
    paper_rank: 31
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.4909
    std: 0.0063
    paper_value: 0.4909
    paper_std: 0.0063
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4909
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5559
    true_std: 0.0027
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.06499999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.5559
    sort_std: 0.0027
    global_rank: 14
    paper_rank: 109
    rank_delta: 95
    rank_delta_abs: 95
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
    value: 0.554
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 15
    sort_value: 0.554
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.487
    std: 0.0063
    paper_value: 0.487
    paper_std: 0.0063
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
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.487
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5411
    true_std: 0.0034
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.05410000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.5411
    sort_std: 0.0034
    global_rank: 25
    paper_rank: 113
    rank_delta: 88
    rank_delta_abs: 88
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FSGNN
    model_key: fsgnn
    model_plain: FSGNN
    value: 0.5274
    std: 0.0083
    paper_value: 0.5274
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5274
    at_pub_std: 0.0083
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5274
    true_std: 0.0083
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5274
    sort_std: 0.0083
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT-sep
    model_key: gat-sep
    model_plain: GAT-sep
    value: 0.527
    std: 0.0062
    paper_value: 0.527
    paper_std: 0.0062
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.527
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.527
    true_std: 0.0062
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.527
    sort_std: 0.0062
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
  - model: GT-sep
    model_key: gt-sep
    model_plain: GT-sep
    value: 0.5218
    std: 0.008
    paper_value: 0.5218
    paper_std: 0.008
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5218
    at_pub_std: 0.008
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5218
    true_std: 0.008
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5218
    sort_std: 0.008
    global_rank: 62
    paper_rank: 62
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet+adj
    model_key: resnet+adj
    model_plain: ResNet+adj
    value: 0.5183
    std: 0.0057
    paper_value: 0.5183
    paper_std: 0.0057
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5183
    true_std: 0.0057
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5183
    sort_std: 0.0057
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.5117
    std: 0.0066
    paper_value: 0.5117
    paper_std: 0.0066
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5117
    at_pub_std: 0.0066
    at_pub_source_arxiv: '2405.15540'
    at_pub_source_title: Bundle Neural Networks for message diffusion on graphs
    at_pub_source_date_iso: '2024-05-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5117
    true_std: 0.0066
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5117
    sort_std: 0.0066
    global_rank: 73
    paper_rank: 73
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DC-GNN
    model_key: dc-gnn
    model_plain: DC-GNN
    value: 0.5111
    std: 0.0047
    paper_value: 0.5111
    paper_std: 0.0047
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5111
    true_std: 0.0047
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5111
    sort_std: 0.0047
    global_rank: 76
    paper_rank: 76
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet+SGC
    model_key: resnet+sgc
    model_plain: ResNet+SGC
    value: 0.5066
    std: 0.0048
    paper_value: 0.5066
    paper_std: 0.0048
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5066
    true_std: 0.0048
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5066
    sort_std: 0.0048
    global_rank: 84
    paper_rank: 84
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
    value: 0.5058
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 85
    sort_value: 0.5058
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS⁴GAT+Performer
    model_key: gps⁴gat+performer
    model_plain: GPS⁴GAT+Performer
    value: 0.4992
    std: 0.0068
    paper_value: 0.4992
    paper_std: 0.0068
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
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4992
    true_std: 0.0068
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4992
    sort_std: 0.0068
    global_rank: 95
    paper_rank: 95
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.3689
    std: 0.0014
    paper_value: 0.3689
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4988
    at_pub_std: 0.004
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.12990000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4988
    true_std: 0.004
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.12990000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.4988
    sort_std: 0.004
    global_rank: 96
    paper_rank: 210
    rank_delta: 114
    rank_delta_abs: 114
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.4488
    std: 0.0034
    paper_value: 0.4488
    paper_std: 0.0034
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4488
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4937
    true_std: 0.0071
    value_gap_source_arxiv: '2505.04808'
    value_gap_source_title: Piecewise Constant Spectral Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.04490000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.4937
    sort_std: 0.0071
    global_rank: 107
    paper_rank: 157
    rank_delta: 50
    rank_delta_abs: 50
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.4355
    std: 0.0048
    paper_value: 0.4355
    paper_std: 0.0048
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4856
    at_pub_std: 0.002
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05009999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4856
    true_std: 0.002
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.05009999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.4856
    sort_std: 0.002
    global_rank: 117
    paper_rank: 173
    rank_delta: 56
    rank_delta_abs: 56
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.4412
    std: 0.003
    paper_value: 0.4412
    paper_std: 0.003
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4632
    at_pub_std: 0.025
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.02200000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4632
    true_std: 0.025
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.02200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.4632
    sort_std: 0.025
    global_rank: 141
    paper_rank: 164
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GBK-GNN
    model_key: gbk-gnn
    model_plain: GBK-GNN
    value: 0.4598
    std: 0.0071
    paper_value: 0.4598
    paper_std: 0.0071
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4598
    at_pub_std: 0.0071
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-03-27'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4598
    true_std: 0.0071
    value_gap_source_arxiv: '2603.26178'
    value_gap_source_title: 'Geometric Evolution Graph Convolutional Networks: Enhancing
      Graph Representation Learning via Ricci Flow'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4598
    sort_std: 0.0071
    global_rank: 145
    paper_rank: 145
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet
    model_key: resnet
    model_plain: ResNet
    value: 0.459
    std: 0.0052
    paper_value: 0.459
    paper_std: 0.0052
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.459
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-03-27'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.459
    true_std: 0.0052
    value_gap_source_arxiv: '2603.26178'
    value_gap_source_title: 'Geometric Evolution Graph Convolutional Networks: Enhancing
      Graph Representation Learning via Ricci Flow'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.459
    sort_std: 0.0052
    global_rank: 146
    paper_rank: 146
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CPGNN
    model_key: cpgnn
    model_plain: CPGNN
    value: 0.3979
    std: 0.0077
    paper_value: 0.3979
    paper_std: 0.0077
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4436
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.04570000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4436
    true_std: 0.0035
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.04570000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.4436
    sort_std: 0.0035
    global_rank: 162
    paper_rank: 203
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: H₂GCN
    model_key: h₂gcn
    model_plain: H₂GCN
    value: 0.3647
    std: 0.0023
    paper_value: 0.3647
    paper_std: 0.0023
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Amazon-ratings as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3647
    true_std: 0.0023
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3647
    sort_std: 0.0023
    global_rank: 212
    paper_rank: 212
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: Cornell
  rows:
  - model: P^2GNN
    model_key: p^2gnn
    model_plain: P^2GNN
    value: 0.9541
    std: 0.0272
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9541
    sort_std: 0.0272
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.7817
    std: 0.0142
    paper_value: 0.7817
    paper_std: 0.0142
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8514
    at_pub_std: 0.0607
    at_pub_source_arxiv: '2211.11761'
    at_pub_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    at_pub_source_date_iso: '2022-11-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.0697000000000001
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.948
    true_std: 0.038
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: false
    value_gap: 0.1663
    has_value_note: false
    value_note: ''
    sort_value: 0.948
    sort_std: 0.038
    global_rank: 2
    paper_rank: 241
    rank_delta: 239
    rank_delta_abs: 239
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RF-GCN
    model_key: rf-gcn
    model_plain: RF-GCN
    value: 0.9429
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 3
    sort_value: 0.9429
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.733
    std: 0.0187
    paper_value: 0.733
    paper_std: 0.0187
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9279
    at_pub_std: 0.0312
    at_pub_source_arxiv: '2302.03228'
    at_pub_source_title: Heterophily-Aware Graph Attention Network
    at_pub_source_date_iso: '2023-02-07'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-02-07'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.19489999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9279
    true_std: 0.0312
    value_gap_source_arxiv: '2302.03228'
    value_gap_source_title: Heterophily-Aware Graph Attention Network
    value_gap_source_is_current_paper: false
    value_gap: 0.19489999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9279
    sort_std: 0.0312
    global_rank: 11
    paper_rank: 308
    rank_delta: 297
    rank_delta_abs: 297
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterophily-Aware Graph Attention Network
    comparison_source_arxiv: '2302.03228'
    is_best: true
    is_std_outlier: false
  - model: GGCN
    model_key: ggcn
    model_plain: GGCN
    value: 0.7135
    std: 0.0081
    paper_value: 0.7135
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8568
    at_pub_std: 0.0663
    at_pub_source_arxiv: '2206.10991'
    at_pub_source_title: Understanding convolution on graphs via energies
    at_pub_source_date_iso: '2022-06-22'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.14329999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.923
    true_std: 0.0367
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.20950000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.923
    sort_std: 0.0367
    global_rank: 15
    paper_rank: 328
    rank_delta: 313
    rank_delta_abs: 313
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding convolution on graphs via energies
    comparison_source_arxiv: '2206.10991'
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6886
    std: 0.0183
    paper_value: 0.6886
    paper_std: 0.0183
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9136
    at_pub_std: 0.007
    at_pub_source_arxiv: '2212.03654'
    at_pub_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.22499999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9136
    true_std: 0.007
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.22499999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9136
    sort_std: 0.007
    global_rank: 25
    paper_rank: 351
    rank_delta: 326
    rank_delta_abs: 326
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    comparison_source_arxiv: '2212.03654'
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.7885
    std: 0.0078
    paper_value: 0.7885
    paper_std: 0.0078
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8426
    at_pub_std: 0.0213
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.05410000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8918
    true_std: 0.0396
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.10330000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8918
    sort_std: 0.0396
    global_rank: 39
    paper_rank: 226
    rank_delta: 187
    rank_delta_abs: 187
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: true
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.8396
    std: 0.0046
    paper_value: 0.8396
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8595
    at_pub_std: 0.051
    at_pub_source_arxiv: '2209.15454'
    at_pub_source_title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel
      Geometric Polynomials'
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-07-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.01990000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8595
    true_std: 0.051
    value_gap_source_arxiv: '2507.20127'
    value_gap_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    value_gap_source_is_current_paper: false
    value_gap: 0.01990000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8595
    sort_std: 0.051
    global_rank: 93
    paper_rank: 138
    rank_delta: 45
    rank_delta_abs: 45
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DC-GNN
    model_key: dc-gnn
    model_plain: DC-GNN
    value: 0.8468
    std: 0.0024
    paper_value: 0.8468
    paper_std: 0.0024
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8468
    true_std: 0.0024
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8468
    sort_std: 0.0024
    global_rank: 120
    paper_rank: 120
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.8346
    std: 0.0061
    paper_value: 0.8346
    paper_std: 0.0061
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7784
    at_pub_std: 0.058
    at_pub_source_arxiv: '2209.15454'
    at_pub_source_title: 'GPNet: Simplifying Graph Neural Networks via Multi-channel
      Geometric Polynomials'
    at_pub_source_date_iso: '2022-09-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05620000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8346
    true_std: 0.0061
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8346
    sort_std: 0.0061
    global_rank: 148
    paper_rank: 148
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8269
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
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 165
    sort_value: 0.8269
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H_2GCN
    model_key: h_2gcn
    model_plain: H_2GCN
    value: 0.7846
    std: 0.0075
    paper_value: 0.7846
    paper_std: 0.0075
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.822
    at_pub_std: 0.06
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-05-29'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.03739999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.822
    true_std: 0.06
    value_gap_source_arxiv: '2005.14612'
    value_gap_source_title: Non-Local Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.03739999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.06
    global_rank: 179
    paper_rank: 232
    rank_delta: 53
    rank_delta_abs: 53
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7896
    std: 0.0157
    paper_value: 0.7896
    paper_std: 0.0157
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.819
    at_pub_std: 0.054
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.02939999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.819
    true_std: 0.054
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.02939999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.819
    sort_std: 0.054
    global_rank: 190
    paper_rank: 224
    rank_delta: 34
    rank_delta_abs: 34
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WRGAT
    model_key: wrgat
    model_plain: WRGAT
    value: 0.7111
    std: 0.0048
    paper_value: 0.7111
    paper_std: 0.0048
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8162
    at_pub_std: 0.039
    at_pub_source_arxiv: '2111.06748'
    at_pub_source_title: Simplifying approach to Node Classification in Graph Neural
      Networks
    at_pub_source_date_iso: '2021-11-12'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2026-05-20'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.10510000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8162
    true_std: 0.039
    value_gap_source_arxiv: '2605.21247'
    value_gap_source_title: Graph Navier–Stokes Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.10510000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.8162
    sort_std: 0.039
    global_rank: 192
    paper_rank: 332
    rank_delta: 140
    rank_delta_abs: 140
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simplifying approach to Node Classification in Graph
      Neural Networks
    comparison_source_arxiv: '2111.06748'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8015
    std: 0.0037
    paper_value: 0.8015
    paper_std: 0.0037
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.792
    at_pub_std: 0.063
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-07-01'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.009499999999999953
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8082
    true_std: 0.036
    value_gap_source_arxiv: '2602.05358'
    value_gap_source_title: Bayesian Neighborhood Adaptation for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.006700000000000039
    has_value_note: false
    value_note: ''
    sort_value: 0.8082
    sort_std: 0.036
    global_rank: 203
    paper_rank: 210
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.7852
    std: 0.0122
    paper_value: 0.7852
    paper_std: 0.0122
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
    variant_inference_reason: 'dataset: fuzzy match to cornell (score=93)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard heterophilous node classification task.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.795
    at_pub_std: 0.063
    at_pub_source_arxiv: '2110.08128'
    at_pub_source_title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    at_pub_source_date_iso: '2021-10-15'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-15'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.009800000000000031
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.795
    true_std: 0.063
    value_gap_source_arxiv: '2110.08128'
    value_gap_source_title: Label-Wise Graph Convolutional Network for Heterophilic
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.009800000000000031
    has_value_note: false
    value_note: ''
    sort_value: 0.795
    sort_std: 0.063
    global_rank: 218
    paper_rank: 231
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
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
- &id004
  dataset: Minesweeper
  rows:
  - model: BuNN
    model_key: bunn
    model_plain: BuNN
    value: 0.9899
    std: 0.0016
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2405.15540'
    title: Bundle Neural Networks for message diffusion on graphs
    date: May 24, 2024
    date_display: May 2024
    date_iso: '2024-05-24'
    venue: arXiv.org
    codebase_url: https://github.com/jacobbamberger/BuNN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9899
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DC-GNN
    model_key: dc-gnn
    model_plain: DC-GNN
    value: 0.985
    std: 0.0021
    paper_value: 0.985
    paper_std: 0.0021
    metric: ROC-AUC
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.985
    true_std: 0.0021
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.985
    sort_std: 0.0021
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Polynormer-r
    model_key: polynormer-r
    model_plain: Polynormer-r
    value: 0.9746
    std: 0.0036
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/cornell-zhang/Polynormer
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9746
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9201
    std: 0.0068
    paper_value: 0.9201
    paper_std: 0.0068
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.921
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.0009000000000000119
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9391
    true_std: 0.0035
    value_gap_source_arxiv: '2510.21267'
    value_gap_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.019000000000000017
    has_value_note: false
    value_note: ''
    sort_value: 0.9391
    sort_std: 0.0035
    global_rank: 33
    paper_rank: 53
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT-sep
    model_key: gat-sep
    model_plain: GAT-sep
    value: 0.9391
    std: 0.0035
    paper_value: 0.9391
    paper_std: 0.0035
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9391
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9391
    true_std: 0.0035
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9391
    sort_std: 0.0035
    global_rank: 34
    paper_rank: 34
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
    value: 0.9358
    std: 0.0005
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.17531'
    title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    date: Aug 24, 2025
    date_display: Aug 2025
    date_iso: '2025-08-24'
    venue: European Conference on Artificial Intelligence
    codebase_url: https://github.com/Bobowner/Gumbel-Softmax-MPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 38
    sort_value: 0.9358
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9351
    std: 0.0057
    paper_value: 0.9351
    paper_std: 0.0057
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9351
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9351
    true_std: 0.0057
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9351
    sort_std: 0.0057
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
  - model: GT-sep
    model_key: gt-sep
    model_plain: GT-sep
    value: 0.9229
    std: 0.0047
    paper_value: 0.9229
    paper_std: 0.0047
    metric: ROC-AUC
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
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9229
    at_pub_std: 0.0047
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9229
    true_std: 0.0047
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9229
    sort_std: 0.0047
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.9185
    std: 0.0076
    paper_value: 0.9185
    paper_std: 0.0076
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9185
    at_pub_std: 0.0076
    at_pub_source_arxiv: '2405.15540'
    at_pub_source_title: Bundle Neural Networks for message diffusion on graphs
    at_pub_source_date_iso: '2024-05-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9185
    true_std: 0.0076
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9185
    sort_std: 0.0076
    global_rank: 56
    paper_rank: 56
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
    value: 0.8975
    std: 0.0052
    paper_value: 0.8975
    paper_std: 0.0052
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8975
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.915
    true_std: 0.0006
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.01750000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.915
    sort_std: 0.0006
    global_rank: 60
    paper_rank: 80
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS⁴GAT+Performer
    model_key: gps⁴gat+performer
    model_plain: GPS⁴GAT+Performer
    value: 0.9108
    std: 0.0058
    paper_value: 0.9108
    paper_std: 0.0058
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9108
    true_std: 0.0058
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9108
    sort_std: 0.0058
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GBK-GNN
    model_key: gbk-gnn
    model_plain: GBK-GNN
    value: 0.9085
    std: 0.0058
    paper_value: 0.9085
    paper_std: 0.0058
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9085
    at_pub_std: 0.0058
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9085
    true_std: 0.0058
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9085
    sort_std: 0.0058
    global_rank: 68
    paper_rank: 68
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FSGNN
    model_key: fsgnn
    model_plain: FSGNN
    value: 0.9008
    std: 0.007
    paper_value: 0.9008
    paper_std: 0.007
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9008
    at_pub_std: 0.007
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9008
    true_std: 0.007
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9008
    sort_std: 0.007
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
  - model: H₂GCN
    model_key: h₂gcn
    model_plain: H₂GCN
    value: 0.8971
    std: 0.0031
    paper_value: 0.8971
    paper_std: 0.0031
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8971
    true_std: 0.0031
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8971
    sort_std: 0.0031
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
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.8817
    std: 0.0073
    paper_value: 0.8817
    paper_std: 0.0073
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8969
    at_pub_std: 0.006
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.015199999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8969
    true_std: 0.006
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.015199999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.8969
    sort_std: 0.006
    global_rank: 83
    paper_rank: 95
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.8966
    std: 0.004
    paper_value: 0.8966
    paper_std: 0.004
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
    table_ref: Table 1
    source_ref: muller2023attending
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8966
    at_pub_std: 0.004
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8966
    true_std: 0.004
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8966
    sort_std: 0.004
    global_rank: 85
    paper_rank: 85
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8624
    std: 0.0061
    paper_value: 0.8624
    paper_std: 0.0061
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8624
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8624
    true_std: 0.0061
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8624
    sort_std: 0.0061
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
  - model: CPGNN
    model_key: cpgnn
    model_plain: CPGNN
    value: 0.5203
    std: 0.0546
    paper_value: 0.5203
    paper_std: 0.0546
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
    table_ref: Table 1
    source_ref: platonov2023critical
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7127
    at_pub_std: 0.0114
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.19240000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7127
    true_std: 0.0114
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.19240000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7127
    sort_std: 0.0114
    global_rank: 131
    paper_rank: 149
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: ResNet+SGC
    model_key: resnet+sgc
    model_plain: ResNet+SGC
    value: 0.7088
    std: 0.009
    paper_value: 0.7088
    paper_std: 0.009
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7088
    true_std: 0.009
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7088
    sort_std: 0.009
    global_rank: 134
    paper_rank: 134
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.5108
    std: 0.0123
    paper_value: 0.5108
    paper_std: 0.0123
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6253
    at_pub_std: 0.0134
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.11449999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6253
    true_std: 0.0134
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.11449999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.6253
    sort_std: 0.0134
    global_rank: 142
    paper_rank: 149
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.5099
    std: 0.0147
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2602.07256'
    title: 'Graph homophily booster: Reimagining the role of discrete features in
      heterophilic graph learning'
    date: Feb 6, 2026
    date_display: Feb 2026
    date_iso: '2026-02-06'
    venue: ICLR 2026
    codebase_url: https://github.com/q-rz/ICLR26-GRAPHITE
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 150
    sort_value: 0.5099
    sort_std: 0.0147
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet
    model_key: resnet
    model_plain: ResNet
    value: 0.5089
    std: 0.0139
    paper_value: 0.5089
    paper_std: 0.0139
    metric: ROC-AUC
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
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5095
    at_pub_std: 0.0112
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.0005999999999999339
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.5095
    true_std: 0.0112
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.0005999999999999339
    has_value_note: false
    value_note: ''
    sort_value: 0.5095
    sort_std: 0.0112
    global_rank: 151
    paper_rank: 152
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet+adj
    model_key: resnet+adj
    model_plain: ResNet+adj
    value: 0.5042
    std: 0.0083
    paper_value: 0.5042
    paper_std: 0.0083
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5042
    true_std: 0.0083
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5042
    sort_std: 0.0083
    global_rank: 154
    paper_rank: 154
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
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id007
  dataset: Penn94
  rows:
  - model: ChebNet2D
    model_key: chebnet2d
    model_plain: ChebNet2D
    value: 0.8762
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.04559'
    title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    venue: null
    codebase_url: https://github.com/jianhao2016/GPRGNN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8762
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DC-GNN
    model_key: dc-gnn
    model_plain: DC-GNN
    value: 0.8669
    std: 0.0022
    paper_value: 0.8669
    paper_std: 0.0022
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8669
    true_std: 0.0022
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8669
    sort_std: 0.0022
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: M2M-GNN
    model_key: m2m-gnn
    model_plain: M2M-GNN
    value: 0.8594
    std: 0.004
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.20652'
    title: 'Sign is Not a Remedy: Multiset-to-Multiset Message Passing for Learning
      on Heterophilic Graphs'
    date: May 31, 2024
    date_display: May 2024
    date_iso: '2024-05-31'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/Jinx-byebye/m2mgnn
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8594
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.8574
    std: 0.0042
    paper_value: 0.8574
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8574
    at_pub_std: 0.0042
    at_pub_source_arxiv: '2312.14438'
    at_pub_source_title: 'PC-Conv: Unifying Homophily and Heterophily with Two-fold
      Filtering'
    at_pub_source_date_iso: '2023-12-22'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8574
    true_std: 0.0042
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8574
    sort_std: 0.0042
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
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.8471
    std: 0.0052
    paper_value: 0.8471
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8515
    at_pub_std: 0.002
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0044000000000000705
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8515
    true_std: 0.002
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.0044000000000000705
    has_value_note: false
    value_note: ''
    sort_value: 0.8515
    sort_std: 0.002
    global_rank: 8
    paper_rank: 14
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.8347
    std: 0.0071
    paper_value: 0.8347
    paper_std: 0.0071
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8409
    at_pub_std: 0.002
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.006199999999999983
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8409
    true_std: 0.002
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.006199999999999983
    has_value_note: false
    value_note: ''
    sort_value: 0.8409
    sort_std: 0.002
    global_rank: 21
    paper_rank: 26
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8138
    std: 0.0016
    paper_value: 0.8138
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8354
    at_pub_std: 0.0032
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.021600000000000064
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8354
    true_std: 0.0032
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: false
    value_gap: 0.021600000000000064
    has_value_note: false
    value_note: ''
    sort_value: 0.8354
    sort_std: 0.0032
    global_rank: 26
    paper_rank: 44
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8247
    std: 0.0027
    paper_value: 0.8247
    paper_std: 0.0027
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8323
    at_pub_std: 0.002
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.007600000000000051
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8323
    true_std: 0.002
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.007600000000000051
    has_value_note: false
    value_note: ''
    sort_value: 0.8323
    sort_std: 0.002
    global_rank: 30
    paper_rank: 37
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Shape-aware Graph Spectral Learning
    comparison_source_arxiv: '2310.10064'
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.8131
    std: 0.006
    paper_value: 0.8131
    paper_std: 0.006
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.832
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.018899999999999917
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.832
    true_std: 0.0055
    value_gap_source_arxiv: '2306.02285'
    value_gap_source_title: Clarify Confused Nodes via Separated Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.018899999999999917
    has_value_note: false
    value_note: ''
    sort_value: 0.832
    sort_std: 0.0055
    global_rank: 31
    paper_rank: 44
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Clarify Confused Nodes via Separated Learning
    comparison_source_arxiv: '2306.02285'
    is_best: false
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.8252
    std: 0.0096
    paper_value: 0.8252
    paper_std: 0.0096
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8298
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0045999999999999375
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8298
    true_std: 0.0063
    value_gap_source_arxiv: '2306.02285'
    value_gap_source_title: Clarify Confused Nodes via Separated Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0045999999999999375
    has_value_note: false
    value_note: ''
    sort_value: 0.8298
    sort_std: 0.0063
    global_rank: 33
    paper_rank: 37
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.8292
    std: 0.0059
    paper_value: 0.8292
    paper_std: 0.0059
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8292
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8292
    true_std: 0.0059
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8292
    sort_std: 0.0059
    global_rank: 34
    paper_rank: 34
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
    value: 0.8268
    std: 0.0032
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2311.05185'
    title: Mixture of Weak & Strong Experts on Graphs
    date: Nov 9, 2023
    date_display: Nov 2023
    date_iso: '2023-11-09'
    venue: Accepted for publication in ICLR 2024
    codebase_url: https://github.com/VITA-Group/Graph-Mixture-of-Experts
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 36
    sort_value: 0.8268
    sort_std: 0.0032
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8153
    std: 0.0055
    paper_value: 0.8153
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8153
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2311.05185'
    at_pub_source_title: Mixture of Weak & Strong Experts on Graphs
    at_pub_source_date_iso: '2023-11-09'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8153
    true_std: 0.0055
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8153
    sort_std: 0.0055
    global_rank: 43
    paper_rank: 43
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
    value: 0.7361
    std: 0.004
    paper_value: 0.7361
    paper_std: 0.004
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7534
    at_pub_std: 0.0064
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.017299999999999982
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7534
    true_std: 0.0064
    value_gap_source_arxiv: '2306.02285'
    value_gap_source_title: Clarify Confused Nodes via Separated Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.017299999999999982
    has_value_note: false
    value_note: ''
    sort_value: 0.7534
    sort_std: 0.0064
    global_rank: 60
    paper_rank: 67
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Clarify Confused Nodes via Separated Learning
    comparison_source_arxiv: '2306.02285'
    is_best: false
    is_std_outlier: false
  - model: WRGAT
    model_key: wrgat
    model_plain: WRGAT
    value: 0.7432
    std: 0.0053
    paper_value: 0.7432
    paper_std: 0.0053
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7432
    at_pub_std: 0.0053
    at_pub_source_arxiv: '2312.14438'
    at_pub_source_title: 'PC-Conv: Unifying Homophily and Heterophily with Two-fold
      Filtering'
    at_pub_source_date_iso: '2023-12-22'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7432
    true_std: 0.0053
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7432
    sort_std: 0.0053
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GGCN
    model_key: ggcn
    model_plain: GGCN
    value: 0.7362
    std: 0.0061
    paper_value: 0.7362
    paper_std: 0.0061
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on Penn94
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7362
    true_std: 0.0061
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7362
    sort_std: 0.0061
    global_rank: 67
    paper_rank: 67
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id006
  dataset: Questions
  rows:
  - model: UniGAP
    model_key: unigap
    model_plain: UniGAP
    value: 0.8421
    std: 0.008
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8421
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN + AdaEdge
    model_key: h2gcn + adaedge
    model_plain: H2GCN + AdaEdge
    value: 0.8134
    std: 0.007
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8134
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN +AdaEdge
    model_key: gcn +adaedge
    model_plain: GCN +AdaEdge
    value: 0.8085
    std: 0.008
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8085
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.6359
    std: 0.0146
    paper_value: 0.6359
    paper_std: 0.0146
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6359
    at_pub_std: 0.0146
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7928
    true_std: 0.008
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_gap_source_is_current_paper: false
    value_gap: 0.15689999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7928
    sort_std: 0.008
    global_rank: 9
    paper_rank: 127
    rank_delta: 118
    rank_delta_abs: 118
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
    value: 0.7609
    std: 0.0127
    paper_value: 0.7609
    paper_std: 0.0127
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7609
    at_pub_std: 0.0127
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7902
    true_std: 0.006
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_gap_source_is_current_paper: false
    value_gap: 0.029299999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7902
    sort_std: 0.006
    global_rank: 12
    paper_rank: 55
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DC-GNN
    model_key: dc-gnn
    model_plain: DC-GNN
    value: 0.7896
    std: 0.006
    paper_value: 0.7896
    paper_std: 0.006
    metric: ROC-AUC
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7896
    true_std: 0.006
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7896
    sort_std: 0.006
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FSGNN
    model_key: fsgnn
    model_plain: FSGNN
    value: 0.7886
    std: 0.0092
    paper_value: 0.7886
    paper_std: 0.0092
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7886
    at_pub_std: 0.0092
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7886
    true_std: 0.0092
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7886
    sort_std: 0.0092
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
  - model: GT-sep
    model_key: gt-sep
    model_plain: GT-sep
    value: 0.7805
    std: 0.0093
    paper_value: 0.7805
    paper_std: 0.0093
    metric: ROC-AUC
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
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7805
    at_pub_std: 0.0093
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7805
    true_std: 0.0093
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7805
    sort_std: 0.0093
    global_rank: 24
    paper_rank: 24
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.7795
    std: 0.0068
    paper_value: 0.7795
    paper_std: 0.0068
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7795
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2405.15540'
    at_pub_source_title: Bundle Neural Networks for message diffusion on graphs
    at_pub_source_date_iso: '2024-05-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7795
    true_std: 0.0068
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7795
    sort_std: 0.0068
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7743
    std: 0.012
    paper_value: 0.7743
    paper_std: 0.012
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7743
    at_pub_std: 0.012
    at_pub_source_arxiv: '2403.12529'
    at_pub_source_title: Contextualized Messages Boost Graph Representations
    at_pub_source_date_iso: '2024-03-19'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7743
    true_std: 0.012
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7743
    sort_std: 0.012
    global_rank: 33
    paper_rank: 33
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.7724
    std: 0.0126
    paper_value: 0.7724
    paper_std: 0.0126
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7724
    at_pub_std: 0.0126
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7724
    true_std: 0.0126
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7724
    sort_std: 0.0126
    global_rank: 38
    paper_rank: 38
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
    value: 0.7721
    std: 0.013
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 41
    sort_value: 0.7721
    sort_std: 0.013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS GAT+Performer
    model_key: gps gat+performer
    model_plain: GPS GAT+Performer
    value: 0.7714
    std: 0.0149
    paper_value: 0.7714
    paper_std: 0.0149
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7714
    true_std: 0.0149
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7714
    sort_std: 0.0149
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
  - model: GAT-sep
    model_key: gat-sep
    model_plain: GAT-sep
    value: 0.7679
    std: 0.0071
    paper_value: 0.7679
    paper_std: 0.0071
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7679
    at_pub_std: 0.0071
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7679
    true_std: 0.0071
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7679
    sort_std: 0.0071
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.7644
    std: 0.0062
    paper_value: 0.7644
    paper_std: 0.0062
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7644
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7644
    true_std: 0.0062
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7644
    sort_std: 0.0062
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet+SGC
    model_key: resnet+sgc
    model_plain: ResNet+SGC
    value: 0.7581
    std: 0.0096
    paper_value: 0.7581
    paper_std: 0.0096
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7581
    true_std: 0.0096
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7581
    sort_std: 0.0096
    global_rank: 57
    paper_rank: 57
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet+adj
    model_key: resnet+adj
    model_plain: ResNet+adj
    value: 0.7577
    std: 0.0124
    paper_value: 0.7577
    paper_std: 0.0124
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7577
    true_std: 0.0124
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7577
    sort_std: 0.0124
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
  - model: GBK-GNN
    model_key: gbk-gnn
    model_plain: GBK-GNN
    value: 0.7447
    std: 0.0086
    paper_value: 0.7447
    paper_std: 0.0086
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7447
    at_pub_std: 0.0086
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7447
    true_std: 0.0086
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7447
    sort_std: 0.0086
    global_rank: 76
    paper_rank: 76
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.7388
    std: 0.0116
    paper_value: 0.7388
    paper_std: 0.0116
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7388
    at_pub_std: 0.0116
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7388
    true_std: 0.0116
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7388
    sort_std: 0.0116
    global_rank: 80
    paper_rank: 80
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.5548
    std: 0.0091
    paper_value: 0.5548
    paper_std: 0.0091
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5548
    at_pub_std: 0.0091
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7341
    true_std: 0.0124
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.17930000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7341
    sort_std: 0.0124
    global_rank: 81
    paper_rank: 146
    rank_delta: 65
    rank_delta_abs: 65
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
    value: 0.7082
    std: 0.001
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2508.17531'
    title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    date: Aug 24, 2025
    date_display: Aug 2025
    date_iso: '2025-08-24'
    venue: European Conference on Artificial Intelligence
    codebase_url: https://github.com/Bobowner/Gumbel-Softmax-MPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 91
    sort_value: 0.7082
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet
    model_key: resnet
    model_plain: ResNet
    value: 0.7034
    std: 0.0076
    paper_value: 0.7034
    paper_std: 0.0076
    metric: ROC-AUC
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7034
    at_pub_std: 0.0076
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7034
    true_std: 0.0076
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7034
    sort_std: 0.0076
    global_rank: 96
    paper_rank: 96
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.6574
    std: 0.0119
    paper_value: 0.6574
    paper_std: 0.0119
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6574
    at_pub_std: 0.0119
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6715
    true_std: 0.0192
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.014100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.6715
    sort_std: 0.0192
    global_rank: 115
    paper_rank: 119
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CPGNN
    model_key: cpgnn
    model_plain: CPGNN
    value: 0.6596
    std: 0.0195
    paper_value: 0.6596
    paper_std: 0.0195
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for Questions as per caption
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6596
    at_pub_std: 0.0195
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6709
    true_std: 0.0263
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.011300000000000088
    has_value_note: false
    value_note: ''
    sort_value: 0.6709
    sort_std: 0.0263
    global_rank: 116
    paper_rank: 119
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: Roman-empire
  rows:
  - model: Dir-Poly
    model_key: dir-poly
    model_plain: Dir-Poly
    value: 0.9451
    std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 1
    sort_value: 0.9451
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: D-CDE
    model_key: d-cde
    model_plain: D-CDE
    value: 0.9387
    std: 0.0041
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.05274'
    title: Distributed-Order Fractional Graph Operating Network
    date: Nov 8, 2024
    date_display: Nov 2024
    date_iso: '2024-11-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/zknus/NeurIPS-2024-DRAGON
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9387
    sort_std: 0.0041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LargeScaleNet
    model_key: largescalenet
    model_plain: LargeScaleNet
    value: 0.9358
    std: 0.0024
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2411.19392'
    title: Scale-aware Message Passing For Graph Node Classification
    date: Nov 28, 2024
    date_display: Nov 2024
    date_iso: '2024-11-28'
    venue: null
    codebase_url: https://github.com/Qin87/ScaleNet
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9358
    sort_std: 0.0024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9106
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.17939'
    title: Directed Semi-Simplicial Learning with Applications to Brain Activity Decoding
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    venue: null
    codebase_url: https://github.com/ManuelLecha/ssn
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 24
    sort_value: 0.9106
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DC-GNN
    model_key: dc-gnn
    model_plain: DC-GNN
    value: 0.8996
    std: 0.0035
    paper_value: 0.8996
    paper_std: 0.0035
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8996
    true_std: 0.0035
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8996
    sort_std: 0.0035
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
  - model: GAT-sep
    model_key: gat-sep
    model_plain: GAT-sep
    value: 0.8875
    std: 0.0041
    paper_value: 0.8875
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8875
    at_pub_std: 0.0041
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8875
    true_std: 0.0041
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8875
    sort_std: 0.0041
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GT-sep
    model_key: gt-sep
    model_plain: GT-sep
    value: 0.8732
    std: 0.0039
    paper_value: 0.8732
    paper_std: 0.0039
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8732
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8732
    true_std: 0.0039
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8732
    sort_std: 0.0039
    global_rank: 55
    paper_rank: 55
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPSⁿGAT+Performer
    model_key: gpsⁿgat+performer
    model_plain: GPSⁿGAT+Performer
    value: 0.8704
    std: 0.0058
    paper_value: 0.8704
    paper_std: 0.0058
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
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8704
    true_std: 0.0058
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8704
    sort_std: 0.0058
    global_rank: 56
    paper_rank: 56
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.8651
    std: 0.0073
    paper_value: 0.8651
    paper_std: 0.0073
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8651
    at_pub_std: 0.0073
    at_pub_source_arxiv: '2405.15540'
    at_pub_source_title: Bundle Neural Networks for message diffusion on graphs
    at_pub_source_date_iso: '2024-05-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8651
    true_std: 0.0073
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8651
    sort_std: 0.0073
    global_rank: 59
    paper_rank: 59
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8574
    std: 0.0067
    paper_value: 0.8574
    paper_std: 0.0067
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8574
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-07-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8574
    true_std: 0.0067
    value_gap_source_arxiv: '2507.14484'
    value_gap_source_title: 'ReDiSC: A Reparameterized Masked Diffusion Model for
      Scalable Node Classification with Structured Predictions'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8574
    sort_std: 0.0067
    global_rank: 64
    paper_rank: 64
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
    value: 0.7369
    std: 0.0074
    paper_value: 0.7369
    paper_std: 0.0074
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
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7369
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8272
    true_std: 0.0082
    value_gap_source_arxiv: '2407.11596'
    value_gap_source_title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    value_gap_source_is_current_paper: false
    value_gap: 0.09030000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8272
    sort_std: 0.0082
    global_rank: 75
    paper_rank: 116
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8087
    std: 0.003
    paper_value: 0.8087
    paper_std: 0.003
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8102
    at_pub_std: 0.0046
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0015000000000000568
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8145
    true_std: 0.0009
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.005800000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.8145
    sort_std: 0.0009
    global_rank: 82
    paper_rank: 83
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FSGNN
    model_key: fsgnn
    model_plain: FSGNN
    value: 0.7992
    std: 0.0056
    paper_value: 0.7992
    paper_std: 0.0056
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7992
    at_pub_std: 0.0056
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7992
    true_std: 0.0056
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7992
    sort_std: 0.0056
    global_rank: 91
    paper_rank: 91
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GBK-GNN
    model_key: gbk-gnn
    model_plain: GBK-GNN
    value: 0.7457
    std: 0.0047
    paper_value: 0.7457
    paper_std: 0.0047
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7587
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.013000000000000012
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7587
    true_std: 0.0043
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.013000000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.7587
    sort_std: 0.0043
    global_rank: 107
    paper_rank: 110
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.6522
    std: 0.0056
    paper_value: 0.6522
    paper_std: 0.0056
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7053
    at_pub_std: 0.0099
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.053100000000000036
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7571
    true_std: 0.0139
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.1049
    has_value_note: false
    value_note: ''
    sort_value: 0.7571
    sort_std: 0.0139
    global_rank: 108
    paper_rank: 148
    rank_delta: 40
    rank_delta_abs: 40
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.7114
    std: 0.0042
    paper_value: 0.7114
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7435
    at_pub_std: 0.006
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03210000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7435
    true_std: 0.006
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.03210000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7435
    sort_std: 0.006
    global_rank: 113
    paper_rank: 128
    rank_delta: 15
    rank_delta_abs: 15
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: ResNet+SGC
    model_key: resnet+sgc
    model_plain: ResNet+SGC
    value: 0.739
    std: 0.0051
    paper_value: 0.739
    paper_std: 0.0051
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.739
    true_std: 0.0051
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.739
    sort_std: 0.0051
    global_rank: 116
    paper_rank: 116
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.6485
    std: 0.0027
    paper_value: 0.6485
    paper_std: 0.0027
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7337
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-11-08'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.08520000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7337
    true_std: 0.0068
    value_gap_source_arxiv: '2411.05274'
    value_gap_source_title: Distributed-Order Fractional Graph Operating Network
    value_gap_source_is_current_paper: false
    value_gap: 0.08520000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.7337
    sort_std: 0.0068
    global_rank: 118
    paper_rank: 150
    rank_delta: 32
    rank_delta_abs: 32
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.5963
    std: 0.0069
    paper_value: 0.5963
    paper_std: 0.0069
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6739
    at_pub_std: 0.003
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0776
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6739
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.0776
    has_value_note: false
    value_note: ''
    sort_value: 0.6739
    sort_std: 0.003
    global_rank: 138
    paper_rank: 174
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6665
    std: 0.0047
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.11596'
    title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: https://github.com/Foisunt/HyperAggregation
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 141
    sort_value: 0.6665
    sort_std: 0.0047
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet
    model_key: resnet
    model_plain: ResNet
    value: 0.6588
    std: 0.0038
    paper_value: 0.6588
    paper_std: 0.0038
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6588
    at_pub_std: 0.0038
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-03-27'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6588
    true_std: 0.0038
    value_gap_source_arxiv: '2603.26178'
    value_gap_source_title: 'Geometric Evolution Graph Convolutional Networks: Enhancing
      Graph Representation Learning via Ricci Flow'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6588
    sort_std: 0.0038
    global_rank: 147
    paper_rank: 147
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CPGNN
    model_key: cpgnn
    model_plain: CPGNN
    value: 0.6396
    std: 0.0062
    paper_value: 0.6396
    paper_std: 0.0062
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6396
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6396
    true_std: 0.0062
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6396
    sort_std: 0.0062
    global_rank: 159
    paper_rank: 159
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H₂GCN
    model_key: h₂gcn
    model_plain: H₂GCN
    value: 0.6011
    std: 0.0052
    paper_value: 0.6011
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6011
    true_std: 0.0052
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6011
    sort_std: 0.0052
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
  - model: ResNet+adj
    model_key: resnet+adj
    model_plain: ResNet+adj
    value: 0.5225
    std: 0.004
    paper_value: 0.5225
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy reported for Roman-empire as per Platonov et al. 2023
      protocol.
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5225
    true_std: 0.004
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5225
    sort_std: 0.004
    global_rank: 193
    paper_rank: 193
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id005
  dataset: Tolokers
  rows:
  - model: Polynormer-r
    model_key: polynormer-r
    model_plain: Polynormer-r
    value: 0.8591
    std: 0.0074
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2403.01232'
    title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear Time'
    date: Mar 2, 2024
    date_display: Mar 2024
    date_iso: '2024-03-02'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/cornell-zhang/Polynormer
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8591
    sort_std: 0.0074
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DC-GNN
    model_key: dc-gnn
    model_plain: DC-GNN
    value: 0.8588
    std: 0.0081
    paper_value: 0.8588
    paper_std: 0.0081
    metric: ROC-AUC
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8588
    true_std: 0.0081
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8588
    sort_std: 0.0081
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
  - model: Polynormer + Wideformer
    model_key: polynormer + wideformer
    model_plain: Polynormer + Wideformer
    value: 0.8533
    std: 0.0023
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8533
    sort_std: 0.0023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.837
    std: 0.0047
    paper_value: 0.837
    paper_std: 0.0047
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.837
    at_pub_std: 0.0047
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-06-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8443
    true_std: 0.01
    value_gap_source_arxiv: '2406.06642'
    value_gap_source_title: 'TopoBench: A Framework for Benchmarking Topological Deep
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.007300000000000084
    has_value_note: false
    value_note: ''
    sort_value: 0.8443
    sort_std: 0.01
    global_rank: 18
    paper_rank: 36
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS GAT+Performer
    model_key: gps gat+performer
    model_plain: GPS GAT+Performer
    value: 0.8438
    std: 0.0091
    paper_value: 0.8438
    paper_std: 0.0091
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8438
    true_std: 0.0091
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8438
    sort_std: 0.0091
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT-sep
    model_key: gat-sep
    model_plain: GAT-sep
    value: 0.8378
    std: 0.0043
    paper_value: 0.8378
    paper_std: 0.0043
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8378
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8378
    true_std: 0.0043
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8378
    sort_std: 0.0043
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8364
    std: 0.0067
    paper_value: 0.8364
    paper_std: 0.0067
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8364
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8364
    true_std: 0.0067
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8364
    sort_std: 0.0067
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.8323
    std: 0.0064
    paper_value: 0.8323
    paper_std: 0.0064
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8323
    at_pub_std: 0.0064
    at_pub_source_arxiv: '2405.15540'
    at_pub_source_title: Bundle Neural Networks for message diffusion on graphs
    at_pub_source_date_iso: '2024-05-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8323
    true_std: 0.0064
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8323
    sort_std: 0.0064
    global_rank: 50
    paper_rank: 50
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FSGNN
    model_key: fsgnn
    model_plain: FSGNN
    value: 0.8276
    std: 0.0061
    paper_value: 0.8276
    paper_std: 0.0061
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
    table_ref: Table 1
    source_ref: platonov2023critical
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8276
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8276
    true_std: 0.0061
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8276
    sort_std: 0.0061
    global_rank: 56
    paper_rank: 56
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GT-sep
    model_key: gt-sep
    model_plain: GT-sep
    value: 0.8252
    std: 0.0092
    paper_value: 0.8252
    paper_std: 0.0092
    metric: ROC-AUC
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
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8252
    at_pub_std: 0.0092
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8252
    true_std: 0.0092
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8252
    sort_std: 0.0092
    global_rank: 65
    paper_rank: 65
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8243
    std: 0.0044
    paper_value: 0.8243
    paper_std: 0.0044
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
    table_ref: Table 1
    source_ref: li2022finding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8243
    at_pub_std: 0.0044
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8243
    true_std: 0.0044
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8243
    sort_std: 0.0044
    global_rank: 68
    paper_rank: 68
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
    value: 0.8243
    std: 0.0044
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 69
    sort_value: 0.8243
    sort_std: 0.0044
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GBK-GNN
    model_key: gbk-gnn
    model_plain: GBK-GNN
    value: 0.8101
    std: 0.0067
    paper_value: 0.8101
    paper_std: 0.0067
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
    table_ref: Table 1
    source_ref: platonov2023critical
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8101
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8101
    true_std: 0.0067
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8101
    sort_std: 0.0067
    global_rank: 79
    paper_rank: 79
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet+SGC
    model_key: resnet+sgc
    model_plain: ResNet+SGC
    value: 0.807
    std: 0.0097
    paper_value: 0.807
    paper_std: 0.0097
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.807
    true_std: 0.0097
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.807
    sort_std: 0.0097
    global_rank: 84
    paper_rank: 84
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet+adj
    model_key: resnet+adj
    model_plain: ResNet+adj
    value: 0.7878
    std: 0.0111
    paper_value: 0.7878
    paper_std: 0.0111
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7878
    true_std: 0.0111
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7878
    sort_std: 0.0111
    global_rank: 99
    paper_rank: 99
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.7335
    std: 0.0101
    paper_value: 0.7335
    paper_std: 0.0101
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
    table_ref: Table 1
    source_ref: platonov2023critical
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7335
    at_pub_std: 0.0101
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7815
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.04799999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7815
    sort_std: null
    global_rank: 108
    paper_rank: 137
    rank_delta: 29
    rank_delta_abs: 29
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.7775
    std: 0.0105
    paper_value: 0.7775
    paper_std: 0.0105
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
    table_ref: Table 1
    source_ref: platonov2023critical
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7775
    at_pub_std: 0.0105
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7812
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0037000000000000366
    has_value_note: false
    value_note: ''
    sort_value: 0.7812
    sort_std: null
    global_rank: 111
    paper_rank: 117
    rank_delta: 6
    rank_delta_abs: 6
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
    value: 0.7362
    std: 0.002
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2508.17531'
    title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    date: Aug 24, 2025
    date_display: Aug 2025
    date_iso: '2025-08-24'
    venue: European Conference on Artificial Intelligence
    codebase_url: https://github.com/Bobowner/Gumbel-Softmax-MPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 135
    sort_value: 0.7362
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.7339
    std: 0.0117
    paper_value: 0.7339
    paper_std: 0.0117
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
    table_ref: Table 1
    source_ref: platonov2023critical
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7339
    at_pub_std: 0.0117
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7339
    true_std: 0.0117
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7339
    sort_std: 0.0117
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
  - model: CPGNN
    model_key: cpgnn
    model_plain: CPGNN
    value: 0.7336
    std: 0.0101
    paper_value: 0.7336
    paper_std: 0.0101
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
    table_ref: Table 1
    source_ref: platonov2023critical
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7336
    at_pub_std: 0.0101
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7336
    true_std: 0.0101
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7336
    sort_std: 0.0101
    global_rank: 137
    paper_rank: 137
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ResNet
    model_key: resnet
    model_plain: ResNet
    value: 0.7295
    std: 0.0106
    paper_value: 0.7295
    paper_std: 0.0106
    metric: ROC-AUC
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7295
    at_pub_std: 0.0106
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7295
    true_std: 0.0106
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7295
    sort_std: 0.0106
    global_rank: 139
    paper_rank: 139
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.7294
    std: 0.0097
    paper_value: 0.7294
    paper_std: 0.0097
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
    table_ref: Table 1
    source_ref: platonov2023critical
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7294
    at_pub_std: 0.0097
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7294
    true_std: 0.0097
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7294
    sort_std: 0.0097
    global_rank: 140
    paper_rank: 140
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.6866
    std: 0.0065
    paper_value: 0.6866
    paper_std: 0.0065
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
    table_ref: Table 1
    source_ref: muller2023attending
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: ROC AUC reported for heterophilous datasets in Table 1
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6866
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6866
    true_std: 0.0065
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6866
    sort_std: 0.0065
    global_rank: 151
    paper_rank: 151
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
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Heterophilic Graphs
  datasets:
  - *id001
- benchmark: Heterophily Benchmark
  datasets:
  - *id002
  - *id003
  - *id004
  - *id005
  - *id006
- benchmark: LINKX Benchmarks
  datasets:
  - *id007
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Cornell
      dataset_slug: cornell
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Roman-empire
      dataset_slug: roman-empire
    - dataset: Amazon-ratings
      dataset_slug: amazon-ratings
    - dataset: Minesweeper
      dataset_slug: minesweeper
    - dataset: Tolokers
      dataset_slug: tolokers
    - dataset: Questions
      dataset_slug: questions
  - benchmark: LINKX Benchmarks
    benchmark_slug: linkx-benchmarks
    datasets:
    - dataset: Penn94
      dataset_slug: penn94
single_proposed_model: DC-GNN
main_figure: /figures/2405.16185/main_figure.jpegoptim.jpg
---

