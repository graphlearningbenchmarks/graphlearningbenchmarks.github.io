---
title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
arxiv_id: '2411.01157'
source_url: ''
authors:
- name: Yunhui Liu
  orcid: null
  s2_author_id: '2313929373'
  s2_url: null
- name: Tieke He
  orcid: null
  s2_author_id: '2278776738'
  s2_url: null
- name: Tao Zheng
  orcid: null
  s2_author_id: '2313993478'
  s2_url: null
- name: Jianhua Zhao
  orcid: null
  s2_author_id: '2314168612'
  s2_url: null
published_date: Oct 1, 2024
published_date_iso: '2024-10-01'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph Contrastive Learning (GCL) has recently emerged as a promising graph
  self-supervised learning framework for learning discriminative node representations
  without labels. The widely adopted objective function of GCL benefits from two key
  properties: alignment and uniformity, which align representations of positive node
  pairs while uniformly distributing all representations on the hypersphere. The uniformity
  property plays a critical role in preventing representation collapse and is achieved
  by pushing apart augmented views of different nodes (negative pairs). As such, existing
  GCL methods inherently rely on increasing the quantity and quality of negative samples,
  resulting in heavy computational demands, memory overhead, and potential class collision
  issues. In this study, we propose a negative-free objective to achieve uniformity,
  inspired by the fact that points distributed according to a normalized isotropic
  Gaussian are uniformly spread across the unit hypersphere. Therefore, we can minimize
  the distance between the distribution of learned representations and the isotropic
  Gaussian distribution to promote the uniformity of node representations. Our method
  also distinguishes itself from other approaches by eliminating the need for a parameterized
  mutual information estimator, an additional projector, asymmetric structures, and,
  crucially, negative samples. Extensive experiments over seven graph benchmarks demonstrate
  that our proposal achieves competitive performance with fewer parameters, shorter
  training times, and lower memory consumption compared to existing GCL methods.'
codebase_url: https://github.com/Cloudy1225/SSGE
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SSGE
mrr: 0.0073
adjusted_mrr: 0.0073
mrr_dataset_count: 5
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 5
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id003
  dataset: CiteSeer
  rows:
  - model: CNA
    model_key: cna
    model_plain: CNA
    value: 0.9575
    std: 0.0058
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9575
    sort_std: 0.0058
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: IS-GIB
    model_key: is-gib
    model_plain: IS-GIB
    value: 0.939
    std: 0.0187
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.939
    sort_std: 0.0187
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EERM
    model_key: eerm
    model_plain: EERM
    value: 0.9112
    std: 0.0145
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2306.15902'
    title: Individual and Structural Graph Information Bottlenecks for Out-of-Distribution
      Generalization
    date: Jun 28, 2023
    date_display: Jun 2023
    date_iso: '2023-06-28'
    venue: IEEE Transactions on Knowledge and Data Engineering
    codebase_url: https://github.com/YangLing0818/GraphOOD
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9112
    sort_std: 0.0145
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8774
    std: 0.0041
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2305.06142'
    title: Feature Expansion for Graph Neural Networks
    date: May 10, 2023
    date_display: May 2023
    date_iso: '2023-05-10'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/sajqavril/Feature-Extension-Graph-Neural-Networks
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 20
    sort_value: 0.8774
    sort_std: 0.0041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.702
    std: 0.004
    paper_value: 0.702
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8769
    at_pub_std: 0.004
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.17490000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8769
    true_std: 0.004
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.17490000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 673
    rank_delta: 652
    rank_delta_abs: 652
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.725
    std: 0.007
    paper_value: 0.725
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.808
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2305.06142'
    at_pub_source_title: Feature Expansion for Graph Neural Networks
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.08300000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.808
    true_std: 0.0026
    value_gap_source_arxiv: '2305.06142'
    value_gap_source_title: Feature Expansion for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08300000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.0026
    global_rank: 46
    paper_rank: 440
    rank_delta: 394
    rank_delta_abs: 394
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Feature Expansion for Graph Neural Networks
    comparison_source_arxiv: '2305.06142'
    is_best: false
    is_std_outlier: false
  - model: CCA-SSG
    model_key: cca-ssg
    model_plain: CCA-SSG
    value: 0.73
    std: 0.003
    paper_value: 0.73
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.754
    at_pub_std: 0.01
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.02400000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.796
    true_std: 0.0101
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.06600000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.796
    sort_std: 0.0101
    global_rank: 69
    paper_rank: 378
    rank_delta: 309
    rank_delta_abs: 309
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.718
    std: 0.007
    paper_value: 0.718
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.789
    at_pub_std: 0.002
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.07100000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.789
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.07100000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.789
    sort_std: 0.002
    global_rank: 83
    paper_rank: 533
    rank_delta: 450
    rank_delta_abs: 450
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.724
    std: 0.001
    paper_value: 0.724
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7869
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.06290000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7869
    true_std: 0.0016
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.06290000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.7869
    sort_std: 0.0016
    global_rank: 90
    paper_rank: 460
    rank_delta: 370
    rank_delta_abs: 370
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.733
    std: 0.005
    paper_value: 0.733
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7808
    at_pub_std: 0.0006
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.047800000000000065
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7808
    true_std: 0.0006
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.047800000000000065
    has_value_note: false
    value_note: ''
    sort_value: 0.7808
    sort_std: 0.0006
    global_rank: 108
    paper_rank: 340
    rank_delta: 232
    rank_delta_abs: 232
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.711
    std: 0.008
    paper_value: 0.711
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.76
    at_pub_std: 0.002
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.049000000000000044
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.76
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.049000000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.76
    sort_std: 0.002
    global_rank: 171
    paper_rank: 612
    rank_delta: 441
    rank_delta_abs: 441
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: GGD
    model_key: ggd
    model_plain: GGD
    value: 0.73
    std: 0.006
    paper_value: 0.73
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.755
    at_pub_std: 0.001
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.025000000000000022
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.755
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.025000000000000022
    has_value_note: false
    value_note: ''
    sort_value: 0.755
    sort_std: 0.001
    global_rank: 199
    paper_rank: 378
    rank_delta: 179
    rank_delta_abs: 179
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.711
    std: 0.004
    paper_value: 0.711
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.719
    at_pub_std: 0.004
    at_pub_source_arxiv: '2402.10468'
    at_pub_source_title: Adversarial Curriculum Graph Contrastive Learning with Pair-wise
      Augmentation
    at_pub_source_date_iso: '2024-02-16'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.008000000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7523
    true_std: 0.0119
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0413
    has_value_note: false
    value_note: ''
    sort_value: 0.7523
    sort_std: 0.0119
    global_rank: 211
    paper_rank: 612
    rank_delta: 401
    rank_delta_abs: 401
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Adversarial Curriculum Graph Contrastive Learning with
      Pair-wise Augmentation
    comparison_source_arxiv: '2402.10468'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.713
    std: 0.003
    paper_value: 0.713
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.745
    at_pub_std: 0.001
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.03200000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.745
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.03200000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.001
    global_rank: 245
    paper_rank: 587
    rank_delta: 342
    rank_delta_abs: 342
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: SSGE
    model_key: ssge
    model_plain: SSGE
    value: 0.741
    std: 0.003
    paper_value: 0.741
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.741
    true_std: 0.003
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.741
    sort_std: 0.003
    global_rank: 273
    paper_rank: 273
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MERIT
    model_key: merit
    model_plain: MERIT
    value: 0.735
    std: 0.007
    paper_value: 0.735
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6813
    at_pub_std: 0.0023
    at_pub_source_arxiv: '2304.07509'
    at_pub_source_title: Multi-View Graph Representation Learning Beyond Homophily
    at_pub_source_date_iso: '2023-04-15'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05369999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.735
    true_std: 0.007
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.735
    sort_std: 0.007
    global_rank: 325
    paper_rank: 325
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Multi-View Graph Representation Learning Beyond Homophily
    comparison_source_arxiv: '2304.07509'
    is_best: false
    is_std_outlier: false
  - model: COSTA
    model_key: costa
    model_plain: COSTA
    value: 0.707
    std: 0.005
    paper_value: 0.707
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.707
    at_pub_std: 0.005
    at_pub_source_arxiv: '2306.09614'
    at_pub_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-06-16'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.729
    true_std: 0.003
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.02200000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.729
    sort_std: 0.003
    global_rank: 389
    paper_rank: 639
    rank_delta: 250
    rank_delta_abs: 250
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: G-BT
    model_key: g-bt
    model_plain: G-BT
    value: 0.729
    std: 0.004
    paper_value: 0.729
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.729
    true_std: 0.004
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.729
    sort_std: 0.004
    global_rank: 398
    paper_rank: 398
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
    value: 0.542
    std: 0.001
    paper_value: 0.542
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.719
    at_pub_std: 0.0169
    at_pub_source_arxiv: '2310.00183'
    at_pub_source_title: On the Equivalence of Graph Convolution and Mixup
    at_pub_source_date_iso: '2023-09-29'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.17699999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7289
    true_std: 0.001
    value_gap_source_arxiv: '2508.17531'
    value_gap_source_title: 'Gumbel-MPNN: Graph Rewiring with Gumbel-Softmax'
    value_gap_source_is_current_paper: false
    value_gap: 0.18689999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.7289
    sort_std: 0.001
    global_rank: 401
    paper_rank: 937
    rank_delta: 536
    rank_delta_abs: 536
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Equivalence of Graph Convolution and Mixup
    comparison_source_arxiv: '2310.00183'
    is_best: false
    is_std_outlier: false
  - model: gCooL
    model_key: gcool
    model_plain: gCooL
    value: 0.72
    std: 0.003
    paper_value: 0.72
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.727
    true_std: 0.004
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.007000000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.727
    sort_std: 0.004
    global_rank: 421
    paper_rank: 514
    rank_delta: 93
    rank_delta_abs: 93
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.694
    std: 0.002
    paper_value: 0.694
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.694
    at_pub_std: 0.002
    at_pub_source_arxiv: '2306.09614'
    at_pub_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-06-16'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.726
    true_std: 0.003
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.03200000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.726
    sort_std: 0.003
    global_rank: 426
    paper_rank: 703
    rank_delta: 277
    rank_delta_abs: 277
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HomoGCL
    model_key: homogcl
    model_plain: HomoGCL
    value: 0.723
    std: 0.007
    paper_value: 0.723
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.723
    at_pub_std: 0.007
    at_pub_source_arxiv: '2306.09614'
    at_pub_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-06-16'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.723
    true_std: 0.007
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.723
    sort_std: 0.007
    global_rank: 479
    paper_rank: 479
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGRL
    model_key: rgrl
    model_plain: RGRL
    value: 0.715
    std: 0.009
    paper_value: 0.715
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.715
    true_std: 0.009
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.715
    sort_std: 0.009
    global_rank: 571
    paper_rank: 571
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.683
    std: 0.004
    paper_value: 0.683
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.699
    at_pub_std: 0.0057
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.015999999999999903
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.699
    true_std: 0.0057
    value_gap_source_arxiv: '2206.03601'
    value_gap_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.015999999999999903
    has_value_note: false
    value_note: ''
    sort_value: 0.699
    sort_std: 0.0057
    global_rank: 689
    paper_rank: 741
    rank_delta: 52
    rank_delta_abs: 52
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.498
    std: 0.002
    paper_value: 0.498
    paper_std: 0.002
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6785
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.1805
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6785
    true_std: 0.0079
    value_gap_source_arxiv: '2206.03601'
    value_gap_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.1805
    has_value_note: false
    value_note: ''
    sort_value: 0.6785
    sort_std: 0.0079
    global_rank: 759
    paper_rank: 947
    rank_delta: 188
    rank_delta_abs: 188
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.658
    std: 0.004
    paper_value: 0.658
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6639
    at_pub_std: 0.0024
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-06-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.005900000000000016
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.6639
    true_std: 0.0024
    value_gap_source_arxiv: '2206.03601'
    value_gap_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.005900000000000016
    has_value_note: false
    value_note: ''
    sort_value: 0.6639
    sort_std: 0.0024
    global_rank: 806
    paper_rank: 823
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.498
    std: 0.003
    paper_value: 0.498
    paper_std: 0.003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed split) used for node classification.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6552
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.1572
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6552
    true_std: 0.0018
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.1572
    has_value_note: false
    value_note: ''
    sort_value: 0.6552
    sort_std: 0.0018
    global_rank: 832
    paper_rank: 947
    rank_delta: 115
    rank_delta_abs: 115
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
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
- &id005
  dataset: Coauthor-CS
  rows:
  - model: DoG
    model_key: dog
    model_plain: DoG
    value: 0.969
    std: 0.003
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: synthetic graph structures added to the training set
    is_global_top: true
    global_rank: 1
    sort_value: 0.969
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GWN-fa
    model_key: gwn-fa
    model_plain: GWN-fa
    value: 0.9667
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9667
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GWN-sym
    model_key: gwn-sym
    model_plain: GWN-sym
    value: 0.9666
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9593
    std: 0.0025
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 6
    sort_value: 0.9593
    sort_std: 0.0025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9303
    std: 0.0031
    paper_value: 0.9303
    paper_std: 0.0031
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.936
    at_pub_std: 0.015
    at_pub_source_arxiv: '2002.06755'
    at_pub_source_title: Unifying Graph Convolutional Neural Networks and Label Propagation
    at_pub_source_date_iso: '2020-02-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.005700000000000038
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9514
    true_std: 0.0025
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.021100000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.9514
    sort_std: 0.0025
    global_rank: 14
    paper_rank: 73
    rank_delta: 59
    rank_delta_abs: 59
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.9231
    std: 0.0024
    paper_value: 0.9231
    paper_std: 0.0024
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.938
    at_pub_std: 0.004
    at_pub_source_arxiv: '2002.06755'
    at_pub_source_title: Unifying Graph Convolutional Neural Networks and Label Propagation
    at_pub_source_date_iso: '2020-02-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.014899999999999913
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9437
    true_std: 0.0028
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.02059999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9437
    sort_std: 0.0028
    global_rank: 23
    paper_rank: 118
    rank_delta: 95
    rank_delta_abs: 95
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Unifying Graph Convolutional Neural Networks and Label
      Propagation
    comparison_source_arxiv: '2002.06755'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.9215
    std: 0.0063
    paper_value: 0.9215
    paper_std: 0.0063
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9221
    at_pub_std: 0.0029
    at_pub_source_arxiv: '2301.12063'
    at_pub_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    at_pub_source_date_iso: '2023-01-28'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-12-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0006000000000000449
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.935
    true_std: 0.003
    value_gap_source_arxiv: '2412.21151'
    value_gap_source_title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    value_gap_source_is_current_paper: false
    value_gap: 0.013500000000000068
    has_value_note: false
    value_note: ''
    sort_value: 0.935
    sort_std: 0.003
    global_rank: 47
    paper_rank: 124
    rank_delta: 77
    rank_delta_abs: 77
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SSGE
    model_key: ssge
    model_plain: SSGE
    value: 0.9346
    std: 0.0045
    paper_value: 0.9346
    paper_std: 0.0045
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9346
    true_std: 0.0045
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9346
    sort_std: 0.0045
    global_rank: 50
    paper_rank: 50
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CCA-SSG
    model_key: cca-ssg
    model_plain: CCA-SSG
    value: 0.9301
    std: 0.002
    paper_value: 0.9301
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9337
    at_pub_std: 0.002
    at_pub_source_arxiv: '2212.07035'
    at_pub_source_title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive
      Learning'
    at_pub_source_date_iso: '2022-12-14'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-12-14'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0035999999999999366
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9337
    true_std: 0.002
    value_gap_source_arxiv: '2212.07035'
    value_gap_source_title: 'MA-GCL: Model Augmentation Tricks for Graph Contrastive
      Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.0035999999999999366
    has_value_note: false
    value_note: ''
    sort_value: 0.9337
    sort_std: 0.002
    global_rank: 54
    paper_rank: 74
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.931
    std: 0.0001
    paper_value: 0.931
    paper_std: 0.0001
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9332
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2211.14065'
    at_pub_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    at_pub_source_date_iso: '2022-11-25'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-11-25'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.0021999999999999797
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9332
    true_std: 0.0012
    value_gap_source_arxiv: '2211.14065'
    value_gap_source_title: 'Beyond Smoothing: Unsupervised Graph Representation Learning
      with Edge Heterophily Discriminating'
    value_gap_source_is_current_paper: false
    value_gap: 0.0021999999999999797
    has_value_note: false
    value_note: ''
    sort_value: 0.9332
    sort_std: 0.0012
    global_rank: 57
    paper_rank: 69
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Beyond Smoothing: Unsupervised Graph Representation
      Learning with Edge Heterophily Discriminating'
    comparison_source_arxiv: '2211.14065'
    is_best: false
    is_std_outlier: false
  - model: gCooL
    model_key: gcool
    model_plain: gCooL
    value: 0.9275
    std: 0.0001
    paper_value: 0.9275
    paper_std: 0.0001
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9332
    true_std: 0.0002
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.005700000000000038
    has_value_note: false
    value_note: ''
    sort_value: 0.9332
    sort_std: 0.0002
    global_rank: 58
    paper_rank: 101
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.9272
    std: 0.0003
    paper_value: 0.9272
    paper_std: 0.0003
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9331
    at_pub_std: 0.0013
    at_pub_source_arxiv: '2210.00643'
    at_pub_source_title: Spectral Augmentation for Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2022-10-02'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.005900000000000016
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9331
    true_std: 0.0013
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.005900000000000016
    has_value_note: false
    value_note: ''
    sort_value: 0.9331
    sort_std: 0.0013
    global_rank: 59
    paper_rank: 102
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Spectral Augmentation for Self-Supervised Learning on
      Graphs
    comparison_source_arxiv: '2210.00643'
    is_best: false
    is_std_outlier: false
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.9307
    std: 0.0017
    paper_value: 0.9307
    paper_std: 0.0017
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9327
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2312.02619'
    at_pub_source_title: Rethinking and Simplifying Bootstrapped Graph Latents
    at_pub_source_date_iso: '2023-12-05'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-12-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0020000000000000018
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.933
    true_std: 0.002
    value_gap_source_arxiv: '2412.21151'
    value_gap_source_title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    value_gap_source_is_current_paper: false
    value_gap: 0.0023000000000000798
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.002
    global_rank: 62
    paper_rank: 72
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.9217
    std: 0.0004
    paper_value: 0.9217
    paper_std: 0.0004
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9295
    at_pub_std: 0.0003
    at_pub_source_arxiv: '2407.16726'
    at_pub_source_title: Topology Reorganized Graph Contrastive Learning with Mitigating
      Semantic Drift
    at_pub_source_date_iso: '2024-07-23'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-02-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.007800000000000029
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9301
    true_std: 0.0003
    value_gap_source_arxiv: '2502.20885'
    value_gap_source_title: A Fused Gromov-Wasserstein Approach to Subgraph Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.008400000000000074
    has_value_note: false
    value_note: ''
    sort_value: 0.9301
    sort_std: 0.0003
    global_rank: 75
    paper_rank: 124
    rank_delta: 49
    rank_delta_abs: 49
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Topology Reorganized Graph Contrastive Learning with
      Mitigating Semantic Drift
    comparison_source_arxiv: '2407.16726'
    is_best: false
    is_std_outlier: false
  - model: COSTA
    model_key: costa
    model_plain: COSTA
    value: 0.9294
    std: 0.001
    paper_value: 0.9294
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9295
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2312.02619'
    at_pub_source_title: Rethinking and Simplifying Bootstrapped Graph Latents
    at_pub_source_date_iso: '2023-12-05'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9295
    true_std: 0.0012
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.9295
    sort_std: 0.0012
    global_rank: 83
    paper_rank: 87
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: G-BT
    model_key: g-bt
    model_plain: G-BT
    value: 0.9291
    std: 0.0025
    paper_value: 0.9291
    paper_std: 0.0025
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9295
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2402.15270'
    at_pub_source_title: Smoothed Graph Contrastive Learning via Seamless Proximity
      Integration
    at_pub_source_date_iso: '2024-02-23'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9295
    true_std: 0.0017
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.9295
    sort_std: 0.0017
    global_rank: 84
    paper_rank: 90
    rank_delta: 6
    rank_delta_abs: 6
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGRL
    model_key: rgrl
    model_plain: RGRL
    value: 0.9294
    std: 0.0013
    paper_value: 0.9294
    paper_std: 0.0013
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9294
    true_std: 0.0013
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9294
    sort_std: 0.0013
    global_rank: 89
    paper_rank: 89
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
    value: 0.9037
    std: 0.0
    paper_value: 0.9037
    paper_std: 0.0
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.917
    at_pub_std: 0.014
    at_pub_source_arxiv: '2002.06755'
    at_pub_source_title: Unifying Graph Convolutional Neural Networks and Label Propagation
    at_pub_source_date_iso: '2020-02-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.01330000000000009
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.928
    true_std: 0.002
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: false
    value_gap: 0.0243000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.928
    sort_std: 0.002
    global_rank: 96
    paper_rank: 172
    rank_delta: 76
    rank_delta_abs: 76
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HomoGCL
    model_key: homogcl
    model_plain: HomoGCL
    value: 0.9228
    std: 0.0003
    paper_value: 0.9228
    paper_std: 0.0003
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9216
    at_pub_std: 0.0005
    at_pub_source_arxiv: '2407.16726'
    at_pub_source_title: Topology Reorganized Graph Contrastive Learning with Mitigating
      Semantic Drift
    at_pub_source_date_iso: '2024-07-23'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.0011999999999999789
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9274
    true_std: 0.0022
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.0046000000000000485
    has_value_note: false
    value_note: ''
    sort_value: 0.9274
    sort_std: 0.0022
    global_rank: 102
    paper_rank: 121
    rank_delta: 19
    rank_delta_abs: 19
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Topology Reorganized Graph Contrastive Learning with
      Mitigating Semantic Drift
    comparison_source_arxiv: '2407.16726'
    is_best: false
    is_std_outlier: false
  - model: GGD
    model_key: ggd
    model_plain: GGD
    value: 0.923
    std: 0.0023
    paper_value: 0.923
    paper_std: 0.0023
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-03-16'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.927
    true_std: 0.004
    value_gap_source_arxiv: '2503.12563'
    value_gap_source_title: 'Diffusion on Graph: Augmentation of Graph Structure for
      Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.927
    sort_std: 0.004
    global_rank: 106
    paper_rank: 118
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MERIT
    model_key: merit
    model_plain: MERIT
    value: 0.9251
    std: 0.0014
    paper_value: 0.9251
    paper_std: 0.0014
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.924
    at_pub_std: 0.004
    at_pub_source_arxiv: '2202.08480'
    at_pub_source_title: Eliciting Structural and Semantic Global Knowledge in Unsupervised
      Graph Contrastive Learning
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0010999999999999899
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9251
    true_std: 0.0014
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9251
    sort_std: 0.0014
    global_rank: 111
    paper_rank: 111
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.9211
    std: 0.0009
    paper_value: 0.9211
    paper_std: 0.0009
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9211
    at_pub_std: 0.09
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9211
    true_std: 0.0009
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9211
    sort_std: 0.0009
    global_rank: 127
    paper_rank: 127
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.9211
    std: 0.0012
    paper_value: 0.9211
    paper_std: 0.0012
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9211
    at_pub_std: 0.12
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9211
    true_std: 0.0012
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9211
    sort_std: 0.0012
    global_rank: 126
    paper_rank: 126
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.8878
    std: 0.0012
    paper_value: 0.8878
    paper_std: 0.0012
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9108
    at_pub_std: 0.0056
    at_pub_source_arxiv: '2407.16726'
    at_pub_source_title: Topology Reorganized Graph Contrastive Learning with Mitigating
      Semantic Drift
    at_pub_source_date_iso: '2024-07-23'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-23'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.02300000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9108
    true_std: 0.0056
    value_gap_source_arxiv: '2407.16726'
    value_gap_source_title: Topology Reorganized Graph Contrastive Learning with Mitigating
      Semantic Drift
    value_gap_source_is_current_paper: false
    value_gap: 0.02300000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9108
    sort_std: 0.0056
    global_rank: 165
    paper_rank: 186
    rank_delta: 21
    rank_delta_abs: 21
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Topology Reorganized Graph Contrastive Learning with
      Mitigating Semantic Drift
    comparison_source_arxiv: '2407.16726'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.9001
    std: 0.0071
    paper_value: 0.9001
    paper_std: 0.0071
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9005
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2301.12063'
    at_pub_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    at_pub_source_date_iso: '2023-01-28'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-01-28'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.00039999999999995595
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.9005
    true_std: 0.0035
    value_gap_source_arxiv: '2301.12063'
    value_gap_source_title: 'HAT-GAE: Self-Supervised Graph Auto-encoders with Hierarchical
      Adaptive Masking and Trainable Corruption'
    value_gap_source_is_current_paper: false
    value_gap: 0.00039999999999995595
    has_value_note: false
    value_note: ''
    sort_value: 0.9005
    sort_std: 0.0035
    global_rank: 179
    paper_rank: 179
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.8508
    std: 0.0003
    paper_value: 0.8508
    paper_std: 0.0003
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.851
    at_pub_std: 0.0
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.851
    true_std: 0.0
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.851
    sort_std: 0.0
    global_rank: 201
    paper_rank: 201
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.8461
    std: 0.0022
    paper_value: 0.8461
    paper_std: 0.0022
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
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=95)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on CoauthorCS
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8461
    at_pub_std: 0.22
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8461
    true_std: 0.0022
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8461
    sort_std: 0.0022
    global_rank: 205
    paper_rank: 205
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: Cora
  rows:
  - model: MATE
    model_key: mate
    model_plain: MATE
    value: 0.946
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.946
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE+CNA
    model_key: graphsage+cna
    model_plain: GraphSAGE+CNA
    value: 0.9418
    std: 0.0033
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.04064'
    title: Graph Neural Networks Need Cluster-Normalize-Activate Modules
    date: Dec 5, 2024
    date_display: Dec 2024
    date_iso: '2024-12-05'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/ml-research/cna_modules
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9418
    sort_std: 0.0033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DropAggr
    model_key: dropaggr
    model_plain: DropAggr
    value: 0.938
    std: 0.011
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.20067'
    title: 'xAI-Drop: Don''t Use What You Cannot Explain'
    date: Jul 29, 2024
    date_display: Jul 2024
    date_iso: '2024-07-29'
    venue: Learning on Graphs Conference
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.938
    sort_std: 0.011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.815
    std: 0.004
    paper_value: 0.815
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9004
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.08540000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9004
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.08540000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9004
    sort_std: null
    global_rank: 31
    paper_rank: 657
    rank_delta: 626
    rank_delta_abs: 626
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8911
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    venue: Trans. Mach. Learn. Res.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 61
    sort_value: 0.8911
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.83
    std: 0.007
    paper_value: 0.83
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.889
    at_pub_std: 0.0
    at_pub_source_arxiv: '2009.09232'
    at_pub_source_title: Learned Low Precision Graph Neural Networks
    at_pub_source_date_iso: '2020-09-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.05900000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8897
    true_std: 0.0014
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.059700000000000086
    has_value_note: false
    value_note: ''
    sort_value: 0.8897
    sort_std: 0.0014
    global_rank: 67
    paper_rank: 498
    rank_delta: 431
    rank_delta_abs: 431
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learned Low Precision Graph Neural Networks
    comparison_source_arxiv: '2009.09232'
    is_best: false
    is_std_outlier: false
  - model: CCA-SSG
    model_key: cca-ssg
    model_plain: CCA-SSG
    value: 0.839
    std: 0.004
    paper_value: 0.839
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.846
    at_pub_std: 0.007
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.007000000000000006
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8739
    true_std: 0.0089
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.03490000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.8739
    sort_std: 0.0089
    global_rank: 167
    paper_rank: 372
    rank_delta: 205
    rank_delta_abs: 205
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.827
    std: 0.006
    paper_value: 0.827
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.873
    at_pub_std: 0.001
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.04600000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.873
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.04600000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.873
    sort_std: 0.001
    global_rank: 170
    paper_rank: 524
    rank_delta: 354
    rank_delta_abs: 354
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.819
    std: 0.004
    paper_value: 0.819
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.872
    at_pub_std: 0.002
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.05300000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.872
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.05300000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.872
    sort_std: 0.002
    global_rank: 176
    paper_rank: 618
    rank_delta: 442
    rank_delta_abs: 442
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.835
    std: 0.004
    paper_value: 0.835
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.868
    at_pub_std: 0.005
    at_pub_source_arxiv: '2307.01053'
    at_pub_source_title: 'ENGAGE: Explanation Guided Data Augmentation for Graph Representation
      Learning'
    at_pub_source_date_iso: '2023-07-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.03300000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.868
    true_std: 0.005
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.03300000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.868
    sort_std: 0.005
    global_rank: 205
    paper_rank: 435
    rank_delta: 230
    rank_delta_abs: 230
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'ENGAGE: Explanation Guided Data Augmentation for Graph
      Representation Learning'
    comparison_source_arxiv: '2307.01053'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.823
    std: 0.006
    paper_value: 0.823
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.863
    at_pub_std: 0.002
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.040000000000000036
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.863
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.863
    sort_std: 0.002
    global_rank: 227
    paper_rank: 566
    rank_delta: 339
    rank_delta_abs: 339
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: GGD
    model_key: ggd
    model_plain: GGD
    value: 0.835
    std: 0.006
    paper_value: 0.835
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.862
    at_pub_std: 0.002
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.027000000000000024
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.862
    true_std: 0.002
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.027000000000000024
    has_value_note: false
    value_note: ''
    sort_value: 0.862
    sort_std: 0.002
    global_rank: 231
    paper_rank: 435
    rank_delta: 204
    rank_delta_abs: 204
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.83
    std: 0.003
    paper_value: 0.83
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8526
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.022600000000000064
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8526
    true_std: 0.0008
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.022600000000000064
    has_value_note: false
    value_note: ''
    sort_value: 0.8526
    sort_std: 0.0008
    global_rank: 276
    paper_rank: 498
    rank_delta: 222
    rank_delta_abs: 222
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: HomoGCL
    model_key: homogcl
    model_plain: HomoGCL
    value: 0.841
    std: 0.005
    paper_value: 0.841
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.845
    at_pub_std: 0.005
    at_pub_source_arxiv: '2306.09614'
    at_pub_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-06-16'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.0040000000000000036
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.845
    true_std: 0.005
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.845
    sort_std: 0.005
    global_rank: 315
    paper_rank: 351
    rank_delta: 36
    rank_delta_abs: 36
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: COSTA
    model_key: costa
    model_plain: COSTA
    value: 0.822
    std: 0.002
    paper_value: 0.822
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.822
    at_pub_std: 0.002
    at_pub_source_arxiv: '2306.09614'
    at_pub_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-06-16'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.843
    true_std: 0.002
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.02100000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.843
    sort_std: 0.002
    global_rank: 335
    paper_rank: 588
    rank_delta: 253
    rank_delta_abs: 253
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.817
    std: 0.003
    paper_value: 0.817
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.831
    at_pub_std: 0.003
    at_pub_source_arxiv: '2211.03710'
    at_pub_source_title: Graph Contrastive Learning with Implicit Augmentations
    at_pub_source_date_iso: '2022-11-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-04-02'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.014000000000000012
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8409
    true_std: 0.0085
    value_gap_source_arxiv: '2604.01878'
    value_gap_source_title: 'ASPECT: Node-Level Adaptive Spectral Fusion for Graph
      Contrastive Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.023900000000000032
    has_value_note: false
    value_note: ''
    sort_value: 0.8409
    sort_std: 0.0085
    global_rank: 363
    paper_rank: 642
    rank_delta: 279
    rank_delta_abs: 279
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning with Implicit Augmentations
    comparison_source_arxiv: '2211.03710'
    is_best: false
    is_std_outlier: false
  - model: SSGE
    model_key: ssge
    model_plain: SSGE
    value: 0.839
    std: 0.003
    paper_value: 0.839
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.839
    true_std: 0.003
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.839
    sort_std: 0.003
    global_rank: 377
    paper_rank: 377
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.73
    std: 0.003
    paper_value: 0.73
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.836
    at_pub_std: 0.0052
    at_pub_source_arxiv: '2405.14742'
    at_pub_source_title: 'HC-GAE: The Hierarchical Cluster-based Graph Auto-Encoder
      for Graph Representation Learning'
    at_pub_source_date_iso: '2024-05-23'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-05-23'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.10599999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.836
    true_std: 0.0052
    value_gap_source_arxiv: '2405.14742'
    value_gap_source_title: 'HC-GAE: The Hierarchical Cluster-based Graph Auto-Encoder
      for Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.10599999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.0052
    global_rank: 418
    paper_rank: 880
    rank_delta: 462
    rank_delta_abs: 462
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'HC-GAE: The Hierarchical Cluster-based Graph Auto-Encoder
      for Graph Representation Learning'
    comparison_source_arxiv: '2405.14742'
    is_best: false
    is_std_outlier: false
  - model: G-BT
    model_key: g-bt
    model_plain: G-BT
    value: 0.836
    std: 0.0
    paper_value: 0.836
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.836
    true_std: 0.0
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.836
    sort_std: 0.0
    global_rank: 422
    paper_rank: 422
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGRL
    model_key: rgrl
    model_plain: RGRL
    value: 0.835
    std: 0.007
    paper_value: 0.835
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.835
    true_std: 0.007
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.835
    sort_std: 0.007
    global_rank: 440
    paper_rank: 440
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: gCooL
    model_key: gcool
    model_plain: gCooL
    value: 0.828
    std: 0.005
    paper_value: 0.828
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.832
    true_std: 0.005
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.832
    sort_std: 0.005
    global_rank: 481
    paper_rank: 515
    rank_delta: 34
    rank_delta_abs: 34
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.798
    std: 0.002
    paper_value: 0.798
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.813
    at_pub_std: 0.002
    at_pub_source_arxiv: '2402.10468'
    at_pub_source_title: Adversarial Curriculum Graph Contrastive Learning with Pair-wise
      Augmentation
    at_pub_source_date_iso: '2024-02-16'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.014999999999999902
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.832
    true_std: 0.004
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.03399999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.832
    sort_std: 0.004
    global_rank: 479
    paper_rank: 747
    rank_delta: 268
    rank_delta_abs: 268
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Adversarial Curriculum Graph Contrastive Learning with
      Pair-wise Augmentation
    comparison_source_arxiv: '2402.10468'
    is_best: false
    is_std_outlier: false
  - model: MERIT
    model_key: merit
    model_plain: MERIT
    value: 0.831
    std: 0.006
    paper_value: 0.831
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.831
    true_std: 0.006
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.831
    sort_std: 0.006
    global_rank: 491
    paper_rank: 491
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.685
    std: 0.005
    paper_value: 0.685
    paper_std: 0.005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.829
    at_pub_std: null
    at_pub_source_arxiv: '1909.00958'
    at_pub_source_title: 'Graph Representation Learning: A Survey'
    at_pub_source_date_iso: '2019-09-03'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-03'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.1439999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.829
    true_std: null
    value_gap_source_arxiv: '1909.00958'
    value_gap_source_title: 'Graph Representation Learning: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.1439999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.829
    sort_std: null
    global_rank: 508
    paper_rank: 918
    rank_delta: 410
    rank_delta_abs: 410
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Representation Learning: A Survey'
    comparison_source_arxiv: '1909.00958'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.701
    std: 0.004
    paper_value: 0.701
    paper_std: 0.004
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.803
    at_pub_std: null
    at_pub_source_arxiv: '1909.00958'
    at_pub_source_title: 'Graph Representation Learning: A Survey'
    at_pub_source_date_iso: '2019-09-03'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-09-03'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.10200000000000009
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.803
    true_std: null
    value_gap_source_arxiv: '1909.00958'
    value_gap_source_title: 'Graph Representation Learning: A Survey'
    value_gap_source_is_current_paper: false
    value_gap: 0.10200000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.803
    sort_std: null
    global_rank: 728
    paper_rank: 905
    rank_delta: 177
    rank_delta_abs: 177
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Representation Learning: A Survey'
    comparison_source_arxiv: '1909.00958'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.715
    std: 0.004
    paper_value: 0.715
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
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8011
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-02-17'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.08610000000000007
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8011
    true_std: 0.0022
    value_gap_source_arxiv: '2202.08391'
    value_gap_source_title: Graph Masked Autoencoders with Transformers
    value_gap_source_is_current_paper: false
    value_gap: 0.08610000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.8011
    sort_std: 0.0022
    global_rank: 736
    paper_rank: 895
    rank_delta: 159
    rank_delta_abs: 159
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Masked Autoencoders with Transformers
    comparison_source_arxiv: '2202.08391'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.578
    std: 0.002
    paper_value: 0.578
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016 fixed 20-per-class train split)
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7768
    at_pub_std: null
    at_pub_source_arxiv: '2401.09125'
    at_pub_source_title: Understanding Heterophily for Graph Neural Networks
    at_pub_source_date_iso: '2024-01-17'
    at_pub_source_date_label: ICML 2024
    value_gap_source_date_iso: '2024-01-17'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: 0.1988000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7768
    true_std: null
    value_gap_source_arxiv: '2401.09125'
    value_gap_source_title: Understanding Heterophily for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1988000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 806
    paper_rank: 969
    rank_delta: 163
    rank_delta_abs: 163
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Heterophily for Graph Neural Networks
    comparison_source_arxiv: '2401.09125'
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
- &id002
  dataset: PubMed
  rows:
  - model: LGTL
    model_key: lgtl
    model_plain: LGTL
    value: 0.9518
    std: 0.0011
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.15845'
    title: 'Adaptive Tokenization: On the Hop-Overpriority Problem in Tokenized Graph
      Learning Models'
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9518
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MixHop (LO)
    model_key: mixhop (lo)
    model_plain: MixHop (LO)
    value: 0.9513
    std: 0.0038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphSAGE (LO)
    model_key: graphsage (lo)
    model_plain: GraphSAGE (LO)
    value: 0.9511
    std: 0.0036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2405.13902'
    title: 'LOGIN: A Large Language Model Consulted Graph Neural Network Training
      Framework'
    date: May 22, 2024
    date_display: May 2024
    date_iso: '2024-05-22'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/QiaoYRan/LOGIN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9511
    sort_std: 0.0036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.79
    std: 0.002
    paper_value: 0.79
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.10699999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9296
    true_std: 0.0015
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.13959999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: 0.0015
    global_rank: 19
    paper_rank: 641
    rank_delta: 622
    rank_delta_abs: 622
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.79
    std: 0.003
    paper_value: 0.79
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.10699999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9233
    true_std: 0.0018
    value_gap_source_arxiv: '2505.15845'
    value_gap_source_title: 'Adaptive Tokenization: On the Hop-Overpriority Problem
      in Tokenized Graph Learning Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.13329999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: 0.0018
    global_rank: 23
    paper_rank: 641
    rank_delta: 618
    rank_delta_abs: 618
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Tackling Over-Smoothing for General Graph Convolutional
      Networks
    comparison_source_arxiv: '2008.09864'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8881
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.07168'
    title: Efficient Text-Attributed Graph Learning through Selective Annotation and
      Graph Alignment
    date: Jun 8, 2025
    date_display: Jun 2025
    date_iso: '2025-06-08'
    venue: Trans. Mach. Learn. Res.
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 134
    sort_value: 0.8881
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CCA-SSG
    model_key: cca-ssg
    model_plain: CCA-SSG
    value: 0.807
    std: 0.004
    paper_value: 0.807
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.884
    at_pub_std: 0.006
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.07699999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.884
    true_std: 0.006
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.07699999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.884
    sort_std: 0.006
    global_rank: 159
    paper_rank: 443
    rank_delta: 284
    rank_delta_abs: 284
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.796
    std: 0.005
    paper_value: 0.796
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.883
    at_pub_std: 0.001
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.08699999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.883
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.08699999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.883
    sort_std: 0.001
    global_rank: 167
    paper_rank: 538
    rank_delta: 371
    rank_delta_abs: 371
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.801
    std: 0.002
    paper_value: 0.801
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.873
    at_pub_std: 0.001
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.07199999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.873
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.07199999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.873
    sort_std: 0.001
    global_rank: 224
    paper_rank: 491
    rank_delta: 267
    rank_delta_abs: 267
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.799
    std: 0.002
    paper_value: 0.799
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8726
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0736
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8726
    true_std: 0.0016
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.0736
    has_value_note: false
    value_note: ''
    sort_value: 0.8726
    sort_std: 0.0016
    global_rank: 225
    paper_rank: 509
    rank_delta: 284
    rank_delta_abs: 284
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.801
    std: 0.007
    paper_value: 0.801
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8725
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.07150000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8725
    true_std: 0.0012
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.07150000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8725
    sort_std: 0.0012
    global_rank: 226
    paper_rank: 491
    rank_delta: 265
    rank_delta_abs: 265
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.768
    std: 0.006
    paper_value: 0.768
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8708
    at_pub_std: 0.0017
    at_pub_source_arxiv: '2407.19944'
    at_pub_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    at_pub_source_date_iso: '2024-07-29'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.1028
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8708
    true_std: 0.0017
    value_gap_source_arxiv: '2407.19944'
    value_gap_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    value_gap_source_is_current_paper: false
    value_gap: 0.1028
    has_value_note: false
    value_note: ''
    sort_value: 0.8708
    sort_std: 0.0017
    global_rank: 235
    paper_rank: 818
    rank_delta: 583
    rank_delta_abs: 583
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    comparison_source_arxiv: '2407.19944'
    is_best: false
    is_std_outlier: false
  - model: COSTA
    model_key: costa
    model_plain: COSTA
    value: 0.804
    std: 0.003
    paper_value: 0.804
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8698
    at_pub_std: 0.0033
    at_pub_source_arxiv: '2407.19944'
    at_pub_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    at_pub_source_date_iso: '2024-07-29'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.06579999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8698
    true_std: 0.0033
    value_gap_source_arxiv: '2407.19944'
    value_gap_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    value_gap_source_is_current_paper: false
    value_gap: 0.06579999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8698
    sort_std: 0.0033
    global_rank: 239
    paper_rank: 460
    rank_delta: 221
    rank_delta_abs: 221
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Noise-Resilient Unsupervised Graph Representation Learning
      via Multi-Hop Feature Quality Estimation
    comparison_source_arxiv: '2407.19944'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.728
    std: 0.002
    paper_value: 0.728
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.869
    at_pub_std: 0.0074
    at_pub_source_arxiv: '2310.00183'
    at_pub_source_title: On the Equivalence of Graph Convolution and Mixup
    at_pub_source_date_iso: '2023-09-29'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.14100000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.869
    true_std: 0.0074
    value_gap_source_arxiv: '2310.00183'
    value_gap_source_title: On the Equivalence of Graph Convolution and Mixup
    value_gap_source_is_current_paper: false
    value_gap: 0.14100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.869
    sort_std: 0.0074
    global_rank: 243
    paper_rank: 902
    rank_delta: 659
    rank_delta_abs: 659
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Equivalence of Graph Convolution and Mixup
    comparison_source_arxiv: '2310.00183'
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.662
    std: 0.007
    paper_value: 0.662
    paper_std: 0.007
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8652
    at_pub_std: 0.0012
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.20319999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8652
    true_std: 0.0012
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.20319999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8652
    sort_std: 0.0012
    global_rank: 255
    paper_rank: 945
    rank_delta: 690
    rank_delta_abs: 690
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.698
    std: 0.007
    paper_value: 0.698
    paper_std: 0.007
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.852
    at_pub_std: 0.0002
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.15400000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.852
    true_std: 0.0002
    value_gap_source_arxiv: '2203.12265'
    value_gap_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    value_gap_source_is_current_paper: false
    value_gap: 0.15400000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.852
    sort_std: 0.0002
    global_rank: 287
    paper_rank: 924
    rank_delta: 637
    rank_delta_abs: 637
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.795
    std: 0.005
    paper_value: 0.795
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8128
    at_pub_std: 0.0085
    at_pub_source_arxiv: '2202.08391'
    at_pub_source_title: Graph Masked Autoencoders with Transformers
    at_pub_source_date_iso: '2022-02-17'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.017799999999999927
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8512
    true_std: 0.0023
    value_gap_source_arxiv: '2410.15355'
    value_gap_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    value_gap_source_is_current_paper: false
    value_gap: 0.05619999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.8512
    sort_std: 0.0023
    global_rank: 291
    paper_rank: 556
    rank_delta: 265
    rank_delta_abs: 265
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Masked Autoencoders with Transformers
    comparison_source_arxiv: '2202.08391'
    is_best: false
    is_std_outlier: false
  - model: MERIT
    model_key: merit
    model_plain: MERIT
    value: 0.801
    std: 0.004
    paper_value: 0.801
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8505
    at_pub_std: 0.001
    at_pub_source_arxiv: '2304.07509'
    at_pub_source_title: Multi-View Graph Representation Learning Beyond Homophily
    at_pub_source_date_iso: '2023-04-15'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-04-15'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.04949999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8505
    true_std: 0.001
    value_gap_source_arxiv: '2304.07509'
    value_gap_source_title: Multi-View Graph Representation Learning Beyond Homophily
    value_gap_source_is_current_paper: false
    value_gap: 0.04949999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8505
    sort_std: 0.001
    global_rank: 292
    paper_rank: 491
    rank_delta: 199
    rank_delta_abs: 199
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-View Graph Representation Learning Beyond Homophily
    comparison_source_arxiv: '2304.07509'
    is_best: false
    is_std_outlier: false
  - model: GGD
    model_key: ggd
    model_plain: GGD
    value: 0.81
    std: 0.008
    paper_value: 0.81
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
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.842
    at_pub_std: 0.001
    at_pub_source_arxiv: '2306.02117'
    at_pub_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    at_pub_source_date_iso: '2023-06-03'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.03199999999999992
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.842
    true_std: 0.001
    value_gap_source_arxiv: '2306.02117'
    value_gap_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    value_gap_source_is_current_paper: false
    value_gap: 0.03199999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.842
    sort_std: 0.001
    global_rank: 313
    paper_rank: 420
    rank_delta: 107
    rank_delta_abs: 107
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Oversmoothing: A Nightmare for Graph Contrastive Learning?'
    comparison_source_arxiv: '2306.02117'
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.758
    std: 0.002
    paper_value: 0.758
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8133
    at_pub_std: 0.0069
    at_pub_source_arxiv: '2206.03601'
    at_pub_source_title: Decoupled Self-supervised Learning for Non-Homophilou Graphs
    at_pub_source_date_iso: '2022-06-07'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.055300000000000016
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8307
    true_std: 0.0029
    value_gap_source_arxiv: '2410.15355'
    value_gap_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    value_gap_source_is_current_paper: false
    value_gap: 0.07269999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8307
    sort_std: 0.0029
    global_rank: 342
    paper_rank: 850
    rank_delta: 508
    rank_delta_abs: 508
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Decoupled Self-supervised Learning for Non-Homophilou
      Graphs
    comparison_source_arxiv: '2206.03601'
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.721
    std: 0.005
    paper_value: 0.721
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8189
    at_pub_std: 0.0187
    at_pub_source_arxiv: '2304.07509'
    at_pub_source_title: Multi-View Graph Representation Learning Beyond Homophily
    at_pub_source_date_iso: '2023-04-15'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-10-20'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.09789999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8294
    true_std: 0.0031
    value_gap_source_arxiv: '2410.15355'
    value_gap_source_title: 'LAC: Graph Contrastive Learning with Learnable Augmentation
      in Continuous Space'
    value_gap_source_is_current_paper: false
    value_gap: 0.10840000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8294
    sort_std: 0.0031
    global_rank: 347
    paper_rank: 906
    rank_delta: 559
    rank_delta_abs: 559
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Multi-View Graph Representation Learning Beyond Homophily
    comparison_source_arxiv: '2304.07509'
    is_best: false
    is_std_outlier: false
  - model: SSGE
    model_key: ssge
    model_plain: SSGE
    value: 0.816
    std: 0.001
    paper_value: 0.816
    paper_std: 0.001
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.816
    true_std: 0.001
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.816
    sort_std: 0.001
    global_rank: 388
    paper_rank: 388
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HomoGCL
    model_key: homogcl
    model_plain: HomoGCL
    value: 0.811
    std: 0.003
    paper_value: 0.811
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.811
    at_pub_std: 0.003
    at_pub_source_arxiv: '2306.09614'
    at_pub_source_title: 'HomoGCL: Rethinking Homophily in Graph Contrastive Learning'
    at_pub_source_date_iso: '2023-06-16'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.811
    true_std: 0.003
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.811
    sort_std: 0.003
    global_rank: 414
    paper_rank: 414
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.8
    std: 0.001
    paper_value: 0.8
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.806
    at_pub_std: 0.004
    at_pub_source_arxiv: '2402.10468'
    at_pub_source_title: Adversarial Curriculum Graph Contrastive Learning with Pair-wise
      Augmentation
    at_pub_source_date_iso: '2024-02-16'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.006000000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.808
    true_std: 0.006
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.008000000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.006
    global_rank: 434
    paper_rank: 499
    rank_delta: 65
    rank_delta_abs: 65
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Adversarial Curriculum Graph Contrastive Learning with
      Pair-wise Augmentation
    comparison_source_arxiv: '2402.10468'
    is_best: false
    is_std_outlier: false
  - model: gCooL
    model_key: gcool
    model_plain: gCooL
    value: 0.802
    std: 0.004
    paper_value: 0.802
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.805
    true_std: 0.004
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.0030000000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.805
    sort_std: 0.004
    global_rank: 457
    paper_rank: 479
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: G-BT
    model_key: g-bt
    model_plain: G-BT
    value: 0.804
    std: 0.001
    paper_value: 0.804
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
    protocol_note: Planetoid split (Yang et et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.804
    true_std: 0.006
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.804
    sort_std: 0.006
    global_rank: 464
    paper_rank: 464
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RGRL
    model_key: rgrl
    model_plain: RGRL
    value: 0.798
    std: 0.003
    paper_value: 0.798
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
    protocol_note: Planetoid split (Yang et al. 2016) for node classification
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.798
    true_std: 0.003
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.798
    sort_std: 0.003
    global_rank: 528
    paper_rank: 528
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
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: WikiCS
  rows:
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.7719
    std: 0.0012
    paper_value: 0.7719
    paper_std: 0.0012
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9302
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-04-11'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.1583
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9302
    true_std: 0.0011
    value_gap_source_arxiv: '2204.04874'
    value_gap_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    value_gap_source_is_current_paper: false
    value_gap: 0.1583
    has_value_note: false
    value_note: ''
    sort_value: 0.9302
    sort_std: 0.0011
    global_rank: 1
    paper_rank: 203
    rank_delta: 202
    rank_delta_abs: 202
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: true
    is_std_outlier: false
  - model: RSE + RGCN (70b)
    model_key: rse + rgcn (70b)
    model_plain: RSE + RGCN (70b)
    value: 0.8852
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.18581'
    title: 'Unleashing the Potential of Text-attributed Graphs: Automatic Relation
      Decomposition via Large Language Models'
    date: May 28, 2024
    date_display: May 2024
    date_iso: '2024-05-28'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: mixed
    feature_source_evidence: leverages the capability of Large Language Models (LLMs)
      to decompose the graph structure by analyzing raw text attributes
    is_global_top: true
    global_rank: 2
    sort_value: 0.8852
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LEMP+T
    model_key: lemp+t
    model_plain: LEMP+T
    value: 0.8825
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8825
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8771
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
    arxiv_id: '2505.19762'
    title: 'Language Models as Messengers: Enhancing Message Passing in Heterophilic
      Graph Learning'
    date: May 26, 2025
    date_display: May 2025
    date_iso: '2025-05-26'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 9
    sort_value: 0.8771
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7765
    std: 0.0011
    paper_value: 0.7765
    paper_std: 0.0011
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8279
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2405.18581'
    at_pub_source_title: 'Unleashing the Potential of Text-attributed Graphs: Automatic
      Relation Decomposition via Large Language Models'
    at_pub_source_date_iso: '2024-05-28'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-05-26'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0514
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8533
    true_std: null
    value_gap_source_arxiv: '2505.19762'
    value_gap_source_title: 'Language Models as Messengers: Enhancing Message Passing
      in Heterophilic Graph Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.07679999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.8533
    sort_std: null
    global_rank: 31
    paper_rank: 187
    rank_delta: 156
    rank_delta_abs: 156
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Unleashing the Potential of Text-attributed Graphs:
      Automatic Relation Decomposition via Large Language Models'
    comparison_source_arxiv: '2405.18581'
    is_best: false
    is_std_outlier: false
  - model: RGRL
    model_key: rgrl
    model_plain: RGRL
    value: 0.7878
    std: 0.0064
    paper_value: 0.7878
    paper_std: 0.0064
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8029
    at_pub_std: 0.0072
    at_pub_source_arxiv: '2208.10493'
    at_pub_source_title: Relational Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2022-08-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-08-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.015100000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8029
    true_std: 0.0072
    value_gap_source_arxiv: '2208.10493'
    value_gap_source_title: Relational Self-Supervised Learning on Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.015100000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8029
    sort_std: 0.0072
    global_rank: 89
    paper_rank: 147
    rank_delta: 58
    rank_delta_abs: 58
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Relational Self-Supervised Learning on Graphs
    comparison_source_arxiv: '2208.10493'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.7864
    std: 0.0033
    paper_value: 0.7864
    paper_std: 0.0033
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8014
    at_pub_std: 0.48
    at_pub_source_arxiv: '2102.06514'
    at_pub_source_title: Large-Scale Representation Learning on Graphs via Bootstrapping
    at_pub_source_date_iso: '2021-02-12'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.015000000000000013
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8014
    true_std: 0.0048
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.015000000000000013
    has_value_note: false
    value_note: ''
    sort_value: 0.8014
    sort_std: 0.0048
    global_rank: 94
    paper_rank: 152
    rank_delta: 58
    rank_delta_abs: 58
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BGRL
    model_key: bgrl
    model_plain: BGRL
    value: 0.7841
    std: 0.0009
    paper_value: 0.7841
    paper_std: 0.0009
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-12-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.015900000000000025
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8
    true_std: 0.001
    value_gap_source_arxiv: '2412.21151'
    value_gap_source_title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    value_gap_source_is_current_paper: false
    value_gap: 0.015900000000000025
    has_value_note: false
    value_note: ''
    sort_value: 0.8
    sort_std: 0.001
    global_rank: 100
    paper_rank: 162
    rank_delta: 62
    rank_delta_abs: 62
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning Graph Augmentations to Learn Graph Representations
    comparison_source_arxiv: '2201.09830'
    is_best: false
    is_std_outlier: false
  - model: SSGE
    model_key: ssge
    model_plain: SSGE
    value: 0.7918
    std: 0.0057
    paper_value: 0.7918
    paper_std: 0.0057
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7919
    true_std: 0.0057
    value_gap_source_arxiv: '2506.20362'
    value_gap_source_title: Self-Supervised Graph Learning via Spectral Bootstrapping
      and Laplacian-Based Augmentations
    value_gap_source_is_current_paper: false
    value_gap: 0.00010000000000010001
    has_value_note: false
    value_note: ''
    sort_value: 0.7919
    sort_std: 0.0057
    global_rank: 129
    paper_rank: 129
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: COSTA
    model_key: costa
    model_plain: COSTA
    value: 0.7882
    std: 0.0012
    paper_value: 0.7882
    paper_std: 0.0012
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7912
    at_pub_std: 0.0002
    at_pub_source_arxiv: '2209.13964'
    at_pub_source_title: Graph Soft-Contrastive Learning via Neighborhood Ranking
    at_pub_source_date_iso: '2022-09-28'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2026-05-04'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0030000000000000027
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7912
    true_std: 0.0002
    value_gap_source_arxiv: '2605.03076'
    value_gap_source_title: Adaptive Negative Scheduling for Graph Contrastive Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0030000000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.7912
    sort_std: 0.0002
    global_rank: 130
    paper_rank: 146
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Soft-Contrastive Learning via Neighborhood Ranking
    comparison_source_arxiv: '2209.13964'
    is_best: false
    is_std_outlier: false
  - model: CCA-SSG
    model_key: cca-ssg
    model_plain: CCA-SSG
    value: 0.7792
    std: 0.0065
    paper_value: 0.7792
    paper_std: 0.0065
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7908
    at_pub_std: 0.0053
    at_pub_source_arxiv: '2312.02619'
    at_pub_source_title: Rethinking and Simplifying Bootstrapped Graph Latents
    at_pub_source_date_iso: '2023-12-05'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-08-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.011599999999999944
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7908
    true_std: 0.0053
    value_gap_source_arxiv: '2408.05087'
    value_gap_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.011599999999999944
    has_value_note: false
    value_note: ''
    sort_value: 0.7908
    sort_std: 0.0053
    global_rank: 131
    paper_rank: 177
    rank_delta: 46
    rank_delta_abs: 46
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AFGRL
    model_key: afgrl
    model_plain: AFGRL
    value: 0.7762
    std: 0.0049
    paper_value: 0.7762
    paper_std: 0.0049
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7762
    at_pub_std: 0.0049
    at_pub_source_arxiv: '2112.02472'
    at_pub_source_title: Augmentation-Free Self-Supervised Learning on Graphs
    at_pub_source_date_iso: '2021-12-05'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2024-12-30'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.789
    true_std: 0.006
    value_gap_source_arxiv: '2412.21151'
    value_gap_source_title: 'PyG-SSL: A Graph Self-Supervised Learning Toolkit'
    value_gap_source_is_current_paper: false
    value_gap: 0.012800000000000034
    has_value_note: false
    value_note: ''
    sort_value: 0.789
    sort_std: 0.006
    global_rank: 144
    paper_rank: 187
    rank_delta: 43
    rank_delta_abs: 43
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HomoGCL
    model_key: homogcl
    model_plain: HomoGCL
    value: 0.7826
    std: 0.0032
    paper_value: 0.7826
    paper_std: 0.0032
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.7884
    true_std: 0.0047
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: 0.005800000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.7884
    sort_std: 0.0047
    global_rank: 146
    paper_rank: 168
    rank_delta: 22
    rank_delta_abs: 22
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: gCooL
    model_key: gcool
    model_plain: gCooL
    value: 0.7874
    std: 0.0004
    paper_value: 0.7874
    paper_std: 0.0004
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7874
    at_pub_std: 0.0004
    at_pub_source_arxiv: '2408.05087'
    at_pub_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2024-08-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-05-08'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7874
    true_std: 0.0004
    value_gap_source_arxiv: '2505.05533'
    value_gap_source_title: Rethinking Graph Contrastive Learning through Relative
      Similarity Preservation
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7874
    sort_std: 0.0004
    global_rank: 148
    paper_rank: 148
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.7825
    std: 0.0056
    paper_value: 0.7825
    paper_std: 0.0056
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7825
    at_pub_std: 0.0056
    at_pub_source_arxiv: '2408.05087'
    at_pub_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2024-08-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2025-07-20'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7865
    true_std: 0.069
    value_gap_source_arxiv: '2507.19526'
    value_gap_source_title: Quantizing Text-attributed Graphs for Semantic-Structural
      Integration
    value_gap_source_is_current_paper: false
    value_gap: 0.0040000000000000036
    has_value_note: false
    value_note: ''
    sort_value: 0.7865
    sort_std: 0.069
    global_rank: 152
    paper_rank: 168
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: GGD
    model_key: ggd
    model_plain: GGD
    value: 0.7862
    std: 0.0047
    paper_value: 0.7862
    paper_std: 0.0047
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7862
    true_std: 0.0047
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7862
    sort_std: 0.0047
    global_rank: 154
    paper_rank: 154
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCA
    model_key: gca
    model_plain: GCA
    value: 0.7835
    std: 0.0005
    paper_value: 0.7835
    paper_std: 0.0005
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.784
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.000500000000000056
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.784
    true_std: 0.001
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.000500000000000056
    has_value_note: false
    value_note: ''
    sort_value: 0.784
    sort_std: 0.001
    global_rank: 163
    paper_rank: 164
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MERIT
    model_key: merit
    model_plain: MERIT
    value: 0.7835
    std: 0.0005
    paper_value: 0.7835
    paper_std: 0.0005
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7835
    true_std: 0.0005
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7835
    sort_std: 0.0005
    global_rank: 165
    paper_rank: 165
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAE
    model_key: gae
    model_plain: GAE
    value: 0.7787
    std: 0.0053
    paper_value: 0.7787
    paper_std: 0.0053
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7397
    at_pub_std: 0.0016
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.038999999999999924
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7787
    true_std: 0.0053
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7787
    sort_std: 0.0053
    global_rank: 181
    paper_rank: 181
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    comparison_source_arxiv: '2204.04874'
    is_best: false
    is_std_outlier: false
  - model: VGAE
    model_key: vgae
    model_plain: VGAE
    value: 0.7787
    std: 0.0053
    paper_value: 0.7787
    paper_std: 0.0053
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7563
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.022399999999999975
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7787
    true_std: 0.0053
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7787
    sort_std: 0.0053
    global_rank: 180
    paper_rank: 180
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: MVGRL
    model_key: mvgrl
    model_plain: MVGRL
    value: 0.7757
    std: 0.0046
    paper_value: 0.7757
    paper_std: 0.0046
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7757
    at_pub_std: 0.0046
    at_pub_source_arxiv: '2408.05087'
    at_pub_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2024-08-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7757
    true_std: 0.0046
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7757
    sort_std: 0.0046
    global_rank: 190
    paper_rank: 190
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.7435
    std: 0.0006
    paper_value: 0.7435
    paper_std: 0.0006
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7721
    at_pub_std: null
    at_pub_source_arxiv: '2110.15742'
    at_pub_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    at_pub_source_date_iso: '2021-10-29'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-29'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.02859999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7721
    true_std: null
    value_gap_source_arxiv: '2110.15742'
    value_gap_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    value_gap_source_is_current_paper: false
    value_gap: 0.02859999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.7721
    sort_std: null
    global_rank: 199
    paper_rank: 240
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Barlow Graph Auto-Encoder for Unsupervised Network Embedding
    comparison_source_arxiv: '2110.15742'
    is_best: false
    is_std_outlier: false
  - model: G-BT
    model_key: g-bt
    model_plain: G-BT
    value: 0.7683
    std: 0.0073
    paper_value: 0.7683
    paper_std: 0.0073
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7683
    at_pub_std: 0.0073
    at_pub_source_arxiv: '2408.05087'
    at_pub_source_title: Bootstrap Latents of Nodes and Neighbors for Graph Self-Supervised
      Learning
    at_pub_source_date_iso: '2024-08-09'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-10-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7683
    true_std: 0.0073
    value_gap_source_arxiv: '2411.01157'
    value_gap_source_title: Negative-Free Self-Supervised Gaussian Embedding of Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7683
    sort_std: 0.0073
    global_rank: 212
    paper_rank: 212
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.7485
    std: 0.0008
    paper_value: 0.7485
    paper_std: 0.0008
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
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.749
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.0004999999999999449
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.749
    true_std: 0.001
    value_gap_source_arxiv: '2205.15746'
    value_gap_source_title: Omni-Granular Ego-Semantic Propagation for Self-Supervised
      Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.0004999999999999449
    has_value_note: false
    value_note: ''
    sort_value: 0.749
    sort_std: 0.001
    global_rank: 234
    paper_rank: 234
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7198
    std: 0.0
    paper_value: 0.7198
    paper_std: 0.0
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7272
    at_pub_std: 0.0043
    at_pub_source_arxiv: '2405.20445'
    at_pub_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    at_pub_source_date_iso: '2024-05-30'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2025-12-12'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.007399999999999962
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7469
    true_std: 0.0085
    value_gap_source_arxiv: '2512.11561'
    value_gap_source_title: 'View Space: Learning Representation across Arbitrary
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.027100000000000013
    has_value_note: false
    value_note: ''
    sort_value: 0.7469
    sort_std: 0.0085
    global_rank: 237
    paper_rank: 255
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Fully-inductive Node Classification on Arbitrary Graphs
    comparison_source_arxiv: '2405.20445'
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.7179
    std: 0.0005
    paper_value: 0.7179
    paper_std: 0.0005
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
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard split for WikiCS node classification using logistic regression
      on learned representations.
    date: Oct 1, 2024
    date_display: Oct 2024
    date_iso: '2024-10-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.718
    at_pub_std: 0.001
    at_pub_source_arxiv: '2201.09830'
    at_pub_source_title: Learning Graph Augmentations to Learn Graph Representations
    at_pub_source_date_iso: '2022-01-24'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-01-24'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 9.999999999998899e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.718
    true_std: 0.001
    value_gap_source_arxiv: '2201.09830'
    value_gap_source_title: Learning Graph Augmentations to Learn Graph Representations
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999998899e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.718
    sort_std: 0.001
    global_rank: 261
    paper_rank: 261
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
  - *id003
  - *id004
  - *id005
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Cora
      dataset_slug: cora
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: WikiCS
      dataset_slug: wikics
    - dataset: Coauthor-CS
      dataset_slug: coauthor-cs
single_proposed_model: SSGE
main_figure: /figures/2411.01157/main_figure.jpegoptim.jpg
---

