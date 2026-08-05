---
title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
arxiv_id: '2307.08430'
source_url: ''
authors:
- name: Chao Li
  orcid: null
  s2_author_id: '2150358360'
  s2_url: null
- name: Zijie Guo
  orcid: null
  s2_author_id: '2046803199'
  s2_url: null
- name: Qiuting He
  orcid: null
  s2_author_id: '108500695'
  s2_url: null
- name: Hao Xu
  orcid: null
  s2_author_id: '2108836012'
  s2_url: null
- name: Kun He
  orcid: null
  s2_author_id: '1702188'
  s2_url: null
published_date: Jul 17, 2023
published_date_iso: '2023-07-17'
published_venue: NeurIPS 2023
published_conference: NeurIPS 2023
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: 'Utilizing long-range dependency, a concept extensively studied in homogeneous
  graphs, remains underexplored in heterogeneous graphs, especially on large ones,
  posing two significant challenges: Reducing computational costs while maximizing
  effective information utilization in the presence of heterogeneity, and overcoming
  the over-smoothing issue in graph neural networks. To address this gap, we investigate
  the importance of different meta-paths and introduce an automatic framework for
  utilizing long-range dependency on heterogeneous graphs, denoted as Long-range Meta-path
  Search through Progressive Sampling (LMSPS). Specifically, we develop a search space
  with all meta-paths related to the target node type. By employing a progressive
  sampling algorithm, LMSPS dynamically shrinks the search space with hop-independent
  time complexity. Through a sampling evaluation strategy, LMSPS conducts a specialized
  and effective meta-path selection, leading to retraining with only effective meta-paths,
  thus mitigating costs and over-smoothing. Extensive experiments across diverse heterogeneous
  datasets validate LMSPS''s capability in discovering effective long-range meta-paths,
  surpassing state-of-the-art methods. Our code is available at.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- LMSPS
- LMSPS+LP
- LMSPS+LP+MS
mrr: 0.1395
adjusted_mrr: 0.1395
mrr_dataset_count: 5
benchmark_categories:
- OGB
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 4
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id003
  dataset: ACM
  rows:
  - model: HetGNN
    model_key: hetgnn
    model_plain: HetGNN
    value: 0.8605
    std: 0.0025
    paper_value: 0.8605
    paper_std: 0.0025
    metric: Micro-F1
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
    source_ref: HetGNN2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.8605
    at_pub_std: 0.0025
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.979
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.11849999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.979
    sort_std: null
    global_rank: 1
    paper_rank: 97
    rank_delta: 96
    rank_delta_abs: 96
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: comch
    model_plain: SlotGAT
    value: 0.947
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.05750'
    title: Are Heterogeneous Graph Neural Networks Truly Effective? A Causal Perspective
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    venue: Knowledge-Based Systems
    codebase_url: https://github.com/YXNTU/CausalHGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.947
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LMSPS
    model_key: lmsps
    model_plain: LMSPS
    value: 0.9469
    std: 0.0036
    paper_value: 0.9469
    paper_std: 0.0036
    metric: Micro-F1
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
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9469
    true_std: 0.0036
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9469
    sort_std: 0.0036
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
  - model: SlotGAT
    model_key: slotgat
    model_plain: SlotGAT
    value: 0.9406
    std: 0.0022
    paper_value: 0.9406
    paper_std: 0.0022
    metric: Micro-F1
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
    source_ref: slotgat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9406
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9406
    sort_std: null
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
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.9141
    std: 0.0075
    paper_value: 0.9141
    paper_std: 0.0075
    metric: Micro-F1
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
    source_ref: RGCN2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9141
    at_pub_std: 0.0075
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9402
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.026100000000000012
    has_value_note: false
    value_note: ''
    sort_value: 0.9402
    sort_std: null
    global_rank: 7
    paper_rank: 53
    rank_delta: 46
    rank_delta_abs: 46
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    value: 0.9387
    std: 0.005
    paper_value: 0.9387
    paper_std: 0.005
    metric: Micro-F1
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
    source_ref: yang2022simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9398
    at_pub_std: 0.0036
    at_pub_source_arxiv: '2207.02547'
    at_pub_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    at_pub_source_date_iso: '2022-07-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0010999999999999899
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9398
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.0010999999999999899
    has_value_note: false
    value_note: ''
    sort_value: 0.9398
    sort_std: null
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HINormer
    model_key: hinormer
    model_plain: HINormer
    value: 0.9383
    std: 0.0045
    paper_value: 0.9383
    paper_std: 0.0045
    metric: Micro-F1
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
    source_ref: mao2023hinormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9383
    true_std: 0.0045
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9383
    sort_std: 0.0045
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
  - model: PMMM
    model_key: pmmm
    model_plain: PMMM
    value: 0.9371
    std: 0.0017
    paper_value: 0.9371
    paper_std: 0.0017
    metric: Micro-F1
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
    source_ref: li2022differentiable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9371
    true_std: 0.0017
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9371
    sort_std: 0.0017
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
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    value: 0.9077
    std: 0.0065
    paper_value: 0.9077
    paper_std: 0.0065
    metric: Micro-F1
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
    source_ref: fu2020magnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9077
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9361
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.028400000000000092
    has_value_note: false
    value_note: ''
    sort_value: 0.9361
    sort_std: null
    global_rank: 17
    paper_rank: 59
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Simple-HGN
    model_key: simple-hgn
    model_plain: Simple-HGN
    value: 0.9335
    std: 0.0045
    paper_value: 0.9335
    paper_std: 0.0045
    metric: Micro-F1
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
    source_ref: lv2021we
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9335
    at_pub_std: 0.0045
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9335
    true_std: 0.0045
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9335
    sort_std: 0.0045
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
  - model: NARS
    model_key: nars
    model_plain: NARS
    value: 0.9331
    std: 0.0033
    paper_value: 0.9331
    paper_std: 0.0033
    metric: Micro-F1
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
    source_ref: yu2020scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9331
    true_std: 0.0033
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9331
    sort_std: 0.0033
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9219
    std: 0.0093
    paper_value: 0.9219
    paper_std: 0.0093
    metric: Micro-F1
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
    source_ref: GAT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9278
    at_pub_std: null
    at_pub_source_arxiv: '2007.08294'
    at_pub_source_title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
      Graphs
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-07-16'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.005899999999999905
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9278
    true_std: null
    value_gap_source_arxiv: '2007.08294'
    value_gap_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.005899999999999905
    has_value_note: false
    value_note: ''
    sort_value: 0.9278
    sort_std: null
    global_rank: 31
    paper_rank: 43
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GTN
    model_key: gtn
    model_plain: GTN
    value: 0.912
    std: 0.0071
    paper_value: 0.912
    paper_std: 0.0071
    metric: Micro-F1
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
    source_ref: yun2019graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9258
    at_pub_std: null
    at_pub_source_arxiv: '2007.08294'
    at_pub_source_title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
      Graphs
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-07-16'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.013799999999999923
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9258
    true_std: null
    value_gap_source_arxiv: '2007.08294'
    value_gap_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.013799999999999923
    has_value_note: false
    value_note: ''
    sort_value: 0.9258
    sort_std: null
    global_rank: 34
    paper_rank: 56
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    comparison_source_arxiv: '2007.08294'
    is_best: false
    is_std_outlier: false
  - model: GraphMSE
    model_key: graphmse
    model_plain: GraphMSE
    value: 0.9254
    std: 0.0014
    paper_value: 0.9254
    paper_std: 0.0014
    metric: Micro-F1
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
    source_ref: li2021graphmse
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9254
    true_std: 0.0014
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9254
    sort_std: 0.0014
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9212
    std: 0.0023
    paper_value: 0.9212
    paper_std: 0.0023
    metric: Micro-F1
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
    source_ref: GCN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9246
    at_pub_std: null
    at_pub_source_arxiv: '2007.08294'
    at_pub_source_title: Self-supervised Auxiliary Learning with Meta-paths for Heterogeneous
      Graphs
    at_pub_source_date_iso: '2020-07-16'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-07-16'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.0033999999999999586
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9246
    true_std: null
    value_gap_source_arxiv: '2007.08294'
    value_gap_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.0033999999999999586
    has_value_note: false
    value_note: ''
    sort_value: 0.9246
    sort_std: null
    global_rank: 36
    paper_rank: 45
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Self-supervised Auxiliary Learning with Meta-paths for
      Heterogeneous Graphs
    comparison_source_arxiv: '2007.08294'
    is_best: false
    is_std_outlier: false
  - model: space4HGNN
    model_key: space4hgnn
    model_plain: space4HGNN
    value: 0.9238
    std: 0.001
    paper_value: 0.9238
    paper_std: 0.001
    metric: Micro-F1
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
    source_ref: zhao2022space4hgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9238
    true_std: 0.001
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9238
    sort_std: 0.001
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
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.9079
    std: 0.0043
    paper_value: 0.9079
    paper_std: 0.0043
    metric: Micro-F1
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
    source_ref: wang2019heterogeneous
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9079
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9185
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.010599999999999943
    has_value_note: false
    value_note: ''
    sort_value: 0.9185
    sort_std: null
    global_rank: 50
    paper_rank: 59
    rank_delta: 9
    rank_delta_abs: 9
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.91
    std: 0.0076
    paper_value: 0.91
    paper_std: 0.0076
    metric: Micro-F1
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
    source_ref: HGT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.91
    at_pub_std: 0.0076
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2024-12-01'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.916
    true_std: 0.006
    value_gap_source_arxiv: '2412.00742'
    value_gap_source_title: Revisiting Self-Supervised Heterogeneous Graph Learning
      from Spectral Clustering Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.006000000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.916
    sort_std: 0.006
    global_rank: 53
    paper_rank: 58
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.9082
    std: 0.0093
    paper_value: 0.9082
    paper_std: 0.0093
    metric: Micro-F1
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
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9082
    true_std: 0.0093
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9082
    sort_std: 0.0093
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
  - model: RSHN
    model_key: rshn
    model_plain: RSHN
    value: 0.9032
    std: 0.0154
    paper_value: 0.9032
    paper_std: 0.0154
    metric: Micro-F1
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
    source_ref: RSHN2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9032
    at_pub_std: 0.0154
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9032
    true_std: 0.0154
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9032
    sort_std: 0.0154
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
  - model: HetSANN
    model_key: hetsann
    model_plain: HetSANN
    value: 0.8991
    std: 0.0037
    paper_value: 0.8991
    paper_std: 0.0037
    metric: Micro-F1
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
    source_ref: HetSANN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.8991
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8991
    true_std: 0.0037
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8991
    sort_std: 0.0037
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
  - model: DiffMG
    model_key: diffmg
    model_plain: DiffMG
    value: 0.8807
    std: 0.0304
    paper_value: 0.8807
    paper_std: 0.0304
    metric: Micro-F1
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
    source_ref: DingYZZ21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for ACM
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8807
    true_std: 0.0304
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8807
    sort_std: 0.0304
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
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: DBLP
  rows:
  - model: SlotGAT
    model_key: herec
    model_plain: SlotGAT
    value: 0.9993
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_display: Dec 2019
    date_iso: '2019-12-19'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/didi/hetsann
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9993
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HetSANN
    model_key: hetsann
    model_plain: HetSANN
    value: 0.8056
    std: 0.015
    paper_value: 0.8056
    paper_std: 0.015
    metric: Micro-F1
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
    source_ref: HetSANN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9972
    at_pub_std: null
    at_pub_source_arxiv: '1912.10832'
    at_pub_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    at_pub_source_date_iso: '2019-12-19'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2019-12-19'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: 0.1916
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9972
    true_std: null
    value_gap_source_arxiv: '1912.10832'
    value_gap_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.1916
    has_value_note: false
    value_note: ''
    sort_value: 0.9972
    sort_std: null
    global_rank: 2
    paper_rank: 125
    rank_delta: 123
    rank_delta_abs: 123
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    comparison_source_arxiv: '1912.10832'
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: deepwalk
    model_plain: SlotGAT
    value: 0.9941
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '1912.10832'
    title: An Attention-based Graph Neural Network for Heterogeneous Structural Learning
    date: Dec 19, 2019
    date_display: Dec 2019
    date_iso: '2019-12-19'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/didi/hetsann
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9941
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LMSPS
    model_key: lmsps
    model_plain: LMSPS
    value: 0.9566
    std: 0.002
    paper_value: 0.9566
    paper_std: 0.002
    metric: Micro-F1
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
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9566
    true_std: 0.002
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9566
    sort_std: 0.002
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
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    value: 0.9524
    std: 0.0013
    paper_value: 0.9524
    paper_std: 0.0013
    metric: Micro-F1
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
    source_ref: yang2022simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9542
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2207.02547'
    at_pub_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    at_pub_source_date_iso: '2022-07-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0018000000000000238
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9542
    true_std: 0.0017
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.0018000000000000238
    has_value_note: false
    value_note: ''
    sort_value: 0.9542
    sort_std: 0.0017
    global_rank: 11
    paper_rank: 12
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SlotGAT
    model_key: slotgat
    model_plain: SlotGAT
    value: 0.9531
    std: 0.0019
    paper_value: 0.9531
    paper_std: 0.0019
    metric: Micro-F1
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
    source_ref: slotgat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9531
    true_std: 0.0019
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9531
    sort_std: 0.0019
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
  - model: PMMM
    model_key: pmmm
    model_plain: PMMM
    value: 0.9514
    std: 0.0022
    paper_value: 0.9514
    paper_std: 0.0022
    metric: Micro-F1
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
    source_ref: li2022differentiable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9514
    true_std: 0.0022
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9514
    sort_std: 0.0022
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
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.9207
    std: 0.005
    paper_value: 0.9207
    paper_std: 0.005
    metric: Micro-F1
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
    source_ref: RGCN2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9207
    at_pub_std: 0.005
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.95
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.029299999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.95
    sort_std: null
    global_rank: 18
    paper_rank: 71
    rank_delta: 53
    rank_delta_abs: 53
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HINormer
    model_key: hinormer
    model_plain: HINormer
    value: 0.9494
    std: 0.0021
    paper_value: 0.9494
    paper_std: 0.0021
    metric: Micro-F1
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
    source_ref: mao2023hinormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9494
    at_pub_std: 0.0021
    at_pub_source_arxiv: '2302.11329'
    at_pub_source_title: 'HINormer: Representation Learning On Heterogeneous Information
      Networks with Graph Transformer'
    at_pub_source_date_iso: '2023-02-22'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-02-22'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9494
    true_std: 0.0021
    value_gap_source_arxiv: '2302.11329'
    value_gap_source_title: 'HINormer: Representation Learning On Heterogeneous Information
      Networks with Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9494
    sort_std: 0.0021
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
  - model: space4HGNN
    model_key: space4hgnn
    model_plain: space4HGNN
    value: 0.9463
    std: 0.004
    paper_value: 0.9463
    paper_std: 0.004
    metric: Micro-F1
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
    source_ref: zhao2022space4hgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9463
    true_std: 0.004
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9463
    sort_std: 0.004
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
  - model: NARS
    model_key: nars
    model_plain: NARS
    value: 0.9461
    std: 0.0042
    paper_value: 0.9461
    paper_std: 0.0042
    metric: Micro-F1
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
    source_ref: yu2020scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.804
    at_pub_std: 0.032
    at_pub_source_arxiv: '2208.06129'
    at_pub_source_title: Multiplex Heterogeneous Graph Convolutional Network
    at_pub_source_date_iso: '2022-08-12'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.1421
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9461
    true_std: 0.0042
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9461
    sort_std: 0.0042
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Multiplex Heterogeneous Graph Convolutional Network
    comparison_source_arxiv: '2208.06129'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9147
    std: 0.0034
    paper_value: 0.9147
    paper_std: 0.0034
    metric: Micro-F1
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
    source_ref: GCN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.931
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.016300000000000092
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.946
    true_std: 0.0031
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.031299999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.946
    sort_std: 0.0031
    global_rank: 28
    paper_rank: 76
    rank_delta: 48
    rank_delta_abs: 48
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9339
    std: 0.003
    paper_value: 0.9339
    paper_std: 0.003
    metric: Micro-F1
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
    source_ref: GAT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9339
    at_pub_std: 0.003
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9448
    true_std: 0.0022
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.01090000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9448
    sort_std: 0.0022
    global_rank: 29
    paper_rank: 51
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Simple-HGN
    model_key: simple-hgn
    model_plain: Simple-HGN
    value: 0.9446
    std: 0.0022
    paper_value: 0.9446
    paper_std: 0.0022
    metric: Micro-F1
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
    source_ref: lv2021we
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9446
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9448
    true_std: 0.0038
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.9448
    sort_std: 0.0038
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphMSE
    model_key: graphmse
    model_plain: GraphMSE
    value: 0.9444
    std: 0.0013
    paper_value: 0.9444
    paper_std: 0.0013
    metric: Micro-F1
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
    source_ref: li2021graphmse
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9444
    true_std: 0.0013
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9444
    sort_std: 0.0013
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
  - model: DiffMG
    model_key: diffmg
    model_plain: DiffMG
    value: 0.942
    std: 0.0036
    paper_value: 0.942
    paper_std: 0.0036
    metric: Micro-F1
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
    source_ref: DBLP:conf/kdd/DingYZZ21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.942
    true_std: 0.0036
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.942
    sort_std: 0.0036
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
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.9384
    std: 0.0053
    paper_value: 0.9384
    paper_std: 0.0053
    metric: Micro-F1
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
    protocol_note: Average of 20 random samples of meta-paths
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9384
    true_std: 0.0053
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9384
    sort_std: 0.0053
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
  - model: RSHN
    model_key: rshn
    model_plain: RSHN
    value: 0.9381
    std: 0.0055
    paper_value: 0.9381
    paper_std: 0.0055
    metric: Micro-F1
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
    source_ref: RSHN2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9381
    at_pub_std: 0.0055
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9381
    true_std: 0.0055
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9381
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
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    value: 0.9376
    std: 0.0045
    paper_value: 0.9376
    paper_std: 0.0045
    metric: Micro-F1
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
    source_ref: fu2020magnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9456
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.008000000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9376
    true_std: 0.0045
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9376
    sort_std: 0.0045
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.9205
    std: 0.0062
    paper_value: 0.9205
    paper_std: 0.0062
    metric: Micro-F1
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
    source_ref: wang2019heterogeneous
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9327
    at_pub_std: 0.0058
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-11-14'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.012199999999999989
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9369
    true_std: null
    value_gap_source_arxiv: '2311.07929'
    value_gap_source_title: Variational Graph Autoencoder for Heterogeneous Information
      Networks with Missing and Inaccurate Attributes
    value_gap_source_is_current_paper: false
    value_gap: 0.01639999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9369
    sort_std: null
    global_rank: 46
    paper_rank: 71
    rank_delta: 25
    rank_delta_abs: 25
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    comparison_source_arxiv: '2210.00248'
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.9349
    std: 0.0025
    paper_value: 0.9349
    paper_std: 0.0025
    metric: Micro-F1
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
    source_ref: HGT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9365
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0016000000000000458
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9349
    true_std: 0.0025
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9349
    sort_std: 0.0025
    global_rank: 48
    paper_rank: 48
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HetGNN
    model_key: hetgnn
    model_plain: HetGNN
    value: 0.9233
    std: 0.0041
    paper_value: 0.9233
    paper_std: 0.0041
    metric: Micro-F1
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
    source_ref: HetGNN2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on DBLP
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.9336
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.010299999999999976
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9233
    true_std: 0.0041
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: 0.0041
    global_rank: 67
    paper_rank: 67
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id005
  dataset: Freebase
  rows:
  - model: SlotGAT
    model_key: gc-hgnn
    model_plain: SlotGAT
    value: 0.6247
    std: 0.0042
    metric: Macro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    venue: IEEE Transactions on Big Data
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    is_global_top: true
    global_rank: 1
    sort_value: 0.6247
    sort_std: 0.0042
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: hgmae
    model_plain: SlotGAT
    value: 0.6082
    std: 0.0051
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    venue: IEEE Transactions on Big Data
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    is_global_top: true
    global_rank: 2
    sort_value: 0.6082
    sort_std: 0.0051
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SlotGAT
    model_key: heco
    model_plain: SlotGAT
    value: 0.5987
    std: 0.0033
    metric: Macro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2404.02810'
    title: Generative-Contrastive Heterogeneous Graph Neural Network
    date: Apr 3, 2024
    date_display: Apr 2024
    date_iso: '2024-04-03'
    venue: IEEE Transactions on Big Data
    codebase_url: https://github.com/wangyu0627/GC-HGNN
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: Uses X and A (features and structure)
    is_global_top: true
    global_rank: 3
    sort_value: 0.5987
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.2131
    std: 0.0168
    paper_value: 0.2131
    paper_std: 0.0168
    metric: Macro-F1
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
    source_ref: wang2019heterogeneous
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.6011
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.38799999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.585
    true_std: 0.0093
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.37189999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.585
    sort_std: 0.0093
    global_rank: 8
    paper_rank: 39
    rank_delta: 31
    rank_delta_abs: 31
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.2928
    std: 0.0252
    paper_value: 0.2928
    paper_std: 0.0252
    metric: Macro-F1
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
    source_ref: HGT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.6176
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-04-03'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.32480000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.583
    true_std: 0.0072
    value_gap_source_arxiv: '2404.02810'
    value_gap_source_title: Generative-Contrastive Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.29019999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.583
    sort_std: 0.0072
    global_rank: 9
    paper_rank: 35
    rank_delta: 26
    rank_delta_abs: 26
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: LMSPS
    model_key: lmsps
    model_plain: LMSPS
    value: 0.5326
    std: 0.0047
    paper_value: 0.5326
    paper_std: 0.0047
    metric: Macro-F1
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
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5326
    true_std: 0.0047
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5326
    sort_std: 0.0047
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
  - model: HINormer
    model_key: hinormer
    model_plain: HINormer
    value: 0.5218
    std: 0.0039
    paper_value: 0.5218
    paper_std: 0.0039
    metric: Macro-F1
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
    source_ref: mao2023hinormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5218
    true_std: 0.0039
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5218
    sort_std: 0.0039
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
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    value: 0.5071
    std: 0.0044
    paper_value: 0.5071
    paper_std: 0.0044
    metric: Macro-F1
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
    source_ref: yang2022simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.5187
    at_pub_std: 0.0086
    at_pub_source_arxiv: '2207.02547'
    at_pub_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    at_pub_source_date_iso: '2022-07-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.011600000000000055
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.5187
    true_std: 0.0086
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.011600000000000055
    has_value_note: false
    value_note: ''
    sort_value: 0.5187
    sort_std: 0.0086
    global_rank: 16
    paper_rank: 16
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NARS
    model_key: nars
    model_plain: NARS
    value: 0.4998
    std: 0.0177
    paper_value: 0.4998
    paper_std: 0.0177
    metric: Macro-F1
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
    source_ref: yu2020scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4998
    true_std: 0.0177
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4998
    sort_std: 0.0177
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
  - model: SlotGAT
    model_key: slotgat
    model_plain: SlotGAT
    value: 0.4968
    std: 0.0197
    paper_value: 0.4968
    paper_std: 0.0197
    metric: Macro-F1
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
    source_ref: slotgat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4968
    true_std: 0.0197
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4968
    sort_std: 0.0197
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
  - model: Simple-HGN
    model_key: simple-hgn
    model_plain: Simple-HGN
    value: 0.4772
    std: 0.0148
    paper_value: 0.4772
    paper_std: 0.0148
    metric: Macro-F1
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
    source_ref: lv2021we
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.4772
    at_pub_std: 0.0148
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4772
    true_std: 0.0148
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4772
    sort_std: 0.0148
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
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.4678
    std: 0.0157
    paper_value: 0.4678
    paper_std: 0.0157
    metric: Macro-F1
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
    source_ref: RGCN2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.4678
    at_pub_std: 0.0077
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4678
    true_std: 0.0077
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4678
    sort_std: 0.0077
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
  - model: space4HGNN
    model_key: space4hgnn
    model_plain: space4HGNN
    value: 0.4137
    std: 0.0449
    paper_value: 0.4137
    paper_std: 0.0449
    metric: Macro-F1
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
    source_ref: zhao2022space4hgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4137
    true_std: 0.0449
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4137
    sort_std: 0.0449
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.4074
    std: 0.0258
    paper_value: 0.4074
    paper_std: 0.0258
    metric: Macro-F1
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
    source_ref: GAT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.5109
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.10350000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4074
    true_std: 0.0258
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4074
    sort_std: 0.0258
    global_rank: 31
    paper_rank: 31
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.2784
    std: 0.0313
    paper_value: 0.2784
    paper_std: 0.0313
    metric: Macro-F1
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
    source_ref: GCN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for Freebase
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.609
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.3306
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2935
    true_std: null
    value_gap_source_arxiv: '2403.04780'
    value_gap_source_title: Graph-oriented Instruction Tuning of Large Language Models
      for Generic Graph Mining
    value_gap_source_is_current_paper: false
    value_gap: 0.015100000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.2935
    sort_std: null
    global_rank: 35
    paper_rank: 36
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.2122
    std: 0.0258
    paper_value: 0.2122
    paper_std: 0.0258
    metric: Macro-F1
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
    protocol_note: Average of 20 random samples
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2122
    true_std: 0.0258
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2122
    sort_std: 0.0258
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
  rank_metric: Macro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Macro-F1
  paper_metrics:
  - Macro-F1
  metric: Macro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: IMDB
  rows:
  - model: SlotGAT
    model_key: gat bgnn(m)-sc
    model_plain: SlotGAT
    value: 0.8133
    std: 0.0179
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8133
    sort_std: 0.0179
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: sage ban
    model_plain: SlotGAT
    value: 0.8073
    std: 0.002
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8073
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SlotGAT
    model_key: gat bgnn(m)-cs
    model_plain: SlotGAT
    value: 0.8033
    std: 0.0094
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8033
    sort_std: 0.0094
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    value: 0.6821
    std: 0.0032
    paper_value: 0.6821
    paper_std: 0.0032
    metric: Micro-F1
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
    source_ref: yang2022simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.7342
    at_pub_std: 0.0047
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.052099999999999924
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7342
    true_std: 0.0047
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.052099999999999924
    has_value_note: false
    value_note: ''
    sort_value: 0.7342
    sort_std: 0.0047
    global_rank: 32
    paper_rank: 43
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    comparison_source_arxiv: '2305.19872'
    is_best: false
    is_std_outlier: false
  - model: HetSANN
    model_key: hetsann
    model_plain: HetSANN
    value: 0.5768
    std: 0.0044
    paper_value: 0.5768
    paper_std: 0.0044
    metric: Micro-F1
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
    source_ref: HetSANN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.7311
    at_pub_std: null
    at_pub_source_arxiv: '1912.10832'
    at_pub_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    at_pub_source_date_iso: '2019-12-19'
    at_pub_source_date_label: AAAI 2019
    value_gap_source_date_iso: '2019-12-19'
    value_gap_source_date_label: AAAI 2019
    gap_vs_at_pub: 0.1543
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7311
    true_std: null
    value_gap_source_arxiv: '1912.10832'
    value_gap_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.1543
    has_value_note: false
    value_note: ''
    sort_value: 0.7311
    sort_std: null
    global_rank: 34
    paper_rank: 100
    rank_delta: 66
    rank_delta_abs: 66
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: An Attention-based Graph Neural Network for Heterogeneous
      Structural Learning
    comparison_source_arxiv: '1912.10832'
    is_best: false
    is_std_outlier: false
  - model: LMSPS
    model_key: lmsps
    model_plain: LMSPS
    value: 0.687
    std: 0.0026
    paper_value: 0.687
    paper_std: 0.0026
    metric: Micro-F1
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
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.687
    true_std: 0.0026
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.687
    sort_std: 0.0026
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
  - model: SlotGAT
    model_key: slotgat
    model_plain: SlotGAT
    value: 0.6864
    std: 0.0033
    paper_value: 0.6864
    paper_std: 0.0033
    metric: Micro-F1
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
    source_ref: slotgat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6864
    true_std: 0.0033
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6864
    sort_std: 0.0033
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
  - model: GTN
    model_key: gtn
    model_plain: GTN
    value: 0.6514
    std: 0.0045
    paper_value: 0.6514
    paper_std: 0.0045
    metric: Micro-F1
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
    source_ref: yun2019graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.6827
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.031299999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6827
    true_std: 0.0065
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.031299999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.6827
    sort_std: 0.0065
    global_rank: 43
    paper_rank: 64
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    comparison_source_arxiv: '2305.19872'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6482
    std: 0.0064
    paper_value: 0.6482
    paper_std: 0.0064
    metric: Micro-F1
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
    source_ref: GCN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.6813
    at_pub_std: 0.0083
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.03310000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6813
    true_std: 0.0083
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.03310000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.6813
    sort_std: 0.0083
    global_rank: 45
    paper_rank: 67
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    comparison_source_arxiv: '2305.19872'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.6486
    std: 0.0043
    paper_value: 0.6486
    paper_std: 0.0043
    metric: Micro-F1
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
    source_ref: GAT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.6808
    at_pub_std: 0.0049
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.032200000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6808
    true_std: 0.0049
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.032200000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.6808
    sort_std: 0.0049
    global_rank: 46
    paper_rank: 66
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    comparison_source_arxiv: '2305.19872'
    is_best: false
    is_std_outlier: false
  - model: HINormer
    model_key: hinormer
    model_plain: HINormer
    value: 0.6783
    std: 0.0034
    paper_value: 0.6783
    paper_std: 0.0034
    metric: Micro-F1
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
    source_ref: mao2023hinormer
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.6783
    at_pub_std: 0.0034
    at_pub_source_arxiv: '2302.11329'
    at_pub_source_title: 'HINormer: Representation Learning On Heterogeneous Information
      Networks with Graph Transformer'
    at_pub_source_date_iso: '2023-02-22'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-02-22'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6783
    true_std: 0.0034
    value_gap_source_arxiv: '2302.11329'
    value_gap_source_title: 'HINormer: Representation Learning On Heterogeneous Information
      Networks with Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6783
    sort_std: 0.0034
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
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    value: 0.6467
    std: 0.0167
    paper_value: 0.6467
    paper_std: 0.0167
    metric: Micro-F1
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
    source_ref: fu2020magnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.6782
    at_pub_std: 0.0154
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.03149999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.6782
    true_std: 0.0154
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.03149999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.6782
    sort_std: 0.0154
    global_rank: 48
    paper_rank: 70
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.6463
    std: 0.0058
    paper_value: 0.6463
    paper_std: 0.0058
    metric: Micro-F1
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
    source_ref: wang2019heterogeneous
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.6769
    at_pub_std: 0.0064
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.03059999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6769
    true_std: 0.0064
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.03059999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.6769
    sort_std: 0.0064
    global_rank: 49
    paper_rank: 70
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    comparison_source_arxiv: '2305.19872'
    is_best: false
    is_std_outlier: false
  - model: PMMM
    model_key: pmmm
    model_plain: PMMM
    value: 0.6758
    std: 0.0022
    paper_value: 0.6758
    paper_std: 0.0022
    metric: Micro-F1
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
    source_ref: li2022differentiable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6758
    true_std: 0.0022
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6758
    sort_std: 0.0022
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
  - model: Simple-HGN
    model_key: simple-hgn
    model_plain: Simple-HGN
    value: 0.6736
    std: 0.0057
    paper_value: 0.6736
    paper_std: 0.0057
    metric: Micro-F1
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
    source_ref: lv2021we
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.6736
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6736
    true_std: 0.0057
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6736
    sort_std: 0.0057
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
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.672
    std: 0.0057
    paper_value: 0.672
    paper_std: 0.0057
    metric: Micro-F1
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
    source_ref: HGT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.672
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.672
    true_std: 0.0057
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.672
    sort_std: 0.0057
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
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.6205
    std: 0.0015
    paper_value: 0.6205
    paper_std: 0.0015
    metric: Micro-F1
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
    source_ref: RGCN2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.6651
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.04459999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6651
    true_std: 0.0028
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.04459999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.6651
    sort_std: 0.0028
    global_rank: 61
    paper_rank: 82
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    comparison_source_arxiv: '2305.19872'
    is_best: false
    is_std_outlier: false
  - model: NARS
    model_key: nars
    model_plain: NARS
    value: 0.6618
    std: 0.007
    paper_value: 0.6618
    paper_std: 0.007
    metric: Micro-F1
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
    source_ref: yu2020scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.574
    at_pub_std: 0.0048
    at_pub_source_arxiv: '2208.06129'
    at_pub_source_title: Multiplex Heterogeneous Graph Convolutional Network
    at_pub_source_date_iso: '2022-08-12'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.0878000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6618
    true_std: 0.007
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6618
    sort_std: 0.007
    global_rank: 63
    paper_rank: 63
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Multiplex Heterogeneous Graph Convolutional Network
    comparison_source_arxiv: '2208.06129'
    is_best: false
    is_std_outlier: false
  - model: RSHN
    model_key: rshn
    model_plain: RSHN
    value: 0.6422
    std: 0.0103
    paper_value: 0.6422
    paper_std: 0.0103
    metric: Micro-F1
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
    source_ref: RSHN2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.6422
    at_pub_std: 0.0103
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6422
    true_std: 0.0103
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6422
    sort_std: 0.0103
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
  - model: space4HGNN
    model_key: space4hgnn
    model_plain: space4HGNN
    value: 0.6396
    std: 0.0043
    paper_value: 0.6396
    paper_std: 0.0043
    metric: Micro-F1
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
    source_ref: zhao2022space4hgnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6396
    true_std: 0.0043
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6396
    sort_std: 0.0043
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
  - model: GraphMSE
    model_key: graphmse
    model_plain: GraphMSE
    value: 0.6237
    std: 0.0103
    paper_value: 0.6237
    paper_std: 0.0103
    metric: Micro-F1
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
    source_ref: li2021graphmse
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6237
    true_std: 0.0103
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6237
    sort_std: 0.0103
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
  - model: DiffMG
    model_key: diffmg
    model_plain: DiffMG
    value: 0.5975
    std: 0.0123
    paper_value: 0.5975
    paper_std: 0.0123
    metric: Micro-F1
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
    source_ref: DingYZZ21
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5975
    true_std: 0.0123
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5975
    sort_std: 0.0123
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
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.5383
    std: 0.0066
    paper_value: 0.5383
    paper_std: 0.0066
    metric: Micro-F1
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
    protocol_note: Random meta-paths average of 20 samples
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5383
    true_std: 0.0066
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5383
    sort_std: 0.0066
    global_rank: 114
    paper_rank: 114
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HetGNN
    model_key: hetgnn
    model_plain: HetGNN
    value: 0.5116
    std: 0.0065
    paper_value: 0.5116
    paper_std: 0.0065
    metric: Micro-F1
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
    source_ref: HetGNN2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard HGB benchmark evaluation for IMDB
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.5116
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5116
    true_std: 0.0065
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5116
    sort_std: 0.0065
    global_rank: 121
    paper_rank: 121
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Micro-F1
  metric: Micro-F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: ogbn-mag
  rows:
  - model: LMSPS+LP+MS
    model_key: lmsps+lp+ms
    model_plain: LMSPS+LP+MS
    value: 0.5784
    std: 0.0022
    paper_value: 0.5784
    paper_std: 0.0022
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag leaderboard
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5784
    true_std: 0.0022
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5784
    sort_std: 0.0022
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
  - model: SeHGNN+emb+ms
    model_key: sehgnn+emb+ms
    model_plain: SeHGNN+emb+ms
    value: 0.5719
    std: 0.0012
    paper_value: 0.5719
    paper_std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: yang2022simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag leaderboard
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.5719
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2207.02547'
    at_pub_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    at_pub_source_date_iso: '2022-07-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5719
    true_std: 0.0012
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5719
    sort_std: 0.0012
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
  - model: SeHGNN+LP+MS
    model_key: sehgnn+lp+ms
    model_plain: SeHGNN+LP+MS
    value: 0.5671
    std: 0.0014
    paper_value: 0.5671
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: yang2022simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag leaderboard
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5671
    true_std: 0.0014
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5671
    sort_std: 0.0014
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
  - model: ALS (GraphSAINT)
    model_key: sehgnn+ms
    model_plain: ALS (GraphSAINT)
    value: 0.5671
    std: 0.0014
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2207.02547'
    title: Simple and Efficient Heterogeneous Graph Neural Network
    date: Jul 6, 2022
    date_display: Jul 2022
    date_iso: '2022-07-06'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: https://github.com/ICT-GIMLab/SeHGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.5671
    sort_std: 0.0014
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LMSPS+LP
    model_key: lmsps+lp
    model_plain: LMSPS+LP
    value: 0.551
    std: 0.0011
    paper_value: 0.551
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag leaderboard
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.551
    true_std: 0.0011
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.551
    sort_std: 0.0011
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
  - model: LMSPS
    model_key: lmsps
    model_plain: LMSPS
    value: 0.5483
    std: 0.002
    paper_value: 0.5483
    paper_std: 0.002
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
    protocol_note: Test accuracy on ogbn-mag
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5483
    true_std: 0.002
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5483
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
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    value: 0.5145
    std: 0.0029
    paper_value: 0.5145
    paper_std: 0.0029
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
    source_ref: yang2022simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.5399
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2207.02547'
    at_pub_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    at_pub_source_date_iso: '2022-07-06'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.02540000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.5399
    true_std: 0.0018
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.02540000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.5399
    sort_std: 0.0018
    global_rank: 13
    paper_rank: 26
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    comparison_source_arxiv: '2207.02547'
    is_best: false
    is_std_outlier: false
  - model: SeHGNN+LP
    model_key: sehgnn+lp
    model_plain: SeHGNN+LP
    value: 0.5399
    std: 0.0018
    paper_value: 0.5399
    paper_std: 0.0018
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
    table_ref: Table 2
    source_ref: yang2022simple
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag leaderboard
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5399
    true_std: 0.0018
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5399
    sort_std: 0.0018
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
  - model: NARS
    model_key: nars
    model_plain: NARS
    value: 0.5066
    std: 0.0022
    paper_value: 0.5066
    paper_std: 0.0022
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
    source_ref: yu2020scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.524
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2108.10097'
    at_pub_source_title: Graph Attention MLP with Reliable Label Utilization
    at_pub_source_date_iso: '2021-08-23'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.01739999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.524
    true_std: 0.0016
    value_gap_source_arxiv: '2206.04355'
    value_gap_source_title: Graph Attention Multi-Layer Perceptron
    value_gap_source_is_current_paper: false
    value_gap: 0.01739999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.524
    sort_std: 0.0016
    global_rank: 20
    paper_rank: 28
    rank_delta: 8
    rank_delta_abs: 8
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Attention MLP with Reliable Label Utilization
    comparison_source_arxiv: '2108.10097'
    is_best: false
    is_std_outlier: false
  - model: GAMLP+LP
    model_key: gamlp+lp
    model_plain: GAMLP+LP
    value: 0.5163
    std: 0.0022
    paper_value: 0.5163
    paper_std: 0.0022
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
    table_ref: Table 2
    source_ref: GAMLP2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag leaderboard
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5163
    true_std: 0.0022
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5163
    sort_std: 0.0022
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
  - model: SAGN+LP
    model_key: sagn+lp
    model_plain: SAGN+LP
    value: 0.5117
    std: 0.0032
    paper_value: 0.5117
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: sun2021scalable
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag leaderboard
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5117
    true_std: 0.0032
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5117
    sort_std: 0.0032
    global_rank: 28
    paper_rank: 28
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.4678
    std: 0.0042
    paper_value: 0.4678
    paper_std: 0.0042
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
    source_ref: HGT
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.4927
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2108.10097'
    at_pub_source_title: Graph Attention MLP with Reliable Label Utilization
    at_pub_source_date_iso: '2021-08-23'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.024900000000000033
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4927
    true_std: 0.0061
    value_gap_source_arxiv: '2205.15653'
    value_gap_source_title: Label-Enhanced Graph Neural Network for Semi-supervised
      Node Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.024900000000000033
    has_value_note: false
    value_note: ''
    sort_value: 0.4927
    sort_std: 0.0061
    global_rank: 34
    paper_rank: 39
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Attention MLP with Reliable Label Utilization
    comparison_source_arxiv: '2108.10097'
    is_best: false
    is_std_outlier: false
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.4737
    std: 0.0048
    paper_value: 0.4737
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
    source_ref: RGCN2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.4796
    at_pub_std: null
    at_pub_source_arxiv: '2105.11122'
    at_pub_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    at_pub_source_date_iso: '2021-05-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-10-23'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.005900000000000016
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4811
    true_std: 0.0048
    value_gap_source_arxiv: '2310.14481'
    value_gap_source_title: Efficient Heterogeneous Graph Learning via Random Projection
    value_gap_source_is_current_paper: false
    value_gap: 0.007400000000000018
    has_value_note: false
    value_note: ''
    sort_value: 0.4811
    sort_std: 0.0048
    global_rank: 35
    paper_rank: 39
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    comparison_source_arxiv: '2105.11122'
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.4678
    std: 0.0067
    paper_value: 0.4678
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
    source_ref: hamilton2017inductive
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.3704
    at_pub_std: null
    at_pub_source_arxiv: '2105.11122'
    at_pub_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    at_pub_source_date_iso: '2021-05-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.09739999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4678
    true_std: 0.0067
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4678
    sort_std: 0.0067
    global_rank: 40
    paper_rank: 40
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    comparison_source_arxiv: '2105.11122'
    is_best: false
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.3514
    std: 0.0378
    paper_value: 0.3514
    paper_std: 0.0378
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
    protocol_note: Test accuracy on ogbn-mag using 30 random meta-paths
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3514
    true_std: 0.0378
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3514
    sort_std: 0.0378
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
    is_std_outlier: true
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.2692
    std: 0.0026
    paper_value: 0.2692
    paper_std: 0.0026
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
    source_ref: hu2020open
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy on ogbn-mag
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.3243
    at_pub_std: null
    at_pub_source_arxiv: '2105.11122'
    at_pub_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    at_pub_source_date_iso: '2021-05-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.05509999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2692
    true_std: 0.0026
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2692
    sort_std: 0.0026
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Representation Learning with Relation
      Awareness
    comparison_source_arxiv: '2105.11122'
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
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id002
  - *id003
  - *id004
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbn-mag
      dataset_slug: ogbn-mag
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
    - dataset: ACM
      dataset_slug: acm
    - dataset: IMDB
      dataset_slug: imdb
    - dataset: Freebase
      dataset_slug: freebase
main_figure: /figures/2307.08430/main_figure.jpegoptim.jpg
---

