---
title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
arxiv_id: '2404.04559'
source_url: ''
authors:
- name: Guoming Li
  orcid: null
  s2_author_id: '2295700674'
  s2_url: null
- name: Jian Yang
  orcid: null
  s2_author_id: '2295684729'
  s2_url: null
- name: Shangsong Liang
  orcid: null
  s2_author_id: '2295682615'
  s2_url: null
- name: Dongsheng Luo
  orcid: null
  s2_author_id: '2295654854'
  s2_url: null
published_date: Apr 6, 2024
published_date_iso: '2024-04-06'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Spectral Graph Neural Networks (GNNs) have achieved tremendous success in
  graph learning. As an essential part of spectral GNNs, spectral graph convolution
  extracts crucial frequency information in graph data, leading to superior performance
  of spectral GNNs in downstream tasks. However, in this paper, we show that existing
  spectral GNNs remain critical drawbacks in performing the spectral graph convolution.
  Specifically, considering the spectral graph convolution as a construction operation
  towards target output, we prove that existing popular convolution paradigms cannot
  construct the target output with mild conditions on input graph signals, causing
  spectral GNNs to fall into suboptimal solutions. To address the issues, we rethink
  the spectral graph convolution from a more general two-dimensional (2-D) signal
  convolution perspective and propose a new convolution paradigm, named 2-D graph
  convolution. We prove that 2-D graph convolution unifies existing graph convolution
  paradigms, and is capable to construct arbitrary target output. Based on the proposed
  2-D graph convolution, we further propose ChebNet2D, an efficient and effective
  GNN implementation of 2-D graph convolution through applying Chebyshev interpolation.
  Extensive experiments on benchmark datasets demonstrate both effectiveness and efficiency
  of the ChebNet2D.
codebase_url: https://github.com/jianhao2016/GPRGNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- ChebNet2D
mrr: 0.2656
adjusted_mrr: 0.2656
mrr_dataset_count: 4
benchmark_categories:
- Classic
- Heterophily Benchmark
- LINKX Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 2
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
  - model: H2GCN
    model_key: h2gcn + unigap
    model_plain: H2GCN
    value: 0.6375
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    input_feature_source: null
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
  - model: H2GCN
    model_key: graphsage + unigap
    model_plain: H2GCN
    value: 0.6283
    std: 0.009
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6283
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN
    model_key: gcn + unigap
    model_plain: H2GCN
    value: 0.5976
    std: 0.008
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
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
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.5976
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.4738
    std: 0.004
    paper_value: 0.4738
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Amazon-ratings dataset
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
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
    gap_vs_at_pub: 0.01319999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.06730000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.5411
    sort_std: 0.0034
    global_rank: 26
    paper_rank: 129
    rank_delta: 103
    rank_delta_abs: 103
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.5113
    std: 0.006
    paper_value: 0.5113
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Amazon-ratings dataset
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5268
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-14'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.01550000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5268
    true_std: 0.0026
    value_gap_source_arxiv: '2202.07082'
    value_gap_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.01550000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.5268
    sort_std: 0.0026
    global_rank: 57
    paper_rank: 80
    rank_delta: 23
    rank_delta_abs: 23
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
    is_best: false
    is_std_outlier: false
  - model: ChebNet2D
    model_key: chebnet2d
    model_plain: ChebNet2D
    value: 0.5077
    std: 0.003
    paper_value: 0.5077
    paper_std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Amazon-ratings dataset
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5077
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5077
    sort_std: 0.003
    global_rank: 88
    paper_rank: 88
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
    value: 0.4988
    std: 0.004
    paper_value: 0.4988
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Amazon-ratings dataset
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3728
    at_pub_std: 0.0066
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.126
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4988
    true_std: 0.004
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4988
    sort_std: 0.004
    global_rank: 104
    paper_rank: 104
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.4956
    std: 0.004
    paper_value: 0.4956
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Amazon-ratings dataset
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4488
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.04680000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4956
    true_std: 0.004
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4956
    sort_std: 0.004
    global_rank: 107
    paper_rank: 107
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: OptBasis
    model_key: optbasis
    model_plain: OptBasis
    value: 0.4948
    std: 0.003
    paper_value: 0.4948
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Amazon-ratings dataset
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4948
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4948
    sort_std: 0.003
    global_rank: 110
    paper_rank: 110
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.4943
    std: 0.004
    paper_value: 0.4943
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Amazon-ratings dataset
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4943
    true_std: 0.004
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4943
    sort_std: 0.004
    global_rank: 111
    paper_rank: 111
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Spec-GN*
    model_key: spec-gn
    model_plain: Spec-GN*
    value: 0.4862
    std: 0.008
    paper_value: 0.4862
    paper_std: 0.008
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Amazon-ratings dataset; Spec-GN* is re-implemented
      with unified decoupling architecture
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4862
    true_std: 0.008
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4862
    sort_std: 0.008
    global_rank: 117
    paper_rank: 117
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
    value: 0.4856
    std: 0.002
    paper_value: 0.4856
    paper_std: 0.002
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Amazon-ratings dataset
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4355
    at_pub_std: 0.0048
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05009999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4856
    true_std: 0.002
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4856
    sort_std: 0.002
    global_rank: 118
    paper_rank: 118
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Evolving Computation Graphs
    comparison_source_arxiv: '2306.12943'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.4841
    std: 0.003
    paper_value: 0.4841
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Amazon-ratings dataset
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4841
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4841
    sort_std: 0.003
    global_rank: 119
    paper_rank: 119
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.4548
    std: 0.005
    paper_value: 0.4548
    paper_std: 0.005
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Amazon-ratings dataset
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4386
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.016199999999999992
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4548
    true_std: 0.005
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4548
    sort_std: 0.005
    global_rank: 145
    paper_rank: 145
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
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
  dataset: Cora
  rows:
  - model: SGC+TSC
    model_key: exphormer
    model_plain: SGC+TSC
    value: 0.9635
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9635
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: sgformer
    model_plain: SGC+TSC
    value: 0.9629
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9629
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGC+TSC
    model_key: coral
    model_plain: SGC+TSC
    value: 0.9574
    std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9574
    sort_std: 0.0039
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNet2D
    model_key: chebnet2d
    model_plain: ChebNet2D
    value: 0.9124
    std: 0.009
    paper_value: 0.9124
    paper_std: 0.009
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9124
    true_std: 0.009
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9124
    sort_std: 0.009
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8668
    std: 0.016
    paper_value: 0.8668
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.03359999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9004
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.03359999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 33
    paper_rank: 225
    rank_delta: 192
    rank_delta_abs: 192
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: BernNet
    model_key: bernnet
    model_plain: BernNet
    value: 0.8922
    std: 0.015
    paper_value: 0.8922
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8976
    at_pub_std: 0.016
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.00539999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8976
    true_std: 0.016
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.00539999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8976
    sort_std: 0.016
    global_rank: 41
    paper_rank: 60
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.8941
    std: 0.007
    paper_value: 0.8941
    paper_std: 0.007
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.892
    at_pub_std: 0.016
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0020999999999999908
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8941
    true_std: 0.007
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8941
    sort_std: 0.007
    global_rank: 52
    paper_rank: 52
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OptBasis
    model_key: optbasis
    model_plain: OptBasis
    value: 0.8933
    std: 0.007
    paper_value: 0.8933
    paper_std: 0.007
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8933
    true_std: 0.007
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8933
    sort_std: 0.007
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
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.8932
    std: 0.011
    paper_value: 0.8932
    paper_std: 0.011
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8871
    at_pub_std: 0.0093
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.006099999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8932
    true_std: 0.011
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8932
    sort_std: 0.011
    global_rank: 57
    paper_rank: 57
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.8894
    std: 0.011
    paper_value: 0.8894
    paper_std: 0.011
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8904
    at_pub_std: 0.015
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-16'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0010000000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8904
    true_std: 0.015
    value_gap_source_arxiv: '2310.10064'
    value_gap_source_title: Shape-aware Graph Spectral Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0010000000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.8904
    sort_std: 0.015
    global_rank: 69
    paper_rank: 72
    rank_delta: 3
    rank_delta_abs: 3
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
    value: 0.8851
    std: 0.012
    paper_value: 0.8851
    paper_std: 0.012
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8893
    at_pub_std: 0.0137
    at_pub_source_arxiv: '2308.07134'
    at_pub_source_title: Language is All a Graph Needs
    at_pub_source_date_iso: '2023-08-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-08-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0041999999999999815
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8893
    true_std: 0.0137
    value_gap_source_arxiv: '2308.07134'
    value_gap_source_title: Language is All a Graph Needs
    value_gap_source_is_current_paper: false
    value_gap: 0.0041999999999999815
    has_value_note: false
    value_note: ''
    sort_value: 0.8893
    sort_std: 0.0137
    global_rank: 74
    paper_rank: 101
    rank_delta: 27
    rank_delta_abs: 27
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNN-HF/LF
    model_key: gnn-hf/lf
    model_plain: GNN-HF/LF
    value: 0.8891
    std: 0.008
    paper_value: 0.8891
    paper_std: 0.008
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8891
    true_std: 0.008
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8891
    sort_std: 0.008
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
  - model: PDE-GCN
    model_key: pde-gcn
    model_plain: PDE-GCN
    value: 0.8879
    std: 0.011
    paper_value: 0.8879
    paper_std: 0.011
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.886
    at_pub_std: null
    at_pub_source_arxiv: '2307.16092'
    at_pub_source_title: Feature Transportation Improves Graph Neural Networks
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0019000000000000128
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8879
    true_std: 0.011
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8879
    sort_std: 0.011
    global_rank: 85
    paper_rank: 85
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.8853
    std: 0.012
    paper_value: 0.8853
    paper_std: 0.012
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8833
    at_pub_std: 0.0109
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8853
    true_std: 0.012
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8853
    sort_std: 0.012
    global_rank: 101
    paper_rank: 101
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DSGC
    model_key: dsgc
    model_plain: DSGC
    value: 0.8851
    std: 0.013
    paper_value: 0.8851
    paper_std: 0.013
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8851
    true_std: 0.013
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8851
    sort_std: 0.013
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
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.8773
    std: 0.013
    paper_value: 0.8773
    paper_std: 0.013
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8848
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2401.15569'
    at_pub_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    at_pub_source_date_iso: '2024-01-28'
    at_pub_source_date_label: IJCAI 2024
    value_gap_source_date_iso: '2024-01-28'
    value_gap_source_date_label: IJCAI 2024
    gap_vs_at_pub: 0.007500000000000062
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8848
    true_std: 0.0033
    value_gap_source_arxiv: '2401.15569'
    value_gap_source_title: Efficient Tuning and Inference for Large Language Models
      on Textual Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.007500000000000062
    has_value_note: false
    value_note: ''
    sort_value: 0.8848
    sort_std: 0.0033
    global_rank: 105
    paper_rank: 155
    rank_delta: 50
    rank_delta_abs: 50
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ADC
    model_key: adc
    model_plain: ADC
    value: 0.8843
    std: 0.007
    paper_value: 0.8843
    paper_std: 0.007
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Planetoid split (Yang et al. 2016 fixed 20-per-class
      train split).
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8843
    true_std: 0.007
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8843
    sort_std: 0.007
    global_rank: 106
    paper_rank: 106
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
- &id004
  dataset: Penn94
  rows:
  - model: ChebNet2D
    model_key: chebnet2d
    model_plain: ChebNet2D
    value: 0.8762
    std: 0.002
    paper_value: 0.8762
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Penn94 test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8762
    true_std: 0.002
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8762
    sort_std: 0.002
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
  - model: GloGNN
    model_key: dc-gnn
    model_plain: GloGNN
    value: 0.8669
    std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.16185'
    title: Differentiable Cluster Graph Neural Network
    date: May 25, 2024
    date_display: May 2024
    date_iso: '2024-05-25'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8669
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: m2m-gnn
    model_plain: GloGNN
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
    input_feature_source: null
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
    value: 0.8554
    std: 0.003
    paper_value: 0.8554
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Penn94 test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8574
    at_pub_std: 0.0042
    at_pub_source_arxiv: '2312.14438'
    at_pub_source_title: 'PC-Conv: Unifying Homophily and Heterophily with Two-fold
      Filtering'
    at_pub_source_date_iso: '2023-12-22'
    at_pub_source_date_label: AAAI 2023
    value_gap_source_date_iso: '2023-12-22'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8574
    true_std: 0.0042
    value_gap_source_arxiv: '2312.14438'
    value_gap_source_title: 'PC-Conv: Unifying Homophily and Heterophily with Two-fold
      Filtering'
    value_gap_source_is_current_paper: false
    value_gap: 0.0020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.8574
    sort_std: 0.0042
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.8522
    std: 0.003
    paper_value: 0.8522
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Penn94 test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8486
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0035999999999999366
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8522
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8522
    sort_std: 0.003
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.8515
    std: 0.002
    paper_value: 0.8515
    paper_std: 0.002
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Penn94 test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8471
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0044000000000000705
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8515
    true_std: 0.002
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8515
    sort_std: 0.002
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OptBasis
    model_key: optbasis
    model_plain: OptBasis
    value: 0.8482
    std: 0.006
    paper_value: 0.8482
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Penn94 test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8482
    true_std: 0.006
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8482
    sort_std: 0.006
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
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.8387
    std: 0.006
    paper_value: 0.8387
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Penn94 test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8455
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.006800000000000028
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.8455
    true_std: 0.0054
    value_gap_source_arxiv: '2306.02285'
    value_gap_source_title: Clarify Confused Nodes via Separated Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.006800000000000028
    has_value_note: false
    value_note: ''
    sort_value: 0.8455
    sort_std: 0.0054
    global_rank: 15
    paper_rank: 18
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.8371
    std: 0.003
    paper_value: 0.8371
    paper_std: 0.003
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Penn94 test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8371
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8371
    sort_std: 0.003
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8247
    std: 0.003
    paper_value: 0.8247
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Penn94 test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
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
    global_rank: 25
    paper_rank: 32
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Shape-aware Graph Spectral Learning
    comparison_source_arxiv: '2310.10064'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.7768
    std: 0.004
    paper_value: 0.7768
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Penn94 test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7591
    at_pub_std: 0.002
    at_pub_source_arxiv: '2310.10064'
    at_pub_source_title: Shape-aware Graph Spectral Learning
    at_pub_source_date_iso: '2023-10-16'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.01770000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7768
    true_std: 0.004
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: 0.004
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Shape-aware Graph Spectral Learning
    comparison_source_arxiv: '2310.10064'
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
- &id002
  dataset: Roman-empire
  rows:
  - model: GPS + Mamba
    model_key: dir-nt
    model_plain: GPS + Mamba
    value: 0.9477
    std: 0.0031
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2604.08980'
    title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware Graph
      Learning'
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    venue: arXiv.org
    codebase_url: https://github.com/cf020031308/MoNT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9477
    sort_std: 0.0031
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS + Mamba
    model_key: dir-poly
    model_plain: GPS + Mamba
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
    global_rank: 2
    sort_value: 0.9451
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS + Mamba
    model_key: largescalenet
    model_plain: GPS + Mamba
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
    input_feature_source: null
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5578
    std: 0.004
    paper_value: 0.5578
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Roman-empire test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7369
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.17910000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7882
    true_std: 0.0009
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.23040000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.7882
    sort_std: 0.0009
    global_rank: 99
    paper_rank: 175
    rank_delta: 76
    rank_delta_abs: 76
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
    is_best: false
    is_std_outlier: false
  - model: ChebNet2D
    model_key: chebnet2d
    model_plain: ChebNet2D
    value: 0.7718
    std: 0.005
    paper_value: 0.7718
    paper_std: 0.005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Roman-empire test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7718
    true_std: 0.005
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7718
    sort_std: 0.005
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
    is_std_outlier: false
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.7342
    std: 0.006
    paper_value: 0.7342
    paper_std: 0.006
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Roman-empire test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6449
    at_pub_std: 0.0073
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.08929999999999993
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7483
    true_std: 0.0081
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.014100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7483
    sort_std: 0.0081
    global_rank: 112
    paper_rank: 120
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.7458
    std: 0.003
    paper_value: 0.7458
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Roman-empire test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7458
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7458
    sort_std: 0.003
    global_rank: 113
    paper_rank: 113
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
    value: 0.7435
    std: 0.006
    paper_value: 0.7435
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Roman-empire test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7114
    at_pub_std: 0.0042
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03210000000000002
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7435
    true_std: 0.006
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7435
    sort_std: 0.006
    global_rank: 116
    paper_rank: 116
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Evolving Computation Graphs
    comparison_source_arxiv: '2306.12943'
    is_best: false
    is_std_outlier: false
  - model: OptBasis
    model_key: optbasis
    model_plain: OptBasis
    value: 0.7429
    std: 0.003
    paper_value: 0.7429
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Roman-empire test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7429
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7429
    sort_std: 0.003
    global_rank: 118
    paper_rank: 118
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.7344
    std: 0.003
    paper_value: 0.7344
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Roman-empire test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6485
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.08590000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7344
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7344
    sort_std: 0.003
    global_rank: 120
    paper_rank: 120
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.7274
    std: 0.006
    paper_value: 0.7274
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Roman-empire test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7274
    true_std: 0.006
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7274
    sort_std: 0.006
    global_rank: 122
    paper_rank: 122
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Spec-GN
    model_key: spec-gn
    model_plain: Spec-GN
    value: 0.7129
    std: 0.006
    paper_value: 0.7129
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Roman-empire test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7129
    true_std: 0.006
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7129
    sort_std: 0.006
    global_rank: 128
    paper_rank: 128
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
    value: 0.6739
    std: 0.003
    paper_value: 0.6739
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Roman-empire test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6385
    at_pub_std: 0.0049
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0354000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6739
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6739
    sort_std: 0.003
    global_rank: 138
    paper_rank: 138
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.6481
    std: 0.008
    paper_value: 0.6481
    paper_std: 0.008
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Roman-empire test split
    date: Apr 6, 2024
    date_display: Apr 2024
    date_iso: '2024-04-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5914
    at_pub_std: 0.0045
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05669999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6481
    true_std: 0.008
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6481
    sort_std: 0.008
    global_rank: 150
    paper_rank: 150
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    comparison_source_arxiv: '2202.07082'
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
- benchmark: Heterophily Benchmark
  datasets:
  - *id002
  - *id003
- benchmark: LINKX Benchmarks
  datasets:
  - *id004
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Roman-empire
      dataset_slug: roman-empire
    - dataset: Amazon-ratings
      dataset_slug: amazon-ratings
  - benchmark: LINKX Benchmarks
    benchmark_slug: linkx-benchmarks
    datasets:
    - dataset: Penn94
      dataset_slug: penn94
single_proposed_model: ChebNet2D
main_figure: /figures/2404.04559/main_figure.jpegoptim.jpg
---

