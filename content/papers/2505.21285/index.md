---
title: Learnable Kernel Density Estimation for Graphs
arxiv_id: '2505.21285'
source_url: ''
authors:
- name: Xudong Wang
  orcid: null
  s2_author_id: '2319167912'
  s2_url: null
- name: Ziheng Sun
  orcid: null
  s2_author_id: '2288241482'
  s2_url: null
- name: Chris Ding
  orcid: null
  s2_author_id: '2288212897'
  s2_url: null
- name: Jicong Fan
  orcid: null
  s2_author_id: '2313648344'
  s2_url: null
published_date: May 27, 2025
published_date_iso: '2025-05-27'
published_venue: ICML 2025
published_conference: ICML 2025
published_conference_short: ICML
published_conference_slug: icml
abstract: This work proposes a framework LGKDE that learns kernel density estimation
  for graphs. The key challenge in graph density estimation lies in effectively capturing
  both structural patterns and semantic variations while maintaining theoretical guarantees.
  Combining graph kernels and kernel density estimation (KDE) is a standard approach
  to graph density estimation, but has unsatisfactory performance due to the handcrafted
  and fixed features of kernels. Our method LGKDE leverages graph neural networks
  to represent each graph as a discrete distribution and utilizes maximum mean discrepancy
  to learn the graph metric for multi-scale KDE, where all parameters are learned
  by maximizing the density of graphs relative to the density of their well-designed
  perturbed counterparts. The perturbations are conducted on both node features and
  graph spectra, which helps better characterize the boundary of normal density regions.
  Theoretically, we establish consistency and convergence guarantees for LGKDE, including
  bounds on the mean integrated squared error, robustness, and generalization. We
  validate LGKDE by demonstrating its effectiveness in recovering the underlying density
  of synthetic graph distributions and applying it to graph anomaly detection across
  diverse benchmark datasets. Extensive empirical evaluation shows that LGKDE demonstrates
  superior performance compared to state-of-the-art baselines on most benchmark datasets.
codebase_url: https://github.com/MathAdventurer/LGKDE
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- LGKDE
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 4
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id003
  dataset: COLLAB
  rows:
  - model: SIGNET
    model_key: signet
    model_plain: SIGNET
    value: 0.7245
    std: 0.0011
    paper_value: 0.7245
    paper_std: 0.0011
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.7245
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7245
    true_std: 0.0011
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7245
    sort_std: 0.0011
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
  - model: CVTGAD
    model_key: cvtgad
    model_plain: CVTGAD
    value: 0.7101
    std: 0.0058
    paper_value: 0.7101
    paper_std: 0.0058
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.7101
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7101
    true_std: 0.0058
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7101
    sort_std: 0.0058
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
  - model: GOODAT
    model_key: good-d
    model_plain: GOODAT
    value: 0.6934
    std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.15523'
    title: 'Unifying Unsupervised Graph-Level Anomaly Detection and Out-of-Distribution
      Detection: A Benchmark'
    date: Jun 21, 2024
    date_display: Jun 2024
    date_iso: '2024-06-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/UB-GOLD/UB-GOLD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6934
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LGKDE
    model_key: lgkde
    model_plain: LGKDE
    value: 0.6794
    std: 0.0041
    paper_value: 0.6794
    paper_std: 0.0041
    metric: AUROC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6794
    true_std: 0.0041
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6794
    sort_std: 0.0041
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
  - model: MUSE
    model_key: muse
    model_plain: MUSE
    value: 0.6748
    std: 0.0036
    paper_value: 0.6748
    paper_std: 0.0036
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6748
    true_std: 0.0036
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6748
    sort_std: 0.0036
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
  - model: Uniform
    model_key: uniform
    model_plain: Uniform
    value: 0.6623
    std: 0.0038
    paper_value: 0.6623
    paper_std: 0.0038
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6623
    true_std: 0.0038
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6623
    sort_std: 0.0038
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
  - model: OCGIN
    model_key: ocgin
    model_plain: OCGIN
    value: 0.6058
    std: 0.0027
    paper_value: 0.6058
    paper_std: 0.0027
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6058
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6058
    true_std: 0.0027
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6058
    sort_std: 0.0027
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
  - model: WL-SVM
    model_key: wl-svm
    model_plain: WL-SVM
    value: 0.5462
    std: 0.0128
    paper_value: 0.5462
    paper_std: 0.0128
    metric: AUROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5462
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5462
    true_std: 0.0128
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5462
    sort_std: 0.0128
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
  - model: GLADC
    model_key: gladc
    model_plain: GLADC
    value: 0.5432
    std: 0.0037
    paper_value: 0.5432
    paper_std: 0.0037
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5432
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5432
    true_std: 0.0037
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5432
    sort_std: 0.0037
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GlocalKD
    model_key: glocalkd
    model_plain: GlocalKD
    value: 0.5185
    std: 0.0018
    paper_value: 0.5185
    paper_std: 0.0018
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5185
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5185
    true_std: 0.0018
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5185
    sort_std: 0.0018
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
  - model: WL-iF
    model_key: wl-if
    model_plain: WL-iF
    value: 0.5141
    std: 0.0039
    paper_value: 0.5141
    paper_std: 0.0039
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5141
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5141
    true_std: 0.0039
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5141
    sort_std: 0.0039
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
  - model: PK-iF
    model_key: pk-if
    model_plain: PK-iF
    value: 0.5138
    std: 0.002
    paper_value: 0.5138
    paper_std: 0.002
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5138
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5138
    true_std: 0.002
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5138
    sort_std: 0.002
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
  - model: PK-SVM
    model_key: pk-svm
    model_plain: PK-SVM
    value: 0.4972
    std: 0.006
    paper_value: 0.4972
    paper_std: 0.006
    metric: AUROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.4972
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4972
    true_std: 0.006
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4972
    sort_std: 0.006
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
  - model: OCGTL
    model_key: ocgtl
    model_plain: OCGTL
    value: 0.4813
    std: 0.0041
    paper_value: 0.4813
    paper_std: 0.0041
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.4813
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4813
    true_std: 0.0041
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4813
    sort_std: 0.0041
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
  rank_metric: AUROC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUROC
  metric: AUROC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id004
  dataset: ENZYMES
  rows:
  - model: LGKDE
    model_key: lgkde
    model_plain: LGKDE
    value: 0.7104
    std: 0.0045
    paper_value: 0.7104
    paper_std: 0.0045
    metric: AUROC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7104
    true_std: 0.0045
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7104
    sort_std: 0.0045
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
  - model: Uniform
    model_key: uniform
    model_plain: Uniform
    value: 0.6934
    std: 0.0041
    paper_value: 0.6934
    paper_std: 0.0041
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6934
    true_std: 0.0041
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6934
    sort_std: 0.0041
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
  - model: CVTGAD
    model_key: cvtgad
    model_plain: CVTGAD
    value: 0.6856
    std: 0.0043
    paper_value: 0.6856
    paper_std: 0.0043
    metric: AUROC
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
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6856
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6856
    true_std: 0.0043
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6856
    sort_std: 0.0043
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
  - model: MUSE
    model_key: muse
    model_plain: MUSE
    value: 0.6782
    std: 0.0038
    paper_value: 0.6782
    paper_std: 0.0038
    metric: AUROC
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
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6782
    true_std: 0.0038
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6782
    sort_std: 0.0038
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
  - model: OCGTL
    model_key: ocgtl
    model_plain: OCGTL
    value: 0.6359
    std: 0.0011
    paper_value: 0.6359
    paper_std: 0.0011
    metric: AUROC
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
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6359
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6359
    true_std: 0.0011
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6359
    sort_std: 0.0011
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
  - model: GLADC
    model_key: gladc
    model_plain: GLADC
    value: 0.6344
    std: 0.003
    paper_value: 0.6344
    paper_std: 0.003
    metric: AUROC
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
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6344
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6344
    true_std: 0.003
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6344
    sort_std: 0.003
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
  - model: SIGNET
    model_key: signet
    model_plain: SIGNET
    value: 0.6312
    std: 0.0052
    paper_value: 0.6312
    paper_std: 0.0052
    metric: AUROC
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
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6312
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6312
    true_std: 0.0052
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6312
    sort_std: 0.0052
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
  - model: OCGIN
    model_key: ocgin
    model_plain: OCGIN
    value: 0.6244
    std: 0.0038
    paper_value: 0.6244
    paper_std: 0.0038
    metric: AUROC
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
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6244
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6244
    true_std: 0.0038
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6244
    sort_std: 0.0038
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
  - model: GlocalKD
    model_key: glocalkd
    model_plain: GlocalKD
    value: 0.6175
    std: 0.001
    paper_value: 0.6175
    paper_std: 0.001
    metric: AUROC
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
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6175
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6175
    true_std: 0.001
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6175
    sort_std: 0.001
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
  - model: WL-SVM
    model_key: wl-svm
    model_plain: WL-SVM
    value: 0.5375
    std: 0.0034
    paper_value: 0.5375
    paper_std: 0.0034
    metric: AUROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5375
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5375
    true_std: 0.0034
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5375
    sort_std: 0.0034
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
  - model: PK-SVM
    model_key: pk-svm
    model_plain: PK-SVM
    value: 0.5245
    std: 0.0029
    paper_value: 0.5245
    paper_std: 0.0029
    metric: AUROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5245
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5245
    true_std: 0.0029
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5245
    sort_std: 0.0029
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
  - model: WL-iF
    model_key: wl-if
    model_plain: WL-iF
    value: 0.5103
    std: 0.0042
    paper_value: 0.5103
    paper_std: 0.0042
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5103
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5103
    true_std: 0.0042
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5103
    sort_std: 0.0042
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
  - model: PK-iF
    model_key: pk-if
    model_plain: PK-iF
    value: 0.4982
    std: 0.0067
    paper_value: 0.4982
    paper_std: 0.0067
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Graph-level anomaly detection task using AUROC metric.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.4982
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4982
    true_std: 0.0067
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4982
    sort_std: 0.0067
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
  rank_metric: AUROC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUROC
  metric: AUROC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: MUTAG
  rows:
  - model: LGKDE
    model_key: bwgnn
    model_plain: LGKDE
    value: 0.995
    std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06427'
    title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    date: Nov 10, 2024
    date_display: Nov 2024
    date_iso: '2024-11-10'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/lllyyq1121/UniGAD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.995
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: LGKDE
    model_key: gat
    model_plain: LGKDE
    value: 0.9942
    std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06427'
    title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    date: Nov 10, 2024
    date_display: Nov 2024
    date_iso: '2024-11-10'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/lllyyq1121/UniGAD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9942
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LGKDE
    model_key: gin
    model_plain: LGKDE
    value: 0.9939
    std: null
    metric: AUROC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.06427'
    title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    date: Nov 10, 2024
    date_display: Nov 2024
    date_iso: '2024-11-10'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/lllyyq1121/UniGAD
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9939
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OCGTL
    model_key: ocgtl
    model_plain: OCGTL
    value: 0.8802
    std: 0.0043
    paper_value: 0.8802
    paper_std: 0.0043
    metric: AUROC
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
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.9219
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-10'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.04170000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9219
    true_std: null
    value_gap_source_arxiv: '2411.06427'
    value_gap_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    value_gap_source_is_current_paper: false
    value_gap: 0.04170000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.9219
    sort_std: null
    global_rank: 12
    paper_rank: 17
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: false
    is_std_outlier: false
  - model: LGKDE
    model_key: lgkde
    model_plain: LGKDE
    value: 0.9163
    std: 0.0031
    paper_value: 0.9163
    paper_std: 0.0031
    metric: AUROC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9163
    true_std: 0.0031
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9163
    sort_std: 0.0031
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
  - model: OCGIN
    model_key: ocgin
    model_plain: OCGIN
    value: 0.7955
    std: 0.0022
    paper_value: 0.7955
    paper_std: 0.0022
    metric: AUROC
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
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.895
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-11-10'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.09950000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.895
    true_std: null
    value_gap_source_arxiv: '2411.06427'
    value_gap_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    value_gap_source_is_current_paper: false
    value_gap: 0.09950000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.895
    sort_std: null
    global_rank: 14
    paper_rank: 21
    rank_delta: 7
    rank_delta_abs: 7
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: false
    is_std_outlier: false
  - model: SIGNET
    model_key: signet
    model_plain: SIGNET
    value: 0.8884
    std: 0.0015
    paper_value: 0.8884
    paper_std: 0.0015
    metric: AUROC
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
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8884
    true_std: 0.0015
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8884
    sort_std: 0.0015
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
  - model: Uniform
    model_key: uniform
    model_plain: Uniform
    value: 0.8845
    std: 0.0024
    paper_value: 0.8845
    paper_std: 0.0024
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8845
    true_std: 0.0024
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8845
    sort_std: 0.0024
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
  - model: CVTGAD
    model_key: cvtgad
    model_plain: CVTGAD
    value: 0.8664
    std: 0.0032
    paper_value: 0.8664
    paper_std: 0.0032
    metric: AUROC
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
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8664
    true_std: 0.0032
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8664
    sort_std: 0.0032
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
  - model: GlocalKD
    model_key: glocalkd
    model_plain: GlocalKD
    value: 0.8625
    std: 0.0057
    paper_value: 0.8625
    paper_std: 0.0057
    metric: AUROC
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
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.7277
    at_pub_std: null
    at_pub_source_arxiv: '2411.06427'
    at_pub_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    at_pub_source_date_iso: '2024-11-10'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.13480000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8625
    true_std: 0.0057
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8625
    sort_std: 0.0057
    global_rank: 19
    paper_rank: 19
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'UniGAD: Unifying Multi-level Graph Anomaly Detection'
    comparison_source_arxiv: '2411.06427'
    is_best: false
    is_std_outlier: false
  - model: MUSE
    model_key: muse
    model_plain: MUSE
    value: 0.8592
    std: 0.0028
    paper_value: 0.8592
    paper_std: 0.0028
    metric: AUROC
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
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8592
    true_std: 0.0028
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8592
    sort_std: 0.0028
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
  - model: GLADC
    model_key: gladc
    model_plain: GLADC
    value: 0.8307
    std: 0.0029
    paper_value: 0.8307
    paper_std: 0.0029
    metric: AUROC
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
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8307
    true_std: 0.0029
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8307
    sort_std: 0.0029
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
  - model: WL-iF
    model_key: wl-if
    model_plain: WL-iF
    value: 0.6571
    std: 0.0038
    paper_value: 0.6571
    paper_std: 0.0038
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6571
    true_std: 0.0038
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6571
    sort_std: 0.0038
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
  - model: WL-SVM
    model_key: wl-svm
    model_plain: WL-SVM
    value: 0.6218
    std: 0.0029
    paper_value: 0.6218
    paper_std: 0.0029
    metric: AUROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6218
    true_std: 0.0029
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6218
    sort_std: 0.0029
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
  - model: PK-iF
    model_key: pk-if
    model_plain: PK-iF
    value: 0.4798
    std: 0.0041
    paper_value: 0.4798
    paper_std: 0.0041
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4798
    true_std: 0.0041
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4798
    sort_std: 0.0041
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
  - model: PK-SVM
    model_key: pk-svm
    model_plain: PK-SVM
    value: 0.4606
    std: 0.0047
    paper_value: 0.4606
    paper_std: 0.0047
    metric: AUROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard AUROC for graph-level anomaly detection on MUTAG.
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4606
    true_std: 0.0047
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4606
    sort_std: 0.0047
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
  rank_metric: AUROC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUROC
  metric: AUROC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: NCI1
  rows:
  - model: LGKDE
    model_key: lgkde
    model_plain: LGKDE
    value: 0.7667
    std: 0.003
    paper_value: 0.7667
    paper_std: 0.003
    metric: AUROC
    higher_is_better: true
    is_baseline: false
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7667
    true_std: 0.003
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7667
    sort_std: 0.003
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
  - model: OCGTL
    model_key: ocgtl
    model_plain: OCGTL
    value: 0.7575
    std: 0.0047
    paper_value: 0.7575
    paper_std: 0.0047
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.7575
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7575
    true_std: 0.0047
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7575
    sort_std: 0.0047
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
  - model: MUSE
    model_key: muse
    model_plain: MUSE
    value: 0.7445
    std: 0.0026
    paper_value: 0.7445
    paper_std: 0.0026
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7445
    true_std: 0.0026
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7445
    sort_std: 0.0026
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
  - model: SIGNET
    model_key: signet
    model_plain: SIGNET
    value: 0.7432
    std: 0.0034
    paper_value: 0.7432
    paper_std: 0.0034
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.7432
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7432
    true_std: 0.0034
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7432
    sort_std: 0.0034
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
  - model: Uniform
    model_key: uniform
    model_plain: Uniform
    value: 0.7293
    std: 0.0031
    paper_value: 0.7293
    paper_std: 0.0031
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7293
    true_std: 0.0031
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7293
    sort_std: 0.0031
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
  - model: OCGIN
    model_key: ocgin
    model_plain: OCGIN
    value: 0.6946
    std: 0.0036
    paper_value: 0.6946
    paper_std: 0.0036
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6946
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6946
    true_std: 0.0036
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6946
    sort_std: 0.0036
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
  - model: CVTGAD
    model_key: cvtgad
    model_plain: CVTGAD
    value: 0.6913
    std: 0.0058
    paper_value: 0.6913
    paper_std: 0.0058
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6913
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6913
    true_std: 0.0058
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6913
    sort_std: 0.0058
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
  - model: GLADC
    model_key: gladc
    model_plain: GLADC
    value: 0.6832
    std: 0.0022
    paper_value: 0.6832
    paper_std: 0.0022
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6832
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6832
    true_std: 0.0022
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6832
    sort_std: 0.0022
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
  - model: GlocalKD
    model_key: glocalkd
    model_plain: GlocalKD
    value: 0.6529
    std: 0.0021
    paper_value: 0.6529
    paper_std: 0.0021
    metric: AUROC
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
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.6529
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6529
    true_std: 0.0021
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6529
    sort_std: 0.0021
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: WL-SVM
    model_key: wl-svm
    model_plain: WL-SVM
    value: 0.5418
    std: 0.0067
    paper_value: 0.5418
    paper_std: 0.0067
    metric: AUROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5418
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5418
    true_std: 0.0067
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5418
    sort_std: 0.0067
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
  - model: PK-SVM
    model_key: pk-svm
    model_plain: PK-SVM
    value: 0.5139
    std: 0.0019
    paper_value: 0.5139
    paper_std: 0.0019
    metric: AUROC
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5139
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5139
    true_std: 0.0019
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5139
    sort_std: 0.0019
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
  - model: WL-iF
    model_key: wl-if
    model_plain: WL-iF
    value: 0.5041
    std: 0.0031
    paper_value: 0.5041
    paper_std: 0.0031
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5041
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5041
    true_std: 0.0031
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5041
    sort_std: 0.0031
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
  - model: PK-iF
    model_key: pk-if
    model_plain: PK-iF
    value: 0.5022
    std: 0.0012
    paper_value: 0.5022
    paper_std: 0.0012
    metric: AUROC
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: AUROC reported for graph-level anomaly detection
    date: May 27, 2025
    date_display: May 2025
    date_iso: '2025-05-27'
    published_venue: ICML 2025
    published_conference: ICML 2025
    at_pub_value: 0.5022
    at_pub_std: null
    at_pub_source_arxiv: '2406.15523'
    at_pub_source_title: 'Unifying Unsupervised Graph-Level Anomaly Detection and
      Out-of-Distribution Detection: A Benchmark'
    at_pub_source_date_iso: '2024-06-21'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-27'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5022
    true_std: 0.0012
    value_gap_source_arxiv: '2505.21285'
    value_gap_source_title: Learnable Kernel Density Estimation for Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5022
    sort_std: 0.0012
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
  rank_metric: AUROC
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUROC
  metric: AUROC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: NCI1
      dataset_slug: nci1
    - dataset: COLLAB
      dataset_slug: collab
    - dataset: ENZYMES
      dataset_slug: enzymes
single_proposed_model: LGKDE
---

