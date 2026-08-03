---
title: 'gLSTM: Mitigating Over-Squashing by Increasing Storage Capacity'
arxiv_id: '2510.08450'
source_url: ''
authors:
- name: Hugh Blayney
  orcid: null
  s2_author_id: '2384765555'
  s2_url: null
- name: Alvaro Arroyo
  orcid: null
  s2_author_id: '2238953003'
  s2_url: null
- name: Xiaowen Dong
  orcid: null
  s2_author_id: '2239060705'
  s2_url: null
- name: Michael M. Bronstein
  orcid: null
  s2_author_id: '2261389035'
  s2_url: null
published_date: Oct 9, 2025
published_date_iso: '2025-10-09'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Neural Networks (GNNs) leverage the graph structure to transmit information
  between nodes, typically through the message-passing mechanism. While these models
  have found a wide variety of applications, they are known to suffer from over-squashing,
  where information from a large receptive field of node representations is collapsed
  into a single fixed sized vector, resulting in an information bottleneck. In this
  paper, we re-examine the over-squashing phenomenon through the lens of model storage
  and retrieval capacity, which we define as the amount of information that can be
  stored in a node's representation for later use. We study some of the limitations
  of existing tasks used to measure over-squashing and introduce a new synthetic task
  to demonstrate that an information bottleneck can saturate this capacity. Furthermore,
  we adapt ideas from the sequence modeling literature on associative memories, fast
  weight programmers, and the xLSTM model to develop a novel GNN architecture with
  improved capacity. We demonstrate strong performance of this architecture both on
  our capacity synthetic task, as well as a range of real-world graph benchmarks.
codebase_url: https://github.com/HughBlayney/gLSTM
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MPNNs
mrr: 0.1754
adjusted_mrr: 0.117
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
  - model: SAN+RWSE
    model_key: s^2gcn
    model_plain: SAN+RWSE
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.686
    std: 0.005
    paper_value: 0.686
    paper_std: 0.005
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Tonshoff 2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.686
    at_pub_std: 0.005
    at_pub_source_arxiv: '2405.11951'
    at_pub_source_title: 'Distinguished In Uniform: Self Attention Vs. Virtual Nodes'
    at_pub_source_date_iso: '2024-05-20'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7261
    true_std: 0.0011
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.040099999999999913
    has_value_note: false
    value_note: ''
    sort_value: 0.7261
    sort_std: 0.0011
    global_rank: 2
    paper_rank: 38
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MPNNs
    model_key: mpnns
    model_plain: MPNNs
    value: 0.725
    std: 0.0023
    paper_value: 0.725
    paper_std: 0.0023
    metric: AP
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
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.725
    true_std: 0.0023
    value_gap_source_arxiv: '2510.08450'
    value_gap_source_title: 'gLSTM: Mitigating Over-Squashing by Increasing Storage
      Capacity'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.725
    sort_std: 0.0023
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
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.6765
    std: 0.0047
    paper_value: 0.6765
    paper_std: 0.0047
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6765
    at_pub_std: 0.0047
    at_pub_source_arxiv: '2405.11951'
    at_pub_source_title: 'Distinguished In Uniform: Self Attention Vs. Virtual Nodes'
    at_pub_source_date_iso: '2024-05-20'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7006
    true_std: 0.0033
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.02410000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7006
    sort_std: 0.0033
    global_rank: 22
    paper_rank: 46
    rank_delta: 24
    rank_delta_abs: 24
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRew-GCN
    model_key: drew-gcn
    model_plain: DRew-GCN
    value: 0.6804
    std: 0.0144
    paper_value: 0.6804
    paper_std: 0.0144
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Arroyo 2025
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
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
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.6996
    true_std: 0.0076
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.019199999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.6996
    sort_std: 0.0076
    global_rank: 23
    paper_rank: 44
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: kGCN-SSM
    model_key: kgcn-ssm
    model_plain: kGCN-SSM
    value: 0.6902
    std: 0.0022
    paper_value: 0.6902
    paper_std: 0.0022
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Arroyo 2025
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7212
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2502.10818'
    at_pub_source_title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing
      in GNNs: Bridging Recurrent and Graph Learning'
    at_pub_source_date_iso: '2025-02-15'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-10-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.030999999999999917
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6902
    true_std: 0.0022
    value_gap_source_arxiv: '2510.08450'
    value_gap_source_title: 'gLSTM: Mitigating Over-Squashing by Increasing Storage
      Capacity'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6902
    sort_std: 0.0022
    global_rank: 36
    paper_rank: 36
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing
      in GNNs: Bridging Recurrent and Graph Learning'
    comparison_source_arxiv: '2502.10818'
    is_best: false
    is_std_outlier: false
  - model: GINE
    model_key: gine
    model_plain: GINE
    value: 0.6621
    std: 0.0067
    paper_value: 0.6621
    paper_std: 0.0067
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6621
    at_pub_std: 0.0067
    at_pub_source_arxiv: '2405.11951'
    at_pub_source_title: 'Distinguished In Uniform: Self Attention Vs. Virtual Nodes'
    at_pub_source_date_iso: '2024-05-20'
    at_pub_source_date_label: ICLR 2024
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
    true_value: 0.6621
    true_std: 0.0067
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6621
    sort_std: 0.0067
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
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.6534
    std: 0.0091
    paper_value: 0.6534
    paper_std: 0.0091
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6535
    at_pub_std: 0.0041
    at_pub_source_arxiv: '2404.09774'
    at_pub_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    at_pub_source_date_iso: '2024-04-15'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-04-15'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6535
    true_std: 0.0041
    value_gap_source_arxiv: '2404.09774'
    value_gap_source_title: 'RandAlign: A Parameter-Free Method for Regularizing Graph
      Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.6535
    sort_std: 0.0041
    global_rank: 74
    paper_rank: 74
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
    value: 0.246
    std: 0.0007
    paper_value: 0.246
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Tonshoff 2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
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
    gap_vs_at_pub: 0.003899999999999987
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
    value_gap: 0.003899999999999987
    has_value_note: false
    value_note: ''
    sort_value: 0.2421
    sort_std: 0.0016
    global_rank: 1
    paper_rank: 11
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Can Classic GNNs Be Strong Baselines for Graph-level
      Tasks? Simple Architectures Meet Excellence
    comparison_source_arxiv: '2502.09263'
    is_best: true
    is_std_outlier: false
  - model: SAN+RWSE
    model_key: nba-gin+lappe
    model_plain: SAN+RWSE
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
    global_rank: 2
    sort_value: 0.2424
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SAN+RWSE
    model_key: gin
    model_plain: SAN+RWSE
    value: 0.2429
    std: 0.0019
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
    global_rank: 3
    sort_value: 0.2429
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.2477
    std: 0.0009
    paper_value: 0.2477
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: Tonshoff 2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
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
    gap_vs_at_pub: 0.004599999999999993
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
    value_gap: 0.004599999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.2431
    sort_std: 0.002
    global_rank: 4
    paper_rank: 26
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Can Classic GNNs Be Strong Baselines for Graph-level
      Tasks? Simple Architectures Meet Excellence
    comparison_source_arxiv: '2502.09263'
    is_best: true
    is_std_outlier: false
  - model: GINE
    model_key: gine
    model_plain: GINE
    value: 0.2473
    std: 0.0017
    paper_value: 0.2473
    paper_std: 0.0017
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
    source_ref: Tonshoff 2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2473
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2405.11951'
    at_pub_source_title: 'Distinguished In Uniform: Self Attention Vs. Virtual Nodes'
    at_pub_source_date_iso: '2024-05-20'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-11-19'
    value_gap_source_date_label: KDD 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2473
    true_std: 0.0017
    value_gap_source_arxiv: '2411.12732'
    value_gap_source_title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2473
    sort_std: 0.0017
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
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.2509
    std: 0.0014
    paper_value: 0.2509
    paper_std: 0.0014
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
    table_ref: Table 1
    source_ref: Tonshoff 2023
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2509
    at_pub_std: 0.0014
    at_pub_source_arxiv: '2405.11951'
    at_pub_source_title: 'Distinguished In Uniform: Self Attention Vs. Virtual Nodes'
    at_pub_source_date_iso: '2024-05-20'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-10-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2509
    true_std: 0.0014
    value_gap_source_arxiv: '2510.08450'
    value_gap_source_title: 'gLSTM: Mitigating Over-Squashing by Increasing Storage
      Capacity'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2509
    sort_std: 0.0014
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
  - model: MPNNs
    model_key: mpnns
    model_plain: MPNNs
    value: 0.2527
    std: 0.0015
    paper_value: 0.2527
    paper_std: 0.0015
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
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2527
    true_std: 0.0015
    value_gap_source_arxiv: '2510.08450'
    value_gap_source_title: 'gLSTM: Mitigating Over-Squashing by Increasing Storage
      Capacity'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2527
    sort_std: 0.0015
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
  - model: kGCN-SSM
    model_key: kgcn-ssm
    model_plain: kGCN-SSM
    value: 0.2581
    std: 0.0003
    paper_value: 0.2581
    paper_std: 0.0003
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
    table_ref: Table 1
    source_ref: Arroyo 2025
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2701
    at_pub_std: 0.0007
    at_pub_source_arxiv: '2502.10818'
    at_pub_source_title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing
      in GNNs: Bridging Recurrent and Graph Learning'
    at_pub_source_date_iso: '2025-02-15'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-10-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.01200000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2581
    true_std: 0.0003
    value_gap_source_arxiv: '2510.08450'
    value_gap_source_title: 'gLSTM: Mitigating Over-Squashing by Increasing Storage
      Capacity'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2581
    sort_std: 0.0003
    global_rank: 80
    paper_rank: 80
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'On Vanishing Gradients, Over-Smoothing, and Over-Squashing
      in GNNs: Bridging Recurrent and Graph Learning'
    comparison_source_arxiv: '2502.10818'
    is_best: false
    is_std_outlier: false
  - model: DRew-GCN
    model_key: drew-gcn
    model_plain: DRew-GCN
    value: 0.2766
    std: 0.0019
    paper_value: 0.2766
    paper_std: 0.0019
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
    source_ref: Arroyo 2025
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: LRGB benchmark, standard split
    date: Oct 9, 2025
    date_display: Oct 2025
    date_iso: '2025-10-09'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2536
    at_pub_std: null
    at_pub_source_arxiv: '2410.23686'
    at_pub_source_title: Towards Dynamic Message Passing on Graphs
    at_pub_source_date_iso: '2024-10-31'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2025-10-09'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.02300000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2766
    true_std: 0.0019
    value_gap_source_arxiv: '2510.08450'
    value_gap_source_title: 'gLSTM: Mitigating Over-Squashing by Increasing Storage
      Capacity'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2766
    sort_std: 0.0019
    global_rank: 100
    paper_rank: 100
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Dynamic Message Passing on Graphs
    comparison_source_arxiv: '2410.23686'
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
single_proposed_model: MPNNs
main_figure: /figures/2510.08450/main_figure.jpegoptim.jpg
---

