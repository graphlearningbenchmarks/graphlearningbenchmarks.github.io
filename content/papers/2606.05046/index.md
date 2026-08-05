---
title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for Structure-Aware Graph
  Machine Learning'
arxiv_id: '2606.05046'
source_url: ''
authors:
- name: Meher Chaitanya
  orcid: null
  s2_author_id: '35627410'
  s2_url: null
- name: My Le
  orcid: null
  s2_author_id: '2440608924'
  s2_url: null
- name: Luana Ruiz
  orcid: null
  s2_author_id: '2382917892'
  s2_url: null
published_date: Jun 3, 2026
published_date_iso: '2026-06-03'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'We introduce Graph Cascades, a mesoscopic rewiring strategy for Graph Neural
  Networks (GNNs) and Graph Transformers (GTs) that captures intermediate-scale graph
  structure beyond purely local edges or fully global attention. Using contagion-based
  diffusion processes, Graph Cascades constructs, in O(|V|+|E|) time, an auxiliary
  graph where node pairs supported by repeated multi-hop reinforcement are promoted
  to direct neighbors. We theoretically characterize when reinforcement-based rewiring
  helps: sufficient conditions under which reinforcement-based edge selection is more
  label-aligned than direct adjacency, an SBM witness in which two-hop reinforcement
  is perfectly homophilic, and a formalization of mesoscopic connectivity via graph
  effective resistance. Empirically, across node-classification benchmarks, Graph
  Cascades improves multiple GNN and sparse-GT backbones, with the most reliable gains
  observed on heterophilic and moderate- to high-degree homophilic graphs. The theoretical
  conditions also identify regimes where mesoscopic rewiring is unlikely to be beneficial
  -- low-degree regular graphs and graphs with structural bottlenecks -- and these
  predictions match the observed failures. We additionally observe tight correlations
  between performance and structural properties in the rewired graphs.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- LRGB
- Heterophily Benchmark
benchmark_coverage:
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 2
  total: 5
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 3
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id004
  dataset: Amazon-ratings
  is_multi_metric: true
  rows:
  - model: H2GCN + UniGAP
    model_key: h2gcn + unigap
    model_plain: H2GCN + UniGAP
    metric_values:
    - 0.6375
    - null
    - null
    metric_stds:
    - 0.011
    - null
    - null
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
    published_venue: ''
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.6375
    sort_std: 0.011
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GraphSAGE + UniGAP
    model_key: graphsage + unigap
    model_plain: GraphSAGE + UniGAP
    metric_values:
    - 0.6283
    - null
    - null
    metric_stds:
    - 0.009
    - null
    - null
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
    published_venue: ''
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: true
    sort_value: 0.6283
    sort_std: 0.009
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GCN + UniGAP
    model_key: gcn + unigap
    model_plain: GCN + UniGAP
    metric_values:
    - 0.5976
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
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
    published_venue: ''
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.5976
    sort_std: 0.008
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - 0.5569
    - null
    - null
    metric_stds:
    - 0.0023
    - null
    - null
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
    published_venue: ''
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    is_global_top: true
    global_rank: 14
    is_best: false
    sort_value: 0.5569
    sort_std: 0.0023
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: ACMGCN
    model_key: acmgcn
    model_plain: ACMGCN
    metric_values:
    - 0.5565
    - null
    - null
    metric_stds:
    - 0.0176
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5565
    sort_std: 0.0176
    true_value: 0.5565
    true_std: 0.0176
    paper_value: 0.5565
    paper_std: 0.0176
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 15
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.4931
    - null
    - null
    metric_stds:
    - 0.0123
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5559
    sort_std: 0.0027
    true_value: 0.5559
    true_std: 0.0027
    paper_value: 0.4931
    paper_std: 0.0123
    has_value_gap: true
    has_value_note: false
    value_gap: 0.06279999999999997
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_note: ''
    at_pub_value: 0.5559
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2605.20248'
    at_pub_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    at_pub_source_date_iso: '2026-05-18'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.06279999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled
      Predictions in Node Classification'
    comparison_source_arxiv: '2605.20248'
    is_best: false
    is_std_outlier: false
    global_rank: 16
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - 0.537
    - null
    - null
    metric_stds:
    - 0.0142
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.554
    sort_std: 0.002
    true_value: 0.554
    true_std: 0.002
    paper_value: 0.537
    paper_std: 0.0142
    has_value_gap: true
    has_value_note: false
    value_gap: 0.017000000000000015
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_note: ''
    at_pub_value: 0.554
    at_pub_std: 0.002
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.017000000000000015
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
    is_best: false
    is_std_outlier: false
    global_rank: 17
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.5108
    - 0.387
    - 0.744
    metric_stds:
    - 0.0159
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5411
    sort_std: 0.0034
    true_value: 0.5411
    true_std: 0.0034
    paper_value: 0.5108
    paper_std: 0.0159
    has_value_gap: true
    has_value_note: false
    value_gap: 0.030299999999999994
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_note: ''
    at_pub_value: 0.5411
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2605.20248'
    at_pub_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    at_pub_source_date_iso: '2026-05-18'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.030299999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled
      Predictions in Node Classification'
    comparison_source_arxiv: '2605.20248'
    is_best: false
    is_std_outlier: false
    global_rank: 26
  - model: GCN-MAS
    model_key: gcn-mas
    model_plain: GCN-MAS
    metric_values:
    - 0.5354
    - 0.418
    - 0.771
    metric_stds:
    - 0.0159
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5354
    sort_std: 0.0159
    true_value: 0.5354
    true_std: 0.0159
    paper_value: 0.5354
    paper_std: 0.0159
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 34
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    metric_values:
    - 0.4587
    - null
    - null
    metric_stds:
    - 0.0292
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.5351
    sort_std: 0.0046
    true_value: 0.5351
    true_std: 0.0046
    paper_value: 0.4587
    paper_std: 0.0292
    has_value_gap: true
    has_value_note: false
    value_gap: 0.07640000000000002
    value_gap_source_arxiv: '2510.21267'
    value_gap_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    value_note: ''
    at_pub_value: 0.5351
    at_pub_std: 0.0046
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.07640000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    comparison_source_arxiv: '2402.08678'
    is_best: false
    is_std_outlier: false
    global_rank: 35
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    metric_values:
    - 0.4358
    - 0.292
    - 0.689
    metric_stds:
    - 0.0268
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.5327
    sort_std: 0.0066
    true_value: 0.5327
    true_std: 0.0066
    paper_value: 0.4358
    paper_std: 0.0268
    has_value_gap: true
    has_value_note: false
    value_gap: 0.09689999999999993
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_note: ''
    at_pub_value: 0.5327
    at_pub_std: 0.0066
    at_pub_source_arxiv: '2605.20248'
    at_pub_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    at_pub_source_date_iso: '2026-05-18'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.09689999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled
      Predictions in Node Classification'
    comparison_source_arxiv: '2605.20248'
    is_best: false
    is_std_outlier: false
    global_rank: 42
  - model: GCN-TAS
    model_key: gcn-tas
    model_plain: GCN-TAS
    metric_values:
    - 0.5274
    - 0.402
    - 0.756
    metric_stds:
    - 0.0109
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5274
    sort_std: 0.0109
    true_value: 0.5274
    true_std: 0.0109
    paper_value: 0.5274
    paper_std: 0.0109
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 55
  - model: CMGNN
    model_key: cmgnn
    model_plain: CMGNN
    metric_values:
    - 0.5155
    - null
    - null
    metric_stds:
    - 0.0162
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5257
    sort_std: 0.0082
    true_value: 0.5257
    true_std: 0.0082
    paper_value: 0.5155
    paper_std: 0.0162
    has_value_gap: true
    has_value_note: false
    value_gap: 0.010199999999999987
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_note: ''
    at_pub_value: 0.5257
    at_pub_std: 0.0082
    at_pub_source_arxiv: '2512.14908'
    at_pub_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for Homophilic
      and Heterophilic Graphs'
    at_pub_source_date_iso: '2025-12-16'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.010199999999999987
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 60
  - model: VCR
    model_key: vcr
    model_plain: VCR
    metric_values:
    - 0.5174
    - 0.388
    - 0.731
    metric_stds:
    - 0.0077
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.5174
    sort_std: 0.0077
    true_value: 0.5174
    true_std: 0.0077
    paper_value: 0.5174
    paper_std: 0.0077
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 72
  - model: VCR-TAS
    model_key: vcr-tas
    model_plain: VCR-TAS
    metric_values:
    - 0.5135
    - 0.385
    - 0.74
    metric_stds:
    - 0.0101
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.5135
    sort_std: 0.0101
    true_value: 0.5135
    true_std: 0.0101
    paper_value: 0.5135
    paper_std: 0.0101
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 78
  - model: GT
    model_key: gt
    model_plain: GT
    metric_values:
    - 0.485
    - null
    - null
    metric_stds:
    - 0.0401
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5117
    sort_std: 0.0066
    true_value: 0.5117
    true_std: 0.0066
    paper_value: 0.485
    paper_std: 0.0401
    has_value_gap: true
    has_value_note: false
    value_gap: 0.026700000000000057
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_note: ''
    at_pub_value: 0.5117
    at_pub_std: 0.0066
    at_pub_source_arxiv: '2405.15540'
    at_pub_source_title: Bundle Neural Networks for message diffusion on graphs
    at_pub_source_date_iso: '2024-05-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.026700000000000057
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 81
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.5058
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2401.09125'
    title: Understanding Heterophily for Graph Neural Networks
    published_venue: ''
    date: Jan 17, 2024
    date_display: Jan 2024
    date_iso: '2024-01-17'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 95
    is_best: false
    sort_value: 0.5058
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: SAN
    model_key: san
    model_plain: SAN
    metric_values:
    - 0.5028
    - null
    - null
    metric_stds:
    - 0.0233
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.5028
    sort_std: 0.0233
    true_value: 0.5028
    true_std: 0.0233
    paper_value: 0.5028
    paper_std: 0.0233
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 97
  - model: CR-TAS
    model_key: cr-tas
    model_plain: CR-TAS
    metric_values:
    - 0.4807
    - 0.318
    - 0.704
    metric_stds:
    - 0.0136
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.4807
    sort_std: 0.0136
    true_value: 0.4807
    true_std: 0.0136
    paper_value: 0.4807
    paper_std: 0.0136
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 137
  - model: NAG
    model_key: nag
    model_plain: NAG
    metric_values:
    - 0.4769
    - 0.356
    - 0.7
    metric_stds:
    - 0.0263
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.4769
    sort_std: 0.0263
    true_value: 0.4769
    true_std: 0.0263
    paper_value: 0.4769
    paper_std: 0.0263
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 142
  - model: VCR-MAS
    model_key: vcr-mas
    model_plain: VCR-MAS
    metric_values:
    - 0.4681
    - 0.315
    - 0.711
    metric_stds:
    - 0.014
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.4681
    sort_std: 0.014
    true_value: 0.4681
    true_std: 0.014
    paper_value: 0.4681
    paper_std: 0.014
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 147
  - model: NAG-TAS
    model_key: nag-tas
    model_plain: NAG-TAS
    metric_values:
    - 0.4669
    - 0.332
    - 0.705
    metric_stds:
    - 0.0056
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.4669
    sort_std: 0.0056
    true_value: 0.4669
    true_std: 0.0056
    paper_value: 0.4669
    paper_std: 0.0056
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 149
  - model: NAG-MAS
    model_key: nag-mas
    model_plain: NAG-MAS
    metric_values:
    - 0.4632
    - 0.335
    - 0.699
    metric_stds:
    - 0.0208
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.4632
    sort_std: 0.0208
    true_value: 0.4632
    true_std: 0.0208
    paper_value: 0.4632
    paper_std: 0.0208
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 153
  - model: CR-MAS
    model_key: cr-mas
    model_plain: CR-MAS
    metric_values:
    - 0.463
    - 0.336
    - 0.709
    metric_stds:
    - 0.0163
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.463
    sort_std: 0.0163
    true_value: 0.463
    true_std: 0.0163
    paper_value: 0.463
    paper_std: 0.0163
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 154
  - model: GPS-TAS
    model_key: gps-tas
    model_plain: GPS-TAS
    metric_values:
    - 0.4543
    - 0.284
    - 0.694
    metric_stds:
    - 0.0134
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.4543
    sort_std: 0.0134
    true_value: 0.4543
    true_std: 0.0134
    paper_value: 0.4543
    paper_std: 0.0134
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 162
  - model: GPS-MAS
    model_key: gps-mas
    model_plain: GPS-MAS
    metric_values:
    - 0.4529
    - 0.325
    - 0.71
    metric_stds:
    - 0.0328
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.4529
    sort_std: 0.0328
    true_value: 0.4529
    true_std: 0.0328
    paper_value: 0.4529
    paper_std: 0.0328
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 163
  - model: Gophormer
    model_key: gophormer
    model_plain: Gophormer
    metric_values:
    - 0.4379
    - null
    - null
    metric_stds:
    - 0.011
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.4379
    sort_std: 0.011
    true_value: 0.4379
    true_std: 0.011
    paper_value: 0.4379
    paper_std: 0.011
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 181
  metrics:
  - Accuracy
  - macro-F1
  - AUROC
  primary_metric: Accuracy
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  - macro-F1
  - AUROC
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: COCO-SP
  rows:
  - model: CRaWl
    model_key: crawl
    model_plain: CRaWl
    value: 0.4588
    std: 0.0079
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    sort_value: 0.4588
    sort_std: 0.0079
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.444
    std: 0.0065
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    sort_value: 0.444
    sort_std: 0.0065
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NeuralWalker
    model_key: neuralwalker
    model_plain: NeuralWalker
    value: 0.4398
    std: 0.0033
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2510.12111'
    title: 'Chimera: State Space Models Beyond Sequences'
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/goombalab/chimera
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.4398
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.388
    std: 0.004
    metric: F1
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
    global_rank: 14
    sort_value: 0.388
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.063
    std: null
    paper_value: 0.063
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2078
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2605.13383'
    at_pub_source_title: 'Beyond Oversquashing: Understanding Signal Propagation in
      GNNs Via Observables'
    at_pub_source_date_iso: '2026-05-13'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.1448
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2078
    true_std: 0.0031
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: 0.1448
    has_value_note: false
    value_note: ''
    sort_value: 0.2078
    sort_std: 0.0031
    global_rank: 46
    paper_rank: 71
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    comparison_source_arxiv: '2605.13383'
    is_best: false
    is_std_outlier: false
  - model: VCR-TAS
    model_key: vcr-tas
    model_plain: VCR-TAS
    value: 0.144
    std: null
    paper_value: 0.144
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.144
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.144
    sort_std: null
    global_rank: 52
    paper_rank: 52
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NAG-MAS
    model_key: nag-mas
    model_plain: NAG-MAS
    value: 0.137
    std: null
    paper_value: 0.137
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.137
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.137
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.1339
    std: 0.0044
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_display: Feb 2024
    date_iso: '2024-02-13'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 54
    sort_value: 0.1339
    sort_std: 0.0044
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NAG-TAS
    model_key: nag-tas
    model_plain: NAG-TAS
    value: 0.131
    std: null
    paper_value: 0.131
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.131
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.131
    sort_std: null
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
  - model: VCR-MAS
    model_key: vcr-mas
    model_plain: VCR-MAS
    value: 0.124
    std: null
    paper_value: 0.124
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.124
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.124
    sort_std: null
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
  - model: VCR
    model_key: vcr
    model_plain: VCR
    value: 0.102
    std: null
    paper_value: 0.102
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.102
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.102
    sort_std: null
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
  - model: NAG
    model_key: nag
    model_plain: NAG
    value: 0.074
    std: null
    paper_value: 0.074
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.074
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.074
    sort_std: null
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
  - model: GCN-MAS
    model_key: gcn-mas
    model_plain: GCN-MAS
    value: 0.07
    std: null
    paper_value: 0.07
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.07
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.07
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
  - model: CR-MAS
    model_key: cr-mas
    model_plain: CR-MAS
    value: 0.07
    std: null
    paper_value: 0.07
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.07
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.07
    sort_std: null
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
  - model: CR-TAS
    model_key: cr-tas
    model_plain: CR-TAS
    value: 0.069
    std: null
    paper_value: 0.069
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.069
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.069
    sort_std: null
    global_rank: 70
    paper_rank: 70
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN-TAS
    model_key: gcn-tas
    model_plain: GCN-TAS
    value: 0.068
    std: null
    paper_value: 0.068
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.068
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.068
    sort_std: null
    global_rank: 71
    paper_rank: 71
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.063
    std: null
    paper_value: 0.063
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.063
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.063
    sort_std: null
    global_rank: 72
    paper_rank: 72
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS-MAS
    model_key: gps-mas
    model_plain: GPS-MAS
    value: 0.063
    std: null
    paper_value: 0.063
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.063
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.063
    sort_std: null
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
  - model: GPS-TAS
    model_key: gps-tas
    model_plain: GPS-TAS
    value: 0.063
    std: null
    paper_value: 0.063
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on COCO-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.063
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.063
    sort_std: null
    global_rank: 74
    paper_rank: 74
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
    value: 0.031
    std: 0.016
    metric: F1
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
    global_rank: 77
    sort_value: 0.031
    sort_std: 0.016
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
  dataset: PascalVOC-SP
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.138
    std: null
    paper_value: 0.138
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.78
    at_pub_std: 0.31
    at_pub_source_arxiv: '2411.12732'
    at_pub_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    at_pub_source_date_iso: '2024-11-19'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.642
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.78
    true_std: 0.31
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.642
    has_value_note: false
    value_note: ''
    sort_value: 0.78
    sort_std: 0.31
    global_rank: 1
    paper_rank: 109
    rank_delta: 108
    rank_delta_abs: 108
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Benchmarking Positional Encodings for GNNs and Graph
      Transformers
    comparison_source_arxiv: '2411.12732'
    is_best: true
    is_std_outlier: true
  - model: NeuralWalker
    model_key: neuralwalker
    model_plain: NeuralWalker
    value: 0.4912
    std: 0.0042
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2510.12111'
    title: 'Chimera: State Space Models Beyond Sequences'
    date: Oct 14, 2025
    date_display: Oct 2025
    date_iso: '2025-10-14'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/goombalab/chimera
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.4912
    sort_std: 0.0042
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: PPGT
    model_key: ppgt
    model_plain: PPGT
    value: 0.4641
    std: 0.0033
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2504.12588'
    title: Plain Transformers Can be Powerful Graph Learners
    date: Apr 17, 2025
    date_display: Apr 2025
    date_iso: '2025-04-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: utilize relative random walk probabilities (RRWP) as
      our demonstrating example of graph PE
    is_global_top: true
    global_rank: 3
    sort_value: 0.4641
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    value: 0.092
    std: null
    paper_value: 0.092
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4538
    at_pub_std: 0.83
    at_pub_source_arxiv: '2411.12732'
    at_pub_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    at_pub_source_date_iso: '2024-11-19'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.3618
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.4538
    true_std: 0.83
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.3618
    has_value_note: false
    value_note: ''
    sort_value: 0.4538
    sort_std: 0.83
    global_rank: 6
    paper_rank: 115
    rank_delta: 109
    rank_delta_abs: 109
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: true
  - model: NAG-TAS
    model_key: nag-tas
    model_plain: NAG-TAS
    value: 0.254
    std: null
    paper_value: 0.254
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.254
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.254
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
  - model: VCR-TAS
    model_key: vcr-tas
    model_plain: VCR-TAS
    value: 0.254
    std: null
    paper_value: 0.254
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.254
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.254
    sort_std: null
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
  - model: NAG-MAS
    model_key: nag-mas
    model_plain: NAG-MAS
    value: 0.24
    std: null
    paper_value: 0.24
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.24
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.24
    sort_std: null
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
  - model: VCR-MAS
    model_key: vcr-mas
    model_plain: VCR-MAS
    value: 0.222
    std: null
    paper_value: 0.222
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.222
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.222
    sort_std: null
    global_rank: 97
    paper_rank: 97
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VCR
    model_key: vcr
    model_plain: VCR
    value: 0.196
    std: null
    paper_value: 0.196
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.196
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.196
    sort_std: null
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
  - model: CR-MAS
    model_key: cr-mas
    model_plain: CR-MAS
    value: 0.172
    std: null
    paper_value: 0.172
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.172
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.172
    sort_std: null
    global_rank: 104
    paper_rank: 104
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CR-TAS
    model_key: cr-tas
    model_plain: CR-TAS
    value: 0.171
    std: null
    paper_value: 0.171
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.171
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.171
    sort_std: null
    global_rank: 105
    paper_rank: 105
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN-MAS
    model_key: gcn-mas
    model_plain: GCN-MAS
    value: 0.152
    std: null
    paper_value: 0.152
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.152
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.152
    sort_std: null
    global_rank: 109
    paper_rank: 109
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NAG
    model_key: nag
    model_plain: NAG
    value: 0.138
    std: null
    paper_value: 0.138
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.138
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.138
    sort_std: null
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
  - model: GCN-TAS
    model_key: gcn-tas
    model_plain: GCN-TAS
    value: 0.13
    std: null
    paper_value: 0.13
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.13
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.13
    sort_std: null
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
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.1265
    std: 0.0076
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_display: Feb 2024
    date_iso: '2024-02-13'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 114
    sort_value: 0.1265
    sort_std: 0.0076
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.114
    std: 0.023
    metric: F1
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
    global_rank: 115
    sort_value: 0.114
    sort_std: 0.023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS-MAS
    model_key: gps-mas
    model_plain: GPS-MAS
    value: 0.092
    std: null
    paper_value: 0.092
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.092
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.092
    sort_std: null
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
  - model: GPS-TAS
    model_key: gps-tas
    model_plain: GPS-TAS
    value: 0.092
    std: null
    paper_value: 0.092
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 14
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: macro-F1 on PascalVOC-SP test split
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.092
    true_std: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.092
    sort_std: null
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
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id005
  dataset: Questions
  is_multi_metric: true
  rows:
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    metric_values:
    - null
    - 0.9349
    - 0.492
    metric_stds:
    - null
    - 0.004
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.9349
    sort_std: 0.004
    true_value: 0.9349
    true_std: 0.004
    paper_value: 0.9349
    paper_std: 0.004
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 77
  - model: GraphSAGE + UniGAP
    model_key: graphsage + unigap
    model_plain: GraphSAGE + UniGAP
    metric_values:
    - 0.8421
    - null
    - null
    metric_stds:
    - 0.008
    - null
    - null
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
    published_venue: ''
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: false
    sort_value: 0.8421
    sort_std: 0.008
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: H2GCN + UniGAP
    model_key: h2gcn + unigap
    model_plain: H2GCN + UniGAP
    metric_values:
    - 0.8359
    - null
    - null
    metric_stds:
    - 0.007
    - null
    - null
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
    published_venue: ''
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.8359
    sort_std: 0.007
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GCN + UniGAP
    model_key: gcn + unigap
    model_plain: GCN + UniGAP
    metric_values:
    - 0.8273
    - null
    - null
    metric_stds:
    - 0.009
    - null
    - null
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
    published_venue: ''
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.8273
    sort_std: 0.009
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.54
    - 0.9329
    - 0.486
    metric_stds:
    - null
    - 0.003
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7902
    sort_std: 0.006
    true_value: 0.7902
    true_std: 0.006
    paper_value: 0.54
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.2502
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_note: ''
    at_pub_value: 0.7902
    at_pub_std: 0.006
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.2502
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    comparison_source_arxiv: '2405.20445'
    is_best: false
    is_std_outlier: false
    global_rank: 17
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - 0.7721
    - null
    - null
    metric_stds:
    - 0.013
    - null
    - null
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
    published_venue: ''
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 48
    is_best: false
    sort_value: 0.7721
    sort_std: 0.013
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: NAG-MAS
    model_key: nag-mas
    model_plain: NAG-MAS
    metric_values:
    - 0.713
    - 0.9356
    - 0.528
    metric_stds:
    - null
    - 0.0039
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.713
    sort_std: null
    true_value: 0.713
    true_std: null
    paper_value: 0.713
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 98
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.7082
    - null
    - null
    metric_stds:
    - 0.001
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2508.17531'
    title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    published_venue: ''
    date: Aug 24, 2025
    date_display: Aug 2025
    date_iso: '2025-08-24'
    codebase_url: https://github.com/Bobowner/Gumbel-Softmax-MPNN
    uses_external_data: false
    is_global_top: true
    global_rank: 104
    is_best: false
    sort_value: 0.7082
    sort_std: 0.001
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: CR-MAS
    model_key: cr-mas
    model_plain: CR-MAS
    metric_values:
    - 0.706
    - 0.9351
    - 0.505
    metric_stds:
    - null
    - 0.0043
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.706
    sort_std: null
    true_value: 0.706
    true_std: null
    paper_value: 0.706
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 110
  - model: NAG
    model_key: nag
    model_plain: NAG
    metric_values:
    - 0.702
    - 0.937
    - 0.533
    metric_stds:
    - null
    - 0.0036
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.702
    sort_std: null
    true_value: 0.702
    true_std: null
    paper_value: 0.702
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 114
  - model: CR-TAS
    model_key: cr-tas
    model_plain: CR-TAS
    metric_values:
    - 0.697
    - 0.9376
    - 0.543
    metric_stds:
    - null
    - 0.0038
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.697
    sort_std: null
    true_value: 0.697
    true_std: null
    paper_value: 0.697
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 119
  - model: NAG-TAS
    model_key: nag-tas
    model_plain: NAG-TAS
    metric_values:
    - 0.691
    - 0.9346
    - 0.532
    metric_stds:
    - null
    - 0.004
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.691
    sort_std: null
    true_value: 0.691
    true_std: null
    paper_value: 0.691
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 124
  - model: GPS
    model_key: gps
    model_plain: GPS
    metric_values:
    - 0.681
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.681
    sort_std: null
    true_value: 0.681
    true_std: null
    paper_value: 0.681
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 129
  - model: GPS-MAS
    model_key: gps-mas
    model_plain: GPS-MAS
    metric_values:
    - 0.661
    - 0.9349
    - 0.506
    metric_stds:
    - null
    - 0.0037
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.661
    sort_std: null
    true_value: 0.661
    true_std: null
    paper_value: 0.661
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 135
  - model: GPS-TAS
    model_key: gps-tas
    model_plain: GPS-TAS
    metric_values:
    - 0.657
    - 0.935
    - 0.51
    metric_stds:
    - null
    - 0.0036
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.657
    sort_std: null
    true_value: 0.657
    true_std: null
    paper_value: 0.657
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 138
  - model: GCN-MAS
    model_key: gcn-mas
    model_plain: GCN-MAS
    metric_values:
    - 0.654
    - 0.935
    - 0.517
    metric_stds:
    - null
    - 0.0036
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.654
    sort_std: null
    true_value: 0.654
    true_std: null
    paper_value: 0.654
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 139
  - model: VCR-TAS
    model_key: vcr-tas
    model_plain: VCR-TAS
    metric_values:
    - 0.642
    - 0.9352
    - 0.491
    metric_stds:
    - null
    - 0.0041
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.642
    sort_std: null
    true_value: 0.642
    true_std: null
    paper_value: 0.642
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 143
  - model: GCN-TAS
    model_key: gcn-tas
    model_plain: GCN-TAS
    metric_values:
    - 0.64
    - 0.935
    - 0.489
    metric_stds:
    - null
    - 0.0036
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.64
    sort_std: null
    true_value: 0.64
    true_std: null
    paper_value: 0.64
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 144
  - model: VCR-MAS
    model_key: vcr-mas
    model_plain: VCR-MAS
    metric_values:
    - 0.627
    - 0.9354
    - 0.492
    metric_stds:
    - null
    - 0.0037
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.627
    sort_std: null
    true_value: 0.627
    true_std: null
    paper_value: 0.627
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 148
  - model: VCR
    model_key: vcr
    model_plain: VCR
    metric_values:
    - 0.597
    - 0.935
    - 0.483
    metric_stds:
    - null
    - 0.0036
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.597
    sort_std: null
    true_value: 0.597
    true_std: null
    paper_value: 0.597
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 152
  metrics:
  - ROC-AUC
  - Accuracy
  - macro-F1
  primary_metric: ROC-AUC
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  - macro-F1
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: Roman-empire
  is_multi_metric: true
  rows:
  - model: GPS
    model_key: gps
    model_plain: GPS
    metric_values:
    - null
    - null
    - 0.949
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.949
    sort_std: null
    true_value: 0.949
    true_std: null
    paper_value: 0.949
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 91
  - model: Dir-NT
    model_key: dir-nt
    model_plain: Dir-NT
    metric_values:
    - 0.9477
    - null
    - null
    metric_stds:
    - 0.0031
    - null
    - null
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
    published_venue: ''
    date: Apr 10, 2026
    date_display: Apr 2026
    date_iso: '2026-04-10'
    codebase_url: https://github.com/cf020031308/MoNT
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.9477
    sort_std: 0.0031
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: Dir-Poly
    model_key: dir-poly
    model_plain: Dir-Poly
    metric_values:
    - 0.9451
    - null
    - null
    metric_stds:
    - 0.0022
    - null
    - null
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
    published_venue: ''
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.9451
    sort_std: 0.0022
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: D-CDE
    model_key: d-cde
    model_plain: D-CDE
    metric_values:
    - 0.9387
    - null
    - null
    metric_stds:
    - 0.0041
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.05274'
    title: Distributed-Order Fractional Graph Operating Network
    published_venue: ''
    date: Nov 8, 2024
    date_display: Nov 2024
    date_iso: '2024-11-08'
    codebase_url: https://github.com/zknus/NeurIPS-2024-DRAGON
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.9387
    sort_std: 0.0041
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    metric_values:
    - 0.6664
    - null
    - null
    metric_stds:
    - 0.0127
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9106
    sort_std: 0.0027
    true_value: 0.9106
    true_std: 0.0027
    paper_value: 0.6664
    paper_std: 0.0127
    has_value_gap: true
    has_value_note: false
    value_gap: 0.24419999999999997
    value_gap_source_arxiv: '2505.17939'
    value_gap_source_title: Directed Semi-Simplicial Learning with Applications to
      Brain Activity Decoding
    value_note: ''
    at_pub_value: 0.9106
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2505.17939'
    at_pub_source_title: Directed Semi-Simplicial Learning with Applications to Brain
      Activity Decoding
    at_pub_source_date_iso: '2025-05-23'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-23'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.24419999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Directed Semi-Simplicial Learning with Applications to
      Brain Activity Decoding
    comparison_source_arxiv: '2505.17939'
    is_best: false
    is_std_outlier: false
    global_rank: 29
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    metric_values:
    - 0.6657
    - null
    - null
    metric_stds:
    - 0.0096
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.8903
    sort_std: 0.0037
    true_value: 0.8903
    true_std: 0.0037
    paper_value: 0.6657
    paper_std: 0.0096
    has_value_gap: true
    has_value_note: false
    value_gap: 0.22460000000000002
    value_gap_source_arxiv: '2510.21267'
    value_gap_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    value_note: ''
    at_pub_value: 0.8903
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.22460000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    comparison_source_arxiv: '2402.08678'
    is_best: false
    is_std_outlier: false
    global_rank: 42
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - 0.3831
    - null
    - null
    metric_stds:
    - 0.0173
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8875
    sort_std: 0.0041
    true_value: 0.8875
    true_std: 0.0041
    paper_value: 0.3831
    paper_std: 0.0173
    has_value_gap: true
    has_value_note: false
    value_gap: 0.5044
    value_gap_source_arxiv: '2510.21267'
    value_gap_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    value_note: ''
    at_pub_value: 0.8875
    at_pub_std: 0.0041
    at_pub_source_arxiv: '2510.21267'
    at_pub_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    at_pub_source_date_iso: '2025-10-24'
    at_pub_source_date_label: NeurIPS 2025
    value_gap_source_date_iso: '2025-10-24'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: 0.5044
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Relieving the Over-Aggregating Effect in Graph Transformers
    comparison_source_arxiv: '2510.21267'
    is_best: false
    is_std_outlier: false
    global_rank: 45
  - model: GT
    model_key: gt
    model_plain: GT
    metric_values:
    - 0.6589
    - null
    - null
    metric_stds:
    - 0.0188
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8651
    sort_std: 0.0073
    true_value: 0.8651
    true_std: 0.0073
    paper_value: 0.6589
    paper_std: 0.0188
    has_value_gap: true
    has_value_note: false
    value_gap: 0.20619999999999994
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_note: ''
    at_pub_value: 0.8651
    at_pub_std: 0.0073
    at_pub_source_arxiv: '2405.15540'
    at_pub_source_title: Bundle Neural Networks for message diffusion on graphs
    at_pub_source_date_iso: '2024-05-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.20619999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Bundle Neural Networks for message diffusion on graphs
    comparison_source_arxiv: '2405.15540'
    is_best: false
    is_std_outlier: false
    global_rank: 67
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - 0.8574
    - null
    - null
    metric_stds:
    - 0.0067
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2508.05070'
    title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
    published_venue: ''
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 72
    is_best: false
    sort_value: 0.8574
    sort_std: 0.0067
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: CMGNN
    model_key: cmgnn
    model_plain: CMGNN
    metric_values:
    - 0.6875
    - null
    - null
    metric_stds:
    - 0.0108
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8442
    sort_std: 0.0166
    true_value: 0.8442
    true_std: 0.0166
    paper_value: 0.6875
    paper_std: 0.0108
    has_value_gap: true
    has_value_note: false
    value_gap: 0.15669999999999995
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_note: ''
    at_pub_value: 0.8442
    at_pub_std: 0.0166
    at_pub_source_arxiv: '2512.14908'
    at_pub_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for Homophilic
      and Heterophilic Graphs'
    at_pub_source_date_iso: '2025-12-16'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.15669999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    comparison_source_arxiv: '2512.14908'
    is_best: false
    is_std_outlier: false
    global_rank: 78
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - 0.3681
    - 0.29
    - 0.855
    metric_stds:
    - 0.0055
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8272
    sort_std: 0.0082
    true_value: 0.8272
    true_std: 0.0082
    paper_value: 0.3681
    paper_std: 0.0055
    has_value_gap: true
    has_value_note: false
    value_gap: 0.45910000000000006
    value_gap_source_arxiv: '2407.11596'
    value_gap_source_title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    value_note: ''
    at_pub_value: 0.8272
    at_pub_std: 0.0082
    at_pub_source_arxiv: '2407.11596'
    at_pub_source_title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    at_pub_source_date_iso: '2024-06-30'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.45910000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'HyperAggregation: Aggregating over Graph Edges with
      Hypernetworks'
    comparison_source_arxiv: '2407.11596'
    is_best: false
    is_std_outlier: false
    global_rank: 85
  - model: GraphGPS
    model_key: graphgps
    model_plain: GraphGPS
    metric_values:
    - 0.6681
    - 0.583
    - null
    metric_stds:
    - 0.0028
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.8272
    sort_std: 0.0068
    true_value: 0.8272
    true_std: 0.0068
    paper_value: 0.6681
    paper_std: 0.0028
    has_value_gap: true
    has_value_note: false
    value_gap: 0.15910000000000002
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_note: ''
    at_pub_value: 0.8272
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2411.19392'
    at_pub_source_title: Scale-aware Message Passing For Graph Node Classification
    at_pub_source_date_iso: '2024-11-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.15910000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: Scale-aware Message Passing For Graph Node Classification
    comparison_source_arxiv: '2411.19392'
    is_best: false
    is_std_outlier: false
    global_rank: 86
  - model: SAN
    model_key: san
    model_plain: SAN
    metric_values:
    - 0.6804
    - null
    - null
    metric_stds:
    - 0.0102
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.6804
    sort_std: 0.0102
    true_value: 0.6804
    true_std: 0.0102
    paper_value: 0.6804
    paper_std: 0.0102
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 147
  - model: Gophormer
    model_key: gophormer
    model_plain: Gophormer
    metric_values:
    - 0.6735
    - null
    - null
    metric_stds:
    - 0.0214
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.6735
    sort_std: 0.0214
    true_value: 0.6735
    true_std: 0.0214
    paper_value: 0.6735
    paper_std: 0.0214
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 149
  - model: ACMGCN
    model_key: acmgcn
    model_plain: ACMGCN
    metric_values:
    - 0.6689
    - null
    - null
    metric_stds:
    - 0.0135
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6689
    sort_std: 0.0135
    true_value: 0.6689
    true_std: 0.0135
    paper_value: 0.6689
    paper_std: 0.0135
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 150
  - model: MLP
    model_key: mlp
    model_plain: MLP
    metric_values:
    - 0.6665
    - null
    - null
    metric_stds:
    - 0.0047
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.11596'
    title: 'HyperAggregation: Aggregating over Graph Edges with Hypernetworks'
    published_venue: ''
    date: Jun 30, 2024
    date_display: Jun 2024
    date_iso: '2024-06-30'
    codebase_url: https://github.com/Foisunt/HyperAggregation
    uses_external_data: false
    is_global_top: true
    global_rank: 151
    is_best: false
    sort_value: 0.6665
    sort_std: 0.0047
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: GPS-TAS
    model_key: gps-tas
    model_plain: GPS-TAS
    metric_values:
    - 0.6471
    - 0.557
    - 0.941
    metric_stds:
    - 0.0171
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.6471
    sort_std: 0.0171
    true_value: 0.6471
    true_std: 0.0171
    paper_value: 0.6471
    paper_std: 0.0171
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 162
  - model: NAG-TAS
    model_key: nag-tas
    model_plain: NAG-TAS
    metric_values:
    - 0.6217
    - 0.451
    - 0.919
    metric_stds:
    - 0.0177
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.6217
    sort_std: 0.0177
    true_value: 0.6217
    true_std: 0.0177
    paper_value: 0.6217
    paper_std: 0.0177
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 177
  - model: CR-TAS
    model_key: cr-tas
    model_plain: CR-TAS
    metric_values:
    - 0.5982
    - 0.463
    - 0.913
    metric_stds:
    - 0.0209
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.5982
    sort_std: 0.0209
    true_value: 0.5982
    true_std: 0.0209
    paper_value: 0.5982
    paper_std: 0.0209
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 183
  - model: NAG-MAS
    model_key: nag-mas
    model_plain: NAG-MAS
    metric_values:
    - 0.5908
    - 0.439
    - 0.91
    metric_stds:
    - 0.0172
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.5908
    sort_std: 0.0172
    true_value: 0.5908
    true_std: 0.0172
    paper_value: 0.5908
    paper_std: 0.0172
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 185
  - model: NAG
    model_key: nag
    model_plain: NAG
    metric_values:
    - 0.5808
    - 0.444
    - 0.912
    metric_stds:
    - 0.0159
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.5808
    sort_std: 0.0159
    true_value: 0.5808
    true_std: 0.0159
    paper_value: 0.5808
    paper_std: 0.0159
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 188
  - model: VCR-MAS
    model_key: vcr-mas
    model_plain: VCR-MAS
    metric_values:
    - 0.577
    - 0.442
    - 0.906
    metric_stds:
    - 0.0112
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.577
    sort_std: 0.0112
    true_value: 0.577
    true_std: 0.0112
    paper_value: 0.577
    paper_std: 0.0112
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 189
  - model: VCR-TAS
    model_key: vcr-tas
    model_plain: VCR-TAS
    metric_values:
    - 0.576
    - 0.445
    - 0.906
    metric_stds:
    - 0.0219
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.576
    sort_std: 0.0219
    true_value: 0.576
    true_std: 0.0219
    paper_value: 0.576
    paper_std: 0.0219
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 191
  - model: GPS-MAS
    model_key: gps-mas
    model_plain: GPS-MAS
    metric_values:
    - 0.5759
    - 0.464
    - 0.91
    metric_stds:
    - 0.0075
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.5759
    sort_std: 0.0075
    true_value: 0.5759
    true_std: 0.0075
    paper_value: 0.5759
    paper_std: 0.0075
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 192
  - model: CR-MAS
    model_key: cr-mas
    model_plain: CR-MAS
    metric_values:
    - 0.5519
    - 0.401
    - 0.895
    metric_stds:
    - 0.0097
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.5519
    sort_std: 0.0097
    true_value: 0.5519
    true_std: 0.0097
    paper_value: 0.5519
    paper_std: 0.0097
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 196
  - model: GCN-MAS
    model_key: gcn-mas
    model_plain: GCN-MAS
    metric_values:
    - 0.3636
    - 0.257
    - 0.798
    metric_stds:
    - 0.0101
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3636
    sort_std: 0.0101
    true_value: 0.3636
    true_std: 0.0101
    paper_value: 0.3636
    paper_std: 0.0101
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 219
  - model: GCN-TAS
    model_key: gcn-tas
    model_plain: GCN-TAS
    metric_values:
    - 0.3457
    - 0.264
    - 0.843
    metric_stds:
    - 0.0122
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3457
    sort_std: 0.0122
    true_value: 0.3457
    true_std: 0.0122
    paper_value: 0.3457
    paper_std: 0.0122
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 224
  - model: VCR
    model_key: vcr
    model_plain: VCR
    metric_values:
    - 0.1865
    - 0.108
    - 0.722
    metric_stds:
    - 0.0098
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    sort_value: 0.1865
    sort_std: 0.0098
    true_value: 0.1865
    true_std: 0.0098
    paper_value: 0.1865
    paper_std: 0.0098
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2606.05046'
    value_gap_source_title: 'Graph Cascades: Contagion-Based Mesoscopic Rewiring for
      Structure-Aware Graph Machine Learning'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-06-03'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Jun 3, 2026
    date_display: Jun 2026
    date_iso: '2026-06-03'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 241
  metrics:
  - Accuracy
  - macro-F1
  - AUROC
  primary_metric: Accuracy
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  - macro-F1
  - AUROC
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: LRGB
  datasets:
  - *id001
  - *id002
- benchmark: Heterophily Benchmark
  datasets:
  - *id003
  - *id004
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: PascalVOC-SP
      dataset_slug: pascalvoc-sp
    - dataset: COCO-SP
      dataset_slug: coco-sp
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Roman-empire
      dataset_slug: roman-empire
    - dataset: Amazon-ratings
      dataset_slug: amazon-ratings
    - dataset: Questions
      dataset_slug: questions
main_figure: /figures/2606.05046/main_figure.jpegoptim.jpg
---

