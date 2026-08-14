---
title: Reinforcement Graph Clustering with Unknown Cluster Number
arxiv_id: '2308.06827'
source_url: ''
authors:
- name: Yue Liu
  orcid: null
  s2_author_id: '2119034129'
  s2_url: null
- name: K. Liang
  orcid: null
  s2_author_id: '2024445866'
  s2_url: null
- name: Jun Xia
  orcid: null
  s2_author_id: '2069551655'
  s2_url: null
- name: Xihong Yang
  orcid: null
  s2_author_id: '2154476091'
  s2_url: null
- name: Sihang Zhou
  orcid: null
  s2_author_id: '2516087'
  s2_url: null
- name: Meng Liu
  orcid: null
  s2_author_id: '2152969291'
  s2_url: null
- name: Xinwang Liu
  orcid: null
  s2_author_id: '2130021053'
  s2_url: null
- name: Stan Z. Li
  orcid: null
  s2_author_id: '1390908654'
  s2_url: null
published_date: Aug 13, 2023
published_date_iso: '2023-08-13'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Deep graph clustering, which aims to group nodes into disjoint clusters
  by neural networks in an unsupervised manner, has attracted great attention in recent
  years. Although the performance has been largely improved, the excellent performance
  of the existing methods heavily relies on an accurately predefined cluster number,
  which is not always available in the real-world scenario. To enable the deep graph
  clustering algorithms to work without the guidance of the predefined cluster number,
  we propose a new deep graph clustering method termed Reinforcement Graph Clustering
  (RGC). In our proposed method, cluster number determination and unsupervised representation
  learning are unified into a uniform framework by the reinforcement learning mechanism.
  Concretely, the discriminative node representations are first learned with the contrastive
  pretext task. Then, to capture the clustering state accurately with both local and
  global information in the graph, both node and cluster states are considered. Subsequently,
  at each state, the qualities of different cluster numbers are evaluated by the quality
  network, and the greedy action is executed to determine the cluster number. In order
  to conduct feedback actions, the clustering-oriented reward function is proposed
  to enhance the cohesion of the same clusters and separate the different clusters.
  Extensive experiments demonstrate the effectiveness and efficiency of our proposed
  method. The source code of RGC is shared at https://github.com/yueliu1999/RGC and
  a collection (papers, codes and, datasets) of deep graph clustering is shared at
  https://github.com/yueliu1999/Awesome-Deep-Graph-Clustering on Github.
codebase_url: https://github.com/yueliu1999/RGC
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- RGC
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Hypergraph Benchmarks
benchmark_coverage:
- benchmark: Hypergraph Benchmarks
  benchmark_slug: hypergraph-benchmarks
  evaluated: 2
  total: 10
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: AMAP
  is_multi_metric: true
  rows:
  - model: DCRN
    model_key: dcrn
    model_plain: DCRN
    metric_values:
    - 0.737
    - null
    - null
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
    arxiv_id: '2403.03666'
    title: Provable Filter for Real-world Graph Clustering
    published_venue: ''
    date: Mar 6, 2024
    date_display: Mar 2024
    date_iso: '2024-03-06'
    codebase_url: https://github.com/XieXuanting/PFGC
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.737
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: two unsupervised strategies
    model_key: two unsupervised strategies
    model_plain: two unsupervised strategies
    metric_values:
    - 0.7081
    - null
    - null
    metric_stds:
    - 0.0074
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2403.03666'
    title: Provable Filter for Real-world Graph Clustering
    published_venue: ''
    date: Mar 6, 2024
    date_display: Mar 2024
    date_iso: '2024-03-06'
    codebase_url: https://github.com/XieXuanting/PFGC
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.7081
    sort_std: 0.0074
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: AMLP
    model_key: amlp
    model_plain: AMLP
    metric_values:
    - 0.6977
    - null
    - null
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
    arxiv_id: '2507.20127'
    title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph Message-passing'
    published_venue: ''
    date: Jul 27, 2025
    date_display: Jul 2025
    date_iso: '2025-07-27'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.6977
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: RGC
    model_key: rgc
    model_plain: RGC
    metric_values:
    - null
    - 0.6961
    - 0.5958
    metric_stds:
    - null
    - 0.0036
    - 0.0039
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.6961
    sort_std: 0.0036
    true_value: 0.6961
    true_std: 0.0036
    paper_value: 0.6961
    paper_std: 0.0036
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    metric_values:
    - null
    - 0.6623
    - 0.5828
    metric_stds:
    - null
    - 0.0121
    - 0.0074
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6921
    sort_std: null
    true_value: 0.6921
    true_std: null
    paper_value: 0.6623
    paper_std: 0.0121
    has_value_gap: true
    has_value_note: false
    value_gap: 0.02980000000000005
    value_gap_source_arxiv: '2507.20127'
    value_gap_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-07-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: AGC-DRR
    model_key: agc-drr
    model_plain: AGC-DRR
    metric_values:
    - null
    - 0.6654
    - 0.6015
    metric_stds:
    - null
    - 0.0124
    - 0.0156
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6654
    sort_std: 0.0124
    true_value: 0.6654
    true_std: 0.0124
    paper_value: 0.6654
    paper_std: 0.0124
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: AGE
    model_key: age
    model_plain: AGE
    metric_values:
    - null
    - 0.6538
    - 0.5589
    metric_stds:
    - null
    - 0.0061
    - 0.0134
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6538
    sort_std: 0.0061
    true_value: 0.6538
    true_std: 0.0061
    paper_value: 0.6538
    paper_std: 0.0061
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    metric_values:
    - null
    - 0.6525
    - 0.5812
    metric_stds:
    - null
    - 0.0045
    - 0.0024
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6525
    sort_std: 0.0045
    true_value: 0.6525
    true_std: 0.0045
    paper_value: 0.6525
    paper_std: 0.0045
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    metric_values:
    - null
    - 0.6405
    - 0.5445
    metric_stds:
    - null
    - 0.0015
    - 0.0048
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6405
    sort_std: 0.0015
    true_value: 0.6405
    true_std: 0.0015
    paper_value: 0.6405
    paper_std: 0.0015
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 13
  - model: MGAE
    model_key: mgae
    model_plain: MGAE
    metric_values:
    - null
    - 0.6213
    - 0.4882
    metric_stds:
    - null
    - 0.0279
    - 0.0457
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6213
    sort_std: 0.0279
    true_value: 0.6213
    true_std: 0.0279
    paper_value: 0.6213
    paper_std: 0.0279
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    metric_values:
    - null
    - 0.0637
    - 0.0536
    metric_stds:
    - null
    - 0.0189
    - 0.0214
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.6
    sort_std: 0.04
    true_value: 0.6
    true_std: 0.04
    paper_value: 0.0637
    paper_std: 0.0189
    has_value_gap: true
    has_value_note: false
    value_gap: 0.5363
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 20
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    metric_values:
    - null
    - 0.5836
    - 0.4418
    metric_stds:
    - null
    - 0.0276
    - 0.0441
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5836
    sort_std: 0.0276
    true_value: 0.5836
    true_std: 0.0276
    paper_value: 0.5836
    paper_std: 0.0276
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 22
  - model: AdaGAE
    model_key: adagae
    model_plain: AdaGAE
    metric_values:
    - null
    - 0.5596
    - 0.462
    metric_stds:
    - null
    - 0.0087
    - 0.0045
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.5596
    sort_std: 0.0087
    true_value: 0.5596
    true_std: 0.0087
    paper_value: 0.5596
    paper_std: 0.0087
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 23
  - model: AutoSSL
    model_key: autossl
    model_plain: AutoSSL
    metric_values:
    - null
    - 0.4856
    - 0.2687
    metric_stds:
    - null
    - 0.0071
    - 0.0034
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4856
    sort_std: 0.0071
    true_value: 0.4856
    true_std: 0.0071
    paper_value: 0.4856
    paper_std: 0.0071
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 27
  - model: GCA
    model_key: gca
    model_plain: GCA
    metric_values:
    - null
    - 0.4838
    - 0.2685
    metric_stds:
    - null
    - 0.0238
    - 0.0044
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4838
    sort_std: 0.0238
    true_value: 0.4838
    true_std: 0.0238
    paper_value: 0.4838
    paper_std: 0.0238
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 28
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    metric_values:
    - null
    - 0.4485
    - 0.3121
    metric_stds:
    - null
    - 0.0083
    - 0.0123
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4485
    sort_std: null
    true_value: 0.4485
    true_std: null
    paper_value: 0.4485
    paper_std: 0.0083
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2507.20127'
    value_gap_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-07-27'
    value_gap_source_date_label: '2025'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 29
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    metric_values:
    - null
    - 0.3956
    - 0.3418
    metric_stds:
    - null
    - 0.0039
    - 0.0089
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3956
    sort_std: 0.0039
    true_value: 0.3956
    true_std: 0.0039
    paper_value: 0.3956
    paper_std: 0.0039
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 30
  - model: DCN
    model_key: dcn
    model_plain: DCN
    metric_values:
    - null
    - 0.3876
    - 0.208
    metric_stds:
    - null
    - 0.003
    - 0.0047
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3876
    sort_std: 0.003
    true_value: 0.3876
    true_std: 0.003
    paper_value: 0.3876
    paper_std: 0.003
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 31
  - model: IDEC
    model_key: idec
    model_plain: IDEC
    metric_values:
    - null
    - 0.3783
    - 0.1924
    metric_stds:
    - null
    - 0.0008
    - 0.0007
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.3783
    sort_std: 0.0008
    true_value: 0.3783
    true_std: 0.0008
    paper_value: 0.3783
    paper_std: 0.0008
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 32
  - model: DEC
    model_key: dec
    model_plain: DEC
    metric_values:
    - null
    - 0.3735
    - 0.1859
    metric_stds:
    - null
    - 0.0005
    - 0.0004
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3735
    sort_std: 0.0005
    true_value: 0.3735
    true_std: 0.0005
    paper_value: 0.3735
    paper_std: 0.0005
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 33
  - model: GDCL
    model_key: gdcl
    model_plain: GDCL
    metric_values:
    - null
    - 0.3732
    - 0.2157
    metric_stds:
    - null
    - 0.0028
    - 0.0051
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3732
    sort_std: 0.0028
    true_value: 0.3732
    true_std: 0.0028
    paper_value: 0.3732
    paper_std: 0.0028
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 34
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - null
    - 0.3028
    - 0.1877
    metric_stds:
    - null
    - 0.0394
    - 0.0234
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3689
    sort_std: null
    true_value: 0.3689
    true_std: null
    paper_value: 0.3028
    paper_std: 0.0394
    has_value_gap: true
    has_value_note: false
    value_gap: 0.06609999999999999
    value_gap_source_arxiv: '2507.20127'
    value_gap_source_title: 'Aggregation-aware MLP: An Unsupervised Approach for Graph
      Message-passing'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-07-27'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 35
  metrics:
  - Accuracy
  - NMI
  - ARI
  primary_metric: Accuracy
  rank_metric: NMI
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - NMI
  - ARI
  metric: NMI
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id002
  dataset: BAT
  is_multi_metric: true
  rows:
  - model: RGC
    model_key: rgc
    model_plain: RGC
    metric_values:
    - null
    - 0.5158
    - 0.4716
    metric_stds:
    - null
    - 0.0083
    - 0.0135
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.5158
    sort_std: 0.0083
    true_value: 0.5158
    true_std: 0.0083
    paper_value: 0.5158
    paper_std: 0.0083
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: ARGA
    model_key: arga
    model_plain: ARGA
    metric_values:
    - null
    - 0.4909
    - 0.4202
    metric_stds:
    - null
    - 0.0054
    - 0.0121
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4909
    sort_std: 0.0054
    true_value: 0.4909
    true_std: 0.0054
    paper_value: 0.4909
    paper_std: 0.0054
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: DFCN
    model_key: dfcn
    model_plain: DFCN
    metric_values:
    - null
    - 0.4877
    - 0.3776
    metric_stds:
    - null
    - 0.0051
    - 0.0023
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4877
    sort_std: 0.0051
    true_value: 0.4877
    true_std: 0.0051
    paper_value: 0.4877
    paper_std: 0.0051
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: DCRN
    model_key: dcrn
    model_plain: DCRN
    metric_values:
    - null
    - 0.4723
    - 0.3976
    metric_stds:
    - null
    - 0.0074
    - 0.0087
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.4723
    sort_std: 0.0074
    true_value: 0.4723
    true_std: 0.0074
    paper_value: 0.4723
    paper_std: 0.0074
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: GCA
    model_key: gca
    model_plain: GCA
    metric_values:
    - null
    - 0.3888
    - 0.2669
    metric_stds:
    - null
    - 0.0023
    - 0.0285
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3888
    sort_std: 0.0023
    true_value: 0.3888
    true_std: 0.0023
    paper_value: 0.3888
    paper_std: 0.0023
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: AGE
    model_key: age
    model_plain: AGE
    metric_values:
    - null
    - 0.3604
    - 0.2659
    metric_stds:
    - null
    - 0.0154
    - 0.0183
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3604
    sort_std: 0.0154
    true_value: 0.3604
    true_std: 0.0154
    paper_value: 0.3604
    paper_std: 0.0154
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: GDCL
    model_key: gdcl
    model_plain: GDCL
    metric_values:
    - null
    - 0.317
    - 0.1933
    metric_stds:
    - null
    - 0.0042
    - 0.0057
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.317
    sort_std: 0.0042
    true_value: 0.317
    true_std: 0.0042
    paper_value: 0.317
    paper_std: 0.0042
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    metric_values:
    - null
    - 0.2933
    - 0.1345
    metric_stds:
    - null
    - 0.007
    - 0.0003
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.31
    sort_std: 0.07
    true_value: 0.31
    true_std: 0.07
    paper_value: 0.2933
    paper_std: 0.007
    has_value_gap: true
    has_value_note: false
    value_gap: 0.016699999999999993
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: MGAE
    model_key: mgae
    model_plain: MGAE
    metric_values:
    - null
    - 0.3059
    - 0.2415
    metric_stds:
    - null
    - 0.0206
    - 0.017
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.3059
    sort_std: 0.0206
    true_value: 0.3059
    true_std: 0.0206
    paper_value: 0.3059
    paper_std: 0.0206
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: ProGCL
    model_key: progcl
    model_plain: ProGCL
    metric_values:
    - null
    - 0.2869
    - 0.2184
    metric_stds:
    - null
    - 0.0092
    - 0.0134
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.2869
    sort_std: 0.0092
    true_value: 0.2869
    true_std: 0.0092
    paper_value: 0.2869
    paper_std: 0.0092
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 13
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    metric_values:
    - null
    - 0.2755
    - 0.2189
    metric_stds:
    - null
    - 0.0062
    - 0.0074
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.2755
    sort_std: 0.0062
    true_value: 0.2755
    true_std: 0.0062
    paper_value: 0.2755
    paper_std: 0.0062
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 14
  - model: SUBLIME
    model_key: sublime
    model_plain: SUBLIME
    metric_values:
    - null
    - 0.2203
    - 0.1445
    metric_stds:
    - null
    - 0.0048
    - 0.0087
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.27
    sort_std: 0.05
    true_value: 0.27
    true_std: 0.05
    paper_value: 0.2203
    paper_std: 0.0048
    has_value_gap: true
    has_value_note: false
    value_gap: 0.04970000000000002
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
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
  - model: SDCN
    model_key: sdcn
    model_plain: SDCN
    metric_values:
    - null
    - 0.2574
    - 0.2104
    metric_stds:
    - null
    - 0.0571
    - 0.0497
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.2574
    sort_std: 0.0571
    true_value: 0.2574
    true_std: 0.0571
    paper_value: 0.2574
    paper_std: 0.0571
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 16
  - model: DAEGC
    model_key: daegc
    model_plain: DAEGC
    metric_values:
    - null
    - 0.2143
    - 0.1818
    metric_stds:
    - null
    - 0.0035
    - 0.0029
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.25
    sort_std: 0.04
    true_value: 0.25
    true_std: 0.04
    paper_value: 0.2143
    paper_std: 0.0035
    has_value_gap: true
    has_value_note: false
    value_gap: 0.03570000000000001
    value_gap_source_arxiv: '2508.14097'
    value_gap_source_title: Non-Dissipative Graph Propagation for Non-Local Community
      Detection
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-30'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 17
  - model: MCGC
    model_key: mcgc
    model_plain: MCGC
    metric_values:
    - null
    - 0.2311
    - 0.0841
    metric_stds:
    - null
    - 0.0056
    - 0.0032
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.2311
    sort_std: 0.0056
    true_value: 0.2311
    true_std: 0.0056
    paper_value: 0.2311
    paper_std: 0.0056
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 18
  - model: AGC-DRR
    model_key: agc-drr
    model_plain: AGC-DRR
    metric_values:
    - null
    - 0.1991
    - 0.1459
    metric_stds:
    - null
    - 0.0024
    - 0.0013
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.1991
    sort_std: 0.0024
    true_value: 0.1991
    true_std: 0.0024
    paper_value: 0.1991
    paper_std: 0.0024
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 20
  - model: DCN
    model_key: dcn
    model_plain: DCN
    metric_values:
    - null
    - 0.1803
    - 0.1375
    metric_stds:
    - null
    - 0.0773
    - 0.0605
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.1803
    sort_std: 0.0773
    true_value: 0.1803
    true_std: 0.0773
    paper_value: 0.1803
    paper_std: 0.0773
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 21
  - model: AutoSSL
    model_key: autossl
    model_plain: AutoSSL
    metric_values:
    - null
    - 0.1784
    - 0.1311
    metric_stds:
    - null
    - 0.0098
    - 0.0081
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.1784
    sort_std: 0.0098
    true_value: 0.1784
    true_std: 0.0098
    paper_value: 0.1784
    paper_std: 0.0098
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 22
  - model: AdaGAE
    model_key: adagae
    model_plain: AdaGAE
    metric_values:
    - null
    - 0.1584
    - 0.078
    metric_stds:
    - null
    - 0.0078
    - 0.0041
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.1584
    sort_std: 0.0078
    true_value: 0.1584
    true_std: 0.0078
    paper_value: 0.1584
    paper_std: 0.0078
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 23
  - model: DEC
    model_key: dec
    model_plain: DEC
    metric_values:
    - null
    - 0.141
    - 0.0799
    metric_stds:
    - null
    - 0.0199
    - 0.0121
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.141
    sort_std: 0.0199
    true_value: 0.141
    true_std: 0.0199
    paper_value: 0.141
    paper_std: 0.0199
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 25
  - model: IDEC
    model_key: idec
    model_plain: IDEC
    metric_values:
    - null
    - 0.128
    - 0.0785
    metric_stds:
    - null
    - 0.0174
    - 0.0131
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.128
    sort_std: 0.0174
    true_value: 0.128
    true_std: 0.0174
    paper_value: 0.128
    paper_std: 0.0174
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2308.06827'
    value_gap_source_title: Reinforcement Graph Clustering with Unknown Cluster Number
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-08-13'
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
    date: Aug 13, 2023
    date_display: Aug 2023
    date_iso: '2023-08-13'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 26
  metrics:
  - F1
  - NMI
  - ARI
  primary_metric: F1
  rank_metric: NMI
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - NMI
  - ARI
  metric: NMI
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Hypergraph Benchmarks
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Hypergraph Benchmarks
    benchmark_slug: hypergraph-benchmarks
    datasets:
    - dataset: AMAP
      dataset_slug: amap
    - dataset: BAT
      dataset_slug: bat
single_proposed_model: RGC
main_figure: /figures/2308.06827/main_figure.jpegoptim.jpg
---

