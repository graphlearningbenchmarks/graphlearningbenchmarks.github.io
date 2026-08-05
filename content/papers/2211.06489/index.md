---
title: Equivariance with Learned Canonicalization Functions
arxiv_id: '2211.06489'
source_url: ''
authors:
- name: Sekouba Kaba
  orcid: null
  s2_author_id: '120834291'
  s2_url: null
- name: Arnab Kumar Mondal
  orcid: null
  s2_author_id: '2163155722'
  s2_url: null
- name: Yan Zhang
  orcid: null
  s2_author_id: '49889702'
  s2_url: null
- name: Yoshua Bengio
  orcid: null
  s2_author_id: '1751762'
  s2_url: null
- name: Siamak Ravanbakhsh
  orcid: null
  s2_author_id: '2111187'
  s2_url: null
published_date: Nov 11, 2022
published_date_iso: '2022-11-11'
published_venue: ICML 2022
published_conference: ICML 2022
published_conference_short: ICML
published_conference_slug: icml
abstract: Symmetry-based neural networks often constrain the architecture in order
  to achieve invariance or equivariance to a group of transformations. In this paper,
  we propose an alternative that avoids this architectural constraint by learning
  to produce canonical representations of the data. These canonicalization functions
  can readily be plugged into non-equivariant backbone architectures. We offer explicit
  ways to implement them for some groups of interest. We show that this approach enjoys
  universality while providing interpretable insights. Our main hypothesis, supported
  by our empirical results, is that learning a small neural network to perform canonicalization
  is better than using predefined heuristics. Our experiments show that learning the
  canonicalization function is competitive with existing techniques for learning equivariant
  functions across many tasks, including image classification, $N$-body dynamics prediction,
  point cloud classification and part segmentation, while being faster across the
  board.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- GNNBenchmark
benchmark_coverage:
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 1
  total: 6
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
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
  - model: CNN
    model_key: cnn
    model_plain: CNN
    value: 0.951
    std: 0.002
    paper_value: 0.951
    paper_std: 0.002
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on Rotated-MNIST (test set)
    date: Nov 11, 2022
    date_display: Nov 2022
    date_iso: '2022-11-11'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-13'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9907
    true_std: 0.0007
    value_gap_source_arxiv: '2605.13383'
    value_gap_source_title: 'Beyond Oversquashing: Understanding Signal Propagation
      in GNNs Via Observables'
    value_gap_source_is_current_paper: false
    value_gap: 0.03970000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.9907
    sort_std: 0.0007
    global_rank: 2
    paper_rank: 121
    rank_delta: 119
    rank_delta_abs: 119
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
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
  - model: CN(p64)-CNN
    model_key: cn(p64)-cnn
    model_plain: CN(p64)-CNN
    value: 0.9801
    std: 0.001
    paper_value: 0.9801
    paper_std: 0.001
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on Rotated-MNIST (test set)
    date: Nov 11, 2022
    date_display: Nov 2022
    date_iso: '2022-11-11'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-11'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9801
    true_std: 0.001
    value_gap_source_arxiv: '2211.06489'
    value_gap_source_title: Equivariance with Learned Canonicalization Functions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9801
    sort_std: 0.001
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
  - model: G-CNN (p4)
    model_key: g-cnn (p4)
    model_plain: G-CNN (p4)
    value: 0.9772
    std: 0.0
    paper_value: 0.9772
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on Rotated-MNIST (test set)
    date: Nov 11, 2022
    date_display: Nov 2022
    date_iso: '2022-11-11'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-11'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9772
    true_std: 0.0
    value_gap_source_arxiv: '2211.06489'
    value_gap_source_title: Equivariance with Learned Canonicalization Functions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9772
    sort_std: 0.0
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
  - model: CN(p4)-CNN
    model_key: cn(p4)-cnn
    model_plain: CN(p4)-CNN
    value: 0.9759
    std: 0.001
    paper_value: 0.9759
    paper_std: 0.001
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on Rotated-MNIST (test set)
    date: Nov 11, 2022
    date_display: Nov 2022
    date_iso: '2022-11-11'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-11'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9759
    true_std: 0.001
    value_gap_source_arxiv: '2211.06489'
    value_gap_source_title: Equivariance with Learned Canonicalization Functions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9759
    sort_std: 0.001
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
  - model: CN(PCA)-CNN
    model_key: cn(pca)-cnn
    model_plain: CN(PCA)-CNN
    value: 0.9665
    std: 0.0021
    paper_value: 0.9665
    paper_std: 0.0021
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
    feature_source_evidence: CN(PCA)-CNN uses PCA for canonicalization
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on Rotated-MNIST (test set)
    date: Nov 11, 2022
    date_display: Nov 2022
    date_iso: '2022-11-11'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-11'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9665
    true_std: 0.0021
    value_gap_source_arxiv: '2211.06489'
    value_gap_source_title: Equivariance with Learned Canonicalization Functions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9665
    sort_std: 0.0021
    global_rank: 102
    paper_rank: 102
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CN(OPT)-CNN
    model_key: cn(opt)-cnn
    model_plain: CN(OPT)-CNN
    value: 0.9665
    std: 0.0
    paper_value: 0.9665
    paper_std: 0.0
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on Rotated-MNIST (test set)
    date: Nov 11, 2022
    date_display: Nov 2022
    date_iso: '2022-11-11'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-11'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9665
    true_std: 0.0
    value_gap_source_arxiv: '2211.06489'
    value_gap_source_title: Equivariance with Learned Canonicalization Functions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9665
    sort_std: 0.0
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
  - model: CN(p4 & frozen)-CNN
    model_key: cn(p4 & frozen)-cnn
    model_plain: CN(p4 & frozen)-CNN
    value: 0.9609
    std: 0.0012
    paper_value: 0.9609
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
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: CN(p4 & frozen)-CNN uses frozen parameters
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Accuracy on Rotated-MNIST (test set)
    date: Nov 11, 2022
    date_display: Nov 2022
    date_iso: '2022-11-11'
    published_venue: ICML 2022
    published_conference: ICML 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-11'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9609
    true_std: 0.0012
    value_gap_source_arxiv: '2211.06489'
    value_gap_source_title: Equivariance with Learned Canonicalization Functions
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9609
    sort_std: 0.0012
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
- benchmark: GNNBenchmark
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: MNIST
      dataset_slug: mnist
main_figure: /figures/2211.06489/main_figure.jpegoptim.jpg
---

