---
title: Decimated Framelet System on Graphs and Fast $ $-Framelet Transforms
arxiv_id: '2012.06922'
source_url: ''
authors:
- name: Xuebin Zheng
  orcid: null
  s2_author_id: '47410668'
  s2_url: null
- name: Bingxin Zhou
  orcid: null
  s2_author_id: '65772187'
  s2_url: null
- name: Yu Guang Wang
  orcid: null
  s2_author_id: '97594744'
  s2_url: null
- name: Xiaosheng Zhuang
  orcid: null
  s2_author_id: '145238883'
  s2_url: null
published_date: Dec 12, 2020
published_date_iso: '2020-12-12'
published_venue: JMLR 2020
published_conference: JMLR 2020
published_conference_short: JMLR
published_conference_slug: jmlr
abstract: Graph representation learning has many real-world applications, from self-driving
  LiDAR, 3D computer vision to drug repurposing, protein classification, social networks
  analysis. An adequate representation of graph data is vital to the learning performance
  of a statistical or machine learning model for graph-structured data. This paper
  proposes a novel multiscale representation system for graph data, called decimated
  framelets, which form a localized tight frame on the graph. The decimated framelet
  system allows storage of the graph data representation on a coarse-grained chain
  and processes the graph data at multi scales where at each scale, the data is stored
  on a subgraph. Based on this, we establish decimated $ $-framelet transforms for
  the decomposition and reconstruction of the graph data at multi resolutions via
  a constructive data-driven filter bank. The graph framelets are built on a chain-based
  orthonormal basis that supports fast graph Fourier transforms. From this, we give
  a fast algorithm for the decimated $ $-framelet transforms, or, that has linear
  computational complexity $ N$ for a graph of size $N$. The effectiveness for constructing
  the decimated framelet system and the is demonstrated by a simulated example of
  random graphs and real-world applications, including multiresolution analysis for
  traffic network and representation learning of graph neural networks for graph classification
  tasks.
codebase_url: https://github.com/YuGuangWang/FGT
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- FGConv-Sum
mrr: 0.1034
adjusted_mrr: 0.069
mrr_dataset_count: 2
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 2
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: D&D
  rows:
  - model: GC-GNN (GCN)
    model_key: gc-gnn (gcn)
    model_plain: GC-GNN (GCN)
    value: 0.921
    std: 0.081
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2309.00738'
    title: Rethinking the Power of Graph Canonization in Graph Representation Learning
      with Stability
    date: Sep 1, 2023
    date_display: Sep 2023
    date_iso: '2023-09-01'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: The paper describes GC-GNN as enhancing GNNs with graph
      canonization positional encodings.
    is_global_top: true
    global_rank: 1
    sort_value: 0.921
    sort_std: 0.081
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SUGAR
    model_key: sugar
    model_plain: SUGAR
    value: 0.8403
    std: 0.0133
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2101.08170'
    title: 'SUGAR: Subgraph Neural Network with Reinforcement Pooling and Self-Supervised
      Mutual Information Mechanism'
    date: Jan 20, 2021
    date_display: Jan 2021
    date_iso: '2021-01-20'
    venue: The Web Conference
    codebase_url: https://github.com/RingBDStack/SUGAR
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8403
    sort_std: 0.0133
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Ortho-g-U-Nets
    model_key: ortho-g-u-nets
    model_plain: Ortho-g-U-Nets
    value: 0.8387
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2109.11338'
    title: Orthogonal Graph Neural Networks
    date: Sep 23, 2021
    date_display: Sep 2021
    date_iso: '2021-09-23'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8387
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: g-U-Nets
    model_key: g-u-nets
    model_plain: g-U-Nets
    value: 0.8243
    std: null
    paper_value: 0.8243
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Mean test accuracy reported over 10 repetitions.
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.8243
    at_pub_std: null
    at_pub_source_arxiv: '1905.05178'
    at_pub_source_title: Graph U-Nets
    at_pub_source_date_iso: '2019-05-11'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2021-09-23'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.83
    true_std: null
    value_gap_source_arxiv: '2109.11338'
    value_gap_source_title: Orthogonal Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.005699999999999927
    has_value_note: false
    value_note: ''
    sort_value: 0.83
    sort_std: null
    global_rank: 4
    paper_rank: 6
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FGConv-Sum
    model_key: fgconv-sum
    model_plain: FGConv-Sum
    value: 0.829
    std: 0.0255
    paper_value: 0.829
    paper_std: 0.0255
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
    protocol_note: Mean test accuracy reported over 10 repetitions.
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-12'
    value_gap_source_date_label: JMLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.829
    true_std: 0.0255
    value_gap_source_arxiv: '2012.06922'
    value_gap_source_title: Decimated Framelet System on Graphs and Fast $ $-Framelet
      Transforms
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.829
    sort_std: 0.0255
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8088
    std: 0.0233
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.05416'
    title: Semi-Supervised Hierarchical Graph Classification
    date: Jun 11, 2022
    date_display: Jun 2022
    date_iso: '2022-06-11'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 18
    sort_value: 0.8088
    sort_std: 0.0233
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 0.8064
    std: null
    paper_value: 0.8064
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Mean test accuracy reported over 10 repetitions.
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.8064
    at_pub_std: null
    at_pub_source_arxiv: '1905.05178'
    at_pub_source_title: Graph U-Nets
    at_pub_source_date_iso: '2019-05-11'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2021-09-23'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8064
    true_std: null
    value_gap_source_arxiv: '2109.11338'
    value_gap_source_title: Orthogonal Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8064
    sort_std: null
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
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.7795
    std: null
    paper_value: 0.7795
    paper_std: null
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
    source_ref: niepert2016learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Mean test accuracy reported over 10 repetitions.
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.7978
    at_pub_std: null
    at_pub_source_arxiv: '1704.02901'
    at_pub_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    at_pub_source_date_iso: '2017-04-10'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2024-02-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.018299999999999983
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7978
    true_std: 0.0036
    value_gap_source_arxiv: '2402.16402'
    value_gap_source_title: Graph Learning with Distributional Edge Layouts
    value_gap_source_is_current_paper: false
    value_gap: 0.018299999999999983
    has_value_note: false
    value_note: ''
    sort_value: 0.7978
    sort_std: 0.0036
    global_rank: 29
    paper_rank: 85
    rank_delta: 56
    rank_delta_abs: 56
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Dynamic Edge-Conditioned Filters in Convolutional Neural
      Networks on Graphs
    comparison_source_arxiv: '1704.02901'
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.7937
    std: null
    paper_value: 0.7937
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Mean test accuracy reported over 10 repetitions.
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.7937
    at_pub_std: 0.0094
    at_pub_source_arxiv: '1805.08090'
    at_pub_source_title: Graph Capsule Convolutional Neural Networks
    at_pub_source_date_iso: '2018-05-21'
    at_pub_source_date_label: ICML 2018
    value_gap_source_date_iso: '2021-09-23'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7937
    true_std: null
    value_gap_source_arxiv: '2109.11338'
    value_gap_source_title: Orthogonal Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7937
    sort_std: null
    global_rank: 41
    paper_rank: 41
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGPool
    model_key: sagpool
    model_plain: SAGPool
    value: 0.7707
    std: null
    paper_value: 0.7707
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Mean test accuracy reported over 10 repetitions.
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.787
    at_pub_std: 0.0229
    at_pub_source_arxiv: '2009.05923'
    at_pub_source_title: Contrastive Self-supervised Learning for Graph Classification
    at_pub_source_date_iso: '2020-09-13'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.01629999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.787
    true_std: 0.0229
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.01629999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.787
    sort_std: 0.0229
    global_rank: 62
    paper_rank: 111
    rank_delta: 49
    rank_delta_abs: 49
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EigenPool
    model_key: eigenpool
    model_plain: EigenPool
    value: 0.786
    std: null
    paper_value: 0.786
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Mean test accuracy reported over 10 repetitions.
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.7863
    at_pub_std: 0.0136
    at_pub_source_arxiv: '2009.05923'
    at_pub_source_title: Contrastive Self-supervised Learning for Graph Classification
    at_pub_source_date_iso: '2020-09-13'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2020-09-13'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7863
    true_std: 0.0136
    value_gap_source_arxiv: '2009.05923'
    value_gap_source_title: Contrastive Self-supervised Learning for Graph Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.7863
    sort_std: 0.0136
    global_rank: 63
    paper_rank: 64
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphlet
    model_key: graphlet
    model_plain: Graphlet
    value: 0.7845
    std: null
    paper_value: 0.7845
    paper_std: null
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
    source_ref: niepert2016learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Mean test accuracy reported over 10 repetitions.
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.7845
    at_pub_std: null
    at_pub_source_arxiv: '2007.11202'
    at_pub_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for
      Graph Representation and Learning'
    at_pub_source_date_iso: '2020-07-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-12-12'
    value_gap_source_date_label: JMLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7845
    true_std: null
    value_gap_source_arxiv: '2012.06922'
    value_gap_source_title: Decimated Framelet System on Graphs and Fast $ $-Framelet
      Transforms
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7845
    sort_std: null
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
  - model: PatchySan
    model_key: patchysan
    model_plain: PatchySan
    value: 0.7627
    std: null
    paper_value: 0.7627
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Mean test accuracy reported over 10 repetitions.
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.7627
    at_pub_std: null
    at_pub_source_arxiv: '2007.11202'
    at_pub_source_title: 'MathNet: Haar-Like Wavelet Multiresolution-Analysis for
      Graph Representation and Learning'
    at_pub_source_date_iso: '2020-07-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-12-12'
    value_gap_source_date_label: JMLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7627
    true_std: null
    value_gap_source_arxiv: '2012.06922'
    value_gap_source_title: Decimated Framelet System on Graphs and Fast $ $-Framelet
      Transforms
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7627
    sort_std: null
    global_rank: 123
    paper_rank: 123
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
- &id001
  dataset: MUTAG
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
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
    input_feature_source: raw_features
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
  - model: ID-GNN+BEC
    model_key: id-gnn+bec
    model_plain: ID-GNN+BEC
    value: 0.983
    std: 0.036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_display: Mar 2025
    date_iso: '2025-03-03'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SupCosine
    model_key: supcosine
    model_plain: SupCosine
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
    global_rank: 3
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.894
    std: null
    paper_value: 0.894
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: mean test accuracy (in percentage) over 10 repetitions
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.894
    at_pub_std: 0.056
    at_pub_source_arxiv: '1905.11136'
    at_pub_source_title: Provably Powerful Graph Networks
    at_pub_source_date_iso: '2019-05-27'
    at_pub_source_date_label: NeurIPS 2019
    value_gap_source_date_iso: '2021-12-02'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.933
    true_std: 0.029
    value_gap_source_arxiv: '2112.00911'
    value_gap_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.039000000000000035
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.029
    global_rank: 43
    paper_rank: 254
    rank_delta: 211
    rank_delta_abs: 211
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PatchySan
    model_key: patchysan
    model_plain: PatchySan
    value: 0.9158
    std: null
    paper_value: 0.9158
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: mean test accuracy (in percentage) over 10 repetitions
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.926
    at_pub_std: 0.042
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.010200000000000098
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.926
    true_std: 0.042
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: false
    value_gap: 0.010200000000000098
    has_value_note: false
    value_note: ''
    sort_value: 0.926
    sort_std: 0.042
    global_rank: 61
    paper_rank: 96
    rank_delta: 35
    rank_delta_abs: 35
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
    value: 0.922
    std: 0.044
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_display: Mar 2025
    date_iso: '2025-03-03'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 71
    sort_value: 0.922
    sort_std: 0.044
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FGConv-Sum
    model_key: fgconv-sum
    model_plain: FGConv-Sum
    value: 0.908
    std: 0.025
    paper_value: 0.908
    paper_std: 0.025
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
    protocol_note: mean test accuracy (in percentage) over 10 repetitions
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-12'
    value_gap_source_date_label: JMLR 2020
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.908
    true_std: 0.025
    value_gap_source_arxiv: '2012.06922'
    value_gap_source_title: Decimated Framelet System on Graphs and Fast $ $-Framelet
      Transforms
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.908
    sort_std: 0.025
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
  - model: WL
    model_key: wl
    model_plain: WL
    value: 0.8072
    std: null
    paper_value: 0.8072
    paper_std: null
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
    source_ref: niepert2016learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: mean test accuracy (in percentage) over 10 repetitions
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.904
    at_pub_std: 0.057
    at_pub_source_arxiv: '1912.06058'
    at_pub_source_title: Coloring graph neural networks for node disambiguation
    at_pub_source_date_iso: '2019-12-12'
    at_pub_source_date_label: IJCAI 2019
    value_gap_source_date_iso: '2023-05-23'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.0968
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.904
    true_std: 0.057
    value_gap_source_arxiv: '2305.13987'
    value_gap_source_title: On Structural Expressive Power of Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.0968
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: 0.057
    global_rank: 171
    paper_rank: 659
    rank_delta: 488
    rank_delta_abs: 488
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Coloring graph neural networks for node disambiguation
    comparison_source_arxiv: '1912.06058'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.866
    std: 0.0495
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.04319'
    title: Breaking the Limits of Message Passing Graph Neural Networks
    date: Jun 8, 2021
    date_display: Jun 2021
    date_iso: '2021-06-08'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/balcilar/gnn-matlang
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 430
    sort_value: 0.866
    sort_std: 0.0495
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.8583
    std: null
    paper_value: 0.8583
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: mean test accuracy (in percentage) over 10 repetitions
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.8583
    at_pub_std: null
    at_pub_source_arxiv: '1901.08296'
    at_pub_source_title: 'Deep Learning on Attributed Graphs: A Journey from Graphs
      to Their Embeddings and Back'
    at_pub_source_date_iso: '2018-12-14'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8583
    true_std: 0.0116
    value_gap_source_arxiv: '2412.17856'
    value_gap_source_title: Graph Structure Refinement with Energy-based Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8583
    sort_std: 0.0116
    global_rank: 455
    paper_rank: 455
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SP
    model_key: sp
    model_plain: SP
    value: 0.8579
    std: null
    paper_value: 0.8579
    paper_std: null
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
    source_ref: niepert2016learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: mean test accuracy (in percentage) over 10 repetitions
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.858
    at_pub_std: 0.002
    at_pub_source_arxiv: '1410.3314'
    at_pub_source_title: Propagation Kernels
    at_pub_source_date_iso: '2014-10-13'
    at_pub_source_date_label: '2014'
    value_gap_source_date_iso: '2014-10-13'
    value_gap_source_date_label: '2014'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.858
    true_std: 0.002
    value_gap_source_arxiv: '1410.3314'
    value_gap_source_title: Propagation Kernels
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.858
    sort_std: 0.002
    global_rank: 456
    paper_rank: 460
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RW
    model_key: rw
    model_plain: RW
    value: 0.8368
    std: null
    paper_value: 0.8368
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: niepert2016learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: mean test accuracy (in percentage) over 10 repetitions
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.8368
    at_pub_std: 0.0166
    at_pub_source_arxiv: '1605.05273'
    at_pub_source_title: Learning Convolutional Neural Networks for Graphs
    at_pub_source_date_iso: '2016-05-17'
    at_pub_source_date_label: ICML 2016
    value_gap_source_date_iso: '2021-03-24'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.837
    true_std: 0.015
    value_gap_source_arxiv: '2103.13125'
    value_gap_source_title: Learning Graph Representation by Aggregating Subgraphs
      via Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.837
    sort_std: 0.015
    global_rank: 553
    paper_rank: 556
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Graphlet
    model_key: graphlet
    model_plain: Graphlet
    value: 0.8158
    std: null
    paper_value: 0.8158
    paper_std: null
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
    source_ref: niepert2016learning
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: mean test accuracy (in percentage) over 10 repetitions
    date: Dec 12, 2020
    date_display: Dec 2020
    date_iso: '2020-12-12'
    published_venue: JMLR 2020
    published_conference: JMLR 2020
    at_pub_value: 0.8244
    at_pub_std: 0.0129
    at_pub_source_arxiv: '1603.06186'
    at_pub_source_title: The Multiscale Laplacian Graph Kernel
    at_pub_source_date_iso: '2016-03-01'
    at_pub_source_date_label: NeurIPS 2016
    value_gap_source_date_iso: '2018-01-07'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: 0.008600000000000052
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8244
    true_std: 0.0129
    value_gap_source_arxiv: '1801.02144'
    value_gap_source_title: Covariant Compositional Networks for Learning Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.008600000000000052
    has_value_note: false
    value_note: ''
    sort_value: 0.8244
    sort_std: 0.0129
    global_rank: 607
    paper_rank: 641
    rank_delta: 34
    rank_delta_abs: 34
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
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: D&D
      dataset_slug: d-d
single_proposed_model: FGConv-Sum
main_figure: /figures/2012.06922/main_figure.jpegoptim.jpg
---

