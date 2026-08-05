---
title: A Signed Graph Approach to Understanding and Mitigating Oversmoothing in GNNs
arxiv_id: '2502.11394'
source_url: ''
authors:
- name: Jiaqi Wang
  orcid: null
  s2_author_id: '2279755273'
  s2_url: null
- name: Xinyi Wu
  orcid: null
  s2_author_id: '2180639386'
  s2_url: null
- name: James Cheng
  orcid: null
  s2_author_id: '2345867993'
  s2_url: null
- name: Yifei Wang
  orcid: null
  s2_author_id: '2345821544'
  s2_url: null
published_date: Feb 17, 2025
published_date_iso: '2025-02-17'
published_venue: NeurIPS 2025
published_conference: NeurIPS 2025
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Deep graph neural networks (GNNs) often suffer from oversmoothing, where
  node representations become overly homogeneous with increasing depth. While techniques
  like normalization, residual connections, and edge dropout have been proposed to
  mitigate oversmoothing, they are typically developed independently, with limited
  theoretical understanding of their underlying mechanisms. In this work, we present
  a unified theoretical perspective based on the framework of signed graphs, showing
  that many existing strategies implicitly introduce negative edges that alter message-passing
  to resist oversmoothing. However, we show that merely adding negative edges in an
  unstructured manner is insufficient—the asymptotic behavior of signed propagation
  depends critically on the strength and organization of positive and negative edges.
  To address this limitation, we leverage the theory of structural balance, which
  promotes stable, cluster-preserving dynamics by connecting similar nodes with positive
  edges and dissimilar ones with negative edges. We propose Structural Balanced Propagation
  (SBP), a plug-and-play method that assigns signed edges based on either labels or
  feature similarity to explicitly enhance structural balance in the constructed signed
  graphs. Experiments on nine benchmarks across both homophilic and heterophilic settings
  demonstrate that SBP consistently improves classification accuracy and mitigates
  oversmoothing, even at depths of up to 300 layers. Our results provide a principled
  explanation for prior oversmoothing remedies and introduce a new direction for signed
  message-passing design in deep GNNs.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- OGB
- Heterophilic Graphs
- Heterophily Benchmark
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 2
  total: 6
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 1
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id004
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
    is_std_outlier: true
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
    is_std_outlier: true
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
    is_std_outlier: true
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.4283
    std: 0.0004
    paper_value: 0.4283
    paper_std: 0.0004
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.5066
    at_pub_std: 0.0048
    at_pub_source_arxiv: '2407.18480'
    at_pub_source_title: Scalable Graph Compressed Convolutions
    at_pub_source_date_iso: '2024-07-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.07830000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5066
    true_std: 0.0048
    value_gap_source_arxiv: '2407.18480'
    value_gap_source_title: Scalable Graph Compressed Convolutions
    value_gap_source_is_current_paper: false
    value_gap: 0.07830000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.5066
    sort_std: 0.0048
    global_rank: 92
    paper_rank: 173
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Scalable Graph Compressed Convolutions
    comparison_source_arxiv: '2407.18480'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.3814
    std: 0.0003
    paper_value: 0.3814
    paper_std: 0.0003
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.5058
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.12440000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5058
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.12440000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.5058
    sort_std: null
    global_rank: 93
    paper_rank: 183
    rank_delta: 90
    rank_delta_abs: 90
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.4247
    std: 0.0003
    paper_value: 0.4247
    paper_std: 0.0003
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.4841
    at_pub_std: 0.003
    at_pub_source_arxiv: '2404.04559'
    at_pub_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    at_pub_source_date_iso: '2024-04-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05939999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4841
    true_std: 0.003
    value_gap_source_arxiv: '2404.04559'
    value_gap_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    value_gap_source_is_current_paper: false
    value_gap: 0.05939999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.4841
    sort_std: 0.003
    global_rank: 119
    paper_rank: 176
    rank_delta: 57
    rank_delta_abs: 57
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: ContraNorm
    model_key: contranorm
    model_plain: ContraNorm
    value: 0.4298
    std: 0.0004
    paper_value: 0.4298
    paper_std: 0.0004
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.4298
    sort_std: 0.0004
    global_rank: 173
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Residual
    model_key: residual
    model_plain: Residual
    value: 0.4269
    std: 0.0003
    paper_value: 0.4269
    paper_std: 0.0003
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.4269
    sort_std: 0.0003
    global_rank: 177
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Label-SBP
    model_key: label-sbp
    model_plain: Label-SBP
    value: 0.4241
    std: 0.0002
    paper_value: 0.4241
    paper_std: 0.0002
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.4241
    sort_std: 0.0002
    global_rank: 177
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Feature-SBP
    model_key: feature-sbp
    model_plain: Feature-SBP
    value: 0.4231
    std: 0.0003
    paper_value: 0.4231
    paper_std: 0.0003
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.4231
    sort_std: 0.0003
    global_rank: 177
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PairNorm
    model_key: pairnorm
    model_plain: PairNorm
    value: 0.423
    std: 0.0005
    paper_value: 0.423
    paper_std: 0.0005
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.423
    sort_std: 0.0005
    global_rank: 177
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DropEdge
    model_key: dropedge
    model_plain: DropEdge
    value: 0.423
    std: 0.0009
    paper_value: 0.423
    paper_std: 0.0009
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.423
    sort_std: 0.0009
    global_rank: 177
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.4221
    std: 0.0005
    paper_value: 0.4221
    paper_std: 0.0005
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.4221
    sort_std: 0.0005
    global_rank: 177
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.4061
    std: 0.0003
    paper_value: 0.4061
    paper_std: 0.0003
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.4061
    sort_std: 0.0003
    global_rank: 179
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BatchNorm
    model_key: batchnorm
    model_plain: BatchNorm
    value: 0.3968
    std: 0.0001
    paper_value: 0.3968
    paper_std: 0.0001
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.3968
    sort_std: 0.0001
    global_rank: 182
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
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
- &id003
  dataset: Cornell
  rows:
  - model: R-SoftGraphAIN
    model_key: p^2gnn
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: acm-gcn
    model_plain: R-SoftGraphAIN
    value: 0.948
    std: 0.038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.19785'
    title: Heterophily-informed Message Passing
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/AaltoML/heterophily-imp
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.948
    sort_std: 0.038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: rf-gcn
    model_plain: R-SoftGraphAIN
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
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.6459
    std: 0.033
    paper_value: 0.6459
    paper_std: 0.033
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.9181
    at_pub_std: 0.0196
    at_pub_source_arxiv: '2303.13750'
    at_pub_source_title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
    at_pub_source_date_iso: '2023-03-24'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-24'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.2722
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9181
    true_std: 0.0196
    value_gap_source_arxiv: '2303.13750'
    value_gap_source_title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
    value_gap_source_is_current_paper: false
    value_gap: 0.2722
    has_value_note: false
    value_note: ''
    sort_value: 0.9181
    sort_std: 0.0196
    global_rank: 20
    paper_rank: 352
    rank_delta: 332
    rank_delta_abs: 332
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
    comparison_source_arxiv: '2303.13750'
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6811
    std: 0.0265
    paper_value: 0.6811
    paper_std: 0.0265
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.9136
    at_pub_std: 0.007
    at_pub_source_arxiv: '2212.03654'
    at_pub_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.23249999999999993
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
    value_gap: 0.23249999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.9136
    sort_std: 0.007
    global_rank: 25
    paper_rank: 319
    rank_delta: 294
    rank_delta_abs: 294
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    comparison_source_arxiv: '2212.03654'
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.3973
    std: 0.0272
    paper_value: 0.3973
    paper_std: 0.0272
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.8878
    at_pub_std: null
    at_pub_source_arxiv: '2406.12539'
    at_pub_source_title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering
      GNNs for Heterophilic Graphs'
    at_pub_source_date_iso: '2024-06-18'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-06-18'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.49050000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8878
    true_std: null
    value_gap_source_arxiv: '2406.12539'
    value_gap_source_title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering
      GNNs for Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.49050000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8878
    sort_std: null
    global_rank: 47
    paper_rank: 568
    rank_delta: 521
    rank_delta_abs: 521
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'The Heterophilic Snowflake Hypothesis: Training and
      Empowering GNNs for Heterophilic Graphs'
    comparison_source_arxiv: '2406.12539'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.4487
    std: 0.0324
    paper_value: 0.4487
    paper_std: 0.0324
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.7351
    at_pub_std: 0.0718
    at_pub_source_arxiv: '2211.11761'
    at_pub_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    at_pub_source_date_iso: '2022-11-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-11-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.2864
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7351
    true_std: 0.0718
    value_gap_source_arxiv: '2211.11761'
    value_gap_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.2864
    has_value_note: false
    value_note: ''
    sort_value: 0.7351
    sort_std: 0.0718
    global_rank: 273
    paper_rank: 536
    rank_delta: 263
    rank_delta_abs: 263
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    comparison_source_arxiv: '2211.11761'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.4811
    std: 0.0315
    paper_value: 0.4811
    paper_std: 0.0315
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.735
    at_pub_std: 0.043
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.25389999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.735
    true_std: 0.043
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.25389999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.735
    sort_std: 0.043
    global_rank: 275
    paper_rank: 521
    rank_delta: 246
    rank_delta_abs: 246
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: Feature-SBP
    model_key: feature-sbp
    model_plain: Feature-SBP
    value: 0.7297
    std: 0.0
    paper_value: 0.7297
    paper_std: 0.0
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.7297
    sort_std: 0.0
    global_rank: 278
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Label-SBP
    model_key: label-sbp
    model_plain: Label-SBP
    value: 0.7027
    std: 0.0
    paper_value: 0.7027
    paper_std: 0.0
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.7027
    sort_std: 0.0
    global_rank: 305
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Residual
    model_key: residual
    model_plain: Residual
    value: 0.6189
    std: 0.0391
    paper_value: 0.6189
    paper_std: 0.0391
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6189
    sort_std: 0.0391
    global_rank: 377
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DropEdge
    model_key: dropedge
    model_plain: DropEdge
    value: 0.4595
    std: 0.0705
    paper_value: 0.4595
    paper_std: 0.0705
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.6054
    at_pub_std: 0.053
    at_pub_source_arxiv: '2310.16401'
    at_pub_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    at_pub_source_date_iso: '2023-10-25'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.14590000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6054
    true_std: 0.053
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.14590000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.6054
    sort_std: 0.053
    global_rank: 391
    paper_rank: 532
    rank_delta: 141
    rank_delta_abs: 141
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    comparison_source_arxiv: '2310.16401'
    is_best: false
    is_std_outlier: false
  - model: PairNorm
    model_key: pairnorm
    model_plain: PairNorm
    value: 0.5135
    std: 0.0
    paper_value: 0.5135
    paper_std: 0.0
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.5892
    at_pub_std: 0.0315
    at_pub_source_arxiv: '2206.10991'
    at_pub_source_title: Understanding convolution on graphs via energies
    at_pub_source_date_iso: '2022-06-22'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.07569999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5892
    true_std: null
    value_gap_source_arxiv: '2406.10863'
    value_gap_source_title: Global-Local Graph Neural Networks for Node-Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.07569999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.5892
    sort_std: null
    global_rank: 409
    paper_rank: 496
    rank_delta: 87
    rank_delta_abs: 87
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding convolution on graphs via energies
    comparison_source_arxiv: '2206.10991'
    is_best: false
    is_std_outlier: false
  - model: ContraNorm
    model_key: contranorm
    model_plain: ContraNorm
    value: 0.4863
    std: 0.0016
    paper_value: 0.4863
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.4863
    sort_std: 0.0016
    global_rank: 520
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BatchNorm
    model_key: batchnorm
    model_plain: BatchNorm
    value: 0.4649
    std: 0.0108
    paper_value: 0.4649
    paper_std: 0.0108
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.4649
    sort_std: 0.0108
    global_rank: 530
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
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
- &id002
  dataset: Texas
  rows:
  - model: R-SoftGraphAIN
    model_key: p^2gnn
    model_plain: R-SoftGraphAIN
    value: 0.9672
    std: 0.0147
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
    sort_value: 0.9672
    sort_std: 0.0147
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: dog
    model_plain: R-SoftGraphAIN
    value: 0.966
    std: 0.021
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: true
    input_feature_source: raw_features
    feature_source_evidence: DoG generates synthetic graph structures to boost the
      performance of GNNs.
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: gpf-plus
    model_plain: R-SoftGraphAIN
    value: 0.9583
    std: 0.0419
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.05346'
    title: 'ProG: A Graph Prompt Learning Benchmark'
    date: Jun 8, 2024
    date_display: Jun 2024
    date_iso: '2024-06-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/sheldonresearch/ProG
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9583
    sort_std: 0.0419
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7351
    std: 0.0236
    paper_value: 0.7351
    paper_std: 0.0236
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.923
    at_pub_std: 0.007
    at_pub_source_arxiv: '2401.14580'
    at_pub_source_title: 'Design your own universe: a physics-informed agnostic method
      for enhancing graph neural networks'
    at_pub_source_date_iso: '2024-01-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-01-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.18790000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.923
    true_std: 0.007
    value_gap_source_arxiv: '2401.14580'
    value_gap_source_title: 'Design your own universe: a physics-informed agnostic
      method for enhancing graph neural networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.18790000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.923
    sort_std: 0.007
    global_rank: 43
    paper_rank: 380
    rank_delta: 337
    rank_delta_abs: 337
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Design your own universe: a physics-informed agnostic
      method for enhancing graph neural networks'
    comparison_source_arxiv: '2401.14580'
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.6838
    std: 0.0437
    paper_value: 0.6838
    paper_std: 0.0437
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.9131
    at_pub_std: 0.0197
    at_pub_source_arxiv: '2310.11762'
    at_pub_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    at_pub_source_date_iso: '2023-10-18'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.22930000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9131
    true_std: 0.0197
    value_gap_source_arxiv: '2310.11762'
    value_gap_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.22930000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.9131
    sort_std: 0.0197
    global_rank: 55
    paper_rank: 436
    rank_delta: 381
    rank_delta_abs: 381
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    comparison_source_arxiv: '2310.11762'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.4595
    std: 0.0
    paper_value: 0.4595
    paper_std: 0.0
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.744
    at_pub_std: 0.06
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.2845
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8131
    true_std: 0.033
    value_gap_source_arxiv: '2505.23014'
    value_gap_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in
      the Perspective of A System of Hyperbolic Partial Differential Equations'
    value_gap_source_is_current_paper: false
    value_gap: 0.3536
    has_value_note: false
    value_note: ''
    sort_value: 0.8131
    sort_std: 0.033
    global_rank: 256
    paper_rank: 630
    rank_delta: 374
    rank_delta_abs: 374
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: Feature-SBP
    model_key: feature-sbp
    model_plain: Feature-SBP
    value: 0.7838
    std: 0.0
    paper_value: 0.7838
    paper_std: 0.0
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.7838
    sort_std: 0.0
    global_rank: 310
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Label-SBP
    model_key: label-sbp
    model_plain: Label-SBP
    value: 0.7838
    std: 0.0
    paper_value: 0.7838
    paper_std: 0.0
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.7838
    sort_std: 0.0
    global_rank: 310
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JKNet
    model_key: jknet
    model_plain: JKNet
    value: 0.6
    std: 0.0236
    paper_value: 0.6
    paper_std: 0.0236
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.7751
    at_pub_std: 0.0172
    at_pub_source_arxiv: '2210.03930'
    at_pub_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    at_pub_source_date_iso: '2022-10-08'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.17510000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7751
    true_std: 0.0172
    value_gap_source_arxiv: '2210.03930'
    value_gap_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.17510000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.7751
    sort_std: 0.0172
    global_rank: 320
    paper_rank: 530
    rank_delta: 210
    rank_delta_abs: 210
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    comparison_source_arxiv: '2210.03930'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.6135
    std: 0.0173
    paper_value: 0.6135
    paper_std: 0.0173
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.7027
    at_pub_std: 0.0493
    at_pub_source_arxiv: '2211.11761'
    at_pub_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    at_pub_source_date_iso: '2022-11-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-11-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.08919999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7027
    true_std: 0.0493
    value_gap_source_arxiv: '2211.11761'
    value_gap_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.08919999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.7027
    sort_std: 0.0493
    global_rank: 415
    paper_rank: 517
    rank_delta: 102
    rank_delta_abs: 102
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    comparison_source_arxiv: '2211.11761'
    is_best: false
    is_std_outlier: false
  - model: Residual
    model_key: residual
    model_plain: Residual
    value: 0.6595
    std: 0.0132
    paper_value: 0.6595
    paper_std: 0.0132
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6595
    sort_std: 0.0132
    global_rank: 462
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PairNorm
    model_key: pairnorm
    model_plain: PairNorm
    value: 0.5135
    std: 0.0
    paper_value: 0.5135
    paper_std: 0.0
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.603
    at_pub_std: 0.043
    at_pub_source_arxiv: '2202.02296'
    at_pub_source_title: Graph-Coupled Oscillator Networks
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-02-04'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.08950000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.603
    true_std: 0.043
    value_gap_source_arxiv: '2202.02296'
    value_gap_source_title: Graph-Coupled Oscillator Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08950000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.603
    sort_std: 0.043
    global_rank: 530
    paper_rank: 611
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph-Coupled Oscillator Networks
    comparison_source_arxiv: '2202.02296'
    is_best: false
    is_std_outlier: false
  - model: DropEdge
    model_key: dropedge
    model_plain: DropEdge
    value: 0.5946
    std: 0.0811
    paper_value: 0.5946
    paper_std: 0.0811
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.592
    at_pub_std: 0.0543
    at_pub_source_arxiv: '2303.09778'
    at_pub_source_title: 'SE-GSL: A General and Effective Graph Structure Learning
      Framework through Structural Entropy Optimization'
    at_pub_source_date_iso: '2023-03-17'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-03-17'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.0026000000000000467
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.592
    true_std: 0.0543
    value_gap_source_arxiv: '2303.09778'
    value_gap_source_title: 'SE-GSL: A General and Effective Graph Structure Learning
      Framework through Structural Entropy Optimization'
    value_gap_source_is_current_paper: false
    value_gap: 0.0026000000000000467
    has_value_note: false
    value_note: ''
    sort_value: 0.592
    sort_std: 0.0543
    global_rank: 549
    paper_rank: 542
    rank_delta: -7
    rank_delta_abs: 7
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ContraNorm
    model_key: contranorm
    model_plain: ContraNorm
    value: 0.4838
    std: 0.0443
    paper_value: 0.4838
    paper_std: 0.0443
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.4838
    sort_std: 0.0443
    global_rank: 625
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BatchNorm
    model_key: batchnorm
    model_plain: BatchNorm
    value: 0.3973
    std: 0.0124
    paper_value: 0.3973
    paper_std: 0.0124
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.3973
    sort_std: 0.0124
    global_rank: 639
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
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
  dataset: ogbn-products
  rows:
  - model: LargeGT-full
    model_key: advsyngnn
    model_plain: LargeGT-full
    value: 0.8931
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.17071'
    title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial Synthesis
      and Self-Corrective Propagation'
    date: Feb 19, 2026
    date_display: Feb 2026
    date_iso: '2026-02-19'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8931
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LargeGT-full
    model_key: gofa-f
    model_plain: LargeGT-full
    value: 0.8834
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.09709'
    title: 'GOFA: A Generative One-For-All Model for Joint Graph Language Modeling'
    date: Jul 12, 2024
    date_display: Jul 2024
    date_iso: '2024-07-12'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/JiaruiFeng/GOFA
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8834
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LargeGT-full
    model_key: llms
    model_plain: LargeGT-full
    value: 0.882
    std: 0.0005
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2412.16441'
    title: 'Towards Graph Foundation Models: Learning Generalities Across Graphs via
      Task-Trees'
    date: Dec 21, 2024
    date_display: Dec 2024
    date_iso: '2024-12-21'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/Zehong-Wang/GIT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.882
    sort_std: 0.0005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7396
    std: null
    paper_value: 0.7396
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: 0.8691
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2412.16441'
    at_pub_source_title: 'Towards Graph Foundation Models: Learning Generalities Across
      Graphs via Task-Trees'
    at_pub_source_date_iso: '2024-12-21'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-12-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.12949999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8691
    true_std: 0.0005
    value_gap_source_arxiv: '2412.16441'
    value_gap_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    value_gap_source_is_current_paper: false
    value_gap: 0.12949999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8691
    sort_std: 0.0005
    global_rank: 12
    paper_rank: 296
    rank_delta: 284
    rank_delta_abs: 284
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Towards Graph Foundation Models: Learning Generalities
      Across Graphs via Task-Trees'
    comparison_source_arxiv: '2412.16441'
    is_best: false
    is_std_outlier: false
  - model: Label-SBP
    model_key: label-sbp
    model_plain: Label-SBP
    value: 0.7662
    std: null
    paper_value: 0.7662
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.7662
    sort_std: null
    global_rank: 241
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BatchNorm
    model_key: batchnorm
    model_plain: BatchNorm
    value: 0.7493
    std: null
    paper_value: 0.7493
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.7493
    sort_std: null
    global_rank: 270
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Feature-SBP
    model_key: feature-sbp
    model_plain: Feature-SBP
    value: 0.749
    std: null
    paper_value: 0.749
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 17, 2025
    date_display: Feb 2025
    date_iso: '2025-02-17'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.749
    sort_std: null
    global_rank: 273
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
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
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
- benchmark: Heterophilic Graphs
  datasets:
  - *id002
  - *id003
- benchmark: Heterophily Benchmark
  datasets:
  - *id004
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-products
      dataset_slug: ogbn-products
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Amazon-ratings
      dataset_slug: amazon-ratings
main_figure: /figures/2502.11394/main_figure.jpegoptim.jpg
---

