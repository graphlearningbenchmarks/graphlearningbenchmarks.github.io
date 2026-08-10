---
title: Learning Posterior Predictive Distributions for Node Classification from Synthetic
  Graph Priors
arxiv_id: '2604.19028'
source_url: ''
authors:
- name: Jeongwhan Choi
  orcid: null
  s2_author_id: '67027632'
  s2_url: null
- name: Jongwoo Kim
  orcid: null
  s2_author_id: '2313882839'
  s2_url: null
- name: Woo-Chang Kang
  orcid: null
  s2_author_id: '2302630380'
  s2_url: null
- name: Noseong Park
  orcid: null
  s2_author_id: '2265649308'
  s2_url: null
published_date: Apr 21, 2026
published_date_iso: '2026-04-21'
published_venue: ICLR 2026
published_conference: ICLR 2026
published_conference_short: ICLR
published_conference_slug: iclr
abstract: 'One of the most challenging problems in graph machine learning is generalizing
  across graphs with diverse properties. Graph neural networks (GNNs) face a fundamental
  limitation: they require separate training for each new graph, preventing universal
  generalization across diverse graph datasets. A critical challenge facing GNNs lies
  in their reliance on labeled training data for each individual graph, a requirement
  that hinders the capacity for universal node classification due to the heterogeneity
  inherent in graphs --- differences in homophily levels, community structures, and
  feature distributions across datasets. Inspired by the success of large language
  models (LLMs) that achieve in-context learning through massive-scale pre-training
  on diverse datasets, we introduce NodePFN. This universal node classification method
  generalizes to arbitrary graphs without graph-specific training. NodePFN learns
  posterior predictive distributions (PPDs) by training only on thousands of synthetic
  graphs generated from carefully designed priors. Our synthetic graph generation
  covers real-world graphs through the use of random networks with controllable homophily
  levels and structural causal models for complex feature-label relationships. We
  develop a dual-branch architecture combining context-query attention mechanisms
  with local message passing to enable graph-aware in-context learning. Extensive
  evaluation on 23 benchmarks demonstrates that a single pre-trained NodePFN achieves
  71.27\'
codebase_url: https://github.com/jeongwhanchoi/NodePFN
extraction_model: google/gemma-4-26B-A4B-it
has_results: true
paper_type: method
proposed_models:
- NodePFN
mrr: 0.0038
adjusted_mrr: 0.0038
mrr_dataset_count: 11
benchmark_categories:
- Classic
- Heterophilic Graphs
- Heterogeneous Graph Benchmarks
- Heterophily Benchmark
- LINKX Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 5
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 6
  total: 6
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 1
  total: 4
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 3
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
- &id008
  dataset: Actor
  rows:
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.7623
    std: 0.0042
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7623
    sort_std: 0.0042
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DiGGR
    model_key: diggr
    model_plain: DiGGR
    value: 0.4535
    std: 0.0353
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_display: Aug 2024
    date_iso: '2024-08-24'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.4535
    sort_std: 0.0353
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TRIGON
    model_key: trigon
    model_plain: TRIGON
    value: 0.4402
    std: 0.0028
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.19071'
    title: Dynamic Triangulation-Based Graph Rewiring for Graph Neural Networks
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/Hugo-Attali/TRIGON-CIKM-2025
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.4402
    sort_std: 0.0028
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.4026
    std: 0.0108
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2302.03228'
    title: Heterophily-Aware Graph Attention Network
    date: Feb 7, 2023
    date_display: Feb 2023
    date_iso: '2023-02-07'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 55
    sort_value: 0.4026
    sort_std: 0.0108
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.3394
    std: 0.0095
    paper_value: 0.3394
    paper_std: 0.0095
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
    source_ref: chien2021GPRGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using standard split (Geom-GCN 10 fixed
      splits).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.3992
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2303.13750'
    at_pub_source_title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
    at_pub_source_date_iso: '2023-03-24'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.05980000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3992
    true_std: 0.0067
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.05980000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.3992
    sort_std: 0.0067
    global_rank: 67
    paper_rank: 321
    rank_delta: 254
    rank_delta_abs: 254
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
    comparison_source_arxiv: '2303.13750'
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.3487
    std: 0.0125
    paper_value: 0.3487
    paper_std: 0.0125
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
    source_ref: Bo2021fagcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using standard split (Geom-GCN 10 fixed
      splits).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.397
    at_pub_std: null
    at_pub_source_arxiv: '2101.00797'
    at_pub_source_title: Beyond Low-frequency Information in Graph Convolutional Networks
    at_pub_source_date_iso: '2021-01-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-01-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.04830000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.397
    true_std: null
    value_gap_source_arxiv: '2101.00797'
    value_gap_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.04830000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.397
    sort_std: null
    global_rank: 71
    paper_rank: 285
    rank_delta: 214
    rank_delta_abs: 214
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    comparison_source_arxiv: '2101.00797'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.3899
    std: 0.0085
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11762'
    title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    venue: The Web Conference
    codebase_url: https://github.com/SDS-Lab/QW_Loss
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 87
    sort_value: 0.3899
    sort_std: 0.0085
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.3586
    std: 0.0103
    paper_value: 0.3586
    paper_std: 0.0103
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
    source_ref: zhu2020h2gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using standard split (Geom-GCN 10 fixed
      splits).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.3885
    at_pub_std: 0.0117
    at_pub_source_arxiv: '2603.09195'
    at_pub_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    at_pub_source_date_iso: '2026-03-10'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.029900000000000038
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3885
    true_std: 0.0117
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.029900000000000038
    has_value_note: false
    value_note: ''
    sort_value: 0.3885
    sort_std: 0.0117
    global_rank: 90
    paper_rank: 231
    rank_delta: 141
    rank_delta_abs: 141
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    comparison_source_arxiv: '2603.09195'
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.3299
    std: 0.0109
    paper_value: 0.3299
    paper_std: 0.0109
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: raw_features
    feature_source_evidence: learning PPDs for node classification from synthetic
      graph priors
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Actor dataset using standard split (Geom-GCN 10 fixed
      splits).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3299
    true_std: 0.0109
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3299
    sort_std: 0.0109
    global_rank: 341
    paper_rank: 341
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
  dataset: Amazon-Photo
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9703
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    sort_value: 0.9703
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9186
    std: 0.0107
    paper_value: 0.9186
    paper_std: 0.0107
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
    protocol_note: Accuracy on Amazon-Photo test split (2.1/49.0/49.0 split from Table
      2)
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9498
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.031200000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9669
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.04830000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.9669
    sort_std: 0.0014
    global_rank: 2
    paper_rank: 384
    rank_delta: 382
    rank_delta_abs: 382
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: DAM-GT
    model_key: dam-gt
    model_plain: DAM-GT
    value: 0.9666
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9643
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
    global_rank: 8
    sort_value: 0.9643
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9188
    std: 0.0079
    paper_value: 0.9188
    paper_std: 0.0079
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
    protocol_note: Accuracy on Amazon-Photo test split (2.1/49.0/49.0 split from Table
      2)
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9476
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2310.11025'
    at_pub_source_title: 'SignGT: Signed Attention-based Graph Transformer for Graph
      Representation Learning'
    at_pub_source_date_iso: '2023-10-17'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.028800000000000048
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9632
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.044399999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9632
    sort_std: 0.0008
    global_rank: 9
    paper_rank: 384
    rank_delta: 375
    rank_delta_abs: 375
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    comparison_source_arxiv: '2310.11025'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.682
    std: 0.0088
    paper_value: 0.682
    paper_std: 0.0088
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
    protocol_note: Accuracy on Amazon-Photo test split (2.1/49.0/49.0 split from Table
      2)
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9128
    at_pub_std: 0.0063
    at_pub_source_arxiv: '2306.02285'
    at_pub_source_title: Clarify Confused Nodes via Separated Learning
    at_pub_source_date_iso: '2023-06-04'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.2307999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9128
    true_std: 0.0063
    value_gap_source_arxiv: '2306.02285'
    value_gap_source_title: Clarify Confused Nodes via Separated Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.2307999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9128
    sort_std: 0.0063
    global_rank: 426
    paper_rank: 613
    rank_delta: 187
    rank_delta_abs: 187
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Clarify Confused Nodes via Separated Learning
    comparison_source_arxiv: '2306.02285'
    is_best: false
    is_std_outlier: false
  - model: GraphAny(Products)
    model_key: graphany(products)
    model_plain: GraphAny(Products)
    value: 0.9064
    std: 0.0082
    paper_value: 0.9064
    paper_std: 0.0082
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
    protocol_note: Accuracy on Amazon-Photo test split (2.1/49.0/49.0 split from Table
      2)
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9064
    true_std: 0.0082
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9064
    sort_std: 0.0082
    global_rank: 458
    paper_rank: 458
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.9053
    std: 0.0013
    paper_value: 0.9053
    paper_std: 0.0013
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
    feature_source_evidence: NodePFN learns from synthetic graph priors, not external
      real-world data.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Amazon-Photo test split (2.1/49.0/49.0 split from Table
      2)
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9053
    true_std: 0.0013
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9053
    sort_std: 0.0013
    global_rank: 467
    paper_rank: 467
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
- &id009
  dataset: Chameleon
  rows:
  - model: Hetero-S (GAT 8-layer)
    model_key: hetero-s (gat 8-layer)
    model_plain: Hetero-S (GAT 8-layer)
    value: 0.8693
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
    arxiv_id: '2406.12539'
    title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering GNNs for
      Heterophilic Graphs'
    date: Jun 18, 2024
    date_display: Jun 2024
    date_iso: '2024-06-18'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/bingreeky/HeteroSnoH
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8693
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Trans.Conv+CNA
    model_key: trans.conv+cna
    model_plain: Trans.Conv+CNA
    value: 0.8586
    std: 0.018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8586
    sort_std: 0.018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.856
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
    arxiv_id: '2406.12539'
    title: 'The Heterophilic Snowflake Hypothesis: Training and Empowering GNNs for
      Heterophilic Graphs'
    date: Jun 18, 2024
    date_display: Jun 2024
    date_iso: '2024-06-18'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/bingreeky/HeteroSnoH
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.856
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7033
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
    global_rank: 69
    sort_value: 0.7033
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.3969
    std: 0.0115
    paper_value: 0.3969
    paper_std: 0.0115
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
    source_ref: chien2021GPRGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the predefined split masks from Platonov
      et al. 2023.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.6748
    at_pub_std: 0.004
    at_pub_source_arxiv: '2603.09195'
    at_pub_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    at_pub_source_date_iso: '2026-03-10'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.2779
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6748
    true_std: 0.004
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.2779
    has_value_note: false
    value_note: ''
    sort_value: 0.6748
    sort_std: 0.004
    global_rank: 97
    paper_rank: 305
    rank_delta: 208
    rank_delta_abs: 208
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    comparison_source_arxiv: '2603.09195'
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.3724
    std: 0.0354
    paper_value: 0.3724
    paper_std: 0.0354
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
    source_ref: Bo2021fagcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the predefined split masks from Platonov
      et al. 2023.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.6344
    at_pub_std: 0.0205
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.26199999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6344
    true_std: 0.0205
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: false
    value_gap: 0.26199999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.6344
    sort_std: 0.0205
    global_rank: 135
    paper_rank: 312
    rank_delta: 177
    rank_delta_abs: 177
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Beyond Smoothing: Unsupervised Graph Representation
      Learning with Edge Heterophily Discriminating'
    comparison_source_arxiv: '2211.14065'
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.4107
    std: 0.0265
    paper_value: 0.4107
    paper_std: 0.0265
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
    source_ref: zhu2020h2gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the predefined split masks from Platonov
      et al. 2023.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.603
    at_pub_std: 0.0231
    at_pub_source_arxiv: '2206.14418'
    at_pub_source_title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    at_pub_source_date_iso: '2022-06-29'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-06-29'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.19229999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.603
    true_std: 0.0231
    value_gap_source_arxiv: '2206.14418'
    value_gap_source_title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    value_gap_source_is_current_paper: false
    value_gap: 0.19229999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.603
    sort_std: 0.0231
    global_rank: 164
    paper_rank: 297
    rank_delta: 133
    rank_delta_abs: 133
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Optimization-Induced Graph Implicit Nonlinear Diffusion
    comparison_source_arxiv: '2206.14418'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.5429
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
    global_rank: 208
    sort_value: 0.5429
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.5013
    std: 0.033
    paper_value: 0.5013
    paper_std: 0.033
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: raw_features
    feature_source_evidence: learning PPDs for node classification from synthetic
      graph priors
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Chameleon using the predefined split masks from Platonov
      et al. 2023.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5013
    true_std: 0.033
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5013
    sort_std: 0.033
    global_rank: 239
    paper_rank: 239
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
- &id003
  dataset: CiteSeer
  rows:
  - model: CNA
    model_key: cna
    model_plain: CNA
    value: 0.9575
    std: 0.0058
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9575
    sort_std: 0.0058
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: IS-GIB
    model_key: is-gib
    model_plain: IS-GIB
    value: 0.939
    std: 0.0187
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.939
    sort_std: 0.0187
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EERM
    model_key: eerm
    model_plain: EERM
    value: 0.9112
    std: 0.0145
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9112
    sort_std: 0.0145
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8774
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
    arxiv_id: '2305.06142'
    title: Feature Expansion for Graph Neural Networks
    date: May 10, 2023
    date_display: May 2023
    date_iso: '2023-05-10'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/sajqavril/Feature-Extension-Graph-Neural-Networks
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 20
    sort_value: 0.8774
    sort_std: 0.0041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7289
    std: 0.001
    metric: Accuracy
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
    global_rank: 401
    sort_value: 0.7289
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.673
    std: null
    paper_value: 0.673
    paper_std: null
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
    protocol_note: Accuracy on CiteSeer using the Planetoid split (20 nodes per class
      for training, 500 validation, 1000 test) as per Kipf & Welling 2017 protocol.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.673
    true_std: null
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.673
    sort_std: null
    global_rank: 779
    paper_rank: 779
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TabPFN
    model_key: tabpfn
    model_plain: TabPFN
    value: 0.3294
    std: null
    paper_value: 0.3294
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on CiteSeer using the Planetoid split (20 nodes per class
      for training, 500 validation, 1000 test) as per Kipf & Welling 2017 protocol.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3294
    true_std: null
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3294
    sort_std: null
    global_rank: 975
    paper_rank: 975
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
  dataset: Cora
  rows:
  - model: MATE
    model_key: mate
    model_plain: MATE
    value: 0.946
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.946
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE+CNA
    model_key: graphsage+cna
    model_plain: GraphSAGE+CNA
    value: 0.9418
    std: 0.0033
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9418
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DropAggr
    model_key: dropaggr
    model_plain: DropAggr
    value: 0.938
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.938
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.814
    std: 0.007
    paper_value: 0.814
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
    protocol_note: Cora, Planetoid split (20 nodes per class training, 1000 test).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.08640000000000003
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
    value_gap: 0.08640000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 31
    paper_rank: 662
    rank_delta: 631
    rank_delta_abs: 631
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: TFGNN
    model_key: tfgnn
    model_plain: TFGNN
    value: 0.6003
    std: 0.0
    paper_value: 0.6003
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora, Planetoid split (20 nodes per class training, 1000 test).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8921
    at_pub_std: 0.004
    at_pub_source_arxiv: '2404.15354'
    at_pub_source_title: 'Polynomial Selection in Spectral Graph Neural Networks:
      An Error-Sum of Function Slices Approach'
    at_pub_source_date_iso: '2024-04-15'
    at_pub_source_date_label: WWW 2024
    value_gap_source_date_iso: '2024-04-15'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: 0.29180000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8921
    true_std: 0.004
    value_gap_source_arxiv: '2404.15354'
    value_gap_source_title: 'Polynomial Selection in Spectral Graph Neural Networks:
      An Error-Sum of Function Slices Approach'
    value_gap_source_is_current_paper: false
    value_gap: 0.29180000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8921
    sort_std: 0.004
    global_rank: 59
    paper_rank: 960
    rank_delta: 901
    rank_delta_abs: 901
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Polynomial Selection in Spectral Graph Neural Networks:
      An Error-Sum of Function Slices Approach'
    comparison_source_arxiv: '2404.15354'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8911
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    venue: Trans. Mach. Learn. Res.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 61
    sort_value: 0.8911
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.817
    std: 0.0143
    paper_value: 0.817
    paper_std: 0.0143
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
    protocol_note: Cora, Planetoid split (20 nodes per class training, 1000 test).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8897
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2505.15845'
    at_pub_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in
      Tokenized Graph Learning Models'
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0727000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8897
    true_std: 0.0014
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.0727000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: 0.0014
    global_rank: 67
    paper_rank: 642
    rank_delta: 575
    rank_delta_abs: 575
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    comparison_source_arxiv: '2505.15845'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.782
    std: 0.0
    paper_value: 0.782
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora, Planetoid split (20 nodes per class training, 1000 test).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8683
    at_pub_std: 0.0128
    at_pub_source_arxiv: '2311.18177'
    at_pub_source_title: An Effective Universal Polynomial Basis for Spectral Graph
      Neural Networks
    at_pub_source_date_iso: '2023-11-30'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-05-21'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.08629999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8683
    true_std: 0.0128
    value_gap_source_arxiv: '2405.12474'
    value_gap_source_title: 'How Universal Polynomial Bases Enhance Spectral Graph
      Neural Networks: Heterophily, Over-smoothing, and Over-squashing'
    value_gap_source_is_current_paper: false
    value_gap: 0.08629999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.8683
    sort_std: 0.0128
    global_rank: 202
    paper_rank: 791
    rank_delta: 589
    rank_delta_abs: 589
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Effective Universal Polynomial Basis for Spectral
      Graph Neural Networks
    comparison_source_arxiv: '2311.18177'
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.8206
    std: 0.0029
    paper_value: 0.8206
    paper_std: 0.0029
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
    feature_source_evidence: single pre-trained model... without needing to be trained
      specifically for that dataset
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora, Planetoid split (20 nodes per class training, 1000 test).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8206
    true_std: 0.0029
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8206
    sort_std: 0.0029
    global_rank: 605
    paper_rank: 605
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphAny(Cora)
    model_key: graphany(cora)
    model_plain: GraphAny(Cora)
    value: 0.8018
    std: 0.0013
    paper_value: 0.8018
    paper_std: 0.0013
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
    input_feature_source: unknown
    feature_source_evidence: GraphAny models require training on each specific dataset
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora, Planetoid split (20 nodes per class training, 1000 test).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8018
    true_std: 0.0013
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8018
    sort_std: 0.0013
    global_rank: 734
    paper_rank: 734
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
    value: 0.4842
    std: 0.0063
    paper_value: 0.4842
    paper_std: 0.0063
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
    protocol_note: Cora, Planetoid split (20 nodes per class training, 1000 test).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.7768
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.2926
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7768
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.2926
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 806
    paper_rank: 996
    rank_delta: 190
    rank_delta_abs: 190
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: Linear
    model_key: linear
    model_plain: Linear
    value: 0.528
    std: 0.0
    paper_value: 0.528
    paper_std: 0.0
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora, Planetoid split (20 nodes per class training, 1000 test).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.7237
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2601.21369'
    at_pub_source_title: 'Rethinking Federated Graph Foundation Models: A Graph-Language
      Alignment-based Approach'
    at_pub_source_date_iso: '2026-01-29'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-01-29'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.19569999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7237
    true_std: 0.0033
    value_gap_source_arxiv: '2601.21369'
    value_gap_source_title: 'Rethinking Federated Graph Foundation Models: A Graph-Language
      Alignment-based Approach'
    value_gap_source_is_current_paper: false
    value_gap: 0.19569999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7237
    sort_std: 0.0033
    global_rank: 887
    paper_rank: 985
    rank_delta: 98
    rank_delta_abs: 98
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Rethinking Federated Graph Foundation Models: A Graph-Language
      Alignment-based Approach'
    comparison_source_arxiv: '2601.21369'
    is_best: false
    is_std_outlier: false
  - model: LabelProp
    model_key: labelprop
    model_plain: LabelProp
    value: 0.603
    std: 0.0
    paper_value: 0.603
    paper_std: 0.0
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora, Planetoid split (20 nodes per class training, 1000 test).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.603
    at_pub_std: 0.0
    at_pub_source_arxiv: '2405.20445'
    at_pub_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.603
    true_std: 0.0
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.603
    sort_std: 0.0
    global_rank: 960
    paper_rank: 960
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TabPFN
    model_key: tabpfn
    model_plain: TabPFN
    value: 0.531
    std: null
    paper_value: 0.531
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora, Planetoid split (20 nodes per class training, 1000 test).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.531
    true_std: null
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.531
    sort_std: null
    global_rank: 985
    paper_rank: 985
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGC
    model_key: hgc
    model_plain: HGC
    value: 0.225
    std: 0.0
    paper_value: 0.225
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Cora, Planetoid split (20 nodes per class training, 1000 test).
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.225
    true_std: 0.0
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.225
    sort_std: 0.0
    global_rank: 1012
    paper_rank: 1012
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
- &id007
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
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.4054
    std: 0.0201
    paper_value: 0.4054
    paper_std: 0.0201
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
    source_ref: chien2021GPRGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cornell using Geom-GCN 10 fixed splits.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9157
    at_pub_std: 0.0196
    at_pub_source_arxiv: '2403.03676'
    at_pub_source_title: Simplified PCNet with Robustness
    at_pub_source_date_iso: '2024-03-06'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-03-06'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.5103
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9157
    true_std: 0.0196
    value_gap_source_arxiv: '2403.03676'
    value_gap_source_title: Simplified PCNet with Robustness
    value_gap_source_is_current_paper: false
    value_gap: 0.5103
    has_value_note: false
    value_note: ''
    sort_value: 0.9157
    sort_std: 0.0196
    global_rank: 23
    paper_rank: 629
    rank_delta: 606
    rank_delta_abs: 606
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simplified PCNet with Robustness
    comparison_source_arxiv: '2403.03676'
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9136
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2212.03654'
    title: Node-oriented Spectral Filtering for Graph Neural Networks
    date: Dec 7, 2022
    date_display: Dec 2022
    date_iso: '2022-12-07'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 25
    sort_value: 0.9136
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.6038
    std: 0.0182
    paper_value: 0.6038
    paper_std: 0.0182
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
    source_ref: Bo2021fagcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cornell using Geom-GCN 10 fixed splits.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8852
    at_pub_std: 0.0133
    at_pub_source_arxiv: '2212.03654'
    at_pub_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.2814
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8852
    true_std: 0.0133
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.2814
    has_value_note: false
    value_note: ''
    sort_value: 0.8852
    sort_std: 0.0133
    global_rank: 48
    paper_rank: 443
    rank_delta: 395
    rank_delta_abs: 395
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    comparison_source_arxiv: '2212.03654'
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.6577
    std: 0.068
    paper_value: 0.6577
    paper_std: 0.068
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
    source_ref: zhu2020h2gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cornell using Geom-GCN 10 fixed splits.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8623
    at_pub_std: 0.0471
    at_pub_source_arxiv: '2603.09195'
    at_pub_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    at_pub_source_date_iso: '2026-03-10'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.2046
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8623
    true_std: 0.0471
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.2046
    has_value_note: false
    value_note: ''
    sort_value: 0.8623
    sort_std: 0.0471
    global_rank: 85
    paper_rank: 387
    rank_delta: 302
    rank_delta_abs: 302
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    comparison_source_arxiv: '2603.09195'
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
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.7189
    std: 0.0276
    paper_value: 0.7189
    paper_std: 0.0276
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
    feature_source_evidence: The model learns to extract patterns from context samples
      and apply them to test nodes... without needing to be trained specifically for
      that dataset.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Cornell using Geom-GCN 10 fixed splits.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7189
    true_std: 0.0276
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7189
    sort_std: 0.0276
    global_rank: 325
    paper_rank: 325
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
- &id012
  dataset: DBLP
  rows:
  - model: HG-SCM
    model_key: hg-scm
    model_plain: HG-SCM
    value: 0.949
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.05757'
    title: 'Towards Human-like Perception: Learning Structural Causal Model in Heterogeneous
      Graph'
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    venue: Information Processing & Management
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.949
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    value: 0.9489
    std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.05757'
    title: 'Towards Human-like Perception: Learning Structural Causal Model in Heterogeneous
      Graph'
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    venue: Information Processing & Management
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9489
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AdvSynGNN
    model_key: advsyngnn
    model_plain: AdvSynGNN
    value: 0.9486
    std: 0.0012
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9486
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7387
    std: 0.0135
    paper_value: 0.7387
    paper_std: 0.0135
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
    protocol_note: Accuracy on DBLP using the standard split (49.8% test) as described
      in Table 2.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8859
    at_pub_std: 0.001
    at_pub_source_arxiv: '2206.04739'
    at_pub_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.1472
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8859
    true_std: 0.001
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.1472
    has_value_note: false
    value_note: ''
    sort_value: 0.8859
    sort_std: 0.001
    global_rank: 31
    paper_rank: 121
    rank_delta: 90
    rank_delta_abs: 90
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    comparison_source_arxiv: '2206.04739'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7302
    std: 0.0222
    paper_value: 0.7302
    paper_std: 0.0222
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
    protocol_note: Accuracy on DBLP using the standard split (49.8% test) as described
      in Table 2.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8758
    at_pub_std: 0.002
    at_pub_source_arxiv: '2206.04739'
    at_pub_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.14560000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8758
    true_std: 0.002
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.14560000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8758
    sort_std: 0.002
    global_rank: 36
    paper_rank: 123
    rank_delta: 87
    rank_delta_abs: 87
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    comparison_source_arxiv: '2206.04739'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.5627
    std: 0.0062
    paper_value: 0.5627
    paper_std: 0.0062
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
    protocol_note: Accuracy on DBLP using the standard split (49.8% test) as described
      in Table 2.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8118
    at_pub_std: 0.002
    at_pub_source_arxiv: '2206.04739'
    at_pub_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    at_pub_source_date_iso: '2022-06-09'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.2491
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8118
    true_std: 0.002
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.2491
    has_value_note: false
    value_note: ''
    sort_value: 0.8118
    sort_std: 0.002
    global_rank: 80
    paper_rank: 142
    rank_delta: 62
    rank_delta_abs: 62
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    comparison_source_arxiv: '2206.04739'
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.7471
    std: 0.0039
    paper_value: 0.7471
    paper_std: 0.0039
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: raw_features
    feature_source_evidence: learning PPDs for node classification from synthetic
      graph priors
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on DBLP using the standard split (49.8% test) as described
      in Table 2.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7471
    true_std: 0.0039
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7471
    sort_std: 0.0039
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7455
    std: 0.0061
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.12613'
    title: 'Coden: Efficient Temporal Graph Neural Networks for Continuous Prediction'
    date: Feb 13, 2026
    date_display: Feb 2026
    date_iso: '2026-02-13'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 120
    sort_value: 0.7455
    sort_std: 0.0061
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphAny(Cora)
    model_key: graphany(cora)
    model_plain: GraphAny(Cora)
    value: 0.7173
    std: 0.0094
    paper_value: 0.7173
    paper_std: 0.0094
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
    protocol_note: Accuracy on DBLP using the standard split (49.8% test) as described
      in Table 2.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7173
    true_std: 0.0094
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7173
    sort_std: 0.0094
    global_rank: 127
    paper_rank: 127
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
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id016
  dataset: Deezer
  rows:
  - model: CLP
    model_key: clp
    model_plain: CLP
    value: 0.6569
    std: 0.0032
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_display: May 2022
    date_iso: '2022-05-19'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.6569
    sort_std: 0.0032
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.6504
    std: 0.0045
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_display: May 2022
    date_iso: '2022-05-19'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6504
    sort_std: 0.0045
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CPGNN
    model_key: cpgnn
    model_plain: CPGNN
    value: 0.6495
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
    arxiv_id: '2205.09389'
    title: Simplifying Node Classification on Heterophilous Graphs with Compatible
      Label Propagation
    date: May 19, 2022
    date_display: May 2022
    date_iso: '2022-05-19'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/zhiqiangzhongddu/TMLR-CLP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6495
    sort_std: 0.0039
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.5424
    std: 0.0215
    paper_value: 0.5424
    paper_std: 0.0215
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
    protocol_note: Accuracy on Deezer homophily dataset using standard split (0.1/49.9/49.9)
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.6377
    at_pub_std: 0.003
    at_pub_source_arxiv: '2205.09389'
    at_pub_source_title: Simplifying Node Classification on Heterophilous Graphs with
      Compatible Label Propagation
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: 0.09530000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6377
    true_std: 0.003
    value_gap_source_arxiv: '2205.09389'
    value_gap_source_title: Simplifying Node Classification on Heterophilous Graphs
      with Compatible Label Propagation
    value_gap_source_is_current_paper: false
    value_gap: 0.09530000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.6377
    sort_std: 0.003
    global_rank: 6
    paper_rank: 14
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simplifying Node Classification on Heterophilous Graphs
      with Compatible Label Propagation
    comparison_source_arxiv: '2205.09389'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5369
    std: 0.0229
    paper_value: 0.5369
    paper_std: 0.0229
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
    protocol_note: Accuracy on Deezer homophily dataset using standard split (0.1/49.9/49.9)
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.5994
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2205.09389'
    at_pub_source_title: Simplifying Node Classification on Heterophilous Graphs with
      Compatible Label Propagation
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2022-05-19'
    value_gap_source_date_label: TMLR 2022
    gap_vs_at_pub: 0.0625
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5994
    true_std: 0.0055
    value_gap_source_arxiv: '2205.09389'
    value_gap_source_title: Simplifying Node Classification on Heterophilous Graphs
      with Compatible Label Propagation
    value_gap_source_is_current_paper: false
    value_gap: 0.0625
    has_value_note: false
    value_note: ''
    sort_value: 0.5994
    sort_std: 0.0055
    global_rank: 10
    paper_rank: 14
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simplifying Node Classification on Heterophilous Graphs
      with Compatible Label Propagation
    comparison_source_arxiv: '2205.09389'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.5599
    std: 0.0378
    paper_value: 0.5599
    paper_std: 0.0378
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
    protocol_note: Accuracy on Deezer homophily dataset using standard split (0.1/49.9/49.9)
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.2434
    at_pub_std: 0.0121
    at_pub_source_arxiv: '2205.09389'
    at_pub_source_title: Simplifying Node Classification on Heterophilous Graphs with
      Compatible Label Propagation
    at_pub_source_date_iso: '2022-05-19'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: 0.31649999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5599
    true_std: 0.0378
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5599
    sort_std: 0.0378
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Simplifying Node Classification on Heterophilous Graphs
      with Compatible Label Propagation
    comparison_source_arxiv: '2205.09389'
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.5345
    std: 0.0065
    paper_value: 0.5345
    paper_std: 0.0065
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
    feature_source_evidence: NodePFN learns from synthetic graph priors, not external
      real-world data.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Deezer homophily dataset using standard split (0.1/49.9/49.9)
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5345
    true_std: 0.0065
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5345
    sort_std: 0.0065
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
  - model: GraphAny(Wisconsin)
    model_key: graphany(wisconsin)
    model_plain: GraphAny(Wisconsin)
    value: 0.5213
    std: 0.0302
    paper_value: 0.5213
    paper_std: 0.0302
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
    protocol_note: Accuracy on Deezer homophily dataset using standard split (0.1/49.9/49.9)
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5213
    true_std: 0.0302
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5213
    sort_std: 0.0302
    global_rank: 16
    paper_rank: 16
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
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id014
  dataset: Minesweeper
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9903
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    sort_value: 0.9903
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BuNN
    model_key: bunn
    model_plain: BuNN
    value: 0.9899
    std: 0.0016
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    sort_value: 0.9899
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: M3Dphormer
    model_key: m3dphormer
    model_plain: M3Dphormer
    value: 0.9827
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
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
    global_rank: 3
    sort_value: 0.9827
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8008
    std: 0.0004
    paper_value: 0.8008
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper heterophily dataset using 50/25/25 split
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9201
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2505.15015'
    at_pub_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    at_pub_source_date_iso: '2025-05-21'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.11930000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9786
    true_std: 0.0037
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.17780000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.9786
    sort_std: 0.0037
    global_rank: 5
    paper_rank: 47
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph
      Message Passing
    comparison_source_arxiv: '2505.15015'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8112
    std: 0.0037
    paper_value: 0.8112
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper heterophily dataset using 50/25/25 split
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8975
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2505.15015'
    at_pub_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message
      Passing
    at_pub_source_date_iso: '2025-05-21'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.08629999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9744
    true_std: 0.0017
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.1632
    has_value_note: false
    value_note: ''
    sort_value: 0.9744
    sort_std: 0.0017
    global_rank: 9
    paper_rank: 42
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-Scale Harmonic Encoding for Feature-Wise Graph
      Message Passing
    comparison_source_arxiv: '2505.15015'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9709
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
    global_rank: 11
    sort_value: 0.9709
    sort_std: 0.01
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.8066
    std: 0.0025
    paper_value: 0.8066
    paper_std: 0.0025
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
    feature_source_evidence: NodePFN learns from synthetic graph priors, not the benchmark
      training split.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper heterophily dataset using 50/25/25 split
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8066
    true_std: 0.0025
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8066
    sort_std: 0.0025
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphAny(Cora)
    model_key: graphany(cora)
    model_plain: GraphAny(Cora)
    value: 0.8046
    std: 0.0015
    paper_value: 0.8046
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Minesweeper heterophily dataset using 50/25/25 split
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8046
    true_std: 0.0015
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8046
    sort_std: 0.0015
    global_rank: 46
    paper_rank: 46
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
    value: 0.8
    std: 0.0
    paper_value: 0.8
    paper_std: 0.0
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
    protocol_note: Accuracy on Minesweeper heterophily dataset using 50/25/25 split
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8
    at_pub_std: 0.0
    at_pub_source_arxiv: '2407.11596'
    at_pub_source_title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    at_pub_source_date_iso: '2024-06-30'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8
    true_std: 0.0
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: 0.0
    global_rank: 49
    paper_rank: 49
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
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: PubMed
  rows:
  - model: LGTL
    model_key: lgtl
    model_plain: LGTL
    value: 0.9518
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9518
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MixHop (LO)
    model_key: mixhop (lo)
    model_plain: MixHop (LO)
    value: 0.9513
    std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE (LO)
    model_key: graphsage (lo)
    model_plain: GraphSAGE (LO)
    value: 0.9511
    std: 0.0036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9511
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9296
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 19
    sort_value: 0.9296
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGNN
    model_key: tfgnn
    model_plain: TFGNN
    value: 0.4004
    std: 0.01
    paper_value: 0.4004
    paper_std: 0.01
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 validation,
      1000 test.'
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9
    at_pub_std: 0.002
    at_pub_source_arxiv: '2404.15354'
    at_pub_source_title: 'Polynomial Selection in Spectral Graph Neural Networks:
      An Error-Sum of Function Slices Approach'
    at_pub_source_date_iso: '2024-04-15'
    at_pub_source_date_label: WWW 2024
    value_gap_source_date_iso: '2024-04-15'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: 0.49960000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9
    true_std: 0.002
    value_gap_source_arxiv: '2404.15354'
    value_gap_source_title: 'Polynomial Selection in Spectral Graph Neural Networks:
      An Error-Sum of Function Slices Approach'
    value_gap_source_is_current_paper: false
    value_gap: 0.49960000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9
    sort_std: 0.002
    global_rank: 87
    paper_rank: 971
    rank_delta: 884
    rank_delta_abs: 884
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Polynomial Selection in Spectral Graph Neural Networks:
      An Error-Sum of Function Slices Approach'
    comparison_source_arxiv: '2404.15354'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.7298
    std: 0.0
    paper_value: 0.7298
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 validation,
      1000 test.'
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8832
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2405.13902'
    at_pub_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural Network
      Training Framework'
    at_pub_source_date_iso: '2024-05-22'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.15339999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8832
    true_std: 0.0055
    value_gap_source_arxiv: '2405.13902'
    value_gap_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    value_gap_source_is_current_paper: false
    value_gap: 0.15339999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.8832
    sort_std: 0.0055
    global_rank: 164
    paper_rank: 901
    rank_delta: 737
    rank_delta_abs: 737
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LOGIN: A Large Language Model Consulted Graph Neural
      Network Training Framework'
    comparison_source_arxiv: '2405.13902'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.869
    std: 0.0074
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.00183'
    title: On the Equivalence of Graph Convolution and Mixup
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/ahxt/GraphConv_is_Mixup
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 243
    sort_value: 0.869
    sort_std: 0.0074
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.78
    std: 0.24
    paper_value: 0.78
    paper_std: 0.24
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
    feature_source_evidence: training on synthetic graphs that systematically cover
      the diversity of real-world graphs
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 validation,
      1000 test.'
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.78
    true_std: 0.24
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.78
    sort_std: 0.24
    global_rank: 747
    paper_rank: 747
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: true
  - model: Linear
    model_key: linear
    model_plain: Linear
    value: 0.593
    std: 0.0
    paper_value: 0.593
    paper_std: 0.0
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 validation,
      1000 test.'
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.6866
    at_pub_std: 0.0224
    at_pub_source_arxiv: '2602.09258'
    at_pub_source_title: Generalizing GNNs with Tokenized Mixture of Experts
    at_pub_source_date_iso: '2026-02-09'
    at_pub_source_date_label: KDD 2026
    value_gap_source_date_iso: '2026-02-09'
    value_gap_source_date_label: KDD 2026
    gap_vs_at_pub: 0.09360000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6866
    true_std: 0.0224
    value_gap_source_arxiv: '2602.09258'
    value_gap_source_title: Generalizing GNNs with Tokenized Mixture of Experts
    value_gap_source_is_current_paper: false
    value_gap: 0.09360000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.6866
    sort_std: 0.0224
    global_rank: 934
    paper_rank: 955
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Generalizing GNNs with Tokenized Mixture of Experts
    comparison_source_arxiv: '2602.09258'
    is_best: false
    is_std_outlier: false
  - model: LabelProp
    model_key: labelprop
    model_plain: LabelProp
    value: 0.6344
    std: 0.04
    paper_value: 0.6344
    paper_std: 0.04
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 validation,
      1000 test.'
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6344
    true_std: 0.04
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6344
    sort_std: 0.04
    global_rank: 949
    paper_rank: 949
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGC
    model_key: hgc
    model_plain: HGC
    value: 0.4632
    std: 0.0
    paper_value: 0.4632
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 validation,
      1000 test.'
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4632
    true_std: 0.0
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4632
    sort_std: 0.0
    global_rank: 962
    paper_rank: 962
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
- &id015
  dataset: Questions
  rows:
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9733
    std: 0.0006
    paper_value: 0.9733
    paper_std: 0.0006
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
    protocol_note: Accuracy on Questions dataset using 50/25/25 split as per Table
      2
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9733
    at_pub_std: null
    at_pub_source_arxiv: '2405.20445'
    at_pub_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9733
    true_std: 0.0006
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9733
    sort_std: 0.0006
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
  - model: AGS-GNN
    model_key: ags-gnn
    model_plain: AGS-GNN
    value: 0.9727
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: true
    override_reason: Table 1 reports test accuracy, not ROC-AUC; verified in expanded.tex.
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.07082'
    title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    date: Feb 14, 2022
    date_display: Feb 2022
    date_iso: '2022-02-14'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9727
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MeanGNN
    model_key: meangnn
    model_plain: MeanGNN
    value: 0.9716
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
    arxiv_id: '2506.14291'
    title: 'Equivariance Everywhere All At Once: A Recipe for Graph Foundation Models'
    date: Jun 17, 2025
    date_display: Jun 2025
    date_iso: '2025-06-17'
    venue: null
    codebase_url: https://github.com/benfinkelshtein/EquivarianceEverywhere
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9716
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9715
    std: 0.0004
    paper_value: 0.9715
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using 50/25/25 split as per Table
      2
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9715
    at_pub_std: null
    at_pub_source_arxiv: '2405.20445'
    at_pub_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9715
    true_std: 0.0004
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9715
    sort_std: 0.0004
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9711
    std: 0.0002
    paper_value: 0.9711
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using 50/25/25 split as per Table
      2
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9713
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2506.14291'
    at_pub_source_title: 'Equivariance Everywhere All At Once: A Recipe for Graph
      Foundation Models'
    at_pub_source_date_iso: '2025-06-17'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-06-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.000200000000000089
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9713
    true_std: 0.0005
    value_gap_source_arxiv: '2506.14291'
    value_gap_source_title: 'Equivariance Everywhere All At Once: A Recipe for Graph
      Foundation Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.000200000000000089
    has_value_note: false
    value_note: ''
    sort_value: 0.9713
    sort_std: 0.0005
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
  - model: GraphAny(Wisconsin)
    model_key: graphany(wisconsin)
    model_plain: GraphAny(Wisconsin)
    value: 0.9711
    std: 0.0
    paper_value: 0.9711
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using 50/25/25 split as per Table
      2
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9711
    true_std: 0.0
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9711
    sort_std: 0.0
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.9702
    std: 0.0001
    paper_value: 0.9702
    paper_std: 0.0001
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
    feature_source_evidence: The model is trained on synthetic graph priors to perform
      in-context learning on real graphs.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Questions dataset using 50/25/25 split as per Table
      2
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9702
    true_std: 0.0001
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9702
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.7644
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: true
    override_reason: Table 1 reports test accuracy, not ROC-AUC; verified in expanded.tex.
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2202.07082'
    title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    date: Feb 14, 2022
    date_display: Feb 2022
    date_iso: '2022-02-14'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 33
    sort_value: 0.7644
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id010
  dataset: Squirrel
  rows:
  - model: IBG-NN
    model_key: ibg-nn
    model_plain: IBG-NN
    value: 0.7763
    std: 0.0179
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.18273'
    title: Efficient Learning on Large Graphs using a Densifying Regularity Lemma
    date: Apr 25, 2025
    date_display: Apr 2025
    date_iso: '2025-04-25'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7763
    sort_std: 0.0179
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Trans.Conv+CNA
    model_key: trans.conv+cna
    model_plain: Trans.Conv+CNA
    value: 0.7747
    std: 0.0128
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7747
    sort_std: 0.0128
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DHGNN
    model_key: dhgnn
    model_plain: DHGNN
    value: 0.7684
    std: 0.0161
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.22362'
    title: Directed Homophily-Aware Graph Neural Network
    date: May 28, 2025
    date_display: May 2025
    date_iso: '2025-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7684
    sort_std: 0.0161
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.351
    std: 0.0115
    paper_value: 0.351
    paper_std: 0.0115
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
    source_ref: zhu2020h2gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using filtered datasets from Platonov
      et al. 2023 and predefined split masks from Pei et al. 2020.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.619
    at_pub_std: 0.014
    at_pub_source_arxiv: '2504.18273'
    at_pub_source_title: Efficient Learning on Large Graphs using a Densifying Regularity
      Lemma
    at_pub_source_date_iso: '2025-04-25'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-04-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.268
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.619
    true_std: 0.014
    value_gap_source_arxiv: '2504.18273'
    value_gap_source_title: Efficient Learning on Large Graphs using a Densifying
      Regularity Lemma
    value_gap_source_is_current_paper: false
    value_gap: 0.268
    has_value_note: false
    value_note: ''
    sort_value: 0.619
    sort_std: 0.014
    global_rank: 42
    paper_rank: 248
    rank_delta: 206
    rank_delta_abs: 206
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Learning on Large Graphs using a Densifying
      Regularity Lemma
    comparison_source_arxiv: '2504.18273'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6067
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
    global_rank: 51
    sort_value: 0.6067
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.3895
    std: 0.0199
    paper_value: 0.3895
    paper_std: 0.0199
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
    source_ref: chien2021GPRGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using filtered datasets from Platonov
      et al. 2023 and predefined split masks from Pei et al. 2020.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.5435
    at_pub_std: 0.0087
    at_pub_source_arxiv: '2505.22362'
    at_pub_source_title: Directed Homophily-Aware Graph Neural Network
    at_pub_source_date_iso: '2025-05-28'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-28'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.15399999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5435
    true_std: 0.0087
    value_gap_source_arxiv: '2505.22362'
    value_gap_source_title: Directed Homophily-Aware Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.15399999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.5435
    sort_std: 0.0087
    global_rank: 86
    paper_rank: 195
    rank_delta: 109
    rank_delta_abs: 109
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Directed Homophily-Aware Graph Neural Network
    comparison_source_arxiv: '2505.22362'
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.434
    std: 0.0103
    paper_value: 0.434
    paper_std: 0.0103
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: raw_features
    feature_source_evidence: learning PPDs for node classification from synthetic
      graph priors
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using filtered datasets from Platonov
      et al. 2023 and predefined split masks from Pei et al. 2020.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.434
    true_std: 0.0103
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.434
    sort_std: 0.0103
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
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.3678
    std: 0.0311
    paper_value: 0.3678
    paper_std: 0.0311
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
    source_ref: Bo2021fagcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Squirrel using filtered datasets from Platonov
      et al. 2023 and predefined split masks from Pei et al. 2020.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.4259
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2210.00513'
    at_pub_source_title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2024-06-16'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.058099999999999985
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4259
    true_std: 0.0069
    value_gap_source_arxiv: '2406.10871'
    value_gap_source_title: Graph Neural Reaction Diffusion Models Submitted to the
      editors June 2023. Accepted in March 2024.
    value_gap_source_is_current_paper: false
    value_gap: 0.058099999999999985
    has_value_note: false
    value_note: ''
    sort_value: 0.4259
    sort_std: 0.0069
    global_rank: 159
    paper_rank: 225
    rank_delta: 66
    rank_delta_abs: 66
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Gradient Gating for Deep Multi-Rate Learning on Graphs
    comparison_source_arxiv: '2210.00513'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.393
    std: 0.0079
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    global_rank: 194
    sort_value: 0.393
    sort_std: 0.0079
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
- &id006
  dataset: Texas
  rows:
  - model: P^2GNN
    model_key: p^2gnn
    model_plain: P^2GNN
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
  - model: DoG
    model_key: dog
    model_plain: DoG
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
  - model: GPF-plus
    model_key: gpf-plus
    model_plain: GPF-plus
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
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.6577
    std: 0.0156
    paper_value: 0.6577
    paper_std: 0.0156
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
    source_ref: chien2021GPRGNN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Texas dataset using standard split/task.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9295
    at_pub_std: 0.0131
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.27180000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9295
    true_std: 0.0131
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.27180000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9295
    sort_std: 0.0131
    global_rank: 38
    paper_rank: 517
    rank_delta: 479
    rank_delta_abs: 479
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.923
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2410.05593'
    title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    date: Oct 8, 2024
    date_display: Oct 2024
    date_iso: '2024-10-08'
    venue: International Conference on Learning Representations
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 45
    sort_value: 0.923
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.7658
    std: 0.0156
    paper_value: 0.7658
    paper_std: 0.0156
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
    source_ref: zhu2020h2gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Texas dataset using standard split/task.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.9189
    at_pub_std: 0.0393
    at_pub_source_arxiv: '2411.17296'
    at_pub_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    at_pub_source_date_iso: '2024-11-26'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-11-26'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.1531
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9189
    true_std: 0.0393
    value_gap_source_arxiv: '2411.17296'
    value_gap_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    value_gap_source_is_current_paper: false
    value_gap: 0.1531
    has_value_note: false
    value_note: ''
    sort_value: 0.9189
    sort_std: 0.0393
    global_rank: 52
    paper_rank: 363
    rank_delta: 311
    rank_delta_abs: 311
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GrokFormer: Graph Fourier Kolmogorov-Arnold Transformers'
    comparison_source_arxiv: '2411.17296'
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9001
    std: 0.023
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11762'
    title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    venue: The Web Conference
    codebase_url: https://github.com/SDS-Lab/QW_Loss
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 73
    sort_value: 0.9001
    sort_std: 0.023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.6844
    std: 0.0178
    paper_value: 0.6844
    paper_std: 0.0178
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
    source_ref: Bo2021fagcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Texas dataset using standard split/task.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8961
    at_pub_std: 0.0152
    at_pub_source_arxiv: '2212.03654'
    at_pub_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    at_pub_source_date_iso: '2022-12-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.2117
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8961
    true_std: 0.0152
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.2117
    has_value_note: false
    value_note: ''
    sort_value: 0.8961
    sort_std: 0.0152
    global_rank: 82
    paper_rank: 486
    rank_delta: 404
    rank_delta_abs: 404
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    comparison_source_arxiv: '2212.03654'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.4603
    std: 0.0686
    paper_value: 0.4603
    paper_std: 0.0686
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
    protocol_note: Accuracy on Texas dataset using standard split/task.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8131
    at_pub_std: 0.033
    at_pub_source_arxiv: '2505.23014'
    at_pub_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in the
      Perspective of A System of Hyperbolic Partial Differential Equations'
    at_pub_source_date_iso: '2025-05-29'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.35280000000000006
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
    value_gap: 0.35280000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8131
    sort_std: 0.033
    global_rank: 279
    paper_rank: 692
    rank_delta: 413
    rank_delta_abs: 413
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in
      the Perspective of A System of Hyperbolic Partial Differential Equations'
    comparison_source_arxiv: '2505.23014'
    is_best: false
    is_std_outlier: false
  - model: Linear
    model_key: linear
    model_plain: Linear
    value: 0.3235
    std: 0.053
    paper_value: 0.3235
    paper_std: 0.053
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
    protocol_note: Accuracy on Texas dataset using standard split/task.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.7838
    at_pub_std: 0.0
    at_pub_source_arxiv: '2512.11561'
    at_pub_source_title: 'View Space: Learning Representation across Arbitrary Graphs'
    at_pub_source_date_iso: '2025-12-12'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-12-12'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.46030000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7838
    true_std: 0.0
    value_gap_source_arxiv: '2512.11561'
    value_gap_source_title: 'View Space: Learning Representation across Arbitrary
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.46030000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.7838
    sort_std: 0.0
    global_rank: 334
    paper_rank: 712
    rank_delta: 378
    rank_delta_abs: 378
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'View Space: Learning Representation across Arbitrary
      Graphs'
    comparison_source_arxiv: '2512.11561'
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.7622
    std: 0.0753
    paper_value: 0.7622
    paper_std: 0.0753
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: raw_features
    feature_source_evidence: learning PPDs for node classification from synthetic
      graph priors
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Texas dataset using standard split/task.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7622
    true_std: 0.0753
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7622
    sort_std: 0.0753
    global_rank: 369
    paper_rank: 369
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGC
    model_key: hgc
    model_plain: HGC
    value: 0.5754
    std: 0.063
    paper_value: 0.5754
    paper_std: 0.063
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
    protocol_note: Accuracy on Texas dataset using standard split/task.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5754
    true_std: 0.063
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5754
    sort_std: 0.063
    global_rank: 641
    paper_rank: 641
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LabelProp
    model_key: labelprop
    model_plain: LabelProp
    value: 0.2353
    std: 0.0551
    paper_value: 0.2353
    paper_std: 0.0551
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
    protocol_note: Accuracy on Texas dataset using standard split/task.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2353
    true_std: 0.0551
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2353
    sort_std: 0.0551
    global_rank: 716
    paper_rank: 716
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGNN
    model_key: tfgnn
    model_plain: TFGNN
    value: 0.1991
    std: 0.061
    paper_value: 0.1991
    paper_std: 0.061
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
    protocol_note: Accuracy on Texas dataset using standard split/task.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1991
    true_std: 0.061
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1991
    sort_std: 0.061
    global_rank: 717
    paper_rank: 717
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
- &id013
  dataset: Tolokers
  rows:
  - model: NT*
    model_key: nt
    model_plain: NT*
    value: 0.8591
    std: 0.0083
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2604.08980'
    title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware Graph
      Learning'
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    venue: arXiv.org
    codebase_url: https://github.com/cf020031308/MoNT
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8591
    sort_std: 0.0083
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.8591
    std: 0.0074
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2604.08980'
    title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware Graph
      Learning'
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    venue: arXiv.org
    codebase_url: https://github.com/cf020031308/MoNT
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8591
    sort_std: 0.0074
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Dir-NT
    model_key: dir-nt
    model_plain: Dir-NT
    value: 0.8502
    std: 0.0077
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8502
    sort_std: 0.0077
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.785
    std: 0.0055
    paper_value: 0.785
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using the 50/25/25 split as defined in Table
      2.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.837
    at_pub_std: 0.0047
    at_pub_source_arxiv: '2405.20724'
    at_pub_source_title: on Large Graphs using Intersecting Communities
    at_pub_source_date_iso: '2024-05-31'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-05-31'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.051999999999999935
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.837
    true_std: 0.0047
    value_gap_source_arxiv: '2405.20724'
    value_gap_source_title: on Large Graphs using Intersecting Communities
    value_gap_source_is_current_paper: false
    value_gap: 0.051999999999999935
    has_value_note: false
    value_note: ''
    sort_value: 0.837
    sort_std: 0.0047
    global_rank: 7
    paper_rank: 23
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: on Large Graphs using Intersecting Communities
    comparison_source_arxiv: '2405.20724'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7993
    std: 0.001
    paper_value: 0.7993
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using the 50/25/25 split as defined in Table
      2.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8364
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2405.20724'
    at_pub_source_title: on Large Graphs using Intersecting Communities
    at_pub_source_date_iso: '2024-05-31'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2026-04-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.03710000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8364
    true_std: 0.0067
    value_gap_source_arxiv: '2604.08980'
    value_gap_source_title: 'Neighbourhood Transformer: Switchable Attention for Monophily-Aware
      Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.03710000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8364
    sort_std: 0.0067
    global_rank: 8
    paper_rank: 14
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: on Large Graphs using Intersecting Communities
    comparison_source_arxiv: '2405.20724'
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.7861
    std: 0.0006
    paper_value: 0.7861
    paper_std: 0.0006
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
    feature_source_evidence: The model is trained on synthetic graph priors and performs
      in-context learning on the target dataset.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using the 50/25/25 split as defined in Table
      2.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7861
    true_std: 0.0006
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7861
    sort_std: 0.0006
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
  - model: GraphAny(Wisconsin)
    model_key: graphany(wisconsin)
    model_plain: GraphAny(Wisconsin)
    value: 0.7824
    std: 0.0003
    paper_value: 0.7824
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Tolokers using the 50/25/25 split as defined in Table
      2.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7824
    true_std: 0.0003
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7824
    sort_std: 0.0003
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7816
    std: 0.0002
    paper_value: 0.7816
    paper_std: 0.0002
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
    protocol_note: Accuracy on Tolokers using the 50/25/25 split as defined in Table
      2.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.7295
    at_pub_std: 0.0106
    at_pub_source_arxiv: '2405.20724'
    at_pub_source_title: on Large Graphs using Intersecting Communities
    at_pub_source_date_iso: '2024-05-31'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: 0.052099999999999924
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7816
    true_std: 0.0002
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7816
    sort_std: 0.0002
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: on Large Graphs using Intersecting Communities
    comparison_source_arxiv: '2405.20724'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id005
  dataset: WikiCS
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9302
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2204.04874'
    title: Augmentation-Free Graph Contrastive Learning with Performance Guarantee
    date: Apr 11, 2022
    date_display: Apr 2022
    date_iso: '2022-04-11'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9302
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RSE + RGCN (70b)
    model_key: rse + rgcn (70b)
    model_plain: RSE + RGCN (70b)
    value: 0.8852
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: leverages the capability of Large Language Models (LLMs)
      to decompose the graph structure by analyzing raw text attributes
    is_global_top: true
    global_rank: 2
    sort_value: 0.8852
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LEMP+T
    model_key: lemp+t
    model_plain: LEMP+T
    value: 0.8825
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8825
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8771
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
    global_rank: 9
    sort_value: 0.8771
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LLaGA
    model_key: llaga
    model_plain: LLaGA
    value: 0.7388
    std: null
    paper_value: 0.7388
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: LLaGA is an LLM-based model.
    table_ref: Table 1
    source_ref: chen2024llaga
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: WikiCS node classification under the supervised setting of GLBench;
      metric is Accuracy %.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.8074
    at_pub_std: null
    at_pub_source_arxiv: '2503.03313'
    at_pub_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    at_pub_source_date_iso: '2025-03-05'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-03-05'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0686
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8074
    true_std: null
    value_gap_source_arxiv: '2503.03313'
    value_gap_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.0686
    has_value_note: false
    value_note: ''
    sort_value: 0.8074
    sort_std: null
    global_rank: 79
    paper_rank: 243
    rank_delta: 164
    rank_delta_abs: 164
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'LLM as GNN: Graph Vocabulary Learning for Text-Attributed
      Graph Foundation Models'
    comparison_source_arxiv: '2503.03313'
    is_best: false
    is_std_outlier: false
  - model: OFA
    model_key: ofa
    model_plain: OFA
    value: 0.7734
    std: null
    paper_value: 0.7734
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: OFA is an LLM-based model.
    table_ref: Table 1
    source_ref: liu2024ofa
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: WikiCS node classification under the supervised setting of GLBench;
      metric is Accuracy %.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.7855
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2505.12684'
    at_pub_source_title: Towards Effective Federated Graph Foundation Model via Mitigating
      Knowledge Entanglement
    at_pub_source_date_iso: '2025-05-19'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.0121
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7855
    true_std: 0.0037
    value_gap_source_arxiv: '2505.12684'
    value_gap_source_title: Towards Effective Federated Graph Foundation Model via
      Mitigating Knowledge Entanglement
    value_gap_source_is_current_paper: false
    value_gap: 0.0121
    has_value_note: false
    value_note: ''
    sort_value: 0.7855
    sort_std: 0.0037
    global_rank: 158
    paper_rank: 196
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Effective Federated Graph Foundation Model via
      Mitigating Knowledge Entanglement
    comparison_source_arxiv: '2505.12684'
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.7629
    std: null
    paper_value: 0.7629
    paper_std: null
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
    protocol_note: WikiCS node classification under the supervised setting of GLBench;
      metric is Accuracy %.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7629
    true_std: null
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7629
    sort_std: null
    global_rank: 218
    paper_rank: 218
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
    value: 0.7469
    std: 0.0085
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2512.11561'
    title: 'View Space: Learning Representation across Arbitrary Graphs'
    date: Dec 12, 2025
    date_display: Dec 2025
    date_iso: '2025-12-12'
    venue: Accepted to ICML 2026
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 237
    sort_value: 0.7469
    sort_std: 0.0085
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: InstructGLM
    model_key: instructglm
    model_plain: InstructGLM
    value: 0.4573
    std: null
    paper_value: 0.4573
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: InstructGLM is an LLM-based model.
    table_ref: Table 1
    source_ref: ye2023instructglm
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: WikiCS node classification under the supervised setting of GLBench;
      metric is Accuracy %.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.744
    at_pub_std: null
    at_pub_source_arxiv: '2603.19596'
    at_pub_source_title: 'CO-EVOLVE: Bidirectional Co-Evolution of Graph Structure
      and Semantics for Heterophilous Learning'
    at_pub_source_date_iso: '2026-03-20'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-03-20'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.2867
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.744
    true_std: null
    value_gap_source_arxiv: '2603.19596'
    value_gap_source_title: 'CO-EVOLVE: Bidirectional Co-Evolution of Graph Structure
      and Semantics for Heterophilous Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.2867
    has_value_note: false
    value_note: ''
    sort_value: 0.744
    sort_std: null
    global_rank: 239
    paper_rank: 317
    rank_delta: 78
    rank_delta_abs: 78
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'CO-EVOLVE: Bidirectional Co-Evolution of Graph Structure
      and Semantics for Heterophilous Learning'
    comparison_source_arxiv: '2603.19596'
    is_best: false
    is_std_outlier: false
  - model: TabPFN
    model_key: tabpfn
    model_plain: TabPFN
    value: 0.6225
    std: null
    paper_value: 0.6225
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: WikiCS node classification using the split from Rozemberczki et
      al. 2021; metric is Accuracy %.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.7208
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2512.08798'
    at_pub_source_title: Can TabPFN Compete with GNNs for Node Classification via
      Graph Tabularization?
    at_pub_source_date_iso: '2025-12-09'
    at_pub_source_date_label: LoG 2025
    value_gap_source_date_iso: '2025-12-09'
    value_gap_source_date_label: LoG 2025
    gap_vs_at_pub: 0.09829999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7208
    true_std: 0.0059
    value_gap_source_arxiv: '2512.08798'
    value_gap_source_title: Can TabPFN Compete with GNNs for Node Classification via
      Graph Tabularization?
    value_gap_source_is_current_paper: false
    value_gap: 0.09829999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.7208
    sort_std: 0.0059
    global_rank: 252
    paper_rank: 307
    rank_delta: 55
    rank_delta_abs: 55
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Can TabPFN Compete with GNNs for Node Classification
      via Graph Tabularization?
    comparison_source_arxiv: '2512.08798'
    is_best: false
    is_std_outlier: false
  - model: GraphText
    model_key: graphtext
    model_plain: GraphText
    value: 0.6735
    std: null
    paper_value: 0.6735
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    uses_external_data: 1
    input_feature_source: llm_features
    feature_source_evidence: GraphText is an LLM-based model.
    table_ref: Table 1
    source_ref: zhao2023graphtext
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: WikiCS node classification under the supervised setting of GLBench;
      metric is Accuracy %.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6735
    true_std: null
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6735
    sort_std: null
    global_rank: 283
    paper_rank: 283
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
- &id011
  dataset: Wisconsin
  rows:
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.958
    std: 0.02
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
    global_rank: 1
    sort_value: 0.958
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.938
    std: 0.024
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
    sort_value: 0.938
    sort_std: 0.024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DMD++
    model_key: dmd++
    model_plain: DMD++
    value: 0.919
    std: 0.026
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2410.05593'
    title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    date: Oct 8, 2024
    date_display: Oct 2024
    date_iso: '2024-10-08'
    venue: International Conference on Learning Representations
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.919
    sort_std: 0.026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.918
    std: 0.031
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2410.05593'
    title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    date: Oct 8, 2024
    date_display: Oct 2024
    date_iso: '2024-10-08'
    venue: International Conference on Learning Representations
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 4
    sort_value: 0.918
    sort_std: 0.031
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.831
    std: 0.032
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.02386'
    title: Restructuring Graphs for Higher Homophily via Adaptive Spectral Clustering
    date: Jun 6, 2022
    date_display: Jun 2022
    date_iso: '2022-06-06'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/seanli3/graph_restructure
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 79
    sort_value: 0.831
    sort_std: 0.032
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NodePFN
    model_key: nodepfn
    model_plain: NodePFN
    value: 0.8118
    std: 0.057
    paper_value: 0.8118
    paper_std: 0.057
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
    feature_source_evidence: training on synthetic graphs that systematically cover
      the diversity of real-world graphs
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on Wisconsin using the standard Geom-GCN 10 fixed splits.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8118
    true_std: 0.057
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8118
    sort_std: 0.057
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
  - model: Linear
    model_key: linear
    model_plain: Linear
    value: 0.8
    std: 0.0215
    paper_value: 0.8
    paper_std: 0.0215
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
    protocol_note: Accuracy on Wisconsin using the standard Geom-GCN 10 fixed splits.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8
    true_std: 0.0215
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: 0.0215
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
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.5764
    std: 0.0107
    paper_value: 0.5764
    paper_std: 0.0107
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
    protocol_note: Accuracy on Wisconsin using the standard Geom-GCN 10 fixed splits.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.778
    at_pub_std: 0.047
    at_pub_source_arxiv: '2206.02386'
    at_pub_source_title: Restructuring Graphs for Higher Homophily via Adaptive Spectral
      Clustering
    at_pub_source_date_iso: '2022-06-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.2016
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.778
    true_std: 0.047
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.2016
    has_value_note: false
    value_note: ''
    sort_value: 0.778
    sort_std: 0.047
    global_rank: 113
    paper_rank: 202
    rank_delta: 89
    rank_delta_abs: 89
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    comparison_source_arxiv: '2206.02386'
    is_best: false
    is_std_outlier: false
  - model: HGC
    model_key: hgc
    model_plain: HGC
    value: 0.6432
    std: 0.0251
    paper_value: 0.6432
    paper_std: 0.0251
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
    protocol_note: Accuracy on Wisconsin using the standard Geom-GCN 10 fixed splits.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6432
    true_std: 0.0251
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6432
    sort_std: 0.0251
    global_rank: 173
    paper_rank: 173
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LabelProp
    model_key: labelprop
    model_plain: LabelProp
    value: 0.1608
    std: 0.0215
    paper_value: 0.1608
    paper_std: 0.0215
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
    protocol_note: Accuracy on Wisconsin using the standard Geom-GCN 10 fixed splits.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1608
    true_std: 0.0215
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1608
    sort_std: 0.0215
    global_rank: 255
    paper_rank: 255
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGNN
    model_key: tfgnn
    model_plain: TFGNN
    value: 0.1451
    std: 0.0301
    paper_value: 0.1451
    paper_std: 0.0301
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
    protocol_note: Accuracy on Wisconsin using the standard Geom-GCN 10 fixed splits.
    date: Apr 21, 2026
    date_display: Apr 2026
    date_iso: '2026-04-21'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-21'
    value_gap_source_date_label: ICLR 2026
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1451
    true_std: 0.0301
    value_gap_source_arxiv: '2604.19028'
    value_gap_source_title: Learning Posterior Predictive Distributions for Node Classification
      from Synthetic Graph Priors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1451
    sort_std: 0.0301
    global_rank: 256
    paper_rank: 256
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
  - *id005
- benchmark: Heterophilic Graphs
  datasets:
  - *id006
  - *id007
  - *id008
  - *id009
  - *id010
  - *id011
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id012
- benchmark: Heterophily Benchmark
  datasets:
  - *id013
  - *id014
  - *id015
- benchmark: LINKX Benchmarks
  datasets:
  - *id016
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: WikiCS
      dataset_slug: wikics
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
    - dataset: Actor
      dataset_slug: actor
    - dataset: Chameleon
      dataset_slug: chameleon
    - dataset: Squirrel
      dataset_slug: squirrel
    - dataset: Wisconsin
      dataset_slug: wisconsin
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Tolokers
      dataset_slug: tolokers
    - dataset: Minesweeper
      dataset_slug: minesweeper
    - dataset: Questions
      dataset_slug: questions
  - benchmark: LINKX Benchmarks
    benchmark_slug: linkx-benchmarks
    datasets:
    - dataset: Deezer
      dataset_slug: deezer
single_proposed_model: NodePFN
main_figure: /figures/2604.19028/main_figure.jpegoptim.jpg
---

