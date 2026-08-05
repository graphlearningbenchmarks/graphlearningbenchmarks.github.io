---
title: 'Less Can Be More: Unsupervised Graph Pruning for Large-scale Dynamic Graphs'
arxiv_id: '2305.10673'
source_url: ''
authors:
- name: Jintang Li
  orcid: null
  s2_author_id: '2115953679'
  s2_url: null
- name: Sheng Tian
  orcid: null
  s2_author_id: '2671378'
  s2_url: null
- name: Ruofan Wu
  orcid: null
  s2_author_id: '2087049620'
  s2_url: null
- name: Liang Zhu
  orcid: null
  s2_author_id: '2143509733'
  s2_url: null
- name: Wenlong Zhao
  orcid: null
  s2_author_id: '2217580640'
  s2_url: null
- name: Changhua Meng
  orcid: null
  s2_author_id: '2114323322'
  s2_url: null
- name: Liang Chen
  orcid: null
  s2_author_id: '2146035112'
  s2_url: null
- name: Zibin Zheng
  orcid: null
  s2_author_id: '144291579'
  s2_url: null
- name: Hongzhi Yin
  orcid: null
  s2_author_id: '2416851'
  s2_url: null
published_date: May 18, 2023
published_date_iso: '2023-05-18'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: The prevalence of large-scale graphs poses great challenges in time and
  storage for training and deploying graph neural networks (GNNs). Several recent
  works have explored solutions for pruning the large original graph into a small
  and highly-informative one, such that training and inference on the pruned and large
  graphs have comparable performance. Although empirically effective, current researches
  focus on static or non-temporal graphs, which are not directly applicable to dynamic
  scenarios. In addition, they require labels as ground truth to learn the informative
  structure, limiting their applicability to new problem domains where labels are
  hard to obtain. To solve the dilemma, we propose and study the problem of unsupervised
  graph pruning on dynamic graphs. We approach the problem by our proposed STEP, a
  self-supervised temporal pruning framework that learns to remove potentially redundant
  edges from input dynamic graphs. From a technical and industrial viewpoint, our
  method overcomes the trade-offs between the performance and the time & memory overheads.
  Our results on three real-world datasets demonstrate the advantages on improving
  the efficacy, robustness, and efficiency of GNNs on dynamic node classification
  tasks. Most notably, STEP is able to prune more than 50\
codebase_url: https://github.com/EdisonLeeeee/STEP
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Reddit
  rows:
  - model: SPLASH
    model_key: splash
    model_plain: SPLASH
    value: 0.7358
    std: 0.0028
    metric: AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2504.00328'
    title: Simple yet Effective Node Property Prediction on Edge Streams under Distribution
      Shifts
    date: Apr 1, 2025
    date_display: Apr 2025
    date_iso: '2025-04-01'
    venue: IEEE International Conference on Data Engineering
    codebase_url: https://github.com/jhsk777/SPLASH
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7358
    sort_std: 0.0028
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Backbone (TGAT)
    model_key: backbone (tgat)
    model_plain: Backbone (TGAT)
    value: 0.6822
    std: 0.0052
    paper_value: 0.6822
    paper_std: 0.0052
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard dynamic node classification on Reddit with pruning ratio
      0
    date: May 18, 2023
    date_display: May 2023
    date_iso: '2023-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-18'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6822
    true_std: 0.0052
    value_gap_source_arxiv: '2305.10673'
    value_gap_source_title: 'Less Can Be More: Unsupervised Graph Pruning for Large-scale
      Dynamic Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6822
    sort_std: 0.0052
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
  - model: PINT
    model_key: pint
    model_plain: PINT
    value: 0.6731
    std: 0.002
    metric: AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2209.15059'
    title: Provably expressive temporal graph networks
    date: Sep 29, 2022
    date_display: Sep 2022
    date_iso: '2022-09-29'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6731
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - AUC
  metric: AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Reddit
      dataset_slug: reddit
main_figure: /figures/2305.10673/main_figure.jpegoptim.jpg
---

