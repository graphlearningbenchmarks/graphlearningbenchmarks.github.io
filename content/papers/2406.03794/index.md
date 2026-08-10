---
title: Infusing Self-Consistency into Density Functional Theory Hamiltonian Prediction
  via Deep Equilibrium Models
arxiv_id: '2406.03794'
source_url: ''
authors:
- name: Zun Wang
  orcid: null
  s2_author_id: '2108306910'
  s2_url: null
- name: Chang Liu
  orcid: null
  s2_author_id: '2248334433'
  s2_url: null
- name: Nianlong Zou
  orcid: null
  s2_author_id: '151470916'
  s2_url: null
- name: He Zhang
  orcid: null
  s2_author_id: '2153527929'
  s2_url: null
- name: Xinran Wei
  orcid: null
  s2_author_id: '2110849142'
  s2_url: null
- name: Lin Huang
  orcid: null
  s2_author_id: '2326207974'
  s2_url: null
- name: Lijun Wu
  orcid: null
  s2_author_id: '2303415527'
  s2_url: null
- name: Bin Shao
  orcid: null
  s2_author_id: '2288575521'
  s2_url: null
published_date: Jun 6, 2024
published_date_iso: '2024-06-06'
published_venue: NeurIPS 2024
published_conference: NeurIPS 2024
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: In this study, we introduce a unified neural network architecture, the Deep
  Equilibrium Density Functional Theory Hamiltonian (DEQH) model, which incorporates
  Deep Equilibrium Models (DEQs) for predicting Density Functional Theory (DFT) Hamiltonians.
  The DEQH model inherently captures the self-consistency nature of Hamiltonian, a
  critical aspect often overlooked by traditional machine learning approaches for
  Hamiltonian prediction. By employing DEQ within our model architecture, we circumvent
  the need for DFT calculations during the training phase to introduce the Hamiltonian's
  self-consistency, thus addressing computational bottlenecks associated with large
  or complex systems. We propose a versatile framework that combines DEQ with off-the-shelf
  machine learning models for predicting Hamiltonians. When benchmarked on the MD17
  and QH9 datasets, DEQHNet, an instantiation of the DEQH framework, has demonstrated
  a significant improvement in prediction accuracy. Beyond a predictor, the DEQH model
  is a Hamiltonian solver, in the sense that it uses the fixed-point solving capability
  of the deep equilibrium model to iteratively solve for the Hamiltonian. Ablation
  studies of DEQHNet further elucidate the network's effectiveness, offering insights
  into the potential of DEQ-integrated networks for Hamiltonian learning. We open
  source our implementation at.
codebase_url: https://github.com/Zun-Wang/DEQHNet
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DEQHNet
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Quantum Chemistry
benchmark_coverage:
- benchmark: Quantum Chemistry
  benchmark_slug: quantum-chemistry
  evaluated: 1
  total: 1
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: MD17
  rows:
  - model: PhiSNet (ori)
    model_key: phisnet (ori)
    model_plain: PhiSNet (ori)
    value: 1.073e-05
    std: null
    paper_value: 1.073e-05
    paper_std: null
    metric: H
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
    source_ref: unke2021se
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task on Hamiltonian matrix elements (H) using standard
      split
    date: Jun 6, 2024
    date_display: Jun 2024
    date_iso: '2024-06-06'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-06'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.073e-05
    true_std: null
    value_gap_source_arxiv: '2406.03794'
    value_gap_source_title: Infusing Self-Consistency into Density Functional Theory
      Hamiltonian Prediction via Deep Equilibrium Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.073e-05
    sort_std: null
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
  - model: QHNet
    model_key: qhnet
    model_plain: QHNet
    value: 1.079e-05
    std: null
    paper_value: 1.079e-05
    paper_std: null
    metric: H
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
    source_ref: yu2023efficient
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task on Hamiltonian matrix elements (H) using standard
      split
    date: Jun 6, 2024
    date_display: Jun 2024
    date_iso: '2024-06-06'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-03'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.079e-05
    true_std: null
    value_gap_source_arxiv: '2502.01171'
    value_gap_source_title: Efficient and Scalable Density Functional Theory Hamiltonian
      Prediction through Adaptive Sparsity
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.079e-05
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
  - model: DEQHNet
    model_key: deqhnet
    model_plain: DEQHNet
    value: 1.507e-05
    std: null
    paper_value: 1.507e-05
    paper_std: null
    metric: H
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task on Hamiltonian matrix elements (H) using standard
      split
    date: Jun 6, 2024
    date_display: Jun 2024
    date_iso: '2024-06-06'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-06'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.507e-05
    true_std: null
    value_gap_source_arxiv: '2406.03794'
    value_gap_source_title: Infusing Self-Consistency into Density Functional Theory
      Hamiltonian Prediction via Deep Equilibrium Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.507e-05
    sort_std: null
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
  - model: DeepH
    model_key: deeph
    model_plain: DeepH
    value: 1.727e-05
    std: null
    paper_value: 1.727e-05
    paper_std: null
    metric: H
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
    source_ref: li2022deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task on Hamiltonian matrix elements (H) using standard
      split
    date: Jun 6, 2024
    date_display: Jun 2024
    date_iso: '2024-06-06'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-06'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.727e-05
    true_std: null
    value_gap_source_arxiv: '2406.03794'
    value_gap_source_title: Infusing Self-Consistency into Density Functional Theory
      Hamiltonian Prediction via Deep Equilibrium Models
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.727e-05
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
  - model: SchNOrb
    model_key: schnorb
    model_plain: SchNOrb
    value: 0.0001654
    std: null
    paper_value: 0.0001654
    paper_std: null
    metric: H
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task on Hamiltonian matrix elements (H) using standard
      split
    date: Jun 6, 2024
    date_display: Jun 2024
    date_iso: '2024-06-06'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-03'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0001654
    true_std: null
    value_gap_source_arxiv: '2502.01171'
    value_gap_source_title: Efficient and Scalable Density Functional Theory Hamiltonian
      Prediction through Adaptive Sparsity
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0001654
    sort_std: null
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
  rank_metric: H
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - H
  metric: H
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Quantum Chemistry
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Quantum Chemistry
    benchmark_slug: quantum-chemistry
    datasets:
    - dataset: MD17
      dataset_slug: md17
single_proposed_model: DEQHNet
main_figure: /figures/2406.03794/main_figure.jpegoptim.jpg
---

