---
title: Graph Communal Contrastive Learning
arxiv_id: '2110.14863'
source_url: ''
authors:
- name: Bolian Li
  orcid: null
  s2_author_id: '2381413102'
  s2_url: null
- name: Baoyu Jing
  orcid: null
  s2_author_id: '29860450'
  s2_url: null
- name: Hanghang Tong
  orcid: null
  s2_author_id: '8163721'
  s2_url: null
published_date: Oct 28, 2021
published_date_iso: '2021-10-28'
published_venue: WWW 2021
published_conference: WWW 2021
published_conference_short: WWW
published_conference_slug: www
abstract: 'Graph representation learning is crucial for many real-world applications
  (e.g. social relation analysis). A fundamental problem for graph representation
  learning is how to effectively learn representations without human labeling, which
  is usually costly and time-consuming. Graph contrastive learning (GCL) addresses
  this problem by pulling the positive node pairs (or similar nodes) closer while
  pushing the negative node pairs (or dissimilar nodes) apart in the representation
  space. Despite the success of the existing GCL methods, they primarily sample node
  pairs based on the node-level proximity yet the community structures have rarely
  been taken into consideration. As a result, two nodes from the same community might
  be sampled as a negative pair. We argue that the community information should be
  considered to identify node pairs in the same communities, where the nodes insides
  are semantically similar. To address this issue, we propose a novel Graph Communal
  Contrastive Learning ($gCooL$) framework to jointly learn the community partition
  and learn node representations in an end-to-end fashion. Specifically, the proposed
  $gCooL$ consists of two components: a Dense Community Aggregation ($DeCA$) algorithm
  for community detection and a Reweighted Self-supervised Cross-contrastive ($ReSC$)
  training scheme to utilize the community information. Additionally, the real-world
  graphs are complex and often consist of multiple views. In this paper, we demonstrate
  that the proposed $gCooL$ can also be naturally adapted to multiplex graphs. Finally,
  we comprehensively evaluate the proposed $gCooL$ on a variety of real-world graphs.
  The experimental results show that the $gCooL$ outperforms the state-of-the-art
  methods.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- gCooL_c
- gCooL_e
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 4
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
  dataset: Amazon-Computers
  is_multi_metric: true
  rows:
  - model: gCooL_c
    model_key: gcool_c
    model_plain: gCooL_c
    metric_values:
    - null
    - 0.8885
    - 0.8742
    metric_stds:
    - null
    - 0.14
    - 0.28
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.8885
    sort_std: 0.14
    true_value: 0.8885
    true_std: 0.14
    paper_value: 0.8885
    paper_std: 0.14
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: gCooL_e
    model_key: gcool_e
    model_plain: gCooL_e
    metric_values:
    - null
    - 0.8874
    - 0.8753
    metric_stds:
    - null
    - 0.09
    - 0.26
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.8874
    sort_std: 0.09
    true_value: 0.8874
    true_std: 0.09
    paper_value: 0.8874
    paper_std: 0.09
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 2
  - model: GCA
    model_key: gca
    model_plain: GCA
    metric_values:
    - null
    - 0.8767
    - 0.8588
    metric_stds:
    - null
    - 0.49
    - 0.3
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8767
    sort_std: 0.49
    true_value: 0.8767
    true_std: 0.49
    paper_value: 0.8767
    paper_std: 0.49
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 3
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - null
    - 0.8742
    - 0.8592
    metric_stds:
    - null
    - 0.07
    - 0.11
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8742
    sort_std: 0.07
    true_value: 0.8742
    true_std: 0.07
    paper_value: 0.8742
    paper_std: 0.07
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 4
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    metric_values:
    - null
    - 0.8644
    - 0.8372
    metric_stds:
    - null
    - 0.25
    - 0.12
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8644
    sort_std: 0.25
    true_value: 0.8644
    true_std: 0.25
    paper_value: 0.8644
    paper_std: 0.25
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 5
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.8643
    - 0.8399
    metric_stds:
    - null
    - 0.56
    - 0.61
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8643
    sort_std: 0.56
    true_value: 0.8643
    true_std: 0.56
    paper_value: 0.8643
    paper_std: 0.56
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 6
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    metric_values:
    - null
    - 0.8563
    - 0.8402
    metric_stds:
    - null
    - 0.09
    - 0.1
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.8563
    sort_std: 0.09
    true_value: 0.8563
    true_std: 0.09
    paper_value: 0.8563
    paper_std: 0.09
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 7
  - model: HDI
    model_key: hdi
    model_plain: HDI
    metric_values:
    - null
    - 0.8543
    - 0.8074
    metric_stds:
    - null
    - 0.13
    - 0.25
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8543
    sort_std: 0.13
    true_value: 0.8543
    true_std: 0.13
    paper_value: 0.8543
    paper_std: 0.13
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 8
  - model: GAE
    model_key: gae
    model_plain: GAE
    metric_values:
    - null
    - 0.8518
    - 0.8333
    metric_stds:
    - null
    - 0.21
    - 0.17
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8518
    sort_std: 0.21
    true_value: 0.8518
    true_std: 0.21
    paper_value: 0.8518
    paper_std: 0.21
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 9
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    metric_values:
    - null
    - 0.8438
    - 0.8265
    metric_stds:
    - null
    - 0.08
    - 0.08
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.8438
    sort_std: 0.08
    true_value: 0.8438
    true_std: 0.08
    paper_value: 0.8438
    paper_std: 0.08
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 12
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - null
    - 0.8388
    - 0.793
    metric_stds:
    - null
    - 0.5
    - 0.42
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8388
    sort_std: 0.5
    true_value: 0.8388
    true_std: 0.5
    paper_value: 0.8388
    paper_std: 0.5
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 14
  - model: RawFeatures
    model_key: rawfeatures
    model_plain: RawFeatures
    metric_values:
    - null
    - 0.7382
    - 0.701
    metric_stds:
    - null
    - 0.01
    - 0.04
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.7382
    sort_std: 0.01
    true_value: 0.7382
    true_std: 0.01
    paper_value: 0.7382
    paper_std: 0.01
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 15
  metrics:
  - Accuracy
  - Micro-F1
  - Macro-F1
  primary_metric: Accuracy
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Micro-F1
  - Macro-F1
  metric: Micro-F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: Amazon-Photo
  is_multi_metric: true
  rows:
  - model: gCooL_c
    model_key: gcool_c
    model_plain: gCooL_c
    metric_values:
    - null
    - 0.9318
    - 0.9205
    metric_stds:
    - null
    - 0.0012
    - 0.0017
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.9318
    sort_std: 0.0012
    true_value: 0.9318
    true_std: 0.0012
    paper_value: 0.9318
    paper_std: 0.0012
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: gCooL_e
    model_key: gcool_e
    model_plain: gCooL_e
    metric_values:
    - null
    - 0.9279
    - 0.9157
    metric_stds:
    - null
    - 0.0017
    - 0.0029
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.9279
    sort_std: 0.0017
    true_value: 0.9279
    true_std: 0.0017
    paper_value: 0.9279
    paper_std: 0.0017
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.9251
    - 0.9047
    metric_stds:
    - null
    - 0.0023
    - 0.0032
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9251
    sort_std: 0.0023
    true_value: 0.9251
    true_std: 0.0023
    paper_value: 0.9251
    paper_std: 0.0023
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: GCA
    model_key: gca
    model_plain: GCA
    metric_values:
    - null
    - 0.9239
    - 0.9105
    metric_stds:
    - null
    - 0.0021
    - 0.0013
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9239
    sort_std: 0.0021
    true_value: 0.9239
    true_std: 0.0021
    paper_value: 0.9239
    paper_std: 0.0021
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    metric_values:
    - null
    - 0.9224
    - 0.9004
    metric_stds:
    - null
    - 0.0008
    - 0.0017
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9224
    sort_std: 0.0008
    true_value: 0.9224
    true_std: 0.0008
    paper_value: 0.9224
    paper_std: 0.0008
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - null
    - 0.9174
    - 0.8993
    metric_stds:
    - null
    - 0.0009
    - 0.0009
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9174
    sort_std: 0.0009
    true_value: 0.9174
    true_std: 0.0009
    paper_value: 0.9174
    paper_std: 0.0009
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: GAE
    model_key: gae
    model_plain: GAE
    metric_values:
    - null
    - 0.9168
    - 0.8966
    metric_stds:
    - null
    - 0.0014
    - 0.0009
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9168
    sort_std: 0.0014
    true_value: 0.9168
    true_std: 0.0014
    paper_value: 0.9168
    paper_std: 0.0014
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - null
    - 0.916
    - 0.8931
    metric_stds:
    - null
    - 0.0024
    - 0.0016
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.916
    sort_std: 0.0024
    true_value: 0.916
    true_std: 0.0024
    paper_value: 0.916
    paper_std: 0.0024
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: HDI
    model_key: hdi
    model_plain: HDI
    metric_values:
    - null
    - 0.9009
    - 0.887
    metric_stds:
    - null
    - 0.001
    - 0.0016
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9009
    sort_std: 0.001
    true_value: 0.9009
    true_std: 0.001
    paper_value: 0.9009
    paper_std: 0.001
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    metric_values:
    - null
    - 0.8972
    - 0.8739
    metric_stds:
    - null
    - 0.0008
    - 0.0007
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.8972
    sort_std: 0.0008
    true_value: 0.8972
    true_std: 0.0008
    paper_value: 0.8972
    paper_std: 0.0008
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    metric_values:
    - null
    - 0.8936
    - 0.8692
    metric_stds:
    - null
    - 0.001
    - 0.0002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.8936
    sort_std: 0.001
    true_value: 0.8936
    true_std: 0.001
    paper_value: 0.8936
    paper_std: 0.001
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 11
  - model: RawFeatures
    model_key: rawfeatures
    model_plain: RawFeatures
    metric_values:
    - null
    - 0.7845
    - 0.761
    metric_stds:
    - null
    - 0.0004
    - 0.0001
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.7845
    sort_std: 0.0004
    true_value: 0.7845
    true_std: 0.0004
    paper_value: 0.7845
    paper_std: 0.0004
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 12
  metrics:
  - Accuracy
  - Micro-F1
  - Macro-F1
  primary_metric: Accuracy
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Micro-F1
  - Macro-F1
  metric: Micro-F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id004
  dataset: Coauthor-CS
  is_multi_metric: true
  rows:
  - model: gCooL_c
    model_key: gcool_c
    model_plain: gCooL_c
    metric_values:
    - null
    - 0.9332
    - 0.9165
    metric_stds:
    - null
    - 0.0002
    - 0.0003
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.9332
    sort_std: 0.0002
    true_value: 0.9332
    true_std: 0.0002
    paper_value: 0.9332
    paper_std: 0.0002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: gCooL_e
    model_key: gcool_e
    model_plain: gCooL_e
    metric_values:
    - null
    - 0.9331
    - 0.9163
    metric_stds:
    - null
    - 0.0001
    - 0.0003
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.9331
    sort_std: 0.0001
    true_value: 0.9331
    true_std: 0.0001
    paper_value: 0.9331
    paper_std: 0.0001
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 2
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.9304
    - 0.9102
    metric_stds:
    - null
    - 0.0028
    - 0.0038
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9304
    sort_std: 0.0028
    true_value: 0.9304
    true_std: 0.0028
    paper_value: 0.9304
    paper_std: 0.0028
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 3
  - model: GCA
    model_key: gca
    model_plain: GCA
    metric_values:
    - null
    - 0.9287
    - 0.9076
    metric_stds:
    - null
    - 0.0003
    - 0.0001
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9287
    sort_std: 0.0003
    true_value: 0.9287
    true_std: 0.0003
    paper_value: 0.9287
    paper_std: 0.0003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - null
    - 0.9211
    - 0.905
    metric_stds:
    - null
    - 0.001
    - 0.0012
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9211
    sort_std: 0.001
    true_value: 0.9211
    true_std: 0.001
    paper_value: 0.9211
    paper_std: 0.001
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - null
    - 0.9208
    - 0.9078
    metric_stds:
    - null
    - 0.0068
    - 0.0068
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9208
    sort_std: 0.0068
    true_value: 0.9208
    true_std: 0.0068
    paper_value: 0.9208
    paper_std: 0.0068
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    metric_values:
    - null
    - 0.9208
    - 0.9011
    metric_stds:
    - null
    - 0.0008
    - 0.0006
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9208
    sort_std: 0.0008
    true_value: 0.9208
    true_std: 0.0008
    paper_value: 0.9208
    paper_std: 0.0008
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: RawFeatures
    model_key: rawfeatures
    model_plain: RawFeatures
    metric_values:
    - null
    - 0.904
    - 0.8901
    metric_stds:
    - null
    - 0.0002
    - 0.0006
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.904
    sort_std: 0.0002
    true_value: 0.904
    true_std: 0.0002
    paper_value: 0.904
    paper_std: 0.0002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: GAE
    model_key: gae
    model_plain: GAE
    metric_values:
    - null
    - 0.9
    - 0.8831
    metric_stds:
    - null
    - 0.0075
    - 0.0068
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.9
    sort_std: 0.0075
    true_value: 0.9
    true_std: 0.0075
    paper_value: 0.9
    paper_std: 0.0075
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: HDI
    model_key: hdi
    model_plain: HDI
    metric_values:
    - null
    - 0.8998
    - 0.8673
    metric_stds:
    - null
    - 0.0014
    - 0.0017
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.8998
    sort_std: 0.0014
    true_value: 0.8998
    true_std: 0.0014
    paper_value: 0.8998
    paper_std: 0.0014
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    metric_values:
    - null
    - 0.8511
    - 0.8293
    metric_stds:
    - null
    - 0.0006
    - 0.0011
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.8511
    sort_std: 0.0006
    true_value: 0.8511
    true_std: 0.0006
    paper_value: 0.8511
    paper_std: 0.0006
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 11
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    metric_values:
    - null
    - 0.8471
    - 0.8263
    metric_stds:
    - null
    - 0.0023
    - 0.0019
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.8471
    sort_std: 0.0023
    true_value: 0.8471
    true_std: 0.0023
    paper_value: 0.8471
    paper_std: 0.0023
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 12
  metrics:
  - Accuracy
  - Micro-F1
  - Macro-F1
  primary_metric: Accuracy
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Micro-F1
  - Macro-F1
  metric: Micro-F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id003
  dataset: WikiCS
  is_multi_metric: true
  rows:
  - model: gCooL_c
    model_key: gcool_c
    model_plain: gCooL_c
    metric_values:
    - null
    - 0.7874
    - 0.7592
    metric_stds:
    - null
    - 0.0004
    - 0.0006
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.7874
    sort_std: 0.0004
    true_value: 0.7874
    true_std: 0.0004
    paper_value: 0.7874
    paper_std: 0.0004
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: gCooL_e
    model_key: gcool_e
    model_plain: gCooL_e
    metric_values:
    - null
    - 0.7874
    - 0.7588
    metric_stds:
    - null
    - 0.0003
    - 0.0002
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.7874
    sort_std: 0.0003
    true_value: 0.7874
    true_std: 0.0003
    paper_value: 0.7874
    paper_std: 0.0003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 2
  - model: GCA
    model_key: gca
    model_plain: GCA
    metric_values:
    - null
    - 0.7824
    - 0.7447
    metric_stds:
    - null
    - 0.0001
    - 0.0002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7824
    sort_std: 0.0001
    true_value: 0.7824
    true_std: 0.0001
    paper_value: 0.7824
    paper_std: 0.0001
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - null
    - 0.775
    - 0.7562
    metric_stds:
    - null
    - 0.0008
    - 0.0
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.775
    sort_std: 0.0008
    true_value: 0.775
    true_std: 0.0008
    paper_value: 0.775
    paper_std: 0.0008
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    metric_values:
    - null
    - 0.7711
    - 0.7561
    metric_stds:
    - null
    - 0.0008
    - 0.0019
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7711
    sort_std: 0.0008
    true_value: 0.7711
    true_std: 0.0008
    paper_value: 0.7711
    paper_std: 0.0008
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: HDI
    model_key: hdi
    model_plain: HDI
    metric_values:
    - null
    - 0.7572
    - 0.6805
    metric_stds:
    - null
    - 0.0055
    - 0.008
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7572
    sort_std: 0.0055
    true_value: 0.7572
    true_std: 0.0055
    paper_value: 0.7572
    paper_std: 0.0055
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    metric_values:
    - null
    - 0.7556
    - 0.7412
    metric_stds:
    - null
    - 0.002
    - 0.001
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7556
    sort_std: 0.002
    true_value: 0.7556
    true_std: 0.002
    paper_value: 0.7556
    paper_std: 0.002
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: DGI
    model_key: dgi
    model_plain: DGI
    metric_values:
    - null
    - 0.7535
    - 0.7374
    metric_stds:
    - null
    - 0.0017
    - 0.002
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7535
    sort_std: 0.0017
    true_value: 0.7535
    true_std: 0.0017
    paper_value: 0.7535
    paper_std: 0.0017
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    metric_values:
    - null
    - 0.7425
    - 0.7268
    metric_stds:
    - null
    - 0.0006
    - 0.0015
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.7425
    sort_std: 0.0006
    true_value: 0.7425
    true_std: 0.0006
    paper_value: 0.7425
    paper_std: 0.0006
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
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
  - model: RawFeatures
    model_key: rawfeatures
    model_plain: RawFeatures
    metric_values:
    - null
    - 0.72
    - 0.7028
    metric_stds:
    - null
    - 0.0003
    - 0.0009
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.72
    sort_std: 0.0003
    true_value: 0.72
    true_std: 0.0003
    paper_value: 0.72
    paper_std: 0.0003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    metric_values:
    - null
    - 0.7184
    - 0.7044
    metric_stds:
    - null
    - 0.0009
    - 0.0003
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    sort_value: 0.7184
    sort_std: 0.0009
    true_value: 0.7184
    true_std: 0.0009
    paper_value: 0.7184
    paper_std: 0.0009
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 11
  - model: GAE
    model_key: gae
    model_plain: GAE
    metric_values:
    - null
    - 0.7017
    - 0.6827
    metric_stds:
    - null
    - 0.0005
    - 0.0005
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.7017
    sort_std: 0.0005
    true_value: 0.7017
    true_std: 0.0005
    paper_value: 0.7017
    paper_std: 0.0005
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.14863'
    value_gap_source_title: Graph Communal Contrastive Learning
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-28'
    value_gap_source_date_label: WWW 2021
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
    published_venue: WWW 2021
    date: Oct 28, 2021
    date_display: Oct 2021
    date_iso: '2021-10-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 12
  metrics:
  - Accuracy
  - Micro-F1
  - Macro-F1
  primary_metric: Accuracy
  rank_metric: Micro-F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Micro-F1
  - Macro-F1
  metric: Micro-F1
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
    - dataset: WikiCS
      dataset_slug: wikics
    - dataset: Coauthor-CS
      dataset_slug: coauthor-cs
---

