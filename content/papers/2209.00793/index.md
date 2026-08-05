---
title: Structure-Preserving Graph Representation Learning
arxiv_id: '2209.00793'
source_url: ''
authors:
- name: Ruiyi Fang
  orcid: null
  s2_author_id: '2160814646'
  s2_url: null
- name: Liangjiang Wen
  orcid: null
  s2_author_id: '147383784'
  s2_url: null
- name: Zhao Kang
  orcid: null
  s2_author_id: '152200830'
  s2_url: null
- name: Jianzhuang Liu
  orcid: null
  s2_author_id: '2144167531'
  s2_url: null
published_date: Sep 2, 2022
published_date_iso: '2022-09-02'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Though graph representation learning (GRL) has made significant progress,
  it is still a challenge to extract and embed the rich topological structure and
  feature information in an adequate way. Most existing methods focus on local structure
  and fail to fully incorporate the global topological structure. To this end, we
  propose a novel Structure-Preserving Graph Representation Learning (SPGRL) method,
  to fully capture the structure information of graphs. Specifically, to reduce the
  uncertainty and misinformation of the original graph, we construct a feature graph
  as a complementary view via $k$-Nearest Neighbor method. The feature graph can be
  used to contrast at node-level to capture the local relation. Besides, we retain
  the global topological structure information by maximizing the mutual information
  (MI) of the whole graph and feature embeddings, which is theoretically reduced to
  exchanging the feature embeddings of the feature and the original graphs to reconstruct
  themselves. Extensive experiments show that our method has quite superior performance
  on semi-supervised node classification task and excellent robustness under noise
  perturbation on graph structure or node features. The source code is available at.
codebase_url: https://github.com/uestc-lese/SPGRL
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SPGRL
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
  rows:
  - model: SPGRL
    model_key: spgrl
    model_plain: SPGRL
    value: 0.9398
    std: null
    paper_value: 0.9398
    paper_std: null
    metric: F1
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-02'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9398
    true_std: null
    value_gap_source_arxiv: '2209.00793'
    value_gap_source_title: Structure-Preserving Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9398
    sort_std: null
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
  - model: CDC
    model_key: cdc
    model_plain: CDC
    value: 0.936
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2403.03670'
    title: 'CDC: A Simple Framework for Complex Data Clustering'
    date: Mar 6, 2024
    date_display: Mar 2024
    date_iso: '2024-03-06'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.936
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SynC SSL
    model_key: sync ssl
    model_plain: SynC SSL
    value: 0.9274
    std: 0.0004
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2406.15797'
    title: 'SynC: Synergistic Boosting of Structure and Representation for Deep Graph
      Clustering'
    date: Jun 22, 2024
    date_display: Jun 2024
    date_iso: '2024-06-22'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: https://github.com/Marigoldwu/SynC
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9274
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SCRL
    model_key: scrl
    model_plain: SCRL
    value: 0.9179
    std: null
    paper_value: 0.9179
    paper_std: null
    metric: F1
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
    source_ref: liu2021self
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-02'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9179
    true_std: null
    value_gap_source_arxiv: '2209.00793'
    value_gap_source_title: Structure-Preserving Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9179
    sort_std: null
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8782
    std: null
    paper_value: 0.8782
    paper_std: null
    metric: F1
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
    source_ref: kipf2017semi
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9049
    at_pub_std: null
    at_pub_source_arxiv: '2007.02265'
    at_pub_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-07-05'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
    gap_vs_at_pub: 0.026700000000000057
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9049
    true_std: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.026700000000000057
    has_value_note: false
    value_note: ''
    sort_value: 0.9049
    sort_std: null
    global_rank: 17
    paper_rank: 31
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    comparison_source_arxiv: '2007.02265'
    is_best: false
    is_std_outlier: false
  - model: AMGCN
    model_key: amgcn
    model_plain: AMGCN
    value: 0.9043
    std: null
    paper_value: 0.9043
    paper_std: null
    metric: F1
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
    source_ref: wang2020gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-02'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9043
    true_std: null
    value_gap_source_arxiv: '2209.00793'
    value_gap_source_title: Structure-Preserving Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9043
    sort_std: null
    global_rank: 18
    paper_rank: 18
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
    value: 0.904
    std: null
    paper_value: 0.904
    paper_std: null
    metric: F1
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
    source_ref: veli2018deep
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-02'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.904
    true_std: null
    value_gap_source_arxiv: '2209.00793'
    value_gap_source_title: Structure-Preserving Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.904
    sort_std: null
    global_rank: 20
    paper_rank: 20
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8744
    std: null
    paper_value: 0.8744
    paper_std: null
    metric: F1
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
    source_ref: velickovic2018graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9039
    at_pub_std: null
    at_pub_source_arxiv: '2007.02265'
    at_pub_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-07-05'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
    gap_vs_at_pub: 0.02950000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9039
    true_std: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.02950000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.9039
    sort_std: null
    global_rank: 21
    paper_rank: 31
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    comparison_source_arxiv: '2007.02265'
    is_best: false
    is_std_outlier: false
  - model: GMI
    model_key: gmi
    model_plain: GMI
    value: 0.9
    std: null
    paper_value: 0.9
    paper_std: null
    metric: F1
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
    source_ref: peng2020graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-02'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9
    true_std: null
    value_gap_source_arxiv: '2209.00793'
    value_gap_source_title: Structure-Preserving Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9
    sort_std: null
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.89
    std: null
    paper_value: 0.89
    paper_std: null
    metric: F1
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
    source_ref: Zhu:2020vf
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-02'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.89
    true_std: null
    value_gap_source_arxiv: '2209.00793'
    value_gap_source_title: Structure-Preserving Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.89
    sort_std: null
    global_rank: 28
    paper_rank: 28
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
    value: 0.8879
    std: null
    paper_value: 0.8879
    paper_std: null
    metric: F1
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
    source_ref: zhu2021graph
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-02'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8879
    true_std: null
    value_gap_source_arxiv: '2209.00793'
    value_gap_source_title: Structure-Preserving Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8879
    sort_std: null
    global_rank: 30
    paper_rank: 30
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DEMO-Net
    model_key: demo-net
    model_plain: DEMO-Net
    value: 0.8416
    std: null
    paper_value: 0.8416
    paper_std: null
    metric: F1
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
    source_ref: wu2019net
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8483
    at_pub_std: null
    at_pub_source_arxiv: '2007.02265'
    at_pub_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-07-05'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
    gap_vs_at_pub: 0.006700000000000039
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8483
    true_std: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.006700000000000039
    has_value_note: false
    value_note: ''
    sort_value: 0.8483
    sort_std: null
    global_rank: 35
    paper_rank: 36
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    comparison_source_arxiv: '2007.02265'
    is_best: false
    is_std_outlier: false
  - model: MixHop
    model_key: mixhop
    model_plain: MixHop
    value: 0.814
    std: null
    paper_value: 0.814
    paper_std: null
    metric: F1
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
    source_ref: abu2019mixhop
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8224
    at_pub_std: null
    at_pub_source_arxiv: '2007.02265'
    at_pub_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-07-05'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
    gap_vs_at_pub: 0.008400000000000074
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8224
    true_std: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.008400000000000074
    has_value_note: false
    value_note: ''
    sort_value: 0.8224
    sort_std: null
    global_rank: 38
    paper_rank: 39
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    comparison_source_arxiv: '2007.02265'
    is_best: false
    is_std_outlier: false
  - model: kNN-GCN
    model_key: knn-gcn
    model_plain: kNN-GCN
    value: 0.7814
    std: null
    paper_value: 0.7814
    paper_std: null
    metric: F1
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
    source_ref: wang2020gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8195
    at_pub_std: null
    at_pub_source_arxiv: '2007.02265'
    at_pub_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-07-05'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
    gap_vs_at_pub: 0.03810000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8195
    true_std: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.03810000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8195
    sort_std: null
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    comparison_source_arxiv: '2007.02265'
    is_best: false
    is_std_outlier: false
  - model: ChebNet
    model_key: chebnet
    model_plain: ChebNet
    value: 0.7486
    std: null
    paper_value: 0.7486
    paper_std: null
    metric: F1
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
    source_ref: defferrard2016convolutional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-02'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7486
    true_std: null
    value_gap_source_arxiv: '2209.00793'
    value_gap_source_title: Structure-Preserving Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7486
    sort_std: null
    global_rank: 40
    paper_rank: 40
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
    value: 0.6211
    std: null
    paper_value: 0.6211
    paper_std: null
    metric: F1
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
    source_ref: perozzi2014deepwalk
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6699
    at_pub_std: null
    at_pub_source_arxiv: '2007.02265'
    at_pub_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-07-05'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
    gap_vs_at_pub: 0.048800000000000066
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6699
    true_std: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.048800000000000066
    has_value_note: false
    value_note: ''
    sort_value: 0.6699
    sort_std: null
    global_rank: 41
    paper_rank: 44
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    comparison_source_arxiv: '2007.02265'
    is_best: false
    is_std_outlier: false
  - model: SLAPS
    model_key: slaps
    model_plain: SLAPS
    value: 0.6
    std: null
    paper_value: 0.6
    paper_std: null
    metric: F1
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
    source_ref: fatemi2021slaps
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-09-02'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6
    true_std: null
    value_gap_source_arxiv: '2209.00793'
    value_gap_source_title: Structure-Preserving Graph Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6
    sort_std: null
    global_rank: 51
    paper_rank: 51
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINE
    model_key: line
    model_plain: LINE
    value: 0.4012
    std: null
    paper_value: 0.4012
    paper_std: null
    metric: F1
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
    source_ref: tang2015line
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.4992
    at_pub_std: null
    at_pub_source_arxiv: '2007.02265'
    at_pub_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-07-05'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2020-07-05'
    value_gap_source_date_label: KDD 2020
    gap_vs_at_pub: 0.09799999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4992
    true_std: null
    value_gap_source_arxiv: '2007.02265'
    value_gap_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.09799999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.4992
    sort_std: null
    global_rank: 53
    paper_rank: 53
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    comparison_source_arxiv: '2007.02265'
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - F1
  metric: F1
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
single_proposed_model: SPGRL
main_figure: /figures/2209.00793/main_figure.jpegoptim.jpg
---

