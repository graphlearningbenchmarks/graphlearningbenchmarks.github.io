---
title: 'PREM: A Simple Yet Effective Approach for Node-Level Graph Anomaly Detection'
arxiv_id: '2310.11676'
source_url: ''
authors:
- name: Junjun Pan
  orcid: null
  s2_author_id: '2260294610'
  s2_url: null
- name: Yixin Liu
  orcid: null
  s2_author_id: '2242962967'
  s2_url: null
- name: Yizhen Zheng
  orcid: null
  s2_author_id: '26956796'
  s2_url: null
- name: Shirui Pan
  orcid: null
  s2_author_id: '2256999516'
  s2_url: null
published_date: Oct 18, 2023
published_date_iso: '2023-10-18'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: graph anomaly detection (GAD) plays a critical role in identifying in various
  domains such as medicine, social networks, and e-commerce. However, challenges have
  arisen due to the dearth of labeled data. Existing methodologies - reconstruction-based
  and contrastive learning - while effective, often suffer from efficiency issues,
  stemming from their complex objectives and elaborate modules. To improve the efficiency
  of GAD, we introduce a simple method termed processing and atching (PREM). Our approach
  streamlines GAD, Comprising two modules - a pre-processing module and an ego-neighbor
  matching module - PREM eliminates the necessity for message-passing propagation
  during training, and employs a simple contrastive loss, leading to considerable
  reductions in training time and memory usage. Moreover, through rigorous evaluations
  of five real-world datasets, our method demonstrated robustness and effectiveness.
  Notably, when validated on the ACM dataset, PREM achieved a 5\
codebase_url: https://github.com/CampanulaBells/PREM-GAD
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- PREM
- PREM-b
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: ACM
  rows:
  - model: PREM-b
    model_key: prem-b
    model_plain: PREM-b
    value: 0.9088
    std: null
    paper_value: 0.9088
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Anomaly detection task (AUC) on ACM dataset
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9088
    true_std: null
    value_gap_source_arxiv: '2310.11676'
    value_gap_source_title: 'PREM: A Simple Yet Effective Approach for Node-Level
      Graph Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9088
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
  - model: PREM
    model_key: prem
    model_plain: PREM
    value: 0.9056
    std: null
    paper_value: 0.9056
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Anomaly detection task (AUC) on ACM dataset
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9056
    true_std: null
    value_gap_source_arxiv: '2310.11676'
    value_gap_source_title: 'PREM: A Simple Yet Effective Approach for Node-Level
      Graph Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9056
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
  - model: GRADATE
    model_key: gradate
    model_plain: GRADATE
    value: 0.858
    std: null
    paper_value: 0.858
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Anomaly detection task (AUC) on ACM dataset
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.858
    true_std: null
    value_gap_source_arxiv: '2310.11676'
    value_gap_source_title: 'PREM: A Simple Yet Effective Approach for Node-Level
      Graph Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.858
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
  - model: ANEMONE
    model_key: anemone
    model_plain: ANEMONE
    value: 0.8492
    std: null
    paper_value: 0.8492
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Anomaly detection task (AUC) on ACM dataset
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8492
    true_std: null
    value_gap_source_arxiv: '2310.11676'
    value_gap_source_title: 'PREM: A Simple Yet Effective Approach for Node-Level
      Graph Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8492
    sort_std: null
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
  - model: CoLA
    model_key: cola
    model_plain: CoLA
    value: 0.8375
    std: null
    paper_value: 0.8375
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Anomaly detection task (AUC) on ACM dataset
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8375
    true_std: null
    value_gap_source_arxiv: '2310.11676'
    value_gap_source_title: 'PREM: A Simple Yet Effective Approach for Node-Level
      Graph Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8375
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
  - model: SL-GAD
    model_key: sl-gad
    model_plain: SL-GAD
    value: 0.8143
    std: null
    paper_value: 0.8143
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Anomaly detection task (AUC) on ACM dataset
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8143
    true_std: null
    value_gap_source_arxiv: '2310.11676'
    value_gap_source_title: 'PREM: A Simple Yet Effective Approach for Node-Level
      Graph Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8143
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
  - model: Sub-CR
    model_key: sub-cr
    model_plain: Sub-CR
    value: 0.806
    std: null
    paper_value: 0.806
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Anomaly detection task (AUC) on ACM dataset
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.806
    true_std: null
    value_gap_source_arxiv: '2310.11676'
    value_gap_source_title: 'PREM: A Simple Yet Effective Approach for Node-Level
      Graph Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.806
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
  - model: DOMINANT
    model_key: dominant
    model_plain: DOMINANT
    value: 0.7561
    std: null
    paper_value: 0.7561
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Anomaly detection task (AUC) on ACM dataset
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7561
    true_std: null
    value_gap_source_arxiv: '2310.11676'
    value_gap_source_title: 'PREM: A Simple Yet Effective Approach for Node-Level
      Graph Anomaly Detection'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7561
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
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - AUC
  metric: AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: ACM
      dataset_slug: acm
main_figure: /figures/2310.11676/main_figure.jpegoptim.jpg
---

