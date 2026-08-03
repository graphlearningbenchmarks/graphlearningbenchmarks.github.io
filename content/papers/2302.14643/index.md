---
title: 'Graph-based Knowledge Distillation: A survey and experimental evaluation'
arxiv_id: '2302.14643'
source_url: ''
authors:
- name: Jing Liu
  orcid: null
  s2_author_id: '2153466123'
  s2_url: null
- name: Tongya Zheng
  orcid: null
  s2_author_id: '2062719264'
  s2_url: null
- name: Guanzhen Zhang
  orcid: null
  s2_author_id: '2275887482'
  s2_url: null
- name: Qinfen Hao
  orcid: null
  s2_author_id: '36851883'
  s2_url: null
published_date: Feb 27, 2023
published_date_iso: '2023-02-27'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph, such as citation networks, social networks, and transportation networks,
  are prevalent in the real world. Graph Neural Networks (GNNs) have gained widespread
  attention for their robust expressiveness and exceptional performance in various
  graph applications. However, the efficacy of GNNs is heavily reliant on sufficient
  data labels and complex network models, with the former obtaining hardly and the
  latter computing costly. To address the labeled data scarcity and high complexity
  of GNNs, Knowledge Distillation (KD) has been introduced to enhance existing GNNs.
  This technique involves transferring the soft-label supervision of the large teacher
  model to the small student model while maintaining prediction performance. This
  survey offers a comprehensive overview of Graph-based Knowledge Distillation methods,
  systematically categorizing and summarizing them while discussing their limitations
  and future directions. This paper first introduces the background of graph and KD.
  It then provides a comprehensive summary of three types of Graph-based Knowledge
  Distillation methods, namely Graph-based Knowledge Distillation for deep neural
  networks (DKD), Graph-based Knowledge Distillation for GNNs (GKD), and Self-Knowledge
  Distillation based Graph-based Knowledge Distillation (SKD). Each type is further
  divided into knowledge distillation methods based on the output layer, middle layer,
  and constructed graph. Subsequently, various algorithms' ideas are analyzed and
  compared, concluding with the advantages and disadvantages of each algorithm supported
  by experimental results. In addition, the applications of graph-based knowledge
  distillation in CV, NLP, RS, and other fields are listed. Finally, the graph-based
  knowledge distillation is summarized and prospectively discussed. We have also released
  related resources at https://github.com/liujing1023/Graph-based-Knowledge-Distillation.
codebase_url: https://github.com/liujing1023/Graph-based-Knowledge-Distillation
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
  dataset: Coauthor-Physics
  is_multi_metric: true
  rows:
  - model: GCN+CPF
    model_key: gcn+cpf
    model_plain: GCN+CPF
    metric_values:
    - null
    - 0.9476
    - 0.9304
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9476
    sort_std: null
    true_value: 0.9476
    true_std: null
    paper_value: 0.9476
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.14643'
    value_gap_source_title: 'Graph-based Knowledge Distillation: A survey and experimental
      evaluation'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: GAT+CPF
    model_key: gat+cpf
    model_plain: GAT+CPF
    metric_values:
    - null
    - 0.9407
    - 0.9219
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9407
    sort_std: null
    true_value: 0.9407
    true_std: null
    paper_value: 0.9407
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.14643'
    value_gap_source_title: 'Graph-based Knowledge Distillation: A survey and experimental
      evaluation'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 2
  - model: SAGE+KD
    model_key: sage+kd
    model_plain: SAGE+KD
    metric_values:
    - null
    - 0.9379
    - 0.9163
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9379
    sort_std: null
    true_value: 0.9379
    true_std: null
    paper_value: 0.9379
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.14643'
    value_gap_source_title: 'Graph-based Knowledge Distillation: A survey and experimental
      evaluation'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 3
  - model: SAGE+CPF
    model_key: sage+cpf
    model_plain: SAGE+CPF
    metric_values:
    - null
    - 0.9363
    - 0.9135
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9363
    sort_std: null
    true_value: 0.9363
    true_std: null
    paper_value: 0.9363
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.14643'
    value_gap_source_title: 'Graph-based Knowledge Distillation: A survey and experimental
      evaluation'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: GAT+KD
    model_key: gat+kd
    model_plain: GAT+KD
    metric_values:
    - null
    - 0.935
    - 0.9136
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.935
    sort_std: null
    true_value: 0.935
    true_std: null
    paper_value: 0.935
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.14643'
    value_gap_source_title: 'Graph-based Knowledge Distillation: A survey and experimental
      evaluation'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 5
  - model: GCN+KD
    model_key: gcn+kd
    model_plain: GCN+KD
    metric_values:
    - null
    - 0.9322
    - 0.9107
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9322
    sort_std: null
    true_value: 0.9322
    true_std: null
    paper_value: 0.9322
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.14643'
    value_gap_source_title: 'Graph-based Knowledge Distillation: A survey and experimental
      evaluation'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - null
    - 0.9252
    - 0.9023
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9252
    sort_std: null
    true_value: 0.9252
    true_std: null
    paper_value: 0.9252
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.14643'
    value_gap_source_title: 'Graph-based Knowledge Distillation: A survey and experimental
      evaluation'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - null
    - 0.9239
    - 0.9021
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9239
    sort_std: null
    true_value: 0.9239
    true_std: null
    paper_value: 0.9239
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.14643'
    value_gap_source_title: 'Graph-based Knowledge Distillation: A survey and experimental
      evaluation'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 8
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.9226
    - 0.9002
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9226
    sort_std: null
    true_value: 0.9226
    true_std: null
    paper_value: 0.9226
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2302.14643'
    value_gap_source_title: 'Graph-based Knowledge Distillation: A survey and experimental
      evaluation'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 9
  metrics:
  - Accuracy
  - F1-Micro
  - F1-Macro
  primary_metric: Accuracy
  rank_metric: F1-Micro
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - F1-Micro
  - F1-Macro
  metric: F1-Micro
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
    - dataset: Coauthor-Physics
      dataset_slug: coauthor-physics
---

