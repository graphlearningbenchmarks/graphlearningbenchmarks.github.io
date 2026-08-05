---
title: 'graph2vec: Learning Distributed Representations of Graphs'
arxiv_id: '1707.05005'
source_url: ''
authors:
- name: A. Narayanan
  orcid: null
  s2_author_id: '2075601'
  s2_url: null
- name: Mahinthan Chandramohan
  orcid: null
  s2_author_id: '1735135'
  s2_url: null
- name: R. Venkatesan
  orcid: null
  s2_author_id: '36746267'
  s2_url: null
- name: Lihui Chen
  orcid: null
  s2_author_id: '6187400'
  s2_url: null
- name: Yang Liu
  orcid: null
  s2_author_id: '2152799887'
  s2_url: null
- name: Shantanu Jaiswal
  orcid: null
  s2_author_id: '31275801'
  s2_url: null
published_date: Jul 17, 2017
published_date_iso: '2017-07-17'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Recent works on representation learning for graph structured data predominantly
  focus on learning distributed representations of graph substructures such as nodes
  and subgraphs. However, many graph analytics tasks such as graph classification
  and clustering require representing entire graphs as fixed length feature vectors.
  While the aforementioned approaches are naturally unequipped to learn such representations,
  graph kernels remain as the most effective way of obtaining them. However, these
  graph kernels use handcrafted features (e.g., shortest paths, graphlets, etc.) and
  hence are hampered by problems such as poor generalization. To address this limitation,
  in this work, we propose a neural embedding framework named graph2vec to learn data-driven
  distributed representations of arbitrary sized graphs. graph2vec's embeddings are
  learnt in an unsupervised manner and are task agnostic. Hence, they could be used
  for any downstream task such as graph classification, clustering and even seeding
  supervised representation learning approaches. Our experiments on several benchmark
  and large real-world datasets show that graph2vec achieves significant improvements
  in classification and clustering accuracies over substructure representation learning
  approaches and are competitive with state-of-the-art graph kernels.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- graph2vec
mrr: 0.0028
adjusted_mrr: 0.0009
mrr_dataset_count: 1
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: PROTEINS
  rows:
  - model: Graphormer-SPIS
    model_key: gmn
    model_plain: Graphormer-SPIS
    value: 0.8225
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8225
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: ci-gnn
    model_plain: Graphormer-SPIS
    value: 0.82
    std: 0.02
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2301.01642'
    title: 'CI-GNN: A Granger Causality-Inspired Graph Neural Network for Interpretable
      Brain Network-Based Psychiatric Diagnosis'
    date: Jan 4, 2023
    date_display: Jan 2023
    date_iso: '2023-01-04'
    venue: Neural Networks
    codebase_url: https://github.com/ZKZ-Brain/CI-GNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.82
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: diffpool+gpl
    model_plain: Graphormer-SPIS
    value: 0.8196
    std: 0.0286
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.11361'
    title: 'Graph Structure Prompt Learning: A Novel Methodology to Improve Performance
      of Graph Neural Networks'
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    venue: Applied intelligence (Boston)
    codebase_url: https://github.com/PreckLi/graph_prompt_learning
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8196
    sort_std: 0.0286
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: WL kernel
    model_key: wl kernel
    model_plain: WL kernel
    value: 0.7292
    std: 0.0056
    paper_value: 0.7292
    paper_std: 0.0056
    metric: Accuracy
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
    source_ref: wlk [24]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: '10-fold CV (as per experiment setup: 90% train/10% test with 5-fold
      CV for hyperparameter tuning, though table caption specifies average accuracy/std
      dev for the benchmark)'
    date: Jul 17, 2017
    date_display: Jul 2017
    date_iso: '2017-07-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
    value_gap_source_date_label: AAAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.75
    true_std: 0.031
    value_gap_source_arxiv: '2308.06838'
    value_gap_source_title: 'Weisfeiler and Lehman Go Paths: Learning Topological
      Features via Path Complexes'
    value_gap_source_is_current_paper: false
    value_gap: 0.02080000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.75
    sort_std: 0.031
    global_rank: 258
    paper_rank: 379
    rank_delta: 121
    rank_delta_abs: 121
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: graph2vec
    model_key: graph2vec
    model_plain: graph2vec
    value: 0.733
    std: 0.0205
    paper_value: 0.733
    paper_std: 0.0205
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: '10-fold CV (as per experiment setup: 90% train/10% test with 5-fold
      CV for hyperparameter tuning, though table caption specifies average accuracy/std
      dev for the benchmark)'
    date: Jul 17, 2017
    date_display: Jul 2017
    date_iso: '2017-07-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.733
    true_std: 0.0205
    value_gap_source_arxiv: '2505.11356'
    value_gap_source_title: Fractal Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.733
    sort_std: 0.0205
    global_rank: 361
    paper_rank: 361
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Deep WL kernel
    model_key: deep wl kernel
    model_plain: Deep WL kernel
    value: 0.733
    std: 0.0082
    paper_value: 0.733
    paper_std: 0.0082
    metric: Accuracy
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
    source_ref: dgk [25]
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: '10-fold CV (as per experiment setup: 90% train/10% test with 5-fold
      CV for hyperparameter tuning, though table caption specifies average accuracy/std
      dev for the benchmark)'
    date: Jul 17, 2017
    date_display: Jul 2017
    date_iso: '2017-07-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-07-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.733
    true_std: 0.0082
    value_gap_source_arxiv: '1707.05005'
    value_gap_source_title: 'graph2vec: Learning Distributed Representations of Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.733
    sort_std: 0.0082
    global_rank: 364
    paper_rank: 364
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: nv
    model_key: nv
    model_plain: nv
    value: 0.5749
    std: 0.0357
    paper_value: 0.5749
    paper_std: 0.0357
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: n2v
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: '10-fold CV (as per experiment setup: 90% train/10% test with 5-fold
      CV for hyperparameter tuning, though table caption specifies average accuracy/std
      dev for the benchmark)'
    date: Jul 17, 2017
    date_display: Jul 2017
    date_iso: '2017-07-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-07-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5749
    true_std: 0.0357
    value_gap_source_arxiv: '1707.05005'
    value_gap_source_title: 'graph2vec: Learning Distributed Representations of Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5749
    sort_std: 0.0357
    global_rank: 519
    paper_rank: 519
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: sv
    model_key: sv
    model_plain: sv
    value: 0.5303
    std: 0.0555
    paper_value: 0.5303
    paper_std: 0.0555
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: sub2vec
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: '10-fold CV (as per experiment setup: 90% train/10% test with 5-fold
      CV for hyperparameter tuning, though table caption specifies average accuracy/std
      dev for the benchmark)'
    date: Jul 17, 2017
    date_display: Jul 2017
    date_iso: '2017-07-17'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2017-07-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5303
    true_std: 0.0555
    value_gap_source_arxiv: '1707.05005'
    value_gap_source_title: 'graph2vec: Learning Distributed Representations of Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5303
    sort_std: 0.0555
    global_rank: 522
    paper_rank: 522
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
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: PROTEINS
      dataset_slug: proteins
single_proposed_model: graph2vec
main_figure: /figures/1707.05005/main_figure.jpegoptim.jpg
---

