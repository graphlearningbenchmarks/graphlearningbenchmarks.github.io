---
title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive Learning on Hypergraphs'
arxiv_id: '2206.04739'
source_url: ''
authors:
- name: Dongjin Lee
  orcid: null
  s2_author_id: '2109519939'
  s2_url: null
- name: Kijung Shin
  orcid: null
  s2_author_id: '40553270'
  s2_url: null
published_date: Jun 9, 2022
published_date_iso: '2022-06-09'
published_venue: AAAI 2022
published_conference: AAAI 2022
published_conference_short: AAAI
published_conference_slug: aaai
abstract: Although machine learning on hypergraphs has attracted considerable attention,
  most of the works have focused on (semi-)supervised learning, which may cause heavy
  labeling costs and poor generalization. Recently, contrastive learning has emerged
  as a successful unsupervised representation learning method. Despite the prosperous
  development of contrastive learning in other domains, contrastive learning on hypergraphs
  remains little explored. In this paper, we propose TriCL (-directional ontrastive
  earning), a general framework for contrastive learning on hypergraphs. Its main
  idea is tri-directional contrast, and specifically, it aims to maximize in two augmented
  views the agreement (a) between the same node, (b) between the same group of nodes,
  and (c) between each group and its members. Together with simple but surprisingly
  effective data augmentation and negative sampling schemes, these three forms of
  contrast enable TriCL to capture both node- and group-level structural information
  in node embeddings. Our extensive experiments using 14 baseline approaches, 10 datasets,
  and two tasks demonstrate the effectiveness of TriCL, and most noticeably, TriCL
  almost consistently outperforms not just unsupervised competitors but also (semi-)supervised
  competitors mostly by significant margins for node classification. The code and
  datasets are available at.
codebase_url: https://github.com/wooner49/TriCL
extraction_model: google/gemma-4-26B-A4B-it
has_results: true
paper_type: method
proposed_models:
- TriCL-N
- TriCL-NG
- TriCL (L_n + L_g)
mrr: 0.0022
adjusted_mrr: 0.0015
mrr_dataset_count: 2
benchmark_categories:
- Classic
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
- benchmark: Heterogeneous Graph Benchmarks
  benchmark_slug: heterogeneous-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id002
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
    value: 0.6607
    std: 0.024
    paper_value: 0.6607
    paper_std: 0.024
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split
      (clique expansion applied).
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7943
    at_pub_std: 0.0026
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.13360000000000005
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
    value_gap: 0.21620000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.8769
    sort_std: 0.004
    global_rank: 21
    paper_rank: 819
    rank_delta: 798
    rank_delta_abs: 798
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.6762
    std: 0.025
    paper_value: 0.6762
    paper_std: 0.025
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split
      (clique expansion applied).
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8013
    at_pub_std: 0.0062
    at_pub_source_arxiv: '2110.13094'
    at_pub_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    at_pub_source_date_iso: '2021-10-25'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.1251
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
    value_gap: 0.13180000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.808
    sort_std: 0.0026
    global_rank: 46
    paper_rank: 765
    rank_delta: 719
    rank_delta_abs: 719
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Gophormer: Ego-Graph Transformer for Node Classification'
    comparison_source_arxiv: '2110.13094'
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.6881
    std: 0.018
    paper_value: 0.6881
    paper_std: 0.018
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split
      (clique expansion applied).
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.7882
    at_pub_std: 0.0015
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.10009999999999997
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
    value_gap: 0.10089999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.789
    sort_std: 0.002
    global_rank: 83
    paper_rank: 723
    rank_delta: 640
    rank_delta_abs: 640
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.6865
    std: 0.017
    paper_value: 0.6865
    paper_std: 0.017
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split
      (clique expansion applied).
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.717
    at_pub_std: 0.006
    at_pub_source_arxiv: '2009.07111'
    at_pub_source_title: Contrastive and Generative Graph Convolutional Networks for
      Graph-based Semi-Supervised Learning
    at_pub_source_date_iso: '2020-09-15'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.03049999999999997
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
    value_gap: 0.058499999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.001
    global_rank: 245
    paper_rank: 733
    rank_delta: 488
    rank_delta_abs: 488
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Contrastive and Generative Graph Convolutional Networks
      for Graph-based Semi-Supervised Learning
    comparison_source_arxiv: '2009.07111'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6206
    std: 0.023
    paper_value: 0.6206
    paper_std: 0.023
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6958
    at_pub_std: 0.0231
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2025-08-24'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.07519999999999993
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
    value_gap: 0.10829999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.7289
    sort_std: 0.001
    global_rank: 401
    paper_rank: 886
    rank_delta: 485
    rank_delta_abs: 485
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    comparison_source_arxiv: '2112.13507'
    is_best: false
    is_std_outlier: false
  - model: HyperGCN
    model_key: hypergcn
    model_plain: HyperGCN
    value: 0.5992
    std: 0.096
    paper_value: 0.5992
    paper_std: 0.096
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7276
    true_std: 0.0112
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: false
    value_gap: 0.12840000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.7276
    sort_std: 0.0112
    global_rank: 411
    paper_rank: 907
    rank_delta: 496
    rank_delta_abs: 496
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HNHN
    model_key: hnhn
    model_plain: HNHN
    value: 0.6728
    std: 0.022
    paper_value: 0.6728
    paper_std: 0.022
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7264
    true_std: 0.0157
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: false
    value_gap: 0.05360000000000009
    has_value_note: false
    value_note: ''
    sort_value: 0.7264
    sort_std: 0.0157
    global_rank: 425
    paper_rank: 779
    rank_delta: 354
    rank_delta_abs: 354
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TriCL (L_n + L_g)
    model_key: tricl (l_n + l_g)
    model_plain: TriCL (L_n + L_g)
    value: 0.7202
    std: 0.012
    paper_value: 0.7202
    paper_std: 0.012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7202
    true_std: 0.012
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7202
    sort_std: 0.012
    global_rank: 514
    paper_rank: 514
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TriCL-NG
    model_key: tricl-ng
    model_plain: TriCL-NG
    value: 0.7138
    std: 0.012
    paper_value: 0.7138
    paper_std: 0.012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7138
    true_std: 0.012
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7138
    sort_std: 0.012
    global_rank: 583
    paper_rank: 583
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TriCL-N
    model_key: tricl-n
    model_plain: TriCL-N
    value: 0.7028
    std: 0.015
    paper_value: 0.7028
    paper_std: 0.015
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7028
    true_std: 0.015
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7028
    sort_std: 0.015
    global_rank: 671
    paper_rank: 671
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S2-HHGR
    model_key: s2-hhgr
    model_plain: S2-HHGR
    value: 0.6821
    std: 0.018
    paper_value: 0.6821
    paper_std: 0.018
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6821
    true_std: 0.018
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6821
    sort_std: 0.018
    global_rank: 746
    paper_rank: 746
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AllSet
    model_key: allset
    model_plain: AllSet
    value: 0.6783
    std: 0.018
    paper_value: 0.6783
    paper_std: 0.018
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6783
    true_std: 0.018
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6783
    sort_std: 0.018
    global_rank: 760
    paper_rank: 760
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniGCN
    model_key: unigcn
    model_plain: UniGCN
    value: 0.664
    std: 0.019
    paper_value: 0.664
    paper_std: 0.019
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.664
    true_std: 0.019
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.664
    sort_std: 0.019
    global_rank: 804
    paper_rank: 804
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGNN
    model_key: hgnn
    model_plain: HGNN
    value: 0.6616
    std: 0.023
    paper_value: 0.6616
    paper_std: 0.023
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6616
    true_std: 0.023
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6616
    sort_std: 0.023
    global_rank: 816
    paper_rank: 816
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.5385
    std: 0.019
    paper_value: 0.5385
    paper_std: 0.019
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split
      (clique expansion applied).
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.6552
    at_pub_std: 0.0018
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.11670000000000003
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
    value_gap: 0.11670000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.6552
    sort_std: 0.0018
    global_rank: 832
    paper_rank: 937
    rank_delta: 105
    rank_delta_abs: 105
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: HyperConv
    model_key: hyperconv
    model_plain: HyperConv
    value: 0.6412
    std: 0.026
    paper_value: 0.6412
    paper_std: 0.026
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6412
    true_std: 0.026
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6412
    sort_std: 0.026
    global_rank: 858
    paper_rank: 858
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Random-Init
    model_key: random-init
    model_plain: Random-Init
    value: 0.6044
    std: 0.025
    paper_value: 0.6044
    paper_std: 0.025
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6044
    true_std: 0.025
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6044
    sort_std: 0.025
    global_rank: 901
    paper_rank: 901
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HyperSAGE
    model_key: hypersage
    model_plain: HyperSAGE
    value: 0.5243
    std: 0.094
    paper_value: 0.5243
    paper_std: 0.094
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on CiteSeer using the standard Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5243
    true_std: 0.094
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5243
    sort_std: 0.094
    global_rank: 943
    paper_rank: 943
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
- &id003
  dataset: DBLP
  rows:
  - model: HG-SCM
    model_key: hg-scm
    model_plain: HG-SCM
    value: 0.949
    std: 0.0015
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2312.05757'
    title: 'Towards Human-like Perception: Learning Structural Causal Model in Heterogeneous
      Graph'
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    venue: Information Processing & Management
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.949
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SeHGNN
    model_key: sehgnn
    model_plain: SeHGNN
    value: 0.9489
    std: 0.0018
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2312.05757'
    title: 'Towards Human-like Perception: Learning Structural Causal Model in Heterogeneous
      Graph'
    date: Dec 10, 2023
    date_display: Dec 2023
    date_iso: '2023-12-10'
    venue: Information Processing & Management
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9489
    sort_std: 0.0018
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AdvSynGNN
    model_key: advsyngnn
    model_plain: AdvSynGNN
    value: 0.9486
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.17071'
    title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial Synthesis
      and Self-Corrective Propagation'
    date: Feb 19, 2026
    date_display: Feb 2026
    date_iso: '2026-02-19'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9486
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TriCL (L_n + L_g)
    model_key: tricl (l_n + l_g)
    model_plain: TriCL (L_n + L_g)
    value: 0.9112
    std: 0.001
    paper_value: 0.9112
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9112
    true_std: 0.001
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9112
    sort_std: 0.001
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
  - model: TriCL-NG
    model_key: tricl-ng
    model_plain: TriCL-NG
    value: 0.9094
    std: 0.001
    paper_value: 0.9094
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9094
    true_std: 0.001
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9094
    sort_std: 0.001
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
  - model: TriCL-N
    model_key: tricl-n
    model_plain: TriCL-N
    value: 0.9088
    std: 0.001
    paper_value: 0.9088
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9088
    true_std: 0.001
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9088
    sort_std: 0.001
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
  - model: UniGCN
    model_key: unigcn
    model_plain: UniGCN
    value: 0.9031
    std: 0.002
    paper_value: 0.9031
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9031
    true_std: 0.002
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9031
    sort_std: 0.002
    global_rank: 25
    paper_rank: 25
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AllSet
    model_key: allset
    model_plain: AllSet
    value: 0.9007
    std: 0.003
    paper_value: 0.9007
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9007
    true_std: 0.003
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9007
    sort_std: 0.003
    global_rank: 27
    paper_rank: 27
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HyperConv
    model_key: hyperconv
    model_plain: HyperConv
    value: 0.8883
    std: 0.002
    paper_value: 0.8883
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8883
    true_std: 0.002
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8883
    sort_std: 0.002
    global_rank: 29
    paper_rank: 29
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S²-HHGR
    model_key: s²-hhgr
    model_plain: S²-HHGR
    value: 0.8869
    std: 0.002
    paper_value: 0.8869
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8869
    true_std: 0.002
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8869
    sort_std: 0.002
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
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8859
    std: 0.001
    paper_value: 0.8859
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.718
    at_pub_std: 0.026
    at_pub_source_arxiv: '2004.13970'
    at_pub_source_title: Directed Graph Convolutional Network
    at_pub_source_date_iso: '2020-04-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.16790000000000005
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8859
    true_std: 0.001
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8859
    sort_std: 0.001
    global_rank: 31
    paper_rank: 31
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Directed Graph Convolutional Network
    comparison_source_arxiv: '2004.13970'
    is_best: false
    is_std_outlier: false
  - model: HGNN
    model_key: hgnn
    model_plain: HGNN
    value: 0.8832
    std: 0.003
    paper_value: 0.8832
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8832
    true_std: 0.003
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8832
    sort_std: 0.003
    global_rank: 32
    paper_rank: 32
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
    value: 0.88
    std: 0.002
    paper_value: 0.88
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.832
    at_pub_std: 0.001
    at_pub_source_arxiv: '2006.04131'
    at_pub_source_title: Deep Graph Contrastive Representation Learning
    at_pub_source_date_iso: '2020-06-07'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.04800000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.88
    true_std: 0.002
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.88
    sort_std: 0.002
    global_rank: 34
    paper_rank: 34
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Deep Graph Contrastive Representation Learning
    comparison_source_arxiv: '2006.04131'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8758
    std: 0.002
    paper_value: 0.8758
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.827
    at_pub_std: null
    at_pub_source_arxiv: '2006.04131'
    at_pub_source_title: Deep Graph Contrastive Representation Learning
    at_pub_source_date_iso: '2020-06-07'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.048800000000000066
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8758
    true_std: 0.002
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8758
    sort_std: 0.002
    global_rank: 36
    paper_rank: 36
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Deep Graph Contrastive Representation Learning
    comparison_source_arxiv: '2006.04131'
    is_best: false
    is_std_outlier: false
  - model: HNHN
    model_key: hnhn
    model_plain: HNHN
    value: 0.8671
    std: 0.012
    paper_value: 0.8671
    paper_std: 0.012
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8671
    true_std: 0.012
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8671
    sort_std: 0.012
    global_rank: 39
    paper_rank: 39
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
    value: 0.8118
    std: 0.002
    paper_value: 0.8118
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8118
    true_std: 0.002
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8118
    sort_std: 0.002
    global_rank: 80
    paper_rank: 80
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HyperSAGE
    model_key: hypersage
    model_plain: HyperSAGE
    value: 0.7963
    std: 0.086
    paper_value: 0.7963
    paper_std: 0.086
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7963
    true_std: 0.086
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7963
    sort_std: 0.086
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
    is_std_outlier: true
  - model: Node2Vec
    model_key: node2vec
    model_plain: Node2Vec
    value: 0.7209
    std: 0.003
    paper_value: 0.7209
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.788
    at_pub_std: null
    at_pub_source_arxiv: '2006.04131'
    at_pub_source_title: Deep Graph Contrastive Representation Learning
    at_pub_source_date_iso: '2020-06-07'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-06-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.06710000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.788
    true_std: null
    value_gap_source_arxiv: '2006.04131'
    value_gap_source_title: Deep Graph Contrastive Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.06710000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.788
    sort_std: null
    global_rank: 94
    paper_rank: 125
    rank_delta: 31
    rank_delta_abs: 31
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Deep Graph Contrastive Representation Learning
    comparison_source_arxiv: '2006.04131'
    is_best: false
    is_std_outlier: false
  - model: HyperGCN
    model_key: hypergcn
    model_plain: HyperGCN
    value: 0.7659
    std: 0.076
    paper_value: 0.7659
    paper_std: 0.076
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7659
    true_std: 0.076
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7659
    sort_std: 0.076
    global_rank: 104
    paper_rank: 104
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: Random-Init
    model_key: random-init
    model_plain: Random-Init
    value: 0.7657
    std: 0.006
    paper_value: 0.7657
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on DBLP split
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7657
    true_std: 0.006
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7657
    sort_std: 0.006
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.7455
    std: 0.0061
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2602.12613'
    title: 'Coden: Efficient Temporal Graph Neural Networks for Continuous Prediction'
    date: Feb 13, 2026
    date_display: Feb 2026
    date_iso: '2026-02-13'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 120
    sort_value: 0.7455
    sort_std: 0.0061
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Micro-F1
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
- &id001
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
    value: 0.8263
    std: 0.006
    paper_value: 0.8263
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Node classification on Pubmed using Planetoid split. Note: GCN
      is applied via clique expansion.'
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.07069999999999999
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
    value_gap: 0.10329999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9296
    sort_std: 0.0015
    global_rank: 19
    paper_rank: 357
    rank_delta: 338
    rank_delta_abs: 338
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
    value: 0.8196
    std: 0.007
    paper_value: 0.8196
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Node classification on Pubmed using Planetoid split. Note: GAT
      is applied via clique expansion.'
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.897
    at_pub_std: null
    at_pub_source_arxiv: '2008.09864'
    at_pub_source_title: Tackling Over-Smoothing for General Graph Convolutional Networks
    at_pub_source_date_iso: '2020-08-22'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.07740000000000002
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
    value_gap: 0.10370000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.9233
    sort_std: 0.0018
    global_rank: 23
    paper_rank: 375
    rank_delta: 352
    rank_delta_abs: 352
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
  - model: GRACE
    model_key: grace
    model_plain: GRACE
    value: 0.8008
    std: 0.007
    paper_value: 0.8008
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Node classification on Pubmed using Planetoid split. Note: GRACE
      is applied via clique expansion.'
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8054
    at_pub_std: 0.0036
    at_pub_source_arxiv: '2204.04874'
    at_pub_source_title: Augmentation-Free Graph Contrastive Learning with Performance
      Guarantee
    at_pub_source_date_iso: '2022-04-11'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2023-06-03'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0046000000000000485
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.07220000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.873
    sort_std: 0.001
    global_rank: 224
    paper_rank: 496
    rank_delta: 272
    rank_delta_abs: 272
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGI
    model_key: dgi
    model_plain: DGI
    value: 0.8083
    std: 0.006
    paper_value: 0.8083
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Node classification on Pubmed using Planetoid split. Note: DGI
      is applied via clique expansion.'
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8703
    at_pub_std: 0.0008
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-07-29'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.061999999999999944
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
    value_gap: 0.0625
    has_value_note: false
    value_note: ''
    sort_value: 0.8708
    sort_std: 0.0017
    global_rank: 235
    paper_rank: 432
    rank_delta: 197
    rank_delta_abs: 197
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.7627
    std: 0.011
    paper_value: 0.7627
    paper_std: 0.011
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.8638
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2112.13507'
    at_pub_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    at_pub_source_date_iso: '2021-12-27'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2023-09-29'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: 0.10109999999999997
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
    value_gap: 0.10629999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.869
    sort_std: 0.0074
    global_rank: 243
    paper_rank: 839
    rank_delta: 596
    rank_delta_abs: 596
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Block Modeling-Guided Graph Convolutional Neural Networks
    comparison_source_arxiv: '2112.13507'
    is_best: false
    is_std_outlier: false
  - model: HGNN
    model_key: hgnn
    model_plain: HGNN
    value: 0.8352
    std: 0.007
    paper_value: 0.8352
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8644
    true_std: 0.0044
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: false
    value_gap: 0.029199999999999893
    has_value_note: false
    value_note: ''
    sort_value: 0.8644
    sort_std: 0.0044
    global_rank: 257
    paper_rank: 332
    rank_delta: 75
    rank_delta_abs: 75
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
    value: 0.7875
    std: 0.009
    paper_value: 0.7875
    paper_std: 0.009
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Node classification on Pubmed using Planetoid split. Note: Node2vec
      is applied via clique expansion.'
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: 0.852
    at_pub_std: 0.0002
    at_pub_source_arxiv: '2203.12265'
    at_pub_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    at_pub_source_date_iso: '2022-03-23'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-03-23'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.0645
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
    value_gap: 0.0645
    has_value_note: false
    value_note: ''
    sort_value: 0.852
    sort_std: 0.0002
    global_rank: 287
    paper_rank: 684
    rank_delta: 397
    rank_delta_abs: 397
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Node Representation Learning in Graph via Node-to-Neighbourhood
      Mutual Information Maximization
    comparison_source_arxiv: '2203.12265'
    is_best: false
    is_std_outlier: false
  - model: TriCL (L_n + L_g)
    model_key: tricl (l_n + l_g)
    model_plain: TriCL (L_n + L_g)
    value: 0.8426
    std: 0.006
    paper_value: 0.8426
    paper_std: 0.006
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split. Full Tri-directional
      contrast.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8426
    true_std: 0.006
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8426
    sort_std: 0.006
    global_rank: 310
    paper_rank: 310
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HNHN
    model_key: hnhn
    model_plain: HNHN
    value: 0.8097
    std: 0.009
    paper_value: 0.8097
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8421
    true_std: 0.0064
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: false
    value_gap: 0.032399999999999984
    has_value_note: false
    value_note: ''
    sort_value: 0.8421
    sort_std: 0.0064
    global_rank: 311
    paper_rank: 424
    rank_delta: 113
    rank_delta_abs: 113
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: UniGCN
    model_key: unigcn
    model_plain: UniGCN
    value: 0.8408
    std: 0.007
    paper_value: 0.8408
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8408
    true_std: 0.007
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8408
    sort_std: 0.007
    global_rank: 316
    paper_rank: 316
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TriCL-NG
    model_key: tricl-ng
    model_plain: TriCL-NG
    value: 0.8368
    std: 0.007
    paper_value: 0.8368
    paper_std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split. Variant using
      node- and group-level contrast.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8368
    true_std: 0.007
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8368
    sort_std: 0.007
    global_rank: 326
    paper_rank: 326
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TriCL-N
    model_key: tricl-n
    model_plain: TriCL-N
    value: 0.8344
    std: 0.006
    paper_value: 0.8344
    paper_std: 0.006
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split. Variant using
      only node-level contrast.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8344
    true_std: 0.006
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8344
    sort_std: 0.006
    global_rank: 335
    paper_rank: 335
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HyperConv
    model_key: hyperconv
    model_plain: HyperConv
    value: 0.8342
    std: 0.006
    paper_value: 0.8342
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8342
    true_std: 0.006
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8342
    sort_std: 0.006
    global_rank: 336
    paper_rank: 336
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AllSet
    model_key: allset
    model_plain: AllSet
    value: 0.8285
    std: 0.009
    paper_value: 0.8285
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8285
    true_std: 0.009
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8285
    sort_std: 0.009
    global_rank: 351
    paper_rank: 351
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HyperGCN
    model_key: hypergcn
    model_plain: HyperGCN
    value: 0.784
    std: 0.092
    paper_value: 0.784
    paper_std: 0.092
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-02-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8284
    true_std: 0.0067
    value_gap_source_arxiv: '2603.00599'
    value_gap_source_title: Heterophily-Agnostic Hypergraph Neural Networks with Riemannian
      Local Exchanger
    value_gap_source_is_current_paper: false
    value_gap: 0.044399999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8284
    sort_std: 0.0067
    global_rank: 352
    paper_rank: 711
    rank_delta: 359
    rank_delta_abs: 359
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: S2-HHGR
    model_key: s2-hhgr
    model_plain: S2-HHGR
    value: 0.8213
    std: 0.006
    paper_value: 0.8213
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8213
    true_std: 0.006
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8213
    sort_std: 0.006
    global_rank: 370
    paper_rank: 370
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HyperSAGE
    model_key: hypersage
    model_plain: HyperSAGE
    value: 0.7949
    std: 0.087
    paper_value: 0.7949
    paper_std: 0.087
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7949
    true_std: 0.087
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7949
    sort_std: 0.087
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
    is_std_outlier: true
  - model: Random-Init
    model_key: random-init
    model_plain: Random-Init
    value: 0.6749
    std: 0.022
    paper_value: 0.6749
    paper_std: 0.022
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Pubmed using Planetoid split.
    date: Jun 9, 2022
    date_display: Jun 2022
    date_iso: '2022-06-09'
    published_venue: AAAI 2022
    published_conference: AAAI 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-09'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6749
    true_std: 0.022
    value_gap_source_arxiv: '2206.04739'
    value_gap_source_title: 'I''m Me, We''re Us, and I''m Us: Tri-directional Contrastive
      Learning on Hypergraphs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6749
    sort_std: 0.022
    global_rank: 940
    paper_rank: 940
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: CiteSeer
      dataset_slug: citeseer
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: DBLP
      dataset_slug: dblp
main_figure: /figures/2206.04739/main_figure.jpegoptim.jpg
---

