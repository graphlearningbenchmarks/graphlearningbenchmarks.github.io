---
title: Long-Range Graph Wavelet Networks
arxiv_id: '2509.06743'
source_url: ''
authors:
- name: Filippo Guerranti
  orcid: null
  s2_author_id: '2141201998'
  s2_url: null
- name: F. Forte
  orcid: null
  s2_author_id: '50366388'
  s2_url: null
- name: Simon Geisler
  orcid: null
  s2_author_id: '79462643'
  s2_url: null
- name: Stephan Gunnemann
  orcid: null
  s2_author_id: '51249380'
  s2_url: null
published_date: Sep 8, 2025
published_date_iso: '2025-09-08'
published_venue: NeurIPS 2025
published_conference: NeurIPS 2025
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Modeling long-range interactions, the propagation of information across
  distant parts of a graph, is a central challenge in graph machine learning. Graph
  wavelets, inspired by multi-resolution signal processing, provide a principled way
  to capture both local and global structures. However, existing wavelet-based graph
  neural networks rely on finite-order polynomial approximations, which limit their
  receptive fields and hinder long-range propagation. We propose Long-Range Graph
  Wavelet Networks (LR-GWN), which decompose wavelet filters into complementary local
  and global components. Local aggregation is handled with efficient low-order polynomials,
  while long-range interactions are captured through a flexible spectral-domain parameterization.
  This hybrid design unifies short- and long-distance information flow within a principled
  wavelet framework. Experiments show that LR-GWN achieves state-of-the-art performance
  among wavelet-based methods on long-range benchmarks, while remaining competitive
  on short-range datasets.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- LR-GWN
mrr: 0.0772
adjusted_mrr: 0.0515
mrr_dataset_count: 2
benchmark_categories:
- LRGB
benchmark_coverage:
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 2
  total: 5
task_categories:
- graph_classification
- graph_regression
experiment_scopes:
- graph-level
results:
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
  - model: LR-GWN
    model_key: lr-gwn
    model_plain: LR-GWN
    value: 0.7216
    std: 0.0041
    paper_value: 0.7216
    paper_std: 0.0041
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: TR variant of Peptides-Func
    date: Sep 8, 2025
    date_display: Sep 2025
    date_iso: '2025-09-08'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-08'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7216
    true_std: 0.0041
    value_gap_source_arxiv: '2509.06743'
    value_gap_source_title: Long-Range Graph Wavelet Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7216
    sort_std: 0.0041
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
  - model: WaveGC
    model_key: wavegc
    model_plain: WaveGC
    value: 0.6973
    std: 0.0043
    paper_value: 0.6973
    paper_std: 0.0043
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu_advancing_2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: TR variant of Peptides-Func
    date: Sep 8, 2025
    date_display: Sep 2025
    date_iso: '2025-09-08'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-08'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6973
    true_std: 0.0043
    value_gap_source_arxiv: '2509.06743'
    value_gap_source_title: Long-Range Graph Wavelet Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6973
    sort_std: 0.0043
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
  - model: DEFT
    model_key: deft
    model_plain: DEFT
    value: 0.6695
    std: 0.0063
    paper_value: 0.6695
    paper_std: 0.0063
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: bastos_learnable_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: TR variant of Peptides-Func
    date: Sep 8, 2025
    date_display: Sep 2025
    date_iso: '2025-09-08'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-08'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6695
    true_std: 0.0063
    value_gap_source_arxiv: '2509.06743'
    value_gap_source_title: Long-Range Graph Wavelet Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6695
    sort_std: 0.0063
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
  - model: GWNN
    model_key: gwnn
    model_plain: GWNN
    value: 0.6547
    std: 0.0048
    paper_value: 0.6547
    paper_std: 0.0048
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: xu_graph_2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: TR variant of Peptides-Func
    date: Sep 8, 2025
    date_display: Sep 2025
    date_iso: '2025-09-08'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-08'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6547
    true_std: 0.0048
    value_gap_source_arxiv: '2509.06743'
    value_gap_source_title: Long-Range Graph Wavelet Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6547
    sort_std: 0.0048
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
  - model: SGWT
    model_key: sgwt
    model_plain: SGWT
    value: 0.6023
    std: 0.0027
    paper_value: 0.6023
    paper_std: 0.0027
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: hammond_wavelets_2011
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: TC variant of Peptides-Func
    date: Sep 8, 2025
    date_display: Sep 2025
    date_iso: '2025-09-08'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-08'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6023
    true_std: 0.0027
    value_gap_source_arxiv: '2509.06743'
    value_gap_source_title: Long-Range Graph Wavelet Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6023
    sort_std: 0.0027
    global_rank: 150
    paper_rank: 150
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
  - model: GMN
    model_key: gcn
    model_plain: GMN
    value: 0.2421
    std: 0.0016
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_display: May 2026
    date_iso: '2026-05-12'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.2421
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GMN
    model_key: tango_gps
    model_plain: GMN
    value: 0.2422
    std: 0.0014
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.05070'
    title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential Flows'
    date: Aug 7, 2025
    date_display: Aug 2025
    date_iso: '2025-08-07'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: Tango does not use additional encodings.
    is_global_top: true
    global_rank: 2
    sort_value: 0.2422
    sort_std: 0.0014
    comparison_type: global_top
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
  - model: LR-GWN
    model_key: lr-gwn
    model_plain: LR-GWN
    value: 0.2462
    std: 0.0006
    paper_value: 0.2462
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard split for Peptides-struct (TR variant)
    date: Sep 8, 2025
    date_display: Sep 2025
    date_iso: '2025-09-08'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-08'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2462
    true_std: 0.0006
    value_gap_source_arxiv: '2509.06743'
    value_gap_source_title: Long-Range Graph Wavelet Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2462
    sort_std: 0.0006
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
  - model: WaveGC
    model_key: wavegc
    model_plain: WaveGC
    value: 0.2495
    std: 0.0007000000000000001
    paper_value: 0.2495
    paper_std: 0.0007000000000000001
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: liu_advancing_2024
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard split for Peptides-struct
    date: Sep 8, 2025
    date_display: Sep 2025
    date_iso: '2025-09-08'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-08'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2495
    true_std: 0.0007000000000000001
    value_gap_source_arxiv: '2509.06743'
    value_gap_source_title: Long-Range Graph Wavelet Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2495
    sort_std: 0.0007000000000000001
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
  - model: DEFT
    model_key: deft
    model_plain: DEFT
    value: 0.2506
    std: 0.0013
    paper_value: 0.2506
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: bastos_learnable_2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard split for Peptides-struct
    date: Sep 8, 2025
    date_display: Sep 2025
    date_iso: '2025-09-08'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-08'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2506
    true_std: 0.0013
    value_gap_source_arxiv: '2509.06743'
    value_gap_source_title: Long-Range Graph Wavelet Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2506
    sort_std: 0.0013
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
  - model: SGWT
    model_key: sgwt
    model_plain: SGWT
    value: 0.2539
    std: 0.0021
    paper_value: 0.2539
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: hammond_wavelets_2011
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard split for Peptides-struct
    date: Sep 8, 2025
    date_display: Sep 2025
    date_iso: '2025-09-08'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-08'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2539
    true_std: 0.0021
    value_gap_source_arxiv: '2509.06743'
    value_gap_source_title: Long-Range Graph Wavelet Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2539
    sort_std: 0.0021
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
  - model: GWNN
    model_key: gwnn
    model_plain: GWNN
    value: 0.2734
    std: 0.0004
    paper_value: 0.2734
    paper_std: 0.0004
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
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: xu_graph_2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Standard split for Peptides-struct
    date: Sep 8, 2025
    date_display: Sep 2025
    date_iso: '2025-09-08'
    published_venue: NeurIPS 2025
    published_conference: NeurIPS 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-09-08'
    value_gap_source_date_label: NeurIPS 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2734
    true_std: 0.0004
    value_gap_source_arxiv: '2509.06743'
    value_gap_source_title: Long-Range Graph Wavelet Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2734
    sort_std: 0.0004
    global_rank: 150
    paper_rank: 150
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
results_grouped:
- benchmark: LRGB
  datasets:
  - *id001
  - *id002
datasets_by_scope:
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
single_proposed_model: LR-GWN
main_figure: /figures/2509.06743/main_figure.jpegoptim.jpg
---

