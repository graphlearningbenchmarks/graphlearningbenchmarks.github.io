---
title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
arxiv_id: '2508.05070'
source_url: ''
authors:
- name: Moshe Eliasof
  orcid: null
  s2_author_id: '104172497'
  s2_url: null
- name: Eldad Haber
  orcid: null
  s2_author_id: '2257221683'
  s2_url: null
- name: C. Schönlieb
  orcid: null
  s2_author_id: '1711104'
  s2_url: null
published_date: Aug 7, 2025
published_date_iso: '2025-08-07'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: We introduce TANGO -- a dynamical systems inspired framework for graph representation
  learning that governs node feature evolution through a learned energy landscape
  and its associated descent dynamics. At the core of our approach is a learnable
  Lyapunov function over node embeddings, whose gradient defines an energy-reducing
  direction that guarantees convergence and stability. To enhance flexibility while
  preserving the benefits of energy-based dynamics, we incorporate a novel tangential
  component, learned via message passing, that evolves features while maintaining
  the energy value. This decomposition into orthogonal flows of energy gradient descent
  and tangential evolution yields a flexible form of graph dynamics, and enables effective
  signal propagation even in flat or ill-conditioned energy regions, that often appear
  in graph learning. Our method mitigates oversquashing and is compatible with different
  graph neural network backbones. Empirically, TANGO achieves strong performance across
  a diverse set of node and graph classification and regression benchmarks, demonstrating
  the effectiveness of jointly learned energy functions and tangential flows for graph
  neural networks.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- Tango_GatedGCN
- Tango_GPS
- Tango GatedGCN
- Tango GPS
mrr: 0.0585
adjusted_mrr: 0.0585
mrr_dataset_count: 9
benchmark_categories:
- LRGB
- Heterophily Benchmark
- GNNBenchmark
- Algorithmic Graph Tasks
benchmark_coverage:
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 2
  total: 5
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 5
  total: 5
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 4
  total: 6
- benchmark: Algorithmic Graph Tasks
  benchmark_slug: algorithmic-graph-tasks
  evaluated: 1
  total: 2
task_categories:
- graph_classification
- graph_regression
- node_classification
experiment_scopes:
- graph-level
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
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5681
    at_pub_std: 0.009
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.20340000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5681
    true_std: 0.009
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_gap_source_is_current_paper: false
    value_gap: 0.20340000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.5681
    sort_std: 0.009
    global_rank: 9
    paper_rank: 186
    rank_delta: 177
    rank_delta_abs: 177
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
    global_rank: 14
    paper_rank: 33
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Co-GNN(μ,μ)
    model_key: co-gnn(μ,μ)
    model_plain: Co-GNN(μ,μ)
    value: 0.5417
    std: 0.0037
    paper_value: 0.5417
    paper_std: 0.0037
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5417
    true_std: 0.0037
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5417
    sort_std: 0.0037
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
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.5407
    std: 0.0031
    paper_value: 0.5407
    paper_std: 0.0031
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5407
    at_pub_std: 0.0031
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-02-13'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5407
    true_std: 0.0031
    value_gap_source_arxiv: '2402.08678'
    value_gap_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5407
    sort_std: 0.0031
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
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.5383
    std: 0.0032
    paper_value: 0.5383
    paper_std: 0.0032
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5383
    true_std: 0.0032
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5383
    sort_std: 0.0032
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
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.5351
    std: 0.0046
    paper_value: 0.5351
    paper_std: 0.0046
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5351
    at_pub_std: 0.0046
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5351
    true_std: 0.0046
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5351
    sort_std: 0.0046
    global_rank: 35
    paper_rank: 35
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5274
    at_pub_std: 0.0083
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
    true_value: 0.5274
    true_std: 0.0083
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5274
    sort_std: 0.0083
    global_rank: 54
    paper_rank: 54
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.527
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
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
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.527
    sort_std: 0.0062
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
  - model: Tango_GatedGCN
    model_key: tango_gatedgcn
    model_plain: Tango_GatedGCN
    value: 0.526
    std: 0.0053
    paper_value: 0.526
    paper_std: 0.0053
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.526
    true_std: 0.0053
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.526
    sort_std: 0.0053
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
  - model: GAT (DEG)
    model_key: gat (deg)
    model_plain: GAT (DEG)
    value: 0.5165
    std: 0.006
    paper_value: 0.5165
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5165
    true_std: 0.006
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5165
    sort_std: 0.006
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
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.5126
    std: 0.0072
    paper_value: 0.5126
    paper_std: 0.0072
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5126
    at_pub_std: 0.0072
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5126
    true_std: 0.0072
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5126
    sort_std: 0.0072
    global_rank: 77
    paper_rank: 77
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
  - model: GPS_GAT+Performer (DEG)
    model_key: gps_gat+performer (deg)
    model_plain: GPS_GAT+Performer (DEG)
    value: 0.5103
    std: 0.006
    paper_value: 0.5103
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5103
    true_std: 0.006
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5103
    sort_std: 0.006
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
  - model: GCN (DEG)
    model_key: gcn (deg)
    model_plain: GCN (DEG)
    value: 0.5001
    std: 0.0069
    paper_value: 0.5001
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5001
    true_std: 0.0069
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5001
    sort_std: 0.0069
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
  - model: GPS(RWSE)
    model_key: gps(rwse)
    model_plain: GPS(RWSE)
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4992
    sort_std: 0.0068
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
    global_rank: 104
    paper_rank: 186
    rank_delta: 82
    rank_delta_abs: 82
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: GPS_GCN+Performer (DEG)
    model_key: gps_gcn+performer (deg)
    model_plain: GPS_GCN+Performer (DEG)
    value: 0.4893
    std: 0.0047
    paper_value: 0.4893
    paper_std: 0.0047
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4893
    true_std: 0.0047
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4893
    sort_std: 0.0047
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
    global_rank: 118
    paper_rank: 166
    rank_delta: 48
    rank_delta_abs: 48
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4632
    at_pub_std: 0.025
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-04-26'
    value_gap_source_date_label: ICLR 2024
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
    value_gap_source_arxiv: '2404.17099'
    value_gap_source_title: Unleashing the Potential of Fractional Calculus in Graph
      Neural Networks with FROND
    value_gap_source_is_current_paper: false
    value_gap: 0.02200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.4632
    sort_std: 0.025
    global_rank: 136
    paper_rank: 157
    rank_delta: 21
    rank_delta_abs: 21
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4598
    at_pub_std: 0.0071
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
    true_value: 0.4598
    true_std: 0.0071
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4598
    sort_std: 0.0071
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
  - model: GPS + Mamba
    model_key: gps + mamba
    model_plain: GPS + Mamba
    value: 0.4513
    std: 0.0097
    paper_value: 0.4513
    paper_std: 0.0097
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4513
    at_pub_std: 0.0097
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-02-13'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4513
    true_std: 0.0097
    value_gap_source_arxiv: '2402.08678'
    value_gap_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4513
    sort_std: 0.0097
    global_rank: 149
    paper_rank: 149
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4937
    at_pub_std: 0.0071
    at_pub_source_arxiv: '2505.04808'
    at_pub_source_title: Piecewise Constant Spectral Graph Neural Network
    at_pub_source_date_iso: '2025-05-07'
    at_pub_source_date_label: TMLR 2025
    value_gap_source_date_iso: '2025-12-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.04490000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4488
    true_std: 0.0034
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4488
    sort_std: 0.0034
    global_rank: 152
    paper_rank: 152
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Piecewise Constant Spectral Graph Neural Network
    comparison_source_arxiv: '2505.04808'
    is_best: false
    is_std_outlier: false
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.4461
    std: 0.005
    paper_value: 0.4461
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4461
    at_pub_std: 0.005
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4461
    true_std: 0.005
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4461
    sort_std: 0.005
    global_rank: 156
    paper_rank: 156
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4436
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-04-26'
    value_gap_source_date_label: ICLR 2024
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
    value_gap_source_arxiv: '2404.17099'
    value_gap_source_title: Unleashing the Potential of Fractional Calculus in Graph
      Neural Networks with FROND
    value_gap_source_is_current_paper: false
    value_gap: 0.04570000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.4436
    sort_std: 0.0035
    global_rank: 157
    paper_rank: 181
    rank_delta: 24
    rank_delta_abs: 24
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: Gated-GCN
    model_key: gated-gcn
    model_plain: Gated-GCN
    value: 0.43
    std: 0.0032
    paper_value: 0.43
    paper_std: 0.0032
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on Amazon-ratings split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.43
    at_pub_std: 0.0032
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-02-13'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.43
    true_std: 0.0032
    value_gap_source_arxiv: '2402.08678'
    value_gap_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.43
    sort_std: 0.0032
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
  dataset: CIFAR10
  rows:
  - model: Tango_GPS
    model_key: randalign
    model_plain: Tango_GPS
    value: 0.7942
    std: 0.00072
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2404.09774'
    title: 'RandAlign: A Parameter-Free Method for Regularizing Graph Convolutional
      Networks'
    date: Apr 15, 2024
    date_display: Apr 2024
    date_iso: '2024-04-15'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7942
    sort_std: 0.00072
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: differential encoding
    model_plain: Tango_GPS
    value: 0.79067
    std: 0.00269
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
    sort_value: 0.79067
    sort_std: 0.00269
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Tango_GPS
    model_key: ppgt
    model_plain: Tango_GPS
    value: 0.7856
    std: 0.007
    metric: Accuracy
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
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7856
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.76468
    std: 0.00881
    paper_value: 0.76468
    paper_std: 0.00881
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.76468
    at_pub_std: 0.00881
    at_pub_source_arxiv: '2310.20519'
    at_pub_source_title: Enhancing Graph Neural Networks with Quantum Computed Encodings
    at_pub_source_date_iso: '2023-10-31'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.76468
    true_std: 0.00881
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.76468
    sort_std: 0.00881
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.75783
    std: 0.00261
    paper_value: 0.75783
    paper_std: 0.00261
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.75783
    true_std: 0.00261
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.75783
    sort_std: 0.00261
    global_rank: 11
    paper_rank: 11
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
    value: 0.7035
    std: 0.0063
    paper_value: 0.7035
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: PNA
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7311
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2110.03753'
    at_pub_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure
      Awareness'
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 0.027599999999999958
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7311
    true_std: 0.0011
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: false
    value_gap: 0.027599999999999958
    has_value_note: false
    value_note: ''
    sort_value: 0.7311
    sort_std: 0.0011
    global_rank: 36
    paper_rank: 63
    rank_delta: 27
    rank_delta_abs: 27
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    comparison_source_arxiv: '2110.03753'
    is_best: false
    is_std_outlier: false
  - model: DGN
    model_key: dgn
    model_plain: DGN
    value: 0.72838
    std: 0.00417
    paper_value: 0.72838
    paper_std: 0.00417
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
    source_ref: beaini2021directional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7284
    at_pub_std: 0.0042
    at_pub_source_arxiv: '2110.03753'
    at_pub_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure
      Awareness'
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 2.0000000000020002e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7284
    true_std: 0.0042
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: false
    value_gap: 2.0000000000020002e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.7284
    sort_std: 0.0042
    global_rank: 37
    paper_rank: 37
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN-AK+
    model_key: gin-ak+
    model_plain: GIN-AK+
    value: 0.7219
    std: 0.0013
    paper_value: 0.7219
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
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: zhao2022from
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7239
    at_pub_std: 0.0038
    at_pub_source_arxiv: '2312.05905'
    at_pub_source_title: Improving Subgraph-GNNs via Edge-Level Ego-Network Encodings
    at_pub_source_date_iso: '2023-12-10'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7239
    true_std: 0.0038
    value_gap_source_arxiv: '2312.05905'
    value_gap_source_title: Improving Subgraph-GNNs via Edge-Level Ego-Network Encodings
    value_gap_source_is_current_paper: false
    value_gap: 0.0020000000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.7239
    sort_std: 0.0038
    global_rank: 41
    paper_rank: 46
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.72298
    std: 0.00356
    paper_value: 0.72298
    paper_std: 0.00356
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: rampasek2022graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.72298
    at_pub_std: 0.00356
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
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.72356
    true_std: 0.00323
    value_gap_source_arxiv: '2605.05689'
    value_gap_source_title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive
      Consistency Model'
    value_gap_source_is_current_paper: false
    value_gap: 0.0005800000000000249
    has_value_note: false
    value_note: ''
    sort_value: 0.72356
    sort_std: 0.00323
    global_rank: 43
    paper_rank: 45
    rank_delta: 2
    rank_delta_abs: 2
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
    value: 0.67312
    std: 0.00311
    paper_value: 0.67312
    paper_std: 0.00311
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
    source_ref: gatedgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7133
    at_pub_std: 0.0039
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.040179999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7133
    true_std: 0.0039
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.040179999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7133
    sort_std: 0.0039
    global_rank: 57
    paper_rank: 85
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
    is_best: false
    is_std_outlier: false
  - model: Tango_GatedGCN
    model_key: tango_gatedgcn
    model_plain: Tango_GatedGCN
    value: 0.70894
    std: 0.00329
    paper_value: 0.70894
    paper_std: 0.00329
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.70894
    true_std: 0.00329
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.70894
    sort_std: 0.00329
    global_rank: 60
    paper_rank: 60
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CRaW1
    model_key: craw1
    model_plain: CRaW1
    value: 0.69013
    std: 0.00259
    paper_value: 0.69013
    paper_std: 0.00259
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
    source_ref: tonnshoff2023walking
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.69013
    at_pub_std: 0.00259
    at_pub_source_arxiv: '2402.02005'
    at_pub_source_title: Topology-Informed Graph Transformer
    at_pub_source_date_iso: '2024-02-03'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.69013
    true_std: 0.00259
    value_gap_source_arxiv: '2402.02005'
    value_gap_source_title: Topology-Informed Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.69013
    sort_std: 0.00259
    global_rank: 77
    paper_rank: 77
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.68702
    std: 0.00409
    paper_value: 0.68702
    paper_std: 0.00409
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
    source_ref: hussain2022global
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.68702
    at_pub_std: 0.00409
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.68702
    true_std: 0.00409
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.68702
    sort_std: 0.00409
    global_rank: 78
    paper_rank: 78
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
    value: 0.64223
    std: 0.00455
    paper_value: 0.64223
    paper_std: 0.00455
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
    source_ref: veličković2018graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6611
    at_pub_std: 0.0098
    at_pub_source_arxiv: '2006.07846'
    at_pub_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    at_pub_source_date_iso: '2020-06-14'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-14'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.018870000000000053
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6611
    true_std: 0.0098
    value_gap_source_arxiv: '2006.07846'
    value_gap_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    value_gap_source_is_current_paper: false
    value_gap: 0.018870000000000053
    has_value_note: false
    value_note: ''
    sort_value: 0.6611
    sort_std: 0.0098
    global_rank: 98
    paper_rank: 109
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Formatting Instructions for ICLR 2021 Conference Submissions
    comparison_source_arxiv: '2006.07846'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.55255
    std: 0.01527
    paper_value: 0.55255
    paper_std: 0.01527
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
    source_ref: xu2019how
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.651
    at_pub_std: 0.005
    at_pub_source_arxiv: '2107.04755'
    at_pub_source_title: 'Beyond Low-pass Filtering: Graph Convolutional Networks
      with Automatic Filtering'
    at_pub_source_date_iso: '2021-07-10'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-12-10'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.09845000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5982
    true_std: 0.0033
    value_gap_source_arxiv: '2312.05905'
    value_gap_source_title: Improving Subgraph-GNNs via Edge-Level Ego-Network Encodings
    value_gap_source_is_current_paper: false
    value_gap: 0.04564999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.5982
    sort_std: 0.0033
    global_rank: 118
    paper_rank: 126
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Beyond Low-pass Filtering: Graph Convolutional Networks
      with Automatic Filtering'
    comparison_source_arxiv: '2107.04755'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5571
    std: 0.00381
    paper_value: 0.5571
    paper_std: 0.00381
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
    source_ref: Kipf2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test Accuracy on CIFAR10 superpixels split from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5839
    at_pub_std: 0.0073
    at_pub_source_arxiv: '2110.03753'
    at_pub_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure
      Awareness'
    at_pub_source_date_iso: '2021-10-07'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2021-10-07'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: 0.026799999999999935
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5839
    true_std: 0.0073
    value_gap_source_arxiv: '2110.03753'
    value_gap_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    value_gap_source_is_current_paper: false
    value_gap: 0.026799999999999935
    has_value_note: false
    value_note: ''
    sort_value: 0.5839
    sort_std: 0.0073
    global_rank: 121
    paper_rank: 125
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'From Stars to Subgraphs: Uplifting Any GNN with Local
      Structure Awareness'
    comparison_source_arxiv: '2110.03753'
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
- &id010
  dataset: CLUSTER
  rows:
  - model: Tango_GPS
    model_key: grpe-small
    model_plain: Tango_GPS
    value: 0.81586
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 489.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_display: Jan 2022
    date_iso: '2022-01-30'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.81586
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.80113
    std: 0.00138
    paper_value: 0.80113
    paper_std: 0.00138
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
    protocol_note: Test accuracy on CLUSTER dataset using official splits from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.80113
    true_std: 0.00138
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.80113
    sort_std: 0.00138
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
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.80026
    std: 0.00277
    paper_value: 0.80026
    paper_std: 0.00277
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on CLUSTER dataset using official splits from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8003
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2405.19121'
    at_pub_source_title: Spatio-Spectral Graph Neural Networks
    at_pub_source_date_iso: '2024-05-29'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 4.0000000000040004e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8003
    true_std: 0.0028
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 4.0000000000040004e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.8003
    sort_std: 0.0028
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.79232
    std: 0.00348
    paper_value: 0.79232
    paper_std: 0.00348
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
    source_ref: hussain2022global
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on CLUSTER dataset using official splits from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.79232
    at_pub_std: 0.00348
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.79232
    true_std: 0.00348
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.79232
    sort_std: 0.00348
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
  - model: Tango_GatedGCN
    model_key: tango_gatedgcn
    model_plain: Tango_GatedGCN
    value: 0.78194
    std: 0.00307
    paper_value: 0.78194
    paper_std: 0.00307
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
    protocol_note: Test accuracy on CLUSTER dataset using official splits from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.78194
    true_std: 0.00307
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.78194
    sort_std: 0.00307
    global_rank: 14
    paper_rank: 14
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
    value: 0.78016
    std: 0.0018
    paper_value: 0.78016
    paper_std: 0.0018
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: rampasek2022graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on CLUSTER dataset using official splits from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7802
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2405.19121'
    at_pub_source_title: Spatio-Spectral Graph Neural Networks
    at_pub_source_date_iso: '2024-05-29'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 4.0000000000040004e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7802
    true_std: 0.0018
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 4.0000000000040004e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.7802
    sort_std: 0.0018
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAN
    model_key: san
    model_plain: SAN
    value: 0.76691
    std: 0.0065
    paper_value: 0.76691
    paper_std: 0.0065
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
    source_ref: kreuzer2021rethinking
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on CLUSTER dataset using official splits from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.76691
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.76691
    true_std: 0.0065
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.76691
    sort_std: 0.0065
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
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.7384
    std: 0.00326
    paper_value: 0.7384
    paper_std: 0.00326
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
    source_ref: gatedgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on CLUSTER dataset using official splits from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.76082
    at_pub_std: 0.00196
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-30'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.022420000000000107
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.76082
    true_std: 0.00196
    value_gap_source_arxiv: '2201.12787'
    value_gap_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 0.022420000000000107
    has_value_note: false
    value_note: ''
    sort_value: 0.76082
    sort_std: 0.00196
    global_rank: 55
    paper_rank: 63
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    comparison_source_arxiv: '2201.12787'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.70587
    std: 0.00447
    paper_value: 0.70587
    paper_std: 0.00447
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
    source_ref: veličković2018graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on CLUSTER dataset using official splits from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.70587
    at_pub_std: 0.00447
    at_pub_source_arxiv: '2201.09332'
    at_pub_source_title: How Expressive are Transformers in Spectral Domain for Graphs?
    at_pub_source_date_iso: '2022-01-23'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.70587
    true_std: 0.00447
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.70587
    sort_std: 0.00447
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.68498
    std: 0.00976
    paper_value: 0.68498
    paper_std: 0.00976
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
    source_ref: Kipf2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on CLUSTER dataset using official splits from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.69026
    at_pub_std: 0.01372
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2023-01-01'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: 0.005279999999999951
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.69026
    true_std: 0.01372
    value_gap_source_arxiv: '2003.00982'
    value_gap_source_title: GNNBenchmark
    value_gap_source_is_current_paper: false
    value_gap: 0.005279999999999951
    has_value_note: false
    value_note: ''
    sort_value: 0.69026
    sort_std: 0.01372
    global_rank: 71
    paper_rank: 72
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.64716
    std: 0.01553
    paper_value: 0.64716
    paper_std: 0.01553
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
    source_ref: xu2019how
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on CLUSTER dataset using official splits from dwivedi2023benchmarking
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.64716
    at_pub_std: 0.01553
    at_pub_source_arxiv: '2201.12787'
    at_pub_source_title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    at_pub_source_date_iso: '2022-01-30'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.64716
    true_std: 0.01553
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.64716
    sort_std: 0.01553
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id008
  dataset: MNIST
  rows:
  - model: Tango_GPS
    model_key: schrödinger gnn
    model_plain: Tango_GPS
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
  - model: Tango_GPS
    model_key: cnn
    model_plain: Tango_GPS
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
  - model: Tango_GPS
    model_key: mpnn
    model_plain: Tango_GPS
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
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.9734
    std: 0.00143
    paper_value: 0.9734
    paper_std: 0.00143
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
    source_ref: gatedgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on MNIST superpixels using Dwivedi et al. 2023 split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
    paper_rank: 85
    rank_delta: 74
    rank_delta_abs: 74
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'RandAlign: A Parameter-Free Method for Regularizing
      Graph Convolutional Networks'
    comparison_source_arxiv: '2404.09774'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.96485
    std: 0.00252
    paper_value: 0.96485
    paper_std: 0.00252
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
    source_ref: xu2019how
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on MNIST superpixels using Dwivedi et al. 2023 split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
    gap_vs_at_pub: 0.007450000000000068
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
    value_gap: 0.018449999999999966
    has_value_note: false
    value_note: ''
    sort_value: 0.9833
    sort_std: 0.0011
    global_rank: 31
    paper_rank: 103
    rank_delta: 72
    rank_delta_abs: 72
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph-Coupled Oscillator Networks
    comparison_source_arxiv: '2202.02296'
    is_best: false
    is_std_outlier: false
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.98197
    std: 0.0011
    paper_value: 0.98197
    paper_std: 0.0011
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on MNIST superpixels using Dwivedi et al. 2023 split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.98197
    true_std: 0.0011
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.98197
    sort_std: 0.0011
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
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.98173
    std: 0.00087
    paper_value: 0.98173
    paper_std: 0.00087
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
    source_ref: hussain2022global
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on MNIST superpixels using Dwivedi et al. 2023 split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.98173
    at_pub_std: 0.00087
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.98173
    true_std: 0.00087
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.98173
    sort_std: 0.00087
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
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.98108
    std: 0.00111
    paper_value: 0.98108
    paper_std: 0.00111
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on MNIST superpixels using Dwivedi et al. 2023 split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.98108
    at_pub_std: 0.00111
    at_pub_source_arxiv: '2312.01538'
    at_pub_source_title: Recurrent Distance Filtering for Graph Representation Learning
    at_pub_source_date_iso: '2023-12-03'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-10-14'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.98108
    true_std: 0.00111
    value_gap_source_arxiv: '2510.12369'
    value_gap_source_title: A Hierarchical Quantized Tokenization Framework for Task-Adaptive
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.98108
    sort_std: 0.00111
    global_rank: 54
    paper_rank: 54
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
    value: 0.98051
    std: 0.00126
    paper_value: 0.98051
    paper_std: 0.00126
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: rampasek2022graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on MNIST superpixels using Dwivedi et al. 2023 split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.98051
    at_pub_std: 0.00126
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
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.98082
    true_std: 0.00114
    value_gap_source_arxiv: '2605.05689'
    value_gap_source_title: 'GCCM: Enhancing Generative Graph Prediction via Contrastive
      Consistency Model'
    value_gap_source_is_current_paper: false
    value_gap: 0.00031000000000003247
    has_value_note: false
    value_note: ''
    sort_value: 0.98082
    sort_std: 0.00114
    global_rank: 56
    paper_rank: 57
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CRaW1
    model_key: craw1
    model_plain: CRaW1
    value: 0.97944
    std: 0.0005
    paper_value: 0.97944
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: tonnshoff2023walking
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on MNIST superpixels using Dwivedi et al. 2023 split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.97944
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2402.02005'
    at_pub_source_title: Topology-Informed Graph Transformer
    at_pub_source_date_iso: '2024-02-03'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-02-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.97944
    true_std: 0.0005
    value_gap_source_arxiv: '2402.02005'
    value_gap_source_title: Topology-Informed Graph Transformer
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.97944
    sort_std: 0.0005
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: PNA
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on MNIST superpixels using Dwivedi et al. 2023 split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9794
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-05-30'
    value_gap_source_date_label: '2024'
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
    value_gap_source_arxiv: '2405.19779'
    value_gap_source_title: Automatic Graph Topology-Aware Transformer
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9794
    sort_std: 0.0012
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
  - model: Tango_GatedGCN
    model_key: tango_gatedgcn
    model_plain: Tango_GatedGCN
    value: 0.97788
    std: 0.00105
    paper_value: 0.97788
    paper_std: 0.00105
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on MNIST superpixels using Dwivedi et al. 2023 split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.97788
    true_std: 0.00105
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.97788
    sort_std: 0.00105
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
    value: 0.95535
    std: 0.00205
    paper_value: 0.95535
    paper_std: 0.00205
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
    source_ref: veličković2018graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on MNIST superpixels using Dwivedi et al. 2023 split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
    gap_vs_at_pub: 0.020179999999999976
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
    value_gap: 0.020179999999999976
    has_value_note: false
    value_note: ''
    sort_value: 0.97553
    sort_std: 0.00034
    global_rank: 81
    paper_rank: 114
    rank_delta: 33
    rank_delta_abs: 33
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'RandAlign: A Parameter-Free Method for Regularizing
      Graph Convolutional Networks'
    comparison_source_arxiv: '2404.09774'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.90705
    std: 0.00218
    paper_value: 0.90705
    paper_std: 0.00218
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
    source_ref: Kipf2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on MNIST superpixels using Dwivedi et al. 2023 split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
    gap_vs_at_pub: 0.033459999999999934
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
    value_gap: 0.033459999999999934
    has_value_note: false
    value_note: ''
    sort_value: 0.94051
    sort_std: 0.00052
    global_rank: 129
    paper_rank: 133
    rank_delta: 4
    rank_delta_abs: 4
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
- &id007
  dataset: Minesweeper
  rows:
  - model: Tango_GPS
    model_key: bunn
    model_plain: Tango_GPS
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
  - model: Tango_GPS
    model_key: dc-gnn
    model_plain: Tango_GPS
    value: 0.985
    std: 0.0021
    metric: ROC-AUC
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
    sort_value: 0.985
    sort_std: 0.0021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.9839
    std: 0.0054
    paper_value: 0.9839
    paper_std: 0.0054
    metric: ROC-AUC
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9839
    true_std: 0.0054
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9839
    sort_std: 0.0054
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GatedGCN
    model_key: tango_gatedgcn
    model_plain: Tango_GatedGCN
    value: 0.9832
    std: 0.0059
    paper_value: 0.9832
    paper_std: 0.0059
    metric: ROC-AUC
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9832
    true_std: 0.0059
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9832
    sort_std: 0.0059
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Co-GNN(μ,μ)
    model_key: co-gnn(μ,μ)
    model_plain: Co-GNN(μ,μ)
    value: 0.9731
    std: 0.0041
    paper_value: 0.9731
    paper_std: 0.0041
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9731
    true_std: 0.0041
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9731
    sort_std: 0.0041
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
  - model: GCN (LapPE)
    model_key: gcn (lappe)
    model_plain: GCN (LapPE)
    value: 0.9426
    std: 0.0049
    paper_value: 0.9426
    paper_std: 0.0049
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9426
    true_std: 0.0049
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9426
    sort_std: 0.0049
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9391
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
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
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9391
    sort_std: 0.0035
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
  - model: GPS_GCN+Performer (LapPE)
    model_key: gps_gcn+performer (lappe)
    model_plain: GPS_GCN+Performer (LapPE)
    value: 0.9385
    std: 0.0041
    paper_value: 0.9385
    paper_std: 0.0041
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9385
    true_std: 0.0041
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9385
    sort_std: 0.0041
    global_rank: 32
    paper_rank: 32
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9351
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-14'
    value_gap_source_date_label: '2022'
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
    value_gap_source_arxiv: '2202.07082'
    value_gap_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9351
    sort_std: 0.0057
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
  - model: GAT (LapPE)
    model_key: gat (lappe)
    model_plain: GAT (LapPE)
    value: 0.935
    std: 0.0054
    paper_value: 0.935
    paper_std: 0.0054
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.935
    true_std: 0.0054
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.935
    sort_std: 0.0054
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
  - model: GPS_GAT+Performer (LapPE)
    model_key: gps_gat+performer (lappe)
    model_plain: GPS_GAT+Performer (LapPE)
    value: 0.9262
    std: 0.0079
    paper_value: 0.9262
    paper_std: 0.0079
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9262
    true_std: 0.0079
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9262
    sort_std: 0.0079
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9229
    at_pub_std: 0.0047
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-06-22'
    value_gap_source_date_label: ICML 2023
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
    value_gap_source_arxiv: '2306.12943'
    value_gap_source_title: Evolving Computation Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9229
    sort_std: 0.0047
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
  - model: GPS_GAT+Transformer (LapPE)
    model_key: gps_gat+transformer (lappe)
    model_plain: GPS_GAT+Transformer (LapPE)
    value: 0.9229
    std: 0.0061
    paper_value: 0.9229
    paper_std: 0.0061
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9229
    true_std: 0.0061
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9229
    sort_std: 0.0061
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
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.9074
    std: 0.0053
    paper_value: 0.9074
    paper_std: 0.0053
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9226
    at_pub_std: 0.0056
    at_pub_source_arxiv: '2411.16278'
    at_pub_source_title: Even Sparser Graph Transformers
    at_pub_source_date_iso: '2024-11-25'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-25'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.015199999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9226
    true_std: 0.0056
    value_gap_source_arxiv: '2411.16278'
    value_gap_source_title: Even Sparser Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.015199999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.9226
    sort_std: 0.0056
    global_rank: 51
    paper_rank: 68
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Even Sparser Graph Transformers
    comparison_source_arxiv: '2411.16278'
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9185
    at_pub_std: 0.0076
    at_pub_source_arxiv: '2405.15540'
    at_pub_source_title: Bundle Neural Networks for message diffusion on graphs
    at_pub_source_date_iso: '2024-05-24'
    at_pub_source_date_label: '2024'
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
    true_value: 0.9185
    true_std: 0.0076
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9185
    sort_std: 0.0076
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
  - model: GPS (RWSE)
    model_key: gps (rwse)
    model_plain: GPS (RWSE)
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
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
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
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.9101
    std: 0.0023
    paper_value: 0.9101
    paper_std: 0.0023
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9101
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-02-13'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9101
    true_std: 0.0023
    value_gap_source_arxiv: '2402.08678'
    value_gap_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9101
    sort_std: 0.0023
    global_rank: 66
    paper_rank: 66
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9085
    at_pub_std: 0.0058
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
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
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9008
    at_pub_std: 0.007
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
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
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
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
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8995
    at_pub_std: 0.0038
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2023-05-26'
    value_gap_source_date_label: IJCAI 2023
    gap_vs_at_pub: 0.0023999999999999577
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8995
    true_std: 0.0038
    value_gap_source_arxiv: '2305.16780'
    value_gap_source_title: Graph Neural Convection-Diffusion with Heterophily
    value_gap_source_is_current_paper: false
    value_gap: 0.0023999999999999577
    has_value_note: false
    value_note: ''
    sort_value: 0.8995
    sort_std: 0.0038
    global_rank: 77
    paper_rank: 80
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS + Mamba
    model_key: gps + mamba
    model_plain: GPS + Mamba
    value: 0.8993
    std: 0.0054
    paper_value: 0.8993
    paper_std: 0.0054
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8993
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-02-13'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8993
    true_std: 0.0054
    value_gap_source_arxiv: '2402.08678'
    value_gap_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8993
    sort_std: 0.0054
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8969
    at_pub_std: 0.006
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2023-05-26'
    value_gap_source_date_label: IJCAI 2023
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
    value_gap_source_arxiv: '2305.16780'
    value_gap_source_title: Graph Neural Convection-Diffusion with Heterophily
    value_gap_source_is_current_paper: false
    value_gap: 0.015199999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.8969
    sort_std: 0.006
    global_rank: 83
    paper_rank: 93
    rank_delta: 10
    rank_delta_abs: 10
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8966
    at_pub_std: 0.004
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
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
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
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
  - model: Gated-GCN
    model_key: gated-gcn
    model_plain: Gated-GCN
    value: 0.8754
    std: 0.0122
    paper_value: 0.8754
    paper_std: 0.0122
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8754
    at_pub_std: 0.0122
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-02-13'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8754
    true_std: 0.0122
    value_gap_source_arxiv: '2402.08678'
    value_gap_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8754
    sort_std: 0.0122
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8624
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
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
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8624
    sort_std: 0.0061
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
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.8419
    std: 0.0066
    paper_value: 0.8419
    paper_std: 0.0066
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8419
    at_pub_std: 0.0066
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8419
    true_std: 0.0066
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8419
    sort_std: 0.0066
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
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.8109
    std: 0.0102
    paper_value: 0.8109
    paper_std: 0.0102
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8109
    at_pub_std: 0.0102
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8109
    true_std: 0.0102
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8109
    sort_std: 0.0102
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7127
    at_pub_std: 0.0114
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2023-05-26'
    value_gap_source_date_label: IJCAI 2023
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
    value_gap_source_arxiv: '2305.16780'
    value_gap_source_title: Graph Neural Convection-Diffusion with Heterophily
    value_gap_source_is_current_paper: false
    value_gap: 0.19240000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.7127
    sort_std: 0.0114
    global_rank: 124
    paper_rank: 141
    rank_delta: 17
    rank_delta_abs: 17
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Minesweeper split from Platonov et al. 2023
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6253
    at_pub_std: 0.0134
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2023-05-26'
    value_gap_source_date_label: IJCAI 2023
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
    value_gap_source_arxiv: '2305.16780'
    value_gap_source_title: Graph Neural Convection-Diffusion with Heterophily
    value_gap_source_is_current_paper: false
    value_gap: 0.11449999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.6253
    sort_std: 0.0134
    global_rank: 134
    paper_rank: 141
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
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
- &id011
  dataset: PATTERN
  rows:
  - model: Tango_GPS
    model_key: deepgraph (48)
    model_plain: Tango_GPS
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
  - model: Tango_GPS
    model_key: ppgt
    model_plain: Tango_GPS
    value: 0.89752
    std: 0.0003
    metric: Accuracy
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
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.89752
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Tango_GPS
    model_key: ckgcn
    model_plain: Tango_GPS
    value: 0.88661
    std: 0.00143
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.12588'
    title: Plain Transformers Can be Powerful Graph Learners
    date: Apr 17, 2025
    date_display: Apr 2025
    date_iso: '2025-04-17'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.88661
    sort_std: 0.00143
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.87196
    std: 0.00076
    paper_value: 0.87196
    paper_std: 0.00076
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
    source_ref: ma2023graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the official dwivedi2023benchmarking split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8722
    at_pub_std: 0.0003
    at_pub_source_arxiv: '2411.12732'
    at_pub_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    at_pub_source_date_iso: '2024-11-19'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.00024000000000001798
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8722
    true_std: 0.0003
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.00024000000000001798
    has_value_note: false
    value_note: ''
    sort_value: 0.8722
    sort_std: 0.0003
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
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.87182
    std: 0.00063
    paper_value: 0.87182
    paper_std: 0.00063
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
    protocol_note: Accuracy on the official dwivedi2023benchmarking split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.87182
    true_std: 0.00063
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.87182
    sort_std: 0.00063
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
  - model: EGT
    model_key: egt
    model_plain: EGT
    value: 0.86821
    std: 0.0002
    paper_value: 0.86821
    paper_std: 0.0002
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
    source_ref: hussain2022global
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the official dwivedi2023benchmarking split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86821
    at_pub_std: 0.0002
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86821
    true_std: 0.02
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86821
    sort_std: 0.02
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
    is_std_outlier: true
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.86685
    std: 0.00059
    paper_value: 0.86685
    paper_std: 0.00059
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: rampasek2022graphgps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the official dwivedi2023benchmarking split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86685
    at_pub_std: 0.00059
    at_pub_source_arxiv: '2305.11424'
    at_pub_source_title: IJCAI--23 Formatting Instructions
    at_pub_source_date_iso: '2023-05-19'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86685
    true_std: 0.059
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86685
    sort_std: 0.059
    global_rank: 48
    paper_rank: 48
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: true
  - model: DGN
    model_key: dgn
    model_plain: DGN
    value: 0.8668
    std: 0.00034
    paper_value: 0.8668
    paper_std: 0.00034
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
    source_ref: beaini2021directional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the official dwivedi2023benchmarking split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8668
    at_pub_std: 0.00034
    at_pub_source_arxiv: '2205.12454'
    at_pub_source_title: Recipe for a General, Powerful, Scalable Graph Transformer
    at_pub_source_date_iso: '2022-05-25'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8668
    true_std: 0.034
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8668
    sort_std: 0.034
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
    is_std_outlier: true
  - model: Tango_GatedGCN
    model_key: tango_gatedgcn
    model_plain: Tango_GatedGCN
    value: 0.86672
    std: 0.00071
    paper_value: 0.86672
    paper_std: 0.00071
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
    protocol_note: Accuracy on the official dwivedi2023benchmarking split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86672
    true_std: 0.00071
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86672
    sort_std: 0.00071
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
  - model: SAN
    model_key: san
    model_plain: SAN
    value: 0.86581
    std: 0.00037
    paper_value: 0.86581
    paper_std: 0.00037
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
    source_ref: kreuzer2021rethinking
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the official dwivedi2023benchmarking split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86581
    at_pub_std: 0.00037
    at_pub_source_arxiv: '2202.03036'
    at_pub_source_title: Structure-Aware Transformer for Graph Representation Learning
    at_pub_source_date_iso: '2022-02-07'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86581
    true_std: 0.037
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86581
    sort_std: 0.037
    global_rank: 54
    paper_rank: 54
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.71892
    std: 0.00334
    paper_value: 0.71892
    paper_std: 0.00334
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
    source_ref: Kipf2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the official dwivedi2023benchmarking split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.85614
    at_pub_std: 0.032
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2023-01-01'
    value_gap_source_date_label: JMLR 2023
    gap_vs_at_pub: 0.13722
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.85614
    true_std: 0.032
    value_gap_source_arxiv: '2003.00982'
    value_gap_source_title: GNNBenchmark
    value_gap_source_is_current_paper: false
    value_gap: 0.13722
    has_value_note: false
    value_note: ''
    sort_value: 0.85614
    sort_std: 0.032
    global_rank: 84
    paper_rank: 116
    rank_delta: 32
    rank_delta_abs: 32
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: GNNBenchmark
    comparison_source_arxiv: '2003.00982'
    is_best: false
    is_std_outlier: true
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.85387
    std: 0.00136
    paper_value: 0.85387
    paper_std: 0.00136
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
    source_ref: xu2019how
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the official dwivedi2023benchmarking split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8559
    at_pub_std: 0.0001
    at_pub_source_arxiv: '2010.05421'
    at_pub_source_title: Factorizable Graph Convolutional Networks
    at_pub_source_date_iso: '2020-10-12'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.0020299999999999763
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8559
    true_std: 0.0001
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 0.0020299999999999763
    has_value_note: false
    value_note: ''
    sort_value: 0.8559
    sort_std: 0.0001
    global_rank: 85
    paper_rank: 92
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Factorizable Graph Convolutional Networks
    comparison_source_arxiv: '2010.05421'
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.85568
    std: 0.00088
    paper_value: 0.85568
    paper_std: 0.00088
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
    source_ref: gatedgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the official dwivedi2023benchmarking split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.86508
    at_pub_std: 0.00085
    at_pub_source_arxiv: '2305.11424'
    at_pub_source_title: IJCAI--23 Formatting Instructions
    at_pub_source_date_iso: '2023-05-19'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-06-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.009399999999999964
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8557
    true_std: 0.0009
    value_gap_source_arxiv: '2407.00696'
    value_gap_source_title: Graph in Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 2.0000000000020002e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.8557
    sort_std: 0.0009
    global_rank: 88
    paper_rank: 89
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: IJCAI--23 Formatting Instructions
    comparison_source_arxiv: '2305.11424'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.78271
    std: 0.00186
    paper_value: 0.78271
    paper_std: 0.00186
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
    source_ref: veličković2018graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the official dwivedi2023benchmarking split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.78271
    at_pub_std: 0.00186
    at_pub_source_arxiv: '2201.09332'
    at_pub_source_title: How Expressive are Transformers in Spectral Domain for Graphs?
    at_pub_source_date_iso: '2022-01-23'
    at_pub_source_date_label: TMLR 2022
    value_gap_source_date_iso: '2025-10-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.78271
    true_std: 0.186
    value_gap_source_arxiv: '2510.14336'
    value_gap_source_title: 'DARTS-GT: Differentiable Architecture Search for Graph
      Transformers with Quantifiable Instance-Specific Interpretability Analysis'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.78271
    sort_std: 0.186
    global_rank: 106
    paper_rank: 106
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: true
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
  dataset: Peptides-func
  rows:
  - model: Tango_GPS
    model_key: s^2gcn
    model_plain: Tango_GPS
    value: 0.7311
    std: 0.0066
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_display: Nov 2024
    date_iso: '2024-11-19'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7311
    sort_std: 0.0066
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: s^2 gcn + pe
    model_plain: Tango_GPS
    value: 0.7311
    std: 0.0066
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.19121'
    title: Spatio-Spectral Graph Neural Networks
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: PE is described as stable positional encodings almost
      free of cost for S2GNNs.
    is_global_top: true
    global_rank: 2
    sort_value: 0.7311
    sort_std: 0.0066
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: s4g
    model_plain: Tango_GPS
    value: 0.7293
    std: 0.0004
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    global_rank: 3
    sort_value: 0.7293
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DRew-GCN+LapPE
    model_key: drew-gcn+lappe
    model_plain: DRew-GCN+LapPE
    value: 0.715
    std: 0.0044
    paper_value: 0.715
    paper_std: 0.0044
    metric: AP
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
    feature_source_evidence: All MPNN-based methods include structural and positional
      encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.715
    at_pub_std: 0.0044
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.715
    true_std: 0.0044
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.715
    sort_std: 0.0044
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.7021
    std: 0.0043
    paper_value: 0.7021
    paper_std: 0.0043
    metric: AP
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
    feature_source_evidence: Tango does not use additional encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7021
    true_std: 0.0043
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7021
    sort_std: 0.0043
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
  - model: PH-DGN
    model_key: ph-dgn
    model_plain: PH-DGN
    value: 0.7012
    std: 0.0045
    paper_value: 0.7012
    paper_std: 0.0045
    metric: AP
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
    feature_source_evidence: All MPNN-based methods include structural and positional
      encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7012
    true_std: 0.0045
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7012
    sort_std: 0.0045
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
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.5543
    std: 0.0078
    paper_value: 0.5543
    paper_std: 0.0078
    metric: AP
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
    feature_source_evidence: All MPNN-based methods include structural and positional
      encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5543
    at_pub_std: 0.0078
    at_pub_source_arxiv: '2206.08164'
    at_pub_source_title: LRGB
    at_pub_source_date_iso: '2022-06-16'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-04-27'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.699
    true_std: 0.003
    value_gap_source_arxiv: '2604.24293'
    value_gap_source_title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature
      Evolution via Continuous Phase Transitions'
    value_gap_source_is_current_paper: false
    value_gap: 0.14469999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.699
    sort_std: 0.003
    global_rank: 41
    paper_rank: 174
    rank_delta: 133
    rank_delta_abs: 133
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Tango_GatedGCN
    model_key: tango_gatedgcn
    model_plain: Tango_GatedGCN
    value: 0.6892
    std: 0.004
    paper_value: 0.6892
    paper_std: 0.004
    metric: AP
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
    feature_source_evidence: Tango does not use additional encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6892
    true_std: 0.004
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6892
    sort_std: 0.004
    global_rank: 61
    paper_rank: 61
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop-GCN+LapPE
    model_key: mixhop-gcn+lappe
    model_plain: MixHop-GCN+LapPE
    value: 0.6843
    std: 0.0049
    paper_value: 0.6843
    paper_std: 0.0049
    metric: AP
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
    feature_source_evidence: All MPNN-based methods include structural and positional
      encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6843
    at_pub_std: 0.0049
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6843
    true_std: 0.0049
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6843
    sort_std: 0.0049
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
  - model: DIGL+MPNN+LapPE
    model_key: digl+mpnn+lappe
    model_plain: DIGL+MPNN+LapPE
    value: 0.683
    std: 0.0026
    paper_value: 0.683
    paper_std: 0.0026
    metric: AP
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
    feature_source_evidence: All MPNN-based methods include structural and positional
      encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.683
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.683
    true_std: 0.0026
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.683
    sort_std: 0.0026
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SWAN
    model_key: swan
    model_plain: SWAN
    value: 0.6751
    std: 0.0039
    paper_value: 0.6751
    paper_std: 0.0039
    metric: AP
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
    feature_source_evidence: All MPNN-based methods include structural and positional
      encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6751
    true_std: 0.0039
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6751
    sort_std: 0.0039
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
  - model: GRAND
    model_key: grand
    model_plain: GRAND
    value: 0.5789
    std: 0.0062
    paper_value: 0.5789
    paper_std: 0.0062
    metric: AP
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
    feature_source_evidence: All MPNN-based methods include structural and positional
      encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-04-27'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.663
    true_std: 0.016
    value_gap_source_arxiv: '2604.24293'
    value_gap_source_title: 'Latent-Hysteresis Graph ODEs: Modeling Coupled Topology-Feature
      Evolution via Continuous Phase Transitions'
    value_gap_source_is_current_paper: false
    value_gap: 0.08410000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.663
    sort_std: 0.016
    global_rank: 89
    paper_rank: 171
    rank_delta: 82
    rank_delta_abs: 82
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS+LapPE
    model_key: gps+lappe
    model_plain: GPS+LapPE
    value: 0.6535
    std: 0.0041
    paper_value: 0.6535
    paper_std: 0.0041
    metric: AP
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
    feature_source_evidence: All transformer baselines include positional and structural
      encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6535
    true_std: 0.0041
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6535
    sort_std: 0.0041
    global_rank: 108
    paper_rank: 108
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAN+LapPE
    model_key: san+lappe
    model_plain: SAN+LapPE
    value: 0.6384
    std: 0.0121
    paper_value: 0.6384
    paper_std: 0.0121
    metric: AP
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
    feature_source_evidence: All transformer baselines include positional and structural
      encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6384
    at_pub_std: 0.0121
    at_pub_source_arxiv: '2206.08164'
    at_pub_source_title: LRGB
    at_pub_source_date_iso: '2022-06-16'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6384
    true_std: 0.0121
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6384
    sort_std: 0.0121
    global_rank: 131
    paper_rank: 131
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Transformer+LapPE
    model_key: transformer+lappe
    model_plain: Transformer+LapPE
    value: 0.6326
    std: 0.0126
    paper_value: 0.6326
    paper_std: 0.0126
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All transformer baselines include positional and structural
      encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6326
    at_pub_std: 0.0126
    at_pub_source_arxiv: '2206.08164'
    at_pub_source_title: LRGB
    at_pub_source_date_iso: '2022-06-16'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6326
    true_std: 0.0126
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6326
    sort_std: 0.0126
    global_rank: 133
    paper_rank: 133
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCON
    model_key: graphcon
    model_plain: GraphCON
    value: 0.6022
    std: 0.0068
    paper_value: 0.6022
    paper_std: 0.0068
    metric: AP
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
    feature_source_evidence: All MPNN-based methods include structural and positional
      encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6022
    true_std: 0.0068
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6022
    sort_std: 0.0068
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
  - model: A-DGN
    model_key: a-dgn
    model_plain: A-DGN
    value: 0.5975
    std: 0.0044
    paper_value: 0.5975
    paper_std: 0.0044
    metric: AP
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
    feature_source_evidence: All MPNN-based methods include structural and positional
      encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Peptides-func classification task using official LRGB split; metric
      AP.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5975
    true_std: 0.0044
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5975
    sort_std: 0.0044
    global_rank: 153
    paper_rank: 153
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AP
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: AP
  paper_metrics:
  - AP
  metric: AP
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: Peptides-struct
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.3496
    std: 0.0013
    paper_value: 0.3496
    paper_std: 0.0013
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2421
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2502.09263'
    at_pub_source_title: Can Classic GNNs Be Strong Baselines for Graph-level Tasks?
      Simple Architectures Meet Excellence
    at_pub_source_date_iso: '2025-02-13'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.10750000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2421
    true_std: 0.0016
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.10750000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.2421
    sort_std: 0.0016
    global_rank: 1
    paper_rank: 169
    rank_delta: 168
    rank_delta_abs: 168
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Can Classic GNNs Be Strong Baselines for Graph-level
      Tasks? Simple Architectures Meet Excellence
    comparison_source_arxiv: '2502.09263'
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.2422
    std: 0.0014
    paper_value: 0.2422
    paper_std: 0.0014
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: Tango does not use additional encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2422
    true_std: 0.0014
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2422
    sort_std: 0.0014
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
  - model: GMN
    model_key: nba-gin+lappe
    model_plain: GMN
    value: 0.2424
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2310.07430'
    title: Non-backtracking Graph Neural Networks
    date: Oct 11, 2023
    date_display: Oct 2023
    date_iso: '2023-10-11'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/seonghyun26/nba-gnn
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.2424
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.342
    std: 0.0013
    paper_value: 0.342
    paper_std: 0.0013
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2431
    at_pub_std: 0.002
    at_pub_source_arxiv: '2502.09263'
    at_pub_source_title: Can Classic GNNs Be Strong Baselines for Graph-level Tasks?
      Simple Architectures Meet Excellence
    at_pub_source_date_iso: '2025-02-13'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.09890000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2431
    true_std: 0.002
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.09890000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.2431
    sort_std: 0.002
    global_rank: 7
    paper_rank: 168
    rank_delta: 161
    rank_delta_abs: 161
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Can Classic GNNs Be Strong Baselines for Graph-level
      Tasks? Simple Architectures Meet Excellence
    comparison_source_arxiv: '2502.09263'
    is_best: true
    is_std_outlier: false
  - model: Tango_GatedGCN
    model_key: tango_gatedgcn
    model_plain: Tango_GatedGCN
    value: 0.2451
    std: 0.0006
    paper_value: 0.2451
    paper_std: 0.0006
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: Tango does not use additional encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2451
    true_std: 0.0006
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2451
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
  - model: PH-DGN
    model_key: ph-dgn
    model_plain: PH-DGN
    value: 0.2465
    std: 0.002
    paper_value: 0.2465
    paper_std: 0.002
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2465
    true_std: 0.002
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2465
    sort_std: 0.002
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
  - model: GINE
    model_key: gine
    model_plain: GINE
    value: 0.3547
    std: 0.0045
    paper_value: 0.3547
    paper_std: 0.0045
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2473
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2309.00367'
    at_pub_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    at_pub_source_date_iso: '2023-09-01'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: 0.10740000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2473
    true_std: 0.0017
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.10740000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.2473
    sort_std: 0.0017
    global_rank: 48
    paper_rank: 171
    rank_delta: 123
    rank_delta_abs: 123
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph
      Benchmark
    comparison_source_arxiv: '2309.00367'
    is_best: false
    is_std_outlier: false
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.2473
    std: 0.0025
    paper_value: 0.2473
    paper_std: 0.0025
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 10
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2473
    at_pub_std: 0.0025
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2473
    true_std: 0.0025
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2473
    sort_std: 0.0025
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
  - model: Graph-Mamba
    model_key: graph-mamba
    model_plain: Graph-Mamba
    value: 0.2478
    std: 0.0016
    paper_value: 0.2478
    paper_std: 0.0016
    metric: MAE
    higher_is_better: false
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
    table_ref: Table 10
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2478
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2478
    true_std: 0.0016
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2478
    sort_std: 0.0016
    global_rank: 60
    paper_rank: 60
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SWAN
    model_key: swan
    model_plain: SWAN
    value: 0.2485
    std: 0.0009
    paper_value: 0.2485
    paper_std: 0.0009
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2485
    true_std: 0.0009
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2485
    sort_std: 0.0009
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS+LapPE
    model_key: gps+lappe
    model_plain: GPS+LapPE
    value: 0.25
    std: 0.0005
    paper_value: 0.25
    paper_std: 0.0005
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
    input_feature_source: raw_features
    feature_source_evidence: All transformer baselines include positional and structural
      encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.25
    true_std: 0.0005
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.25
    sort_std: 0.0005
    global_rank: 86
    paper_rank: 86
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRew-GCN+LapPE
    model_key: drew-gcn+lappe
    model_plain: DRew-GCN+LapPE
    value: 0.2536
    std: 0.0015
    paper_value: 0.2536
    paper_std: 0.0015
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
    input_feature_source: raw_features
    feature_source_evidence: All transformer baselines include positional and structural
      encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2536
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.2517
    true_std: 0.0011
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.0019000000000000128
    has_value_note: false
    value_note: ''
    sort_value: 0.2517
    sort_std: 0.0011
    global_rank: 98
    paper_rank: 108
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Transformer+LapPE
    model_key: transformer+lappe
    model_plain: Transformer+LapPE
    value: 0.2529
    std: 0.0016
    paper_value: 0.2529
    paper_std: 0.0016
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All transformer baselines include positional and structural
      encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2529
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2206.08164'
    at_pub_source_title: LRGB
    at_pub_source_date_iso: '2022-06-16'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2529
    true_std: 0.0016
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2529
    sort_std: 0.0016
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
  - model: DRew-GCN
    model_key: drew-gcn
    model_plain: DRew-GCN
    value: 0.2781
    std: 0.0028
    paper_value: 0.2781
    paper_std: 0.0028
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 10
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2536
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2405.19121'
    at_pub_source_title: Spatio-Spectral Graph Neural Networks
    at_pub_source_date_iso: '2024-05-29'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-05-29'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.024500000000000022
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2536
    true_std: 0.0015
    value_gap_source_arxiv: '2405.19121'
    value_gap_source_title: Spatio-Spectral Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.024500000000000022
    has_value_note: false
    value_note: ''
    sort_value: 0.2536
    sort_std: 0.0015
    global_rank: 110
    paper_rank: 152
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spatio-Spectral Graph Neural Networks
    comparison_source_arxiv: '2405.19121'
    is_best: false
    is_std_outlier: false
  - model: MixHop-GCN+LapPE
    model_key: mixhop-gcn+lappe
    model_plain: MixHop-GCN+LapPE
    value: 0.2614
    std: 0.0023
    paper_value: 0.2614
    paper_std: 0.0023
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
    input_feature_source: raw_features
    feature_source_evidence: All transformer baselines include positional and structural
      encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2614
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2614
    true_std: 0.0023
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2614
    sort_std: 0.0023
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
  - model: DIGL+MPNN+LapPE
    model_key: digl+mpnn+lappe
    model_plain: DIGL+MPNN+LapPE
    value: 0.2616
    std: 0.0018
    paper_value: 0.2616
    paper_std: 0.0018
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
    input_feature_source: raw_features
    feature_source_evidence: All transformer baselines include positional and structural
      encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2616
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2616
    true_std: 0.0018
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2616
    sort_std: 0.0018
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
  - model: SAN+LapPE
    model_key: san+lappe
    model_plain: SAN+LapPE
    value: 0.2683
    std: 0.0043
    paper_value: 0.2683
    paper_std: 0.0043
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: All transformer baselines include positional and structural
      encodings.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.268
    at_pub_std: 0.004
    at_pub_source_arxiv: '2502.01122'
    at_pub_source_title: Learning Efficient Positional Encodings with Graph Neural
      Networks
    at_pub_source_date_iso: '2025-02-03'
    at_pub_source_date_label: ICLR 2025
    value_gap_source_date_iso: '2025-02-03'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.268
    true_std: 0.004
    value_gap_source_arxiv: '2502.01122'
    value_gap_source_title: Learning Efficient Positional Encodings with Graph Neural
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.268
    sort_std: 0.004
    global_rank: 146
    paper_rank: 146
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRew-GatedGCN
    model_key: drew-gatedgcn
    model_plain: DRew-GatedGCN
    value: 0.2699
    std: 0.0018
    paper_value: 0.2699
    paper_std: 0.0018
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 10
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2699
    true_std: 0.0018
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2699
    sort_std: 0.0018
    global_rank: 149
    paper_rank: 149
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCON
    model_key: graphcon
    model_plain: GraphCON
    value: 0.2778
    std: 0.0018
    paper_value: 0.2778
    paper_std: 0.0018
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2778
    true_std: 0.0018
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2778
    sort_std: 0.0018
    global_rank: 152
    paper_rank: 152
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRew-GIN
    model_key: drew-gin
    model_plain: DRew-GIN
    value: 0.2799
    std: 0.0016
    paper_value: 0.2799
    paper_std: 0.0016
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 10
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2799
    true_std: 0.0016
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2799
    sort_std: 0.0016
    global_rank: 153
    paper_rank: 153
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: A-DGN
    model_key: a-dgn
    model_plain: A-DGN
    value: 0.2874
    std: 0.0021
    paper_value: 0.2874
    paper_std: 0.0021
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2874
    true_std: 0.0021
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2874
    sort_std: 0.0021
    global_rank: 155
    paper_rank: 155
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MixHop-GCN
    model_key: mixhop-gcn
    model_plain: MixHop-GCN
    value: 0.2921
    std: 0.0023
    paper_value: 0.2921
    paper_std: 0.0023
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 10
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2921
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2921
    true_std: 0.0023
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2921
    sort_std: 0.0023
    global_rank: 156
    paper_rank: 156
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DIGL+MPNN
    model_key: digl+mpnn
    model_plain: DIGL+MPNN
    value: 0.3173
    std: 0.0007
    paper_value: 0.3173
    paper_std: 0.0007
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 10
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3173
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2310.07430'
    at_pub_source_title: Non-backtracking Graph Neural Networks
    at_pub_source_date_iso: '2023-10-11'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3173
    true_std: 0.0007
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3173
    sort_std: 0.0007
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
  - model: GRAND
    model_key: grand
    model_plain: GRAND
    value: 0.3418
    std: 0.0015
    paper_value: 0.3418
    paper_std: 0.0015
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3418
    true_std: 0.0015
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3418
    sort_std: 0.0015
    global_rank: 168
    paper_rank: 168
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.3471
    std: 0.001
    paper_value: 0.3471
    paper_std: 0.001
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
    input_feature_source: raw_features
    feature_source_evidence: Note that all MPNN-based methods include structural and
      positional encoding.
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE on official LRGB split
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3471
    at_pub_std: 0.001
    at_pub_source_arxiv: '2206.08164'
    at_pub_source_title: LRGB
    at_pub_source_date_iso: '2022-06-16'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2023-06-06'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3471
    true_std: 0.001
    value_gap_source_arxiv: '2306.03561'
    value_gap_source_title: 'CIN++: Enhancing Topological Message Passing'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3471
    sort_std: 0.001
    global_rank: 169
    paper_rank: 169
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
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
- &id005
  dataset: Questions
  rows:
  - model: Tango GPS
    model_key: graphsage + unigap
    model_plain: Tango GPS
    value: 0.8421
    std: 0.008
    metric: ROC-AUC
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
    global_rank: 1
    sort_value: 0.8421
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango GPS
    model_key: h2gcn + unigap
    model_plain: Tango GPS
    value: 0.8359
    std: 0.007
    metric: ROC-AUC
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
    global_rank: 2
    sort_value: 0.8359
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango GPS
    model_key: gcn + unigap
    model_plain: Tango GPS
    value: 0.8273
    std: 0.009
    metric: ROC-AUC
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
    sort_value: 0.8273
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango GatedGCN
    model_key: tango gatedgcn
    model_plain: Tango GatedGCN
    value: 0.8039
    std: 0.0104
    paper_value: 0.8039
    paper_std: 0.0104
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8039
    true_std: 0.0104
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8039
    sort_std: 0.0104
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
  - model: Tango GPS
    model_key: tango gps
    model_plain: Tango GPS
    value: 0.8032
    std: 0.0107
    paper_value: 0.8032
    paper_std: 0.0107
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8032
    true_std: 0.0107
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8032
    sort_std: 0.0107
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Co-GNN(Σ,Σ)
    model_key: co-gnn(σ,σ)
    model_plain: Co-GNN(Σ,Σ)
    value: 0.8002
    std: 0.0086
    paper_value: 0.8002
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8002
    true_std: 0.0086
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8002
    sort_std: 0.0086
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7928
    at_pub_std: 0.008
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.15689999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    global_rank: 14
    paper_rank: 137
    rank_delta: 123
    rank_delta_abs: 123
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7886
    at_pub_std: 0.0092
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-19'
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
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7886
    sort_std: 0.0092
    global_rank: 23
    paper_rank: 23
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7805
    at_pub_std: 0.0093
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-06-22'
    value_gap_source_date_label: ICML 2023
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
    value_gap_source_arxiv: '2306.12943'
    value_gap_source_title: Evolving Computation Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7805
    sort_std: 0.0093
    global_rank: 29
    paper_rank: 29
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7795
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2405.15540'
    at_pub_source_title: Bundle Neural Networks for message diffusion on graphs
    at_pub_source_date_iso: '2024-05-24'
    at_pub_source_date_label: '2024'
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
    true_value: 0.7795
    true_std: 0.0068
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7795
    sort_std: 0.0068
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
  - model: GPS GCN+Performer (LapPE)
    model_key: gps gcn+performer (lappe)
    model_plain: GPS GCN+Performer (LapPE)
    value: 0.7785
    std: 0.0125
    paper_value: 0.7785
    paper_std: 0.0125
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7785
    true_std: 0.0125
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7785
    sort_std: 0.0125
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
  - model: GAT (RWSE)
    model_key: gat (rwse)
    model_plain: GAT (RWSE)
    value: 0.7783
    std: 0.0122
    paper_value: 0.7783
    paper_std: 0.0122
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7783
    true_std: 0.0122
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7783
    sort_std: 0.0122
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
  - model: GCN (RWSE)
    model_key: gcn (rwse)
    model_plain: GCN (RWSE)
    value: 0.7781
    std: 0.014
    paper_value: 0.7781
    paper_std: 0.014
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7781
    true_std: 0.014
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7781
    sort_std: 0.014
    global_rank: 36
    paper_rank: 36
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7724
    at_pub_std: 0.0126
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
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
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7724
    sort_std: 0.0126
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
  - model: GPS GAT+Performer (RWSE)
    model_key: gps gat+performer (rwse)
    model_plain: GPS GAT+Performer (RWSE)
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
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7714
    sort_std: 0.0149
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7679
    at_pub_std: 0.0071
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
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
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7679
    sort_std: 0.0071
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
  - model: Gated-GCN
    model_key: gated-gcn
    model_plain: Gated-GCN
    value: 0.7661
    std: 0.0113
    paper_value: 0.7661
    paper_std: 0.0113
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7661
    true_std: 0.0113
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7661
    sort_std: 0.0113
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7644
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-06-22'
    value_gap_source_date_label: ICML 2023
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
    value_gap_source_arxiv: '2306.12943'
    value_gap_source_title: Evolving Computation Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7644
    sort_std: 0.0062
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
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.7576
    std: 0.0166
    paper_value: 0.7576
    paper_std: 0.0166
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7576
    at_pub_std: 0.0166
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7576
    true_std: 0.0166
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7576
    sort_std: 0.0166
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7447
    at_pub_std: 0.0086
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
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
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7447
    sort_std: 0.0086
    global_rank: 81
    paper_rank: 81
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7442
    at_pub_std: 0.013
    at_pub_source_arxiv: '2505.14033'
    at_pub_source_title: 'Partition-wise Graph Filtering: A Unified Perspective Through
      the Lens of Graph Coarsening'
    at_pub_source_date_iso: '2025-05-20'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.08679999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7442
    true_std: 0.013
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: false
    value_gap: 0.08679999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7442
    sort_std: 0.013
    global_rank: 83
    paper_rank: 127
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    comparison_source_arxiv: '2505.14033'
    is_best: false
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.7394
    std: 0.0106
    paper_value: 0.7394
    paper_std: 0.0106
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7394
    at_pub_std: 0.0106
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7394
    true_std: 0.0106
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7394
    sort_std: 0.0106
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7388
    at_pub_std: 0.0116
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
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
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7388
    sort_std: 0.0116
    global_rank: 87
    paper_rank: 87
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.6817
    std: 0.0153
    paper_value: 0.6817
    paper_std: 0.0153
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6817
    at_pub_std: 0.0153
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6817
    true_std: 0.0153
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6817
    sort_std: 0.0153
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6709
    at_pub_std: 0.0263
    at_pub_source_arxiv: '2411.05274'
    at_pub_source_title: Distributed-Order Fractional Graph Operating Network
    at_pub_source_date_iso: '2024-11-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.011300000000000088
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6596
    true_std: 0.0195
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6596
    sort_std: 0.0195
    global_rank: 127
    paper_rank: 127
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Questions dataset split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7341
    at_pub_std: 0.0124
    at_pub_source_arxiv: '2411.05274'
    at_pub_source_title: Distributed-Order Fractional Graph Operating Network
    at_pub_source_date_iso: '2024-11-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.17930000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5548
    true_std: 0.0091
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5548
    sort_std: 0.0091
    global_rank: 157
    paper_rank: 157
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Distributed-Order Fractional Graph Operating Network
    comparison_source_arxiv: '2411.05274'
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
- &id003
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
  - model: Tango_GatedGCN
    model_key: tango_gatedgcn
    model_plain: Tango_GatedGCN
    value: 0.9189
    std: 0.003
    paper_value: 0.9189
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9189
    true_std: 0.003
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9189
    sort_std: 0.003
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
  - model: Co-GNN(Σ,Σ)
    model_key: co-gnn(σ,σ)
    model_plain: Co-GNN(Σ,Σ)
    value: 0.9157
    std: 0.0032
    paper_value: 0.9157
    paper_std: 0.0032
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
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9157
    true_std: 0.0032
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9157
    sort_std: 0.0032
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
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.9108
    std: 0.0057
    paper_value: 0.9108
    paper_std: 0.0057
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9108
    true_std: 0.0057
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9108
    sort_std: 0.0057
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
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.8903
    std: 0.0037
    paper_value: 0.8903
    paper_std: 0.0037
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
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8903
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8903
    true_std: 0.0037
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8903
    sort_std: 0.0037
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8875
    at_pub_std: 0.0041
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
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
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8875
    sort_std: 0.0041
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.8769
    std: 0.005
    paper_value: 0.8769
    paper_std: 0.005
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8769
    at_pub_std: 0.005
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-02-13'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8769
    true_std: 0.005
    value_gap_source_arxiv: '2402.08678'
    value_gap_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.005
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
  - model: GPS_GAT+Performer (RWSE)
    model_key: gps_gat+performer (rwse)
    model_plain: GPS_GAT+Performer (RWSE)
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8704
    sort_std: 0.0058
    global_rank: 60
    paper_rank: 60
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT (RWSE)
    model_key: gat (rwse)
    model_plain: GAT (RWSE)
    value: 0.8662
    std: 0.0053
    paper_value: 0.8662
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8662
    true_std: 0.0053
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8662
    sort_std: 0.0053
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8574
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2202.07082'
    at_pub_source_title: 'Graph Neural Networks for Graphs with Heterophily: A Survey'
    at_pub_source_date_iso: '2022-02-14'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-14'
    value_gap_source_date_label: '2022'
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
    value_gap_source_arxiv: '2202.07082'
    value_gap_source_title: 'Graph Neural Networks for Graphs with Heterophily: A
      Survey'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8574
    sort_std: 0.0067
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
  - model: GCN (RWSE)
    model_key: gcn (rwse)
    model_plain: GCN (RWSE)
    value: 0.8484
    std: 0.0055
    paper_value: 0.8484
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
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8484
    true_std: 0.0055
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8484
    sort_std: 0.0055
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
  - model: GPS_GCN+Performer (RWSE)
    model_key: gps_gcn+performer (rwse)
    model_plain: GPS_GCN+Performer (RWSE)
    value: 0.8472
    std: 0.0065
    paper_value: 0.8472
    paper_std: 0.0065
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8472
    true_std: 0.0065
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8472
    sort_std: 0.0065
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
  - model: GPS + Mamba
    model_key: gps + mamba
    model_plain: GPS + Mamba
    value: 0.831
    std: 0.0028
    paper_value: 0.831
    paper_std: 0.0028
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.831
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-02-13'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.831
    true_std: 0.0028
    value_gap_source_arxiv: '2402.08678'
    value_gap_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.831
    sort_std: 0.0028
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
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.82
    std: 0.0061
    paper_value: 0.82
    paper_std: 0.0061
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.82
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-02-13'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.82
    true_std: 0.0061
    value_gap_source_arxiv: '2402.08678'
    value_gap_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.82
    sort_std: 0.0061
    global_rank: 86
    paper_rank: 86
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7992
    at_pub_std: 0.0056
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
    true_value: 0.7992
    true_std: 0.0056
    value_gap_source_arxiv: '2512.14908'
    value_gap_source_title: 'ATLAS: Adaptive Topology-based Learning at Scale for
      Homophilic and Heterophilic Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7992
    sort_std: 0.0056
    global_rank: 94
    paper_rank: 94
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7587
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-04-26'
    value_gap_source_date_label: ICLR 2024
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
    value_gap_source_arxiv: '2404.17099'
    value_gap_source_title: Unleashing the Potential of Fractional Calculus in Graph
      Neural Networks with FROND
    value_gap_source_is_current_paper: false
    value_gap: 0.013000000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.7587
    sort_std: 0.0043
    global_rank: 110
    paper_rank: 113
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7571
    at_pub_std: 0.0139
    at_pub_source_arxiv: '2406.19249'
    at_pub_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer for
      Node Classification'
    at_pub_source_date_iso: '2024-06-27'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.1049
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
    global_rank: 111
    paper_rank: 147
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    comparison_source_arxiv: '2406.19249'
    is_best: false
    is_std_outlier: false
  - model: Gated-GCN
    model_key: gated-gcn
    model_plain: Gated-GCN
    value: 0.7446
    std: 0.0054
    paper_value: 0.7446
    paper_std: 0.0054
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
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7446
    at_pub_std: 0.0054
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-02-13'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7446
    true_std: 0.0054
    value_gap_source_arxiv: '2402.08678'
    value_gap_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7446
    sort_std: 0.0054
    global_rank: 115
    paper_rank: 115
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
    global_rank: 116
    paper_rank: 130
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
    is_best: false
    is_std_outlier: false
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.7434
    std: 0.0077
    paper_value: 0.7434
    paper_std: 0.0077
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
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7434
    at_pub_std: 0.0077
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7434
    true_std: 0.0077
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7434
    sort_std: 0.0077
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7337
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-04-26'
    value_gap_source_date_label: ICLR 2024
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
    value_gap_source_arxiv: '2404.17099'
    value_gap_source_title: Unleashing the Potential of Fractional Calculus in Graph
      Neural Networks with FROND
    value_gap_source_is_current_paper: false
    value_gap: 0.08520000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.7337
    sort_std: 0.0068
    global_rank: 121
    paper_rank: 149
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Convection-Diffusion with Heterophily
    comparison_source_arxiv: '2305.16780'
    is_best: false
    is_std_outlier: false
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.7159
    std: 0.0125
    paper_value: 0.7159
    paper_std: 0.0125
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
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7159
    at_pub_std: 0.0125
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7159
    true_std: 0.0125
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7159
    sort_std: 0.0125
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
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6809
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2305.16780'
    at_pub_source_title: Graph Neural Convection-Diffusion with Heterophily
    at_pub_source_date_iso: '2023-05-26'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2024-04-26'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.07979999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6809
    true_std: 0.0029
    value_gap_source_arxiv: '2404.17099'
    value_gap_source_title: Unleashing the Potential of Fractional Calculus in Graph
      Neural Networks with FROND
    value_gap_source_is_current_paper: false
    value_gap: 0.07979999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.6809
    sort_std: 0.0029
    global_rank: 136
    paper_rank: 163
    rank_delta: 27
    rank_delta_abs: 27
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
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
    paper_rank: 166
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral GNN via Two-dimensional (2-D) Graph Convolution
    comparison_source_arxiv: '2404.04559'
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: platonov2023a
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy on the standard split for Roman-empire
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6396
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-03-19'
    value_gap_source_date_label: TMLR 2024
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
    value_gap_source_arxiv: '2403.12529'
    value_gap_source_title: Contextualized Messages Boost Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6396
    sort_std: 0.0062
    global_rank: 156
    paper_rank: 156
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
  dataset: SSSP
  rows:
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.2863
    std: 0.1843
    paper_value: 0.2863
    paper_std: 0.1843
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: SAGE
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test set log10(MSE) averaged on 4 random weight initializations.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2863
    at_pub_std: 0.1843
    at_pub_source_arxiv: '2505.18728'
    at_pub_source_title: 'Message-Passing State-Space Models: Improving Graph Learning
      with Modern Sequence Modeling'
    at_pub_source_date_iso: '2025-05-24'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2863
    true_std: 0.1843
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2863
    sort_std: 0.1843
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.6951
    std: 0.1499
    paper_value: 0.6951
    paper_std: 0.1499
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: veličković2018graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test set log10(MSE) averaged on 4 random weight initializations.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6951
    at_pub_std: 0.1499
    at_pub_source_arxiv: '2505.18728'
    at_pub_source_title: 'Message-Passing State-Space Models: Improving Graph Learning
      with Modern Sequence Modeling'
    at_pub_source_date_iso: '2025-05-24'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6951
    true_std: 0.1499
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6951
    sort_std: 0.1499
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9499
    std: 0.0001
    paper_value: 0.9499
    paper_std: 0.0001
    metric: log10(MSE)
    higher_is_better: false
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
    source_ref: Kipf2016
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test set log10(MSE) averaged on 4 random weight initializations.
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9499
    at_pub_std: 0.0001
    at_pub_source_arxiv: '2505.18728'
    at_pub_source_title: 'Message-Passing State-Space Models: Improving Graph Learning
      with Modern Sequence Modeling'
    at_pub_source_date_iso: '2025-05-24'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9499
    true_std: 0.0001
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9499
    sort_std: 0.0001
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
  rank_metric: log10(MSE)
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MSE
  paper_metrics:
  - log10(MSE)
  metric: log10(MSE)
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id006
  dataset: Tolokers
  rows:
  - model: Tango_GPS
    model_key: tango_gps
    model_plain: Tango_GPS
    value: 0.8566
    std: 0.0101
    paper_value: 0.8566
    paper_std: 0.0101
    metric: AUC
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8566
    true_std: 0.0101
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8566
    sort_std: 0.0101
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
  - model: Tango_GatedGCN
    model_key: tango_gatedgcn
    model_plain: Tango_GatedGCN
    value: 0.8551
    std: 0.0098
    paper_value: 0.8551
    paper_std: 0.0098
    metric: AUC
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8551
    true_std: 0.0098
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8551
    sort_std: 0.0098
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
  - model: GCN (RWSE)
    model_key: gcn (rwse)
    model_plain: GCN (RWSE)
    value: 0.8511
    std: 0.0077
    paper_value: 0.8511
    paper_std: 0.0077
    metric: AUC
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8511
    true_std: 0.0077
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8511
    sort_std: 0.0077
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT (RWSE)
    model_key: gat (rwse)
    model_plain: GAT (RWSE)
    value: 0.8502
    std: 0.0067
    paper_value: 0.8502
    paper_std: 0.0067
    metric: AUC
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8502
    true_std: 0.0067
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8502
    sort_std: 0.0067
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS_GCN+Performer (RWSE)
    model_key: gps_gcn+performer (rwse)
    model_plain: GPS_GCN+Performer (RWSE)
    value: 0.8481
    std: 0.0086
    paper_value: 0.8481
    paper_std: 0.0086
    metric: AUC
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8481
    true_std: 0.0086
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8481
    sort_std: 0.0086
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
  - model: GPS_GAT+Transformer (LapPE)
    model_key: gps_gat+transformer (lappe)
    model_plain: GPS_GAT+Transformer (LapPE)
    value: 0.847
    std: 0.0056
    paper_value: 0.847
    paper_std: 0.0056
    metric: AUC
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.847
    true_std: 0.0056
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.847
    sort_std: 0.0056
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS_GAT+Performer (LapPE)
    model_key: gps_gat+performer (lappe)
    model_plain: GPS_GAT+Performer (LapPE)
    value: 0.8462
    std: 0.0054
    paper_value: 0.8462
    paper_std: 0.0054
    metric: AUC
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8462
    true_std: 0.0054
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8462
    sort_std: 0.0054
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
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.8452
    std: 0.0021
    paper_value: 0.8452
    paper_std: 0.0021
    metric: AUC
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8452
    true_std: 0.0021
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8452
    sort_std: 0.0021
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Co-GNN(μ,μ)
    model_key: co-gnn(μ,μ)
    model_plain: Co-GNN(μ,μ)
    value: 0.8445
    std: 0.0117
    paper_value: 0.8445
    paper_std: 0.0117
    metric: AUC
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8445
    true_std: 0.0117
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8445
    sort_std: 0.0117
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
  - model: GAT-sep
    model_key: gat-sep
    model_plain: GAT-sep
    value: 0.8378
    std: 0.0043
    paper_value: 0.8378
    paper_std: 0.0043
    metric: AUC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8378
    sort_std: 0.0043
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
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.8377
    std: 0.0078
    paper_value: 0.8377
    paper_std: 0.0078
    metric: AUC
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8377
    true_std: 0.0078
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8377
    sort_std: 0.0078
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS + Mamba
    model_key: gps + mamba
    model_plain: GPS + Mamba
    value: 0.837
    std: 0.0105
    paper_value: 0.837
    paper_std: 0.0105
    metric: AUC
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.837
    true_std: 0.0105
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.837
    sort_std: 0.0105
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS_GCN+Transformer (RWSE)
    model_key: gps_gcn+transformer (rwse)
    model_plain: GPS_GCN+Transformer (RWSE)
    value: 0.8353
    std: 0.0106
    paper_value: 0.8353
    paper_std: 0.0106
    metric: AUC
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8353
    true_std: 0.0106
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8353
    sort_std: 0.0106
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
  - model: GT
    model_key: gt
    model_plain: GT
    value: 0.8323
    std: 0.0064
    paper_value: 0.8323
    paper_std: 0.0064
    metric: AUC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8323
    sort_std: 0.0064
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GOAT
    model_key: goat
    model_plain: GOAT
    value: 0.8311
    std: 0.0104
    paper_value: 0.8311
    paper_std: 0.0104
    metric: AUC
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8311
    true_std: 0.0104
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8311
    sort_std: 0.0104
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
    value: 0.8276
    std: 0.0061
    paper_value: 0.8276
    paper_std: 0.0061
    metric: AUC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8276
    sort_std: 0.0061
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
  - model: GT-sep
    model_key: gt-sep
    model_plain: GT-sep
    value: 0.8252
    std: 0.0092
    paper_value: 0.8252
    paper_std: 0.0092
    metric: AUC
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8252
    sort_std: 0.0092
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8243
    std: 0.0044
    paper_value: 0.8243
    paper_std: 0.0044
    metric: AUC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8243
    sort_std: 0.0044
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
  - model: GBK-GNN
    model_key: gbk-gnn
    model_plain: GBK-GNN
    value: 0.8101
    std: 0.0067
    paper_value: 0.8101
    paper_std: 0.0067
    metric: AUC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8101
    sort_std: 0.0067
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
  - model: NAGphormer
    model_key: nagphormer
    model_plain: NAGphormer
    value: 0.7832
    std: 0.0095
    paper_value: 0.7832
    paper_std: 0.0095
    metric: AUC
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7832
    true_std: 0.0095
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7832
    sort_std: 0.0095
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
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.7775
    std: 0.0105
    paper_value: 0.7775
    paper_std: 0.0105
    metric: AUC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7775
    true_std: 0.0105
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7775
    sort_std: 0.0105
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
  - model: Gated-GCN
    model_key: gated-gcn
    model_plain: Gated-GCN
    value: 0.7731
    std: 0.0114
    paper_value: 0.7731
    paper_std: 0.0114
    metric: AUC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7731
    true_std: 0.0114
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7731
    sort_std: 0.0114
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
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.7339
    std: 0.0117
    paper_value: 0.7339
    paper_std: 0.0117
    metric: AUC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7339
    sort_std: 0.0117
    global_rank: 23
    paper_rank: 23
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
    metric: AUC
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7336
    sort_std: 0.0101
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
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.7335
    std: 0.0101
    paper_value: 0.7335
    paper_std: 0.0101
    metric: AUC
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7335
    true_std: 0.0101
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7335
    sort_std: 0.0101
    global_rank: 25
    paper_rank: 25
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
    metric: AUC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7294
    sort_std: 0.0097
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
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.6866
    std: 0.0065
    paper_value: 0.6866
    paper_std: 0.0065
    metric: AUC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test AUC on Tolokers split from Platonov et al. 2023a
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-08-07'
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
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6866
    sort_std: 0.0065
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
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - AUC
  metric: AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
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
  - *id006
  - *id007
- benchmark: GNNBenchmark
  datasets:
  - *id008
  - *id009
  - *id010
  - *id011
- benchmark: Algorithmic Graph Tasks
  datasets:
  - *id012
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Roman-empire
      dataset_slug: roman-empire
    - dataset: Amazon-ratings
      dataset_slug: amazon-ratings
    - dataset: Questions
      dataset_slug: questions
    - dataset: Tolokers
      dataset_slug: tolokers
    - dataset: Minesweeper
      dataset_slug: minesweeper
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: CLUSTER
      dataset_slug: cluster
    - dataset: PATTERN
      dataset_slug: pattern
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: Peptides-struct
      dataset_slug: peptides-struct
    - dataset: Peptides-func
      dataset_slug: peptides-func
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: MNIST
      dataset_slug: mnist
    - dataset: CIFAR10
      dataset_slug: cifar10
  - benchmark: Algorithmic Graph Tasks
    benchmark_slug: algorithmic-graph-tasks
    datasets:
    - dataset: SSSP
      dataset_slug: sssp
main_figure: /figures/2508.05070/main_figure.jpegoptim.jpg
---

