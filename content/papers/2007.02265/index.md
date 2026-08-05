---
title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
arxiv_id: '2007.02265'
source_url: ''
authors:
- name: Xiao Wang
  orcid: null
  s2_author_id: '2118449003'
  s2_url: null
- name: Meiqi Zhu
  orcid: null
  s2_author_id: '2109834004'
  s2_url: null
- name: Deyu Bo
  orcid: null
  s2_author_id: '1491450638'
  s2_url: null
- name: Peng Cui
  orcid: null
  s2_author_id: '143738684'
  s2_url: null
- name: Chuan Shi
  orcid: null
  s2_author_id: '144123161'
  s2_url: null
- name: Jian Pei
  orcid: null
  s2_author_id: '145525190'
  s2_url: null
published_date: Jul 5, 2020
published_date_iso: '2020-07-05'
published_venue: KDD 2020
published_conference: KDD 2020
published_conference_short: KDD
published_conference_slug: kdd
abstract: Graph Convolutional Networks (GCNs) have gained great popularity in tackling
  various analytics tasks on graph and network data. However, some recent studies
  raise concerns about whether GCNs can optimally integrate node features and topological
  structures in a complex graph with rich information. In this paper, we first present
  an experimental investigation. Surprisingly, our experimental results clearly show
  that the capability of the state-of-the-art GCNs in fusing node features and topological
  structures is distant from optimal or even satisfactory. The weakness may severely
  hinder the capability of GCNs in some classification tasks, since GCNs may not be
  able to adaptively learn some deep correlation information between topological structures
  and node features. Can we remedy the weakness and design a new type of GCNs that
  can retain the advantages of the state-of-the-art GCNs and, at the same time, enhance
  the capability of fusing topological structures and node features substantially?
  We tackle the challenge and propose an adaptive multi-channel graph convolutional
  networks for semi-supervised classification (AM-GCN). The central idea is that we
  extract the specific and common embeddings from node features, topological structures,
  and their combinations simultaneously, and use the attention mechanism to learn
  adaptive importance weights of the embeddings. Our extensive experiments on benchmark
  data sets clearly show that AM-GCN extracts the most correlated information from
  both node features and topological structures substantially, and improves the classification
  accuracy with a clear margin.
codebase_url: https://github.com/thunlp/OpenNE
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GCN
- AM-GCN
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
  is_multi_metric: true
  rows:
  - model: AM-GCN
    model_key: am-gcn
    model_plain: AM-GCN
    metric_values:
    - null
    - 0.9142
    - 0.9136
    metric_stds:
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.9142
    sort_std: null
    true_value: 0.9142
    true_std: null
    paper_value: 0.9142
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
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
    published_venue: KDD 2020
    date: Jul 5, 2020
    date_display: Jul 2020
    date_iso: '2020-07-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.9054
    - 0.9049
    metric_stds:
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9054
    sort_std: null
    true_value: 0.9054
    true_std: null
    paper_value: 0.9054
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
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
    published_venue: KDD 2020
    date: Jul 5, 2020
    date_display: Jul 2020
    date_iso: '2020-07-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 2
  - model: GAT
    model_key: gat
    model_plain: GAT
    metric_values:
    - null
    - 0.904
    - 0.9039
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
    sort_value: 0.904
    sort_std: null
    true_value: 0.904
    true_std: null
    paper_value: 0.904
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
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
    published_venue: KDD 2020
    date: Jul 5, 2020
    date_display: Jul 2020
    date_iso: '2020-07-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 3
  - model: DEMO-Net
    model_key: demo-net
    model_plain: DEMO-Net
    metric_values:
    - null
    - 0.8655
    - 0.8483
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
    sort_value: 0.8655
    sort_std: null
    true_value: 0.8655
    true_std: null
    paper_value: 0.8655
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
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
    published_venue: KDD 2020
    date: Jul 5, 2020
    date_display: Jul 2020
    date_iso: '2020-07-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 4
  - model: Chebyshev
    model_key: chebyshev
    model_plain: Chebyshev
    metric_values:
    - null
    - 0.8543
    - 0.8526
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
    sort_value: 0.8543
    sort_std: null
    true_value: 0.8543
    true_std: null
    paper_value: 0.8543
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
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
    published_venue: KDD 2020
    date: Jul 5, 2020
    date_display: Jul 2020
    date_iso: '2020-07-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 5
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    metric_values:
    - null
    - 0.8309
    - 0.8224
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
    sort_value: 0.8309
    sort_std: null
    true_value: 0.8309
    true_std: null
    paper_value: 0.8309
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
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
    published_venue: KDD 2020
    date: Jul 5, 2020
    date_display: Jul 2020
    date_iso: '2020-07-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 6
  - model: kNN-GCN
    model_key: knn-gcn
    model_plain: kNN-GCN
    metric_values:
    - null
    - 0.82
    - 0.8195
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
    sort_value: 0.82
    sort_std: null
    true_value: 0.82
    true_std: null
    paper_value: 0.82
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
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
    published_venue: KDD 2020
    date: Jul 5, 2020
    date_display: Jul 2020
    date_iso: '2020-07-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 7
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    metric_values:
    - null
    - 0.6703
    - 0.6699
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.6703
    sort_std: null
    true_value: 0.6703
    true_std: null
    paper_value: 0.6703
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
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
    published_venue: KDD 2020
    date: Jul 5, 2020
    date_display: Jul 2020
    date_iso: '2020-07-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 12
  - model: LINE
    model_key: line
    model_plain: LINE
    metric_values:
    - null
    - 0.5041
    - 0.4992
    metric_stds:
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.5041
    sort_std: null
    true_value: 0.5041
    true_std: null
    paper_value: 0.5041
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
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
    published_venue: KDD 2020
    date: Jul 5, 2020
    date_display: Jul 2020
    date_iso: '2020-07-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 24
  metrics:
  - Micro-F1
  - ACC
  - F1
  primary_metric: Micro-F1
  rank_metric: ACC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - ACC
  - F1
  metric: ACC
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
main_figure: /figures/2007.02265/main_figure.jpegoptim.jpg
---

