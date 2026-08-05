---
title: Are Heterogeneous Graph Neural Networks Truly Effective? A Causal Perspective
arxiv_id: '2510.05750'
source_url: ''
authors:
- name: Xiao Yang
  orcid: null
  s2_author_id: '2336941173'
  s2_url: null
- name: Xuejiao Zhao
  orcid: null
  s2_author_id: '2336953480'
  s2_url: null
- name: Zhiqi Shen
  orcid: null
  s2_author_id: '2337319682'
  s2_url: null
published_date: Oct 7, 2025
published_date_iso: '2025-10-07'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph neural networks (GNNs) have achieved remarkable success in node classification.
  Building on this progress, heterogeneous graph neural networks (HGNNs) integrate
  relation types and node and edge semantics to leverage heterogeneous information.
  Causal analysis for HGNNs is advancing rapidly, aiming to separate genuine causal
  effects from spurious correlations. However, whether HGNNs are intrinsically effective
  remains underexamined, and most studies implicitly assume rather than establish
  this effectiveness. In this work, we examine HGNNs from two perspectives: model
  architecture and heterogeneous information. We conduct a systematic reproduction
  across 21 datasets and 20 baselines, complemented by comprehensive hyperparameter
  retuning. To further disentangle the source of performance gains, we develop a causal
  effect estimation framework that constructs and evaluates candidate factors under
  standard assumptions through factual and counterfactual analyses, with robustness
  validated via minimal sufficient adjustment sets, cross-method consistency checks,
  and sensitivity analyses. Our results lead to two conclusions. First, model architecture
  and complexity have no causal effect on performance. Second, heterogeneous information
  exerts a positive causal effect by increasing homophily and local–global distribution
  discrepancy, which makes node classes more distinguishable. The implementation is
  publicly available at https://github.com/YXNTU/CausalHGNN.'
codebase_url: https://github.com/YXNTU/CausalHGNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- RGCN
mrr: 0.0542
adjusted_mrr: 0.0542
mrr_dataset_count: 4
benchmark_categories:
- TU Dortmund
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 3
  total: 4
task_categories:
- graph_classification
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id003
  dataset: ACM
  rows:
  - model: HetGNN
    model_key: hetgnn
    model_plain: HetGNN
    value: 0.979
    std: null
    paper_value: 0.979
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8605
    at_pub_std: 0.0025
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.11849999999999994
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.979
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.979
    sort_std: null
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Heterogeneous Graph Benchmarks
    comparison_source_arxiv: '2112.14936'
    is_best: true
    is_std_outlier: false
  - model: ComCH
    model_key: comch
    model_plain: ComCH
    value: 0.947
    std: null
    paper_value: 0.947
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.947
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.947
    sort_std: null
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
  - model: SlotGAT
    model_key: lmsps
    model_plain: SlotGAT
    value: 0.9469
    std: 0.0036
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2307.08430'
    title: Long-range Meta-path Search on Large-scale Heterogeneous Graphs
    date: Jul 17, 2023
    date_display: Jul 2023
    date_iso: '2023-07-17'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9469
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SlotGAT
    model_key: slotgat
    model_plain: SlotGAT
    value: 0.9406
    std: null
    paper_value: 0.9406
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9406
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2307.08430'
    at_pub_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    at_pub_source_date_iso: '2023-07-17'
    at_pub_source_date_label: NeurIPS 2023
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
    value_gap_source_is_current_paper: true
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
  - model: RpHGNN
    model_key: rphgnn
    model_plain: RpHGNN
    value: 0.9404
    std: null
    paper_value: 0.9404
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9404
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2310.14481'
    at_pub_source_title: Efficient Heterogeneous Graph Learning via Random Projection
    at_pub_source_date_iso: '2023-10-23'
    at_pub_source_date_label: '2023'
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
    true_value: 0.9404
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9404
    sort_std: null
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
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.9402
    std: null
    paper_value: 0.9402
    paper_std: null
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
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9141
    at_pub_std: 0.0075
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.026100000000000012
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9402
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9402
    sort_std: null
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Heterogeneous Graph Benchmarks
    comparison_source_arxiv: '2112.14936'
    is_best: false
    is_std_outlier: false
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    value: 0.9398
    std: null
    paper_value: 0.9398
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9398
    at_pub_std: 0.0036
    at_pub_source_arxiv: '2207.02547'
    at_pub_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    at_pub_source_date_iso: '2022-07-06'
    at_pub_source_date_label: AAAI 2022
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
    true_value: 0.9398
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9398
    sort_std: null
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
  - model: MHGCN
    model_key: mhgcn
    model_plain: MHGCN
    value: 0.9375
    std: null
    paper_value: 0.9375
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9197
    at_pub_std: 0.0068
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.017800000000000038
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9375
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9375
    sort_std: null
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    comparison_source_arxiv: '2305.19872'
    is_best: false
    is_std_outlier: false
  - model: PHGT
    model_key: phgt
    model_plain: PHGT
    value: 0.9372
    std: null
    paper_value: 0.9372
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.9372
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9372
    sort_std: null
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
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    value: 0.9361
    std: null
    paper_value: 0.9361
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9077
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.028400000000000092
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9361
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9361
    sort_std: null
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Heterogeneous Graph Benchmarks
    comparison_source_arxiv: '2112.14936'
    is_best: false
    is_std_outlier: false
  - model: HGSL
    model_key: hgsl
    model_plain: HGSL
    value: 0.9337
    std: null
    paper_value: 0.9337
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.9337
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9337
    sort_std: null
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
  - model: simpleHGN
    model_key: simplehgn
    model_plain: simpleHGN
    value: 0.9335
    std: null
    paper_value: 0.9335
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9335
    at_pub_std: 0.0045
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
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
    true_value: 0.9335
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9335
    sort_std: null
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
  - model: HOAE
    model_key: hoae
    model_plain: HOAE
    value: 0.9303
    std: null
    paper_value: 0.9303
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.9303
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9303
    sort_std: null
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
  - model: HERO
    model_key: hero
    model_plain: HERO
    value: 0.921
    std: null
    paper_value: 0.921
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.921
    at_pub_std: 0.007
    at_pub_source_arxiv: '2412.00742'
    at_pub_source_title: Revisiting Self-Supervised Heterogeneous Graph Learning from
      Spectral Clustering Perspective
    at_pub_source_date_iso: '2024-12-01'
    at_pub_source_date_label: NeurIPS 2024
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
    true_value: 0.921
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.921
    sort_std: null
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
  - model: HAN
    model_key: han
    model_plain: HAN
    value: 0.9185
    std: null
    paper_value: 0.9185
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9147
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2409.17386'
    at_pub_source_title: 'Beyond Redundancy: Information-aware Unsupervised Multiplex
      Graph Structure Learning'
    at_pub_source_date_iso: '2024-09-25'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0038000000000000256
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9185
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9185
    sort_std: null
    global_rank: 50
    paper_rank: 50
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Beyond Redundancy: Information-aware Unsupervised Multiplex
      Graph Structure Learning'
    comparison_source_arxiv: '2409.17386'
    is_best: false
    is_std_outlier: false
  - model: DMGI
    model_key: dmgi
    model_plain: DMGI
    value: 0.898
    std: null
    paper_value: 0.898
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.898
    at_pub_std: null
    at_pub_source_arxiv: '2009.06211'
    at_pub_source_title: Implicit Graph Neural Networks
    at_pub_source_date_iso: '2020-09-14'
    at_pub_source_date_label: NeurIPS 2020
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
    true_value: 0.898
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.898
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
  - model: HeCo
    model_key: heco
    model_plain: HeCo
    value: 0.8871
    std: null
    paper_value: 0.8871
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8897
    at_pub_std: 0.0112
    at_pub_source_arxiv: '2210.00248'
    at_pub_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    at_pub_source_date_iso: '2022-10-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-10-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0026000000000000467
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8897
    true_std: 0.0112
    value_gap_source_arxiv: '2210.00248'
    value_gap_source_title: Heterogeneous Graph Contrastive Multi-view Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0026000000000000467
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: 0.0112
    global_rank: 75
    paper_rank: 76
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NSHE
    model_key: nshe
    model_plain: NSHE
    value: 0.8495
    std: null
    paper_value: 0.8495
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for ACM node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.8495
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8495
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
  - model: SlotGAT
    model_key: hetsann
    model_plain: SlotGAT
    value: 0.9972
    std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
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
    global_rank: 2
    sort_value: 0.9972
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
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
  - model: RpHGNN
    model_key: rphgnn
    model_plain: RpHGNN
    value: 0.9337
    std: null
    paper_value: 0.9337
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9555
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2310.14481'
    at_pub_source_title: Efficient Heterogeneous Graph Learning via Random Projection
    at_pub_source_date_iso: '2023-10-23'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-10-23'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.02180000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9555
    true_std: 0.0029
    value_gap_source_arxiv: '2310.14481'
    value_gap_source_title: Efficient Heterogeneous Graph Learning via Random Projection
    value_gap_source_is_current_paper: false
    value_gap: 0.02180000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9555
    sort_std: 0.0029
    global_rank: 9
    paper_rank: 51
    rank_delta: 42
    rank_delta_abs: 42
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Efficient Heterogeneous Graph Learning via Random Projection
    comparison_source_arxiv: '2310.14481'
    is_best: false
    is_std_outlier: false
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    value: 0.9526
    std: null
    paper_value: 0.9526
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9542
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2207.02547'
    at_pub_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    at_pub_source_date_iso: '2022-07-06'
    at_pub_source_date_label: AAAI 2022
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
    true_value: 0.9542
    true_std: 0.0017
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.0016000000000000458
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
    value: 0.9527
    std: null
    paper_value: 0.9527
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9531
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2307.08430'
    at_pub_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    at_pub_source_date_iso: '2023-07-17'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-07-17'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9531
    true_std: 0.0019
    value_gap_source_arxiv: '2307.08430'
    value_gap_source_title: Long-range Meta-path Search on Large-scale Heterogeneous
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.9531
    sort_std: 0.0019
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MHGCN
    model_key: mhgcn
    model_plain: MHGCN
    value: 0.9375
    std: null
    paper_value: 0.9375
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.952
    at_pub_std: 0.0203
    at_pub_source_arxiv: '2208.06129'
    at_pub_source_title: Multiplex Heterogeneous Graph Convolutional Network
    at_pub_source_date_iso: '2022-08-12'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2022-08-12'
    value_gap_source_date_label: KDD 2022
    gap_vs_at_pub: 0.014499999999999957
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.952
    true_std: 0.0203
    value_gap_source_arxiv: '2208.06129'
    value_gap_source_title: Multiplex Heterogeneous Graph Convolutional Network
    value_gap_source_is_current_paper: false
    value_gap: 0.014499999999999957
    has_value_note: false
    value_note: ''
    sort_value: 0.952
    sort_std: 0.0203
    global_rank: 13
    paper_rank: 45
    rank_delta: 32
    rank_delta_abs: 32
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.95
    std: null
    paper_value: 0.95
    paper_std: null
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
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9207
    at_pub_std: 0.005
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.029299999999999993
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.95
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.95
    sort_std: null
    global_rank: 18
    paper_rank: 18
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Heterogeneous Graph Benchmarks
    comparison_source_arxiv: '2112.14936'
    is_best: false
    is_std_outlier: false
  - model: HINormer
    model_key: hinormer
    model_plain: HINormer
    value: 0.9445
    std: null
    paper_value: 0.9445
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9494
    at_pub_std: 0.0021
    at_pub_source_arxiv: '2302.11329'
    at_pub_source_title: 'HINormer: Representation Learning On Heterogeneous Information
      Networks with Graph Transformer'
    at_pub_source_date_iso: '2023-02-22'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-02-22'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.0049000000000000155
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9494
    true_std: 0.0021
    value_gap_source_arxiv: '2302.11329'
    value_gap_source_title: 'HINormer: Representation Learning On Heterogeneous Information
      Networks with Graph Transformer'
    value_gap_source_is_current_paper: false
    value_gap: 0.0049000000000000155
    has_value_note: false
    value_note: ''
    sort_value: 0.9494
    sort_std: 0.0021
    global_rank: 20
    paper_rank: 32
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'HINormer: Representation Learning On Heterogeneous Information
      Networks with Graph Transformer'
    comparison_source_arxiv: '2302.11329'
    is_best: false
    is_std_outlier: false
  - model: MECCH
    model_key: mecch
    model_plain: MECCH
    value: 0.9475
    std: null
    paper_value: 0.9475
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.9475
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9475
    sort_std: null
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
  - model: simpleHGN
    model_key: simplehgn
    model_plain: simpleHGN
    value: 0.9418
    std: null
    paper_value: 0.9418
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9446
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2302.11329'
    at_pub_source_title: 'HINormer: Representation Learning On Heterogeneous Information
      Networks with Graph Transformer'
    at_pub_source_date_iso: '2023-02-22'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.0028000000000000247
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9446
    true_std: 0.0022
    value_gap_source_arxiv: '2305.19872'
    value_gap_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    value_gap_source_is_current_paper: false
    value_gap: 0.0028000000000000247
    has_value_note: false
    value_note: ''
    sort_value: 0.9446
    sort_std: 0.0022
    global_rank: 31
    paper_rank: 37
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'HINormer: Representation Learning On Heterogeneous Information
      Networks with Graph Transformer'
    comparison_source_arxiv: '2302.11329'
    is_best: false
    is_std_outlier: false
  - model: PHGT
    model_key: phgt
    model_plain: PHGT
    value: 0.9444
    std: null
    paper_value: 0.9444
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.9444
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9444
    sort_std: null
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
  - model: HERO
    model_key: hero
    model_plain: HERO
    value: 0.9397
    std: null
    paper_value: 0.9397
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.944
    at_pub_std: 0.004
    at_pub_source_arxiv: '2412.00742'
    at_pub_source_title: Revisiting Self-Supervised Heterogeneous Graph Learning from
      Spectral Clustering Perspective
    at_pub_source_date_iso: '2024-12-01'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-12-01'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.0042999999999999705
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.944
    true_std: 0.004
    value_gap_source_arxiv: '2412.00742'
    value_gap_source_title: Revisiting Self-Supervised Heterogeneous Graph Learning
      from Spectral Clustering Perspective
    value_gap_source_is_current_paper: false
    value_gap: 0.0042999999999999705
    has_value_note: false
    value_note: ''
    sort_value: 0.944
    sort_std: 0.004
    global_rank: 35
    paper_rank: 40
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Revisiting Self-Supervised Heterogeneous Graph Learning
      from Spectral Clustering Perspective
    comparison_source_arxiv: '2412.00742'
    is_best: false
    is_std_outlier: false
  - model: GTN
    model_key: gtn
    model_plain: GTN
    value: 0.9293
    std: null
    paper_value: 0.9293
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9417
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2310.16401'
    at_pub_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    at_pub_source_date_iso: '2023-10-25'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-10-25'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.012399999999999967
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9417
    true_std: 0.0026
    value_gap_source_arxiv: '2310.16401'
    value_gap_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.012399999999999967
    has_value_note: false
    value_note: ''
    sort_value: 0.9417
    sort_std: 0.0026
    global_rank: 39
    paper_rank: 56
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Neural Networks with a Distribution of Parametrized
      Graphs
    comparison_source_arxiv: '2310.16401'
    is_best: false
    is_std_outlier: false
  - model: ComCH
    model_key: comch
    model_plain: ComCH
    value: 0.9391
    std: null
    paper_value: 0.9391
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.9391
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9391
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
  - model: MAGNN
    model_key: magnn
    model_plain: MAGNN
    value: 0.9336
    std: null
    paper_value: 0.9336
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9456
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.01200000000000001
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
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.9376
    sort_std: 0.0045
    global_rank: 45
    paper_rank: 51
    rank_delta: 6
    rank_delta_abs: 6
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
    value: 0.8728
    std: null
    paper_value: 0.8728
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9365
    at_pub_std: null
    at_pub_source_arxiv: '2012.10024'
    at_pub_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    at_pub_source_date_iso: '2020-12-18'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.06369999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9349
    true_std: 0.0025
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.06209999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.9349
    sort_std: 0.0025
    global_rank: 48
    paper_rank: 86
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Leveraging Meta-path Contexts for Classification in Heterogeneous
      Information Networks
    comparison_source_arxiv: '2012.10024'
    is_best: false
    is_std_outlier: false
  - model: HGSL
    model_key: hgsl
    model_plain: HGSL
    value: 0.9253
    std: null
    paper_value: 0.9253
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for DBLP node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.902
    at_pub_std: 0.0396
    at_pub_source_arxiv: '2208.06129'
    at_pub_source_title: Multiplex Heterogeneous Graph Convolutional Network
    at_pub_source_date_iso: '2022-08-12'
    at_pub_source_date_label: KDD 2022
    value_gap_source_date_iso: '2025-10-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.023299999999999987
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9253
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9253
    sort_std: null
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
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
  - model: model*
    model_key: model
    model_plain: model*
    value: 0.72
    std: null
    paper_value: 0.72
    paper_std: null
    metric: Micro-F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for IMDB node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.72
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.72
    sort_std: null
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
  - model: GTN
    model_key: gtn
    model_plain: GTN
    value: 0.5737
    std: null
    paper_value: 0.5737
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for IMDB node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6827
    at_pub_std: 0.0065
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.10899999999999999
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
    value_gap: 0.10899999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.6827
    sort_std: 0.0065
    global_rank: 43
    paper_rank: 100
    rank_delta: 57
    rank_delta_abs: 57
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    comparison_source_arxiv: '2305.19872'
    is_best: false
    is_std_outlier: false
  - model: HGT
    model_key: hgt
    model_plain: HGT
    value: 0.4951
    std: null
    paper_value: 0.4951
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for IMDB node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.672
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2112.14936'
    at_pub_source_title: Heterogeneous Graph Benchmarks
    at_pub_source_date_iso: '2021-08-14'
    at_pub_source_date_label: KDD 2021
    value_gap_source_date_iso: '2022-07-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.17690000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.672
    true_std: 0.0057
    value_gap_source_arxiv: '2207.02547'
    value_gap_source_title: Simple and Efficient Heterogeneous Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.17690000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.672
    sort_std: 0.0057
    global_rank: 55
    paper_rank: 126
    rank_delta: 71
    rank_delta_abs: 71
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterogeneous Graph Benchmarks
    comparison_source_arxiv: '2112.14936'
    is_best: false
    is_std_outlier: false
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.6395
    std: null
    paper_value: 0.6395
    paper_std: null
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
    protocol_note: Standard split for IMDB node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6651
    at_pub_std: 0.0028
    at_pub_source_arxiv: '2305.19872'
    at_pub_source_title: Spectral Heterogeneous Graph Convolutions via Positive Noncommutative
      Polynomials
    at_pub_source_date_iso: '2023-05-31'
    at_pub_source_date_label: WWW 2023
    value_gap_source_date_iso: '2023-05-31'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.025600000000000067
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
    value_gap: 0.025600000000000067
    has_value_note: false
    value_note: ''
    sort_value: 0.6651
    sort_std: 0.0028
    global_rank: 61
    paper_rank: 74
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Heterogeneous Graph Convolutions via Positive
      Noncommutative Polynomials
    comparison_source_arxiv: '2305.19872'
    is_best: false
    is_std_outlier: false
  - model: DMGI
    model_key: dmgi
    model_plain: DMGI
    value: 0.6164
    std: null
    paper_value: 0.6164
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for IMDB node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.648
    at_pub_std: null
    at_pub_source_arxiv: '2009.06211'
    at_pub_source_title: Implicit Graph Neural Networks
    at_pub_source_date_iso: '2020-09-14'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2020-09-14'
    value_gap_source_date_label: NeurIPS 2020
    gap_vs_at_pub: 0.03160000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.648
    true_std: null
    value_gap_source_arxiv: '2009.06211'
    value_gap_source_title: Implicit Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.03160000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.648
    sort_std: null
    global_rank: 69
    paper_rank: 83
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Implicit Graph Neural Networks
    comparison_source_arxiv: '2009.06211'
    is_best: false
    is_std_outlier: false
  - model: HDHGR
    model_key: hdhgr
    model_plain: HDHGR
    value: 0.5951
    std: null
    paper_value: 0.5951
    paper_std: null
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for IMDB node classification
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.5951
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5951
    sort_std: null
    global_rank: 92
    paper_rank: 92
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
  dataset: MUTAG
  rows:
  - model: ECC
    model_key: msh-gnn
    model_plain: ECC
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
    input_feature_source: null
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
  - model: ECC
    model_key: supcosine
    model_plain: ECC
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
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: cauemo
    model_plain: ECC
    value: 0.9692
    std: 0.0136
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.06283'
    title: 'Soft causal learning for generalized molecule property prediction: An
      environment modeling perspective'
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9692
    sort_std: 0.0136
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGCN
    model_key: rgcn
    model_plain: RGCN
    value: 0.8458
    std: null
    paper_value: 0.8458
    paper_std: null
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
    protocol_note: 10-fold CV
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.8458
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8458
    sort_std: null
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
  - model: model*
    model_key: model
    model_plain: model*
    value: 0.8235
    std: null
    paper_value: 0.8235
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV
    date: Oct 7, 2025
    date_display: Oct 2025
    date_iso: '2025-10-07'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.8235
    true_std: null
    value_gap_source_arxiv: '2510.05750'
    value_gap_source_title: Are Heterogeneous Graph Neural Networks Truly Effective?
      A Causal Perspective
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8235
    sort_std: null
    global_rank: 560
    paper_rank: 560
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
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id002
  - *id003
  - *id004
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
    - dataset: ACM
      dataset_slug: acm
    - dataset: IMDB
      dataset_slug: imdb
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
single_proposed_model: RGCN
main_figure: /figures/2510.05750/main_figure.jpegoptim.jpg
---

