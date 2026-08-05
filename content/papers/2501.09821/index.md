---
title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
arxiv_id: '2501.09821'
source_url: ''
authors:
- name: Daniele Castellana
  orcid: null
  s2_author_id: '46201245'
  s2_url: null
- name: Filippo Maria Bianchi
  orcid: null
  s2_author_id: '2320313843'
  s2_url: null
published_date: Jan 16, 2025
published_date_iso: '2025-01-16'
published_venue: TMLR 2025
published_conference: TMLR 2025
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: We introduce BN-Pool, the first clustering-based pooling method for Graph
  Neural Networks that adaptively determines the number of supernodes in a coarsened
  graph. BN-Pool leverages a generative model based on a Bayesian nonparametric framework
  for partitioning graph nodes into an unbounded number of clusters. During training,
  the node-to-cluster assignments are learned by combining the supervised loss of
  the downstream task with an unsupervised auxiliary term, which encourages the reconstruction
  of the original graph topology while penalizing unnecessary proliferation of clusters.
  By automatically discovering the optimal coarsening level for each graph, BN-Pool
  preserves the performance of soft-clustering pooling methods while avoiding their
  typical redundancy by learning compact pooled graphs. The code is available at https://github.com/NGMLGroup/Bayesian-Nonparametric-Graph-Pooling.
codebase_url: https://github.com/NGMLGroup/Bayesian-Nonparametric-Graph-Pooling
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DiffPool
- BN-Pool
- ecpool
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- graph_classification
- node_classification
experiment_scopes:
- graph-level
- node-level
results:
- &id002
  dataset: DBLP
  is_multi_metric: true
  rows:
  - model: DANE-O
    model_key: dane-o
    model_plain: DANE-O
    metric_values:
    - 0.7721
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
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1706.01860'
    title: Attributed Network Embedding for Learning in a Dynamic Environment
    published_venue: ''
    date: Jun 6, 2017
    date_display: Jun 2017
    date_iso: '2017-06-06'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.7721
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
  - model: DANE
    model_key: dane
    model_plain: DANE
    metric_values:
    - 0.7664
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
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '1706.01860'
    title: Attributed Network Embedding for Learning in a Dynamic Environment
    published_venue: ''
    date: Jun 6, 2017
    date_display: Jun 2017
    date_iso: '2017-06-06'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.7664
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
  - model: NE
    model_key: ne
    model_plain: NE
    metric_values:
    - 0.7574
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
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.10866'
    title: Unsupervised Network Embedding Beyond Homophily
    published_venue: ''
    date: Mar 21, 2022
    date_display: Mar 2022
    date_iso: '2022-03-21'
    codebase_url: https://github.com/zhiqiangzhongddu/SELENE
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.7574
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
  - model: BN-Pool
    model_key: bn-pool
    model_plain: BN-Pool
    metric_values:
    - null
    - 0.752
    - 0.585
    metric_stds:
    - null
    - 0.007
    - 0.007
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.752
    sort_std: 0.007
    true_value: 0.752
    true_std: 0.007
    paper_value: 0.752
    paper_std: 0.007
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
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
    published_venue: TMLR 2025
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
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
  - model: MinCut
    model_key: mincut
    model_plain: MinCut
    metric_values:
    - null
    - 0.692
    - 0.525
    metric_stds:
    - null
    - 0.034
    - 0.039
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    sort_value: 0.692
    sort_std: 0.034
    true_value: 0.692
    true_std: 0.034
    paper_value: 0.692
    paper_std: 0.034
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
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
    published_venue: TMLR 2025
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
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
  - model: jbgnn
    model_key: jbgnn
    model_plain: jbgnn
    metric_values:
    - null
    - 0.686
    - 0.53
    metric_stds:
    - null
    - 0.018
    - 0.044
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.686
    sort_std: 0.018
    true_value: 0.686
    true_std: 0.018
    paper_value: 0.686
    paper_std: 0.018
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
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
    published_venue: TMLR 2025
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
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
  - model: DMoN
    model_key: dmon
    model_plain: DMoN
    metric_values:
    - null
    - 0.637
    - 0.454
    metric_stds:
    - null
    - 0.032
    - 0.013
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.637
    sort_std: 0.032
    true_value: 0.637
    true_std: 0.032
    paper_value: 0.637
    paper_std: 0.032
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
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
    published_venue: TMLR 2025
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
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
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    metric_values:
    - null
    - 0.495
    - 0.574
    metric_stds:
    - null
    - 0.049
    - 0.0
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.495
    sort_std: 0.049
    true_value: 0.495
    true_std: 0.049
    paper_value: 0.495
    paper_std: 0.049
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
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
    published_venue: TMLR 2025
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 19
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    metric_values:
    - 0.4868
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
    arxiv_id: '2203.10866'
    title: Unsupervised Network Embedding Beyond Homophily
    published_venue: ''
    date: Mar 21, 2022
    date_display: Mar 2022
    date_iso: '2022-03-21'
    codebase_url: https://github.com/zhiqiangzhongddu/SELENE
    uses_external_data: false
    is_global_top: true
    global_rank: 20
    is_best: false
    sort_value: 0.4868
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
  metrics:
  - Micro-F1
  - ACC
  - COS
  primary_metric: Micro-F1
  rank_metric: ACC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - ACC
  - COS
  metric: ACC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
  dataset: IMDB-BINARY
  rows:
  - model: kmis
    model_key: kmis
    model_plain: kmis
    value: 620.0
    std: 151.0
    paper_value: 620.0
    paper_std: 151.0
    metric: epochs
    higher_is_better: false
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 620.0
    true_std: 151.0
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 620.0
    sort_std: 151.0
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
  - model: DMoN
    model_key: dmon
    model_plain: DMoN
    value: 690.0
    std: 236.0
    paper_value: 690.0
    paper_std: 236.0
    metric: epochs
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 690.0
    true_std: 236.0
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 690.0
    sort_std: 236.0
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: hosc
    model_key: hosc
    model_plain: hosc
    value: 733.0
    std: 306.0
    paper_value: 733.0
    paper_std: 306.0
    metric: epochs
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 733.0
    true_std: 306.0
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 733.0
    sort_std: 306.0
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: topk
    model_key: topk
    model_plain: topk
    value: 760.0
    std: 323.0
    paper_value: 760.0
    paper_std: 323.0
    metric: epochs
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 760.0
    true_std: 323.0
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 760.0
    sort_std: 323.0
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DiffPool
    model_key: diffpool
    model_plain: DiffPool
    value: 771.0
    std: 117.0
    paper_value: 771.0
    paper_std: 117.0
    metric: epochs
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 771.0
    true_std: 117.0
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 771.0
    sort_std: 117.0
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MinCut
    model_key: mincut
    model_plain: MinCut
    value: 788.0
    std: 206.0
    paper_value: 788.0
    paper_std: 206.0
    metric: epochs
    higher_is_better: false
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 788.0
    true_std: 206.0
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 788.0
    sort_std: 206.0
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graclus
    model_key: graclus
    model_plain: Graclus
    value: 791.0
    std: 193.0
    paper_value: 791.0
    paper_std: 193.0
    metric: epochs
    higher_is_better: false
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 791.0
    true_std: 193.0
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 791.0
    sort_std: 193.0
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: jbgnn
    model_key: jbgnn
    model_plain: jbgnn
    value: 830.0
    std: 493.0
    paper_value: 830.0
    paper_std: 493.0
    metric: epochs
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 830.0
    true_std: 493.0
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 830.0
    sort_std: 493.0
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ecpool
    model_key: ecpool
    model_plain: ecpool
    value: 880.0
    std: 242.0
    paper_value: 880.0
    paper_std: 242.0
    metric: epochs
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 880.0
    true_std: 242.0
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 880.0
    sort_std: 242.0
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BN-Pool
    model_key: bn-pool
    model_plain: BN-Pool
    value: 958.0
    std: 133.0
    paper_value: 958.0
    paper_std: 133.0
    metric: epochs
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
    table_ref: Table 6
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Jan 16, 2025
    date_display: Jan 2025
    date_iso: '2025-01-16'
    published_venue: TMLR 2025
    published_conference: TMLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-01-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 958.0
    true_std: 133.0
    value_gap_source_arxiv: '2501.09821'
    value_gap_source_title: 'BN-Pool: Bayesian Nonparametric Pooling for Graphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 958.0
    sort_std: 133.0
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
  rank_metric: epochs
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - epochs
  metric: epochs
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: IMDB-BINARY
      dataset_slug: imdb-binary
main_figure: /figures/2501.09821/main_figure.jpegoptim.jpg
---

