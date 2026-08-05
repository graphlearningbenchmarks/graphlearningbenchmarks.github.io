---
title: 'Partition-wise Graph Filtering: A Unified Perspective Through the Lens of
  Graph Coarsening'
arxiv_id: '2505.14033'
source_url: ''
authors:
- name: Guoming Li
  orcid: null
  s2_author_id: '2295700674'
  s2_url: null
- name: Jian Yang
  orcid: null
  s2_author_id: '2295684729'
  s2_url: null
- name: Yifan Chen
  orcid: null
  s2_author_id: '2346441666'
  s2_url: null
published_date: May 20, 2025
published_date_iso: '2025-05-20'
published_venue: KDD 2025
published_conference: KDD 2025
published_conference_short: KDD
published_conference_slug: kdd
abstract: 'Filtering-based graph neural networks (GNNs) constitute a distinct class
  of GNNs that employ graph filters to handle graph-structured data, achieving notable
  success in various graph-related tasks. Conventional methods adopt a graph-wise
  filtering paradigm, imposing a uniform filter across all nodes, yet recent findings
  suggest that this rigid paradigm struggles with heterophilic graphs. To overcome
  this, recent works have introduced node-wise filtering, which assigns distinct filters
  to individual nodes, offering enhanced adaptability. However, a fundamental gap
  remains: a comprehensive framework unifying these two strategies is still absent,
  limiting theoretical insights into the filtering paradigms. Moreover, through the
  lens of Contextual Stochastic Block Model, we reveal that a synthesis of graph-wise
  and node-wise filtering provides a sufficient solution for classification on graphs
  exhibiting both homophily and heterophily, suggesting the risk of excessive parameterization
  and potential overfitting with node-wise filtering. To address the limitations,
  this paper introduces Coarsening-guided Partition-wise Filtering (CPF). CPF innovates
  by performing filtering on node partitions. The method begins with partition-wise
  filtering, which filters node partitions obtained via graph coarsening algorithms,
  and then performs partition-wise filtering, refining node embeddings via filtering
  on clusters produced by $k$-means clustering over features. In-depth analysis is
  conducted for each phase of CPF, showing its superiority over other paradigms. Finally,
  benchmark node classification experiments, along with a real-world graph anomaly
  detection application, validate CPF''s efficacy and practical utility. Code is available
  with the Github repository:.'
codebase_url: https://github.com/vasile-paskardlgm/CPF
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CPF
mrr: 0.3523
adjusted_mrr: 0.3523
mrr_dataset_count: 3
benchmark_categories:
- Heterophily Benchmark
- LINKX Benchmarks
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Heterophily Benchmark
  benchmark_slug: heterophily-benchmark
  evaluated: 1
  total: 5
- benchmark: LINKX Benchmarks
  benchmark_slug: linkx-benchmarks
  evaluated: 1
  total: 6
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id003
  dataset: Amazon2M
  rows:
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.953
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.08331'
    title: Model Stealing Attacks Against Inductive Graph Neural Networks
    date: Dec 15, 2021
    date_display: Dec 2021
    date_iso: '2021-12-15'
    venue: IEEE Symposium on Security and Privacy
    codebase_url: https://github.com/xinleihe/GNNStealing
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.953
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.937
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.08331'
    title: Model Stealing Attacks Against Inductive Graph Neural Networks
    date: Dec 15, 2021
    date_display: Dec 2021
    date_iso: '2021-12-15'
    venue: IEEE Symposium on Security and Privacy
    codebase_url: https://github.com/xinleihe/GNNStealing
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.937
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.932
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.21151'
    title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    date: Dec 30, 2024
    date_display: Dec 2024
    date_iso: '2024-12-30'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/iDEA-iSAIL-Lab-UIUC/pyg-ssl
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.932
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.4209
    std: 0.006
    paper_value: 0.4209
    paper_std: 0.006
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.8651
    at_pub_std: 0.005
    at_pub_source_arxiv: '2212.07035'
    at_pub_source_title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive
      Learning'
    at_pub_source_date_iso: '2022-12-14'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-12-14'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.4442
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8651
    true_std: 0.005
    value_gap_source_arxiv: '2212.07035'
    value_gap_source_title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.4442
    has_value_note: false
    value_note: ''
    sort_value: 0.8651
    sort_std: 0.005
    global_rank: 18
    paper_rank: 88
    rank_delta: 70
    rank_delta_abs: 70
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive
      Learning'
    comparison_source_arxiv: '2212.07035'
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.856
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.08331'
    title: Model Stealing Attacks Against Inductive Graph Neural Networks
    date: Dec 15, 2021
    date_display: Dec 2021
    date_iso: '2021-12-15'
    venue: IEEE Symposium on Security and Privacy
    codebase_url: https://github.com/xinleihe/GNNStealing
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 20
    sort_value: 0.856
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6346
    std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2602.19622'
    title: 'VecFormer: Towards Efficient and Generalizable Graph Transformer with
      Graph Token Attention'
    date: Feb 23, 2026
    date_display: Feb 2026
    date_iso: '2026-02-23'
    venue: The Web Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 44
    sort_value: 0.6346
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.4219
    std: 0.006
    paper_value: 0.4219
    paper_std: 0.006
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.4988
    at_pub_std: 0.0044
    at_pub_source_arxiv: '2412.19106'
    at_pub_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    at_pub_source_date_iso: '2024-12-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-12-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.07690000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4988
    true_std: 0.0044
    value_gap_source_arxiv: '2412.19106'
    value_gap_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    value_gap_source_is_current_paper: false
    value_gap: 0.07690000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.4988
    sort_std: 0.0044
    global_rank: 52
    paper_rank: 87
    rank_delta: 35
    rank_delta_abs: 35
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    comparison_source_arxiv: '2412.19106'
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.4148
    std: 0.006
    paper_value: 0.4148
    paper_std: 0.006
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.4956
    at_pub_std: 0.0047
    at_pub_source_arxiv: '2412.19106'
    at_pub_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    at_pub_source_date_iso: '2024-12-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-12-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.08079999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4956
    true_std: 0.0047
    value_gap_source_arxiv: '2412.19106'
    value_gap_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    value_gap_source_is_current_paper: false
    value_gap: 0.08079999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.4956
    sort_std: 0.0047
    global_rank: 53
    paper_rank: 92
    rank_delta: 39
    rank_delta_abs: 39
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    comparison_source_arxiv: '2412.19106'
    is_best: false
    is_std_outlier: false
  - model: OptBasis
    model_key: optbasis
    model_plain: OptBasis
    value: 0.4163
    std: 0.008
    paper_value: 0.4163
    paper_std: 0.008
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.4948
    at_pub_std: 0.0036
    at_pub_source_arxiv: '2412.19106'
    at_pub_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    at_pub_source_date_iso: '2024-12-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-12-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.07850000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4948
    true_std: 0.0036
    value_gap_source_arxiv: '2412.19106'
    value_gap_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    value_gap_source_is_current_paper: false
    value_gap: 0.07850000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.4948
    sort_std: 0.0036
    global_rank: 54
    paper_rank: 90
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    comparison_source_arxiv: '2412.19106'
    is_best: false
    is_std_outlier: false
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.4244
    std: 0.009
    paper_value: 0.4244
    paper_std: 0.009
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.4943
    at_pub_std: 0.0041
    at_pub_source_arxiv: '2412.19106'
    at_pub_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    at_pub_source_date_iso: '2024-12-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-12-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.06990000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4943
    true_std: 0.0041
    value_gap_source_arxiv: '2412.19106'
    value_gap_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    value_gap_source_is_current_paper: false
    value_gap: 0.06990000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.4943
    sort_std: 0.0041
    global_rank: 55
    paper_rank: 83
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    comparison_source_arxiv: '2412.19106'
    is_best: false
    is_std_outlier: false
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.4218
    std: 0.004
    paper_value: 0.4218
    paper_std: 0.004
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.4856
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2412.19106'
    at_pub_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    at_pub_source_date_iso: '2024-12-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-12-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.06379999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4856
    true_std: 0.0022
    value_gap_source_arxiv: '2412.19106'
    value_gap_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    value_gap_source_is_current_paper: false
    value_gap: 0.06379999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.4856
    sort_std: 0.0022
    global_rank: 59
    paper_rank: 88
    rank_delta: 29
    rank_delta_abs: 29
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    comparison_source_arxiv: '2412.19106'
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.3717
    std: 0.005
    paper_value: 0.3717
    paper_std: 0.005
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.4652
    at_pub_std: 0.007
    at_pub_source_arxiv: '2412.19106'
    at_pub_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    at_pub_source_date_iso: '2024-12-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-12-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.09350000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4652
    true_std: 0.007
    value_gap_source_arxiv: '2412.19106'
    value_gap_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    value_gap_source_is_current_paper: false
    value_gap: 0.09350000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.4652
    sort_std: 0.007
    global_rank: 64
    paper_rank: 99
    rank_delta: 35
    rank_delta_abs: 35
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    comparison_source_arxiv: '2412.19106'
    is_best: false
    is_std_outlier: false
  - model: CPF
    model_key: cpf
    model_plain: CPF
    value: 0.4612
    std: 0.007
    paper_value: 0.4612
    paper_std: 0.007
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4612
    true_std: 0.007
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4612
    sort_std: 0.007
    global_rank: 66
    paper_rank: 66
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.4089
    std: 0.004
    paper_value: 0.4089
    paper_std: 0.004
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.4362
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2412.19106'
    at_pub_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    at_pub_source_date_iso: '2024-12-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.02729999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4429
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.03400000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.4429
    sort_std: null
    global_rank: 75
    paper_rank: 95
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    comparison_source_arxiv: '2412.19106'
    is_best: false
    is_std_outlier: false
  - model: NIGCN
    model_key: nigcn
    model_plain: NIGCN
    value: 0.4266
    std: 0.004
    paper_value: 0.4266
    paper_std: 0.004
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4266
    true_std: 0.004
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4266
    sort_std: 0.004
    global_rank: 83
    paper_rank: 83
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node-MoE
    model_key: node-moe
    model_plain: Node-MoE
    value: 0.4233
    std: 0.012
    paper_value: 0.4233
    paper_std: 0.012
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4233
    true_std: 0.012
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4233
    sort_std: 0.012
    global_rank: 85
    paper_rank: 85
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AdaptKry
    model_key: adaptkry
    model_plain: AdaptKry
    value: 0.4231
    std: 0.011
    paper_value: 0.4231
    paper_std: 0.011
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4231
    true_std: 0.011
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4231
    sort_std: 0.011
    global_rank: 86
    paper_rank: 86
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NFGNN
    model_key: nfgnn
    model_plain: NFGNN
    value: 0.4219
    std: 0.003
    paper_value: 0.4219
    paper_std: 0.003
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4219
    true_std: 0.003
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4219
    sort_std: 0.003
    global_rank: 88
    paper_rank: 88
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Specformer
    model_key: specformer
    model_plain: Specformer
    value: 0.4206
    std: 0.008
    paper_value: 0.4206
    paper_std: 0.008
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4206
    true_std: 0.008
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4206
    sort_std: 0.008
    global_rank: 90
    paper_rank: 90
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.4157
    std: 0.006
    paper_value: 0.4157
    paper_std: 0.006
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4157
    true_std: 0.006
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4157
    sort_std: 0.006
    global_rank: 91
    paper_rank: 91
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniFilter
    model_key: unifilter
    model_plain: UniFilter
    value: 0.4137
    std: 0.006
    paper_value: 0.4137
    paper_std: 0.006
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4137
    true_std: 0.006
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4137
    sort_std: 0.006
    global_rank: 93
    paper_rank: 93
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OrderGNN
    model_key: ordergnn
    model_plain: OrderGNN
    value: 0.4093
    std: 0.005
    paper_value: 0.4093
    paper_std: 0.005
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4093
    true_std: 0.005
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4093
    sort_std: 0.005
    global_rank: 95
    paper_rank: 95
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ACMGCN
    model_key: acmgcn
    model_plain: ACMGCN
    value: 0.3953
    std: 0.009
    paper_value: 0.3953
    paper_std: 0.009
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3953
    true_std: 0.009
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3953
    sort_std: 0.009
    global_rank: 98
    paper_rank: 98
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.3881
    std: 0.007
    paper_value: 0.3881
    paper_std: 0.007
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.3819
    at_pub_std: 0.0041
    at_pub_source_arxiv: '2412.19106'
    at_pub_source_title: 'ERGNN: Spectral Graph Neural Network With Explicitly-Optimized
      Rational Graph Filters'
    at_pub_source_date_iso: '2024-12-26'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.006199999999999983
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3881
    true_std: 0.007
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3881
    sort_std: 0.007
    global_rank: 99
    paper_rank: 99
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: Questions
  rows:
  - model: GraphSAGE + UniGAP
    model_key: graphsage + unigap
    model_plain: GraphSAGE + UniGAP
    value: 0.8421
    std: 0.008
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8421
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN + UniGAP
    model_key: h2gcn + unigap
    model_plain: H2GCN + UniGAP
    value: 0.8359
    std: 0.007
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.8359
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN + UniGAP
    model_key: gcn + unigap
    model_plain: GCN + UniGAP
    value: 0.8273
    std: 0.009
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8273
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.6442
    std: 0.013
    paper_value: 0.6442
    paper_std: 0.013
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.7928
    at_pub_std: 0.008
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.14859999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7928
    true_std: 0.008
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_gap_source_is_current_paper: false
    value_gap: 0.14859999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.7928
    sort_std: 0.008
    global_rank: 14
    paper_rank: 142
    rank_delta: 128
    rank_delta_abs: 128
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7517
    std: 0.008
    paper_value: 0.7517
    paper_std: 0.008
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.7902
    at_pub_std: 0.006
    at_pub_source_arxiv: '2407.19420'
    at_pub_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    at_pub_source_date_iso: '2024-07-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-28'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03849999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7902
    true_std: 0.006
    value_gap_source_arxiv: '2407.19420'
    value_gap_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    value_gap_source_is_current_paper: false
    value_gap: 0.03849999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.7902
    sort_std: 0.006
    global_rank: 17
    paper_rank: 78
    rank_delta: 61
    rank_delta_abs: 61
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach
      to Mitigate Over-Smoothing in Node Classification Tasks'
    comparison_source_arxiv: '2407.19420'
    is_best: false
    is_std_outlier: false
  - model: CPF
    model_key: cpf
    model_plain: CPF
    value: 0.788
    std: 0.011
    paper_value: 0.788
    paper_std: 0.011
    metric: ROC-AUC
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.788
    true_std: 0.011
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.788
    sort_std: 0.011
    global_rank: 24
    paper_rank: 24
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7721
    std: 0.013
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.19420'
    title: 'UniGAP: A Universal and Adaptive Graph Upsampling Approach to Mitigate
      Over-Smoothing in Node Classification Tasks'
    date: Jul 28, 2024
    date_display: Jul 2024
    date_iso: '2024-07-28'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 48
    sort_value: 0.7721
    sort_std: 0.013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NIGCN
    model_key: nigcn
    model_plain: NIGCN
    value: 0.7568
    std: 0.008
    paper_value: 0.7568
    paper_std: 0.008
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7568
    true_std: 0.008
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7568
    sort_std: 0.008
    global_rank: 70
    paper_rank: 70
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NFGNN
    model_key: nfgnn
    model_plain: NFGNN
    value: 0.7549
    std: 0.009
    paper_value: 0.7549
    paper_std: 0.009
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7549
    true_std: 0.009
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7549
    sort_std: 0.009
    global_rank: 76
    paper_rank: 76
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node-MoE
    model_key: node-moe
    model_plain: Node-MoE
    value: 0.7446
    std: 0.012
    paper_value: 0.7446
    paper_std: 0.012
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7446
    true_std: 0.012
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7446
    sort_std: 0.012
    global_rank: 85
    paper_rank: 85
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.7442
    std: 0.013
    paper_value: 0.7442
    paper_std: 0.013
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.6715
    at_pub_std: 0.0192
    at_pub_source_arxiv: '2411.05274'
    at_pub_source_title: Distributed-Order Fractional Graph Operating Network
    at_pub_source_date_iso: '2024-11-08'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.07269999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7442
    true_std: 0.013
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7442
    sort_std: 0.013
    global_rank: 86
    paper_rank: 86
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Distributed-Order Fractional Graph Operating Network
    comparison_source_arxiv: '2411.05274'
    is_best: false
    is_std_outlier: false
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.7216
    std: 0.013
    paper_value: 0.7216
    paper_std: 0.013
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.7388
    at_pub_std: 0.0116
    at_pub_source_arxiv: '2306.12943'
    at_pub_source_title: Evolving Computation Graphs
    at_pub_source_date_iso: '2023-06-22'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2025-08-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.017199999999999993
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7388
    true_std: 0.0116
    value_gap_source_arxiv: '2508.05070'
    value_gap_source_title: 'TANGO: Graph Neural Dynamics via Learned Energy and Tangential
      Flows'
    value_gap_source_is_current_paper: false
    value_gap: 0.017199999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.7388
    sort_std: 0.0116
    global_rank: 90
    paper_rank: 96
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniFilter
    model_key: unifilter
    model_plain: UniFilter
    value: 0.7383
    std: 0.008
    paper_value: 0.7383
    paper_std: 0.008
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7383
    true_std: 0.008
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7383
    sort_std: 0.008
    global_rank: 91
    paper_rank: 91
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AdaptKry
    model_key: adaptkry
    model_plain: AdaptKry
    value: 0.7255
    std: 0.01
    paper_value: 0.7255
    paper_std: 0.01
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7255
    true_std: 0.01
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7255
    sort_std: 0.01
    global_rank: 95
    paper_rank: 95
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.7232
    std: 0.01
    paper_value: 0.7232
    paper_std: 0.01
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7232
    true_std: 0.01
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7232
    sort_std: 0.01
    global_rank: 96
    paper_rank: 96
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.7128
    std: 0.006
    paper_value: 0.7128
    paper_std: 0.006
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7128
    true_std: 0.006
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7128
    sort_std: 0.006
    global_rank: 99
    paper_rank: 99
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OrderGNN
    model_key: ordergnn
    model_plain: OrderGNN
    value: 0.7082
    std: 0.01
    paper_value: 0.7082
    paper_std: 0.01
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7082
    true_std: 0.01
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7082
    sort_std: 0.01
    global_rank: 105
    paper_rank: 105
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7082
    std: 0.001
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2508.17531'
    title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    date: Aug 24, 2025
    date_display: Aug 2025
    date_iso: '2025-08-24'
    venue: European Conference on Artificial Intelligence
    codebase_url: https://github.com/Bobowner/Gumbel-Softmax-MPNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 104
    sort_value: 0.7082
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Specformer
    model_key: specformer
    model_plain: Specformer
    value: 0.7075
    std: 0.012
    paper_value: 0.7075
    paper_std: 0.012
    metric: ROC-AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7075
    true_std: 0.012
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7075
    sort_std: 0.012
    global_rank: 108
    paper_rank: 108
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.7042
    std: 0.012
    paper_value: 0.7042
    paper_std: 0.012
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7042
    true_std: 0.012
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7042
    sort_std: 0.012
    global_rank: 111
    paper_rank: 111
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: OptBasis
    model_key: optbasis
    model_plain: OptBasis
    value: 0.696
    std: 0.012
    paper_value: 0.696
    paper_std: 0.012
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.696
    true_std: 0.012
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.696
    sort_std: 0.012
    global_rank: 121
    paper_rank: 121
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ACMGCN
    model_key: acmgcn
    model_plain: ACMGCN
    value: 0.6784
    std: 0.005
    paper_value: 0.6784
    paper_std: 0.005
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6784
    true_std: 0.005
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6784
    sort_std: 0.005
    global_rank: 131
    paper_rank: 131
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.6458
    std: 0.012
    paper_value: 0.6458
    paper_std: 0.012
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.5548
    at_pub_std: 0.0091
    at_pub_source_arxiv: '2403.01232'
    at_pub_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in Linear
      Time'
    at_pub_source_date_iso: '2024-03-02'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.09100000000000008
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6458
    true_std: 0.012
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6458
    sort_std: 0.012
    global_rank: 141
    paper_rank: 141
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer
      in Linear Time'
    comparison_source_arxiv: '2403.01232'
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.6385
    std: 0.008
    paper_value: 0.6385
    paper_std: 0.008
    metric: ROC-AUC
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
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6385
    true_std: 0.008
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6385
    sort_std: 0.008
    global_rank: 145
    paper_rank: 145
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: ROC-AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - ROC-AUC
  metric: ROC-AUC
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: twitch-gamers
  rows:
  - model: CPF
    model_key: cpf
    model_plain: CPF
    value: 0.6977
    std: 0.003
    paper_value: 0.6977
    paper_std: 0.003
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6977
    true_std: 0.003
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6977
    sort_std: 0.003
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
  - model: Polynormer + Wideformer
    model_key: polynormer + wideformer
    model_plain: Polynormer + Wideformer
    value: 0.6733
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.6733
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Polynormer
    model_key: polynormer
    model_plain: Polynormer
    value: 0.6715
    std: 0.0003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2510.21267'
    title: Relieving the Over-Aggregating Effect in Graph Transformers
    date: Oct 24, 2025
    date_display: Oct 2025
    date_iso: '2025-10-24'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/sunjss/over-aggregating
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.6715
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NFGNN
    model_key: nfgnn
    model_plain: NFGNN
    value: 0.6685
    std: 0.004
    paper_value: 0.6685
    paper_std: 0.004
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6685
    true_std: 0.004
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6685
    sort_std: 0.004
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
  - model: OptBasis
    model_key: optbasis
    model_plain: OptBasis
    value: 0.6681
    std: 0.004
    paper_value: 0.6681
    paper_std: 0.004
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6681
    true_std: 0.004
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6681
    sort_std: 0.004
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
  - model: NIGCN
    model_key: nigcn
    model_plain: NIGCN
    value: 0.6672
    std: 0.005
    paper_value: 0.6672
    paper_std: 0.005
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6672
    true_std: 0.005
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6672
    sort_std: 0.005
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
  - model: ChebNetII
    model_key: chebnetii
    model_plain: ChebNetII
    value: 0.6644
    std: 0.005
    paper_value: 0.6644
    paper_std: 0.005
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.6503
    at_pub_std: 0.0027
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.014100000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6644
    true_std: 0.005
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6644
    sort_std: 0.005
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: false
    is_std_outlier: false
  - model: Node-MoE
    model_key: node-moe
    model_plain: Node-MoE
    value: 0.6642
    std: 0.002
    paper_value: 0.6642
    paper_std: 0.002
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6642
    true_std: 0.002
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6642
    sort_std: 0.002
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GloGNN
    model_key: glognn
    model_plain: GloGNN
    value: 0.6562
    std: 0.003
    paper_value: 0.6562
    paper_std: 0.003
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.664
    at_pub_std: 0.003
    at_pub_source_arxiv: '2303.06344'
    at_pub_source_title: Graph Contrastive Learning under Heterophily via Graph Filters
    at_pub_source_date_iso: '2023-03-11'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-11'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.007800000000000029
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.664
    true_std: 0.003
    value_gap_source_arxiv: '2303.06344'
    value_gap_source_title: Graph Contrastive Learning under Heterophily via Graph
      Filters
    value_gap_source_is_current_paper: false
    value_gap: 0.007800000000000029
    has_value_note: false
    value_note: ''
    sort_value: 0.664
    sort_std: 0.003
    global_rank: 10
    paper_rank: 24
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning under Heterophily via Graph
      Filters
    comparison_source_arxiv: '2303.06344'
    is_best: false
    is_std_outlier: false
  - model: AdaptKry
    model_key: adaptkry
    model_plain: AdaptKry
    value: 0.6627
    std: 0.003
    paper_value: 0.6627
    paper_std: 0.003
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6627
    true_std: 0.003
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6627
    sort_std: 0.003
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPRGNN
    model_key: gprgnn
    model_plain: GPRGNN
    value: 0.6623
    std: 0.001
    paper_value: 0.6623
    paper_std: 0.001
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.6259
    at_pub_std: 0.004
    at_pub_source_arxiv: '2406.01249'
    at_pub_source_title: Equivariant Machine Learning on Graphs with Nonlinear Spectral
      Filters
    at_pub_source_date_iso: '2024-06-03'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.03639999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6623
    true_std: 0.001
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6623
    sort_std: 0.001
    global_rank: 13
    paper_rank: 13
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Equivariant Machine Learning on Graphs with Nonlinear
      Spectral Filters
    comparison_source_arxiv: '2406.01249'
    is_best: false
    is_std_outlier: false
  - model: OrderGNN
    model_key: ordergnn
    model_plain: OrderGNN
    value: 0.6609
    std: 0.003
    paper_value: 0.6609
    paper_std: 0.003
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6609
    true_std: 0.003
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6609
    sort_std: 0.003
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.6582
    std: 0.004
    paper_value: 0.6582
    paper_std: 0.004
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.6606
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2024-06-03'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.0023999999999999577
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6606
    true_std: 0.002
    value_gap_source_arxiv: '2406.01249'
    value_gap_source_title: Equivariant Machine Learning on Graphs with Nonlinear
      Spectral Filters
    value_gap_source_is_current_paper: false
    value_gap: 0.0023999999999999577
    has_value_note: false
    value_note: ''
    sort_value: 0.6606
    sort_std: 0.002
    global_rank: 17
    paper_rank: 20
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Specformer
    model_key: specformer
    model_plain: Specformer
    value: 0.658
    std: 0.002
    paper_value: 0.658
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.658
    true_std: 0.002
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.658
    sort_std: 0.002
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniFilter
    model_key: unifilter
    model_plain: UniFilter
    value: 0.6575
    std: 0.004
    paper_value: 0.6575
    paper_std: 0.004
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6575
    true_std: 0.004
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6575
    sort_std: 0.004
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.6471
    std: 0.004
    paper_value: 0.6471
    paper_std: 0.004
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.657
    at_pub_std: 0.002
    at_pub_source_arxiv: '2311.05185'
    at_pub_source_title: Mixture of Weak & Strong Experts on Graphs
    at_pub_source_date_iso: '2023-11-09'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2023-11-09'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.00990000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.657
    true_std: 0.002
    value_gap_source_arxiv: '2311.05185'
    value_gap_source_title: Mixture of Weak & Strong Experts on Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.00990000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.657
    sort_std: 0.002
    global_rank: 23
    paper_rank: 36
    rank_delta: 13
    rank_delta_abs: 13
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Mixture of Weak & Strong Experts on Graphs
    comparison_source_arxiv: '2311.05185'
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.6511
    std: 0.003
    paper_value: 0.6511
    paper_std: 0.003
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.6339
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.017199999999999993
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6511
    true_std: 0.003
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6511
    sort_std: 0.003
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: false
    is_std_outlier: false
  - model: ACMGCN
    model_key: acmgcn
    model_plain: ACMGCN
    value: 0.6473
    std: 0.003
    paper_value: 0.6473
    paper_std: 0.003
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6473
    true_std: 0.003
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6473
    sort_std: 0.003
    global_rank: 36
    paper_rank: 36
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.6473
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 35
    sort_value: 0.6473
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6329
    std: 0.005
    paper_value: 0.6329
    paper_std: 0.005
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.6456
    at_pub_std: 0.0019
    at_pub_source_arxiv: '2408.07191'
    at_pub_source_title: Joint Graph Rewiring and Feature Denoising via Spectral Resonance
    at_pub_source_date_iso: '2024-08-13'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2024-08-13'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.012699999999999934
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6456
    true_std: 0.0019
    value_gap_source_arxiv: '2408.07191'
    value_gap_source_title: Joint Graph Rewiring and Feature Denoising via Spectral
      Resonance
    value_gap_source_is_current_paper: false
    value_gap: 0.012699999999999934
    has_value_note: false
    value_note: ''
    sort_value: 0.6456
    sort_std: 0.0019
    global_rank: 38
    paper_rank: 48
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Joint Graph Rewiring and Feature Denoising via Spectral
      Resonance
    comparison_source_arxiv: '2408.07191'
    is_best: false
    is_std_outlier: false
  - model: JacobiConv
    model_key: jacobiconv
    model_plain: JacobiConv
    value: 0.6417
    std: 0.003
    paper_value: 0.6417
    paper_std: 0.003
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6417
    true_std: 0.003
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6417
    sort_std: 0.003
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.6362
    std: 0.004
    paper_value: 0.6362
    paper_std: 0.004
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on heterophilic graphs
    date: May 20, 2025
    date_display: May 2025
    date_iso: '2025-05-20'
    published_venue: KDD 2025
    published_conference: KDD 2025
    at_pub_value: 0.6231
    at_pub_std: 0.0037
    at_pub_source_arxiv: '2202.03580'
    at_pub_source_title: Convolutional Neural Networks on Graphs with Chebyshev Approximation,
      Revisited
    at_pub_source_date_iso: '2022-02-04'
    at_pub_source_date_label: NeurIPS 2022
    value_gap_source_date_iso: '2025-05-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.0131
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6362
    true_std: 0.004
    value_gap_source_arxiv: '2505.14033'
    value_gap_source_title: 'Partition-wise Graph Filtering: A Unified Perspective
      Through the Lens of Graph Coarsening'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6362
    sort_std: 0.004
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    comparison_source_arxiv: '2202.03580'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6114
    std: 0.0006
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2206.14337'
    title: Deformable Graph Transformer
    date: Jun 29, 2022
    date_display: Jun 2022
    date_iso: '2022-06-29'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 59
    sort_value: 0.6114
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: Heterophily Benchmark
  datasets:
  - *id001
- benchmark: LINKX Benchmarks
  datasets:
  - *id002
- benchmark: Other Graph Benchmarks
  datasets:
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophily Benchmark
    benchmark_slug: heterophily-benchmark
    datasets:
    - dataset: Questions
      dataset_slug: questions
  - benchmark: LINKX Benchmarks
    benchmark_slug: linkx-benchmarks
    datasets:
    - dataset: twitch-gamers
      dataset_slug: twitch-gamers
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: Amazon2M
      dataset_slug: amazon2m
single_proposed_model: CPF
main_figure: /figures/2505.14033/main_figure.jpegoptim.jpg
---

