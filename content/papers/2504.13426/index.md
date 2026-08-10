---
title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
arxiv_id: '2504.13426'
source_url: ''
authors:
- name: Jielong Lu
  orcid: null
  s2_author_id: '2203977517'
  s2_url: null
- name: Zhihao Wu
  orcid: null
  s2_author_id: '2355654608'
  s2_url: null
- name: Zhiling Cai
  orcid: null
  s2_author_id: '2296024968'
  s2_url: null
- name: Yueyang Pi
  orcid: null
  s2_author_id: '2302988604'
  s2_url: null
- name: Shiping Wang
  orcid: null
  s2_author_id: '2323362049'
  s2_url: null
published_date: Apr 18, 2025
published_date_iso: '2025-04-18'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'In recent years, Graph Convolutional Networks (GCNs) have gained popularity
  for their exceptional ability to process graph-structured data. Existing GCN-based
  approaches typically employ a shallow model architecture due to the over-smoothing
  phenomenon. Current approaches to mitigating over-smoothing primarily involve adding
  supplementary components to GCN architectures, such as residual connections and
  random edge-dropping strategies. However, these improvements toward deep GCNs have
  achieved only limited success. In this work, we analyze the intrinsic message passing
  mechanism of GCNs and identify a critical issue: messages originating from high-order
  neighbors must traverse through low-order neighbors to reach the target node. This
  repeated reliance on low-order neighbors leads to redundant information aggregation,
  a phenomenon we term over-aggregation. Our analysis demonstrates that over-aggregation
  not only introduces significant redundancy but also serves as the fundamental cause
  of over-smoothing in GCNs. Motivated by this discovery, we introduce a novel framework
  named redundancy-free graph convolutional network, where the neighbors of the graph
  are hierarchically organized so that the multi-order neighbor sets of a specific
  node do not intersect. This organizational structure enables high-order neighbors
  to directly propagate their messages to the target node, thereby effectively avoiding
  duplicate aggregation. The layer number of the proposed method adapts according
  to the graph structure, eliminating the need for manual adjustments to capture node
  information at specific distances. The experimental results on sixteen real-world
  datasets demonstrate the superior performance of the proposed method on node- and
  graph-level tasks. Graph convolutional network, over-smoothing, hierarchical aggregation,
  over-aggregation.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GCN
- RF-GCN
mrr: 0.0774
adjusted_mrr: 0.0774
mrr_dataset_count: 5
benchmark_categories:
- TU Dortmund
- Heterophilic Graphs
- Heterogeneous Graph Benchmarks
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 3
  total: 11
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 2
  total: 6
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
- &id006
  dataset: ACM
  rows:
  - model: SPGRL
    model_key: spgrl
    model_plain: SPGRL
    value: 0.9398
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2209.00793'
    title: Structure-Preserving Graph Representation Learning
    date: Sep 2, 2022
    date_display: Sep 2022
    date_iso: '2022-09-02'
    venue: Industrial Conference on Data Mining
    codebase_url: https://github.com/uestc-lese/SPGRL
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9398
    sort_std: null
    comparison_type: global_top
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
  - model: RF-GCN
    model_key: rf-gcn
    model_plain: RF-GCN
    value: 0.9153
    std: 0.007
    paper_value: 0.9153
    paper_std: 0.007
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
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Standard node classification task on ACM dataset
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9153
    true_std: 0.007
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9153
    sort_std: 0.007
    global_rank: 11
    paper_rank: 11
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
    value: 0.9049
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2007.02265'
    title: 'AM-GCN: Adaptive Multi-channel Graph Convolutional Networks'
    date: Jul 5, 2020
    date_display: Jul 2020
    date_iso: '2020-07-05'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/thunlp/OpenNE
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 17
    sort_value: 0.9049
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
- &id005
  dataset: Actor
  rows:
  - model: NodeFormer
    model_key: nodeformer
    model_plain: NodeFormer
    value: 0.7623
    std: 0.0042
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
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
    sort_value: 0.7623
    sort_std: 0.0042
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DiGGR
    model_key: diggr
    model_plain: DiGGR
    value: 0.4535
    std: 0.0353
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2408.13471'
    title: Disentangled Generative Graph Representation Learning
    date: Aug 24, 2024
    date_display: Aug 2024
    date_iso: '2024-08-24'
    venue: IEEE Transactions on Neural Networks and Learning Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.4535
    sort_std: 0.0353
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TRIGON
    model_key: trigon
    model_plain: TRIGON
    value: 0.4402
    std: 0.0028
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2508.19071'
    title: Dynamic Triangulation-Based Graph Rewiring for Graph Neural Networks
    date: Aug 26, 2025
    date_display: Aug 2025
    date_iso: '2025-08-26'
    venue: International Conference on Information and Knowledge Management
    codebase_url: https://github.com/Hugo-Attali/TRIGON-CIKM-2025
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.4402
    sort_std: 0.0028
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.3567
    std: null
    paper_value: 0.3567
    paper_std: null
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
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.416
    at_pub_std: 0.011
    at_pub_source_arxiv: '2503.12563'
    at_pub_source_title: 'Diffusion on Graph: Augmentation of Graph Structure for
      Node Classification'
    at_pub_source_date_iso: '2025-03-16'
    at_pub_source_date_label: TMLR 2025
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.059299999999999964
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4198
    true_std: 0.0089
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.06309999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.4198
    sort_std: 0.0089
    global_rank: 20
    paper_rank: 239
    rank_delta: 219
    rank_delta_abs: 219
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Diffusion on Graph: Augmentation of Graph Structure
      for Node Classification'
    comparison_source_arxiv: '2503.12563'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.4026
    std: 0.0108
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2302.03228'
    title: Heterophily-Aware Graph Attention Network
    date: Feb 7, 2023
    date_display: Feb 2023
    date_iso: '2023-02-07'
    venue: Pattern Recognition
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 55
    sort_value: 0.4026
    sort_std: 0.0108
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.3899
    std: 0.0085
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11762'
    title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    date: Oct 18, 2023
    date_display: Oct 2023
    date_iso: '2023-10-18'
    venue: The Web Conference
    codebase_url: https://github.com/SDS-Lab/QW_Loss
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 87
    sort_value: 0.3899
    sort_std: 0.0085
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.2688
    std: null
    paper_value: 0.2688
    paper_std: null
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
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.381
    at_pub_std: null
    at_pub_source_arxiv: '2101.00797'
    at_pub_source_title: Beyond Low-frequency Information in Graph Convolutional Networks
    at_pub_source_date_iso: '2021-01-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-01-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.11220000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.381
    true_std: null
    value_gap_source_arxiv: '2101.00797'
    value_gap_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.11220000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.381
    sort_std: null
    global_rank: 106
    paper_rank: 469
    rank_delta: 363
    rank_delta_abs: 363
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    comparison_source_arxiv: '2101.00797'
    is_best: false
    is_std_outlier: false
  - model: LRGNN
    model_key: lrgnn
    model_plain: LRGNN
    value: 0.2437
    std: null
    paper_value: 0.2437
    paper_std: null
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
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3734
    at_pub_std: 0.0178
    at_pub_source_arxiv: '2408.13471'
    at_pub_source_title: Disentangled Generative Graph Representation Learning
    at_pub_source_date_iso: '2024-08-24'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-08-24'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.1297
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3734
    true_std: 0.0178
    value_gap_source_arxiv: '2408.13471'
    value_gap_source_title: Disentangled Generative Graph Representation Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.1297
    has_value_note: false
    value_note: ''
    sort_value: 0.3734
    sort_std: 0.0178
    global_rank: 141
    paper_rank: 500
    rank_delta: 359
    rank_delta_abs: 359
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Disentangled Generative Graph Representation Learning
    comparison_source_arxiv: '2408.13471'
    is_best: false
    is_std_outlier: false
  - model: RF-GCN
    model_key: rf-gcn
    model_plain: RF-GCN
    value: 0.3618
    std: null
    paper_value: 0.3618
    paper_std: null
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
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3618
    true_std: null
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3618
    sort_std: null
    global_rank: 214
    paper_rank: 214
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HOG-GCN
    model_key: hog-gcn
    model_plain: HOG-GCN
    value: 0.3276
    std: null
    paper_value: 0.3276
    paper_std: null
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
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3276
    true_std: null
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3276
    sort_std: null
    global_rank: 344
    paper_rank: 344
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Homophily
    model_key: homophily
    model_plain: Homophily
    value: 0.22
    std: null
    paper_value: 0.22
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.22
    true_std: null
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.22
    sort_std: null
    global_rank: 533
    paper_rank: 533
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
  dataset: COLLAB
  rows:
  - model: WL-MLP
    model_key: wl-mlp
    model_plain: WL-MLP
    value: 0.9792
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2202.10156'
    title: 1-WL Expressiveness Is (Almost) All You Need
    date: Feb 21, 2022
    date_display: Feb 2022
    date_iso: '2022-02-21'
    venue: IEEE International Joint Conference on Neural Network
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: WL-based multi-layer perpetration baseline (WL-MLP) can
      successfully learn the datasets with node features
    is_global_top: true
    global_rank: 1
    sort_value: 0.9792
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.964
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.964
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CoCN
    model_key: cocn
    model_plain: CoCN
    value: 0.8722
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.18480'
    title: Scalable Graph Compressed Convolutions
    date: Jul 26, 2024
    date_display: Jul 2024
    date_iso: '2024-07-26'
    venue: arXiv.org
    codebase_url: https://github.com/sunjss/CoCN
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: use the one-hot encoding of node degrees as node features
    is_global_top: true
    global_rank: 3
    sort_value: 0.8722
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.79
    std: 0.018
    paper_value: 0.79
    paper_std: 0.018
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical record
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.826
    at_pub_std: 0.022
    at_pub_source_arxiv: '2406.11714'
    at_pub_source_title: Scalable Expressiveness through Preprocessed Graph Perturbations
    at_pub_source_date_iso: '2024-06-17'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03599999999999992
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.826
    true_std: 0.022
    value_gap_source_arxiv: '2406.11714'
    value_gap_source_title: Scalable Expressiveness through Preprocessed Graph Perturbations
    value_gap_source_is_current_paper: false
    value_gap: 0.03599999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.826
    sort_std: 0.022
    global_rank: 23
    paper_rank: 164
    rank_delta: 141
    rank_delta_abs: 141
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.802
    std: 0.019
    paper_value: 0.802
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical record
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.822
    at_pub_std: 0.021
    at_pub_source_arxiv: '2406.11714'
    at_pub_source_title: Scalable Expressiveness through Preprocessed Graph Perturbations
    at_pub_source_date_iso: '2024-06-17'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-06-17'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.019999999999999907
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.822
    true_std: 0.021
    value_gap_source_arxiv: '2406.11714'
    value_gap_source_title: Scalable Expressiveness through Preprocessed Graph Perturbations
    value_gap_source_is_current_paper: false
    value_gap: 0.019999999999999907
    has_value_note: false
    value_note: ''
    sort_value: 0.822
    sort_std: 0.021
    global_rank: 30
    paper_rank: 115
    rank_delta: 85
    rank_delta_abs: 85
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCKM
    model_key: gckm
    model_plain: GCKM
    value: 0.817
    std: 0.015
    paper_value: 0.817
    paper_std: 0.015
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical record
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.817
    true_std: 0.015
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.817
    sort_std: 0.015
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
  - model: RF-GCN
    model_key: rf-gcn
    model_plain: RF-GCN
    value: 0.814
    std: 0.015
    paper_value: 0.814
    paper_std: 0.015
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical record
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.814
    true_std: 0.015
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.814
    sort_std: 0.015
    global_rank: 61
    paper_rank: 61
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
    value: 0.797
    std: 0.017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.11025'
    title: 'SignGT: Signed Attention-based Graph Transformer for Graph Representation
      Learning'
    date: Oct 17, 2023
    date_display: Oct 2023
    date_iso: '2023-10-17'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 142
    sort_value: 0.797
    sort_std: 0.017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.792
    std: 0.024
    paper_value: 0.792
    paper_std: 0.024
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical record
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.678
    at_pub_std: 0.032
    at_pub_source_arxiv: '1905.10990'
    at_pub_source_title: Edge Contraction Pooling for Graph Neural Networks
    at_pub_source_date_iso: '2019-05-27'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.11399999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.792
    true_std: 0.024
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.792
    sort_std: 0.024
    global_rank: 157
    paper_rank: 157
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Edge Contraction Pooling for Graph Neural Networks
    comparison_source_arxiv: '1905.10990'
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.737
    std: null
    paper_value: 0.737
    paper_std: null
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical record
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7745
    at_pub_std: null
    at_pub_source_arxiv: '2103.00959'
    at_pub_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    at_pub_source_date_iso: '2021-03-01'
    at_pub_source_date_label: WWW 2021
    value_gap_source_date_iso: '2025-09-01'
    value_gap_source_date_label: IJCAI 2025
    gap_vs_at_pub: 0.03749999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7759
    true_std: 0.0224
    value_gap_source_arxiv: '2512.04530'
    value_gap_source_title: Explainable Graph Representation Learning via Graph Pattern
      Analysis
    value_gap_source_is_current_paper: false
    value_gap: 0.038900000000000046
    has_value_note: false
    value_note: ''
    sort_value: 0.7759
    sort_std: 0.0224
    global_rank: 202
    paper_rank: 293
    rank_delta: 91
    rank_delta_abs: 91
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'CogDL: A Comprehensive Library for Graph Deep Learning'
    comparison_source_arxiv: '2103.00959'
    is_best: false
    is_std_outlier: false
  - model: AWL
    model_key: awl
    model_plain: AWL
    value: 0.739
    std: 0.019
    paper_value: 0.739
    paper_std: 0.019
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical record
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.739
    at_pub_std: 0.019
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.739
    true_std: 0.019
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.739
    sort_std: 0.019
    global_rank: 291
    paper_rank: 291
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PatchySan
    model_key: patchysan
    model_plain: PatchySan
    value: 0.726
    std: 0.042
    paper_value: 0.726
    paper_std: 0.042
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV as per canonical record
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.726
    at_pub_std: 0.022
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.726
    true_std: 0.042
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.726
    sort_std: 0.042
    global_rank: 304
    paper_rank: 304
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id004
  dataset: Cornell
  rows:
  - model: P^2GNN
    model_key: p^2gnn
    model_plain: P^2GNN
    value: 0.9541
    std: 0.0272
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.09195'
    title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    date: Mar 10, 2026
    date_display: Mar 2026
    date_iso: '2026-03-10'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9541
    sort_std: 0.0272
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ACM-GCN
    model_key: acm-gcn
    model_plain: ACM-GCN
    value: 0.8571
    std: null
    paper_value: 0.8571
    paper_std: null
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
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8514
    at_pub_std: 0.0607
    at_pub_source_arxiv: '2211.11761'
    at_pub_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    at_pub_source_date_iso: '2022-11-21'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2025-04-28'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.005699999999999927
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.948
    true_std: 0.038
    value_gap_source_arxiv: '2504.19785'
    value_gap_source_title: Heterophily-informed Message Passing
    value_gap_source_is_current_paper: false
    value_gap: 0.09089999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.948
    sort_std: 0.038
    global_rank: 2
    paper_rank: 97
    rank_delta: 95
    rank_delta_abs: 95
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RF-GCN
    model_key: rf-gcn
    model_plain: RF-GCN
    value: 0.9429
    std: null
    paper_value: 0.9429
    paper_std: null
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
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9429
    true_std: null
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9429
    sort_std: null
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9136
    std: 0.007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2212.03654'
    title: Node-oriented Spectral Filtering for Graph Neural Networks
    date: Dec 7, 2022
    date_display: Dec 2022
    date_iso: '2022-12-07'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 25
    sort_value: 0.9136
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LRGNN
    model_key: lrgnn
    model_plain: LRGNN
    value: 0.8648
    std: null
    paper_value: 0.8648
    paper_std: null
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
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.865
    at_pub_std: 0.057
    at_pub_source_arxiv: '2410.02158'
    at_pub_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph Representation
      Learning'
    at_pub_source_date_iso: '2024-10-03'
    at_pub_source_date_label: TMLR 2024
    value_gap_source_date_iso: '2024-10-03'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.00019999999999997797
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.865
    true_std: 0.057
    value_gap_source_arxiv: '2410.02158'
    value_gap_source_title: 'SCNode: Spatial and Contextual Coordinates for Graph
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.00019999999999997797
    has_value_note: false
    value_note: ''
    sort_value: 0.865
    sort_std: 0.057
    global_rank: 77
    paper_rank: 81
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LINKX
    model_key: linkx
    model_plain: LINKX
    value: 0.7784
    std: null
    paper_value: 0.7784
    paper_std: null
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
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8346
    at_pub_std: 0.0061
    at_pub_source_arxiv: '2405.16185'
    at_pub_source_title: Differentiable Cluster Graph Neural Network
    at_pub_source_date_iso: '2024-05-25'
    at_pub_source_date_label: '2024'
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.05620000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8346
    true_std: 0.0061
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.05620000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.8346
    sort_std: 0.0061
    global_rank: 148
    paper_rank: 248
    rank_delta: 100
    rank_delta_abs: 100
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Differentiable Cluster Graph Neural Network
    comparison_source_arxiv: '2405.16185'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.8269
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
    global_rank: 165
    sort_value: 0.8269
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HOG-GCN
    model_key: hog-gcn
    model_plain: HOG-GCN
    value: 0.7143
    std: null
    paper_value: 0.7143
    paper_std: null
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
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7143
    true_std: null
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7143
    sort_std: null
    global_rank: 328
    paper_rank: 328
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
    value: 0.4742
    std: null
    paper_value: 0.4742
    paper_std: null
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
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6412
    at_pub_std: null
    at_pub_source_arxiv: '2303.01265'
    at_pub_source_title: Steering Graph Neural Networks with Pinning Control
    at_pub_source_date_iso: '2023-03-02'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-03-02'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.16699999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.6412
    true_std: null
    value_gap_source_arxiv: '2303.01265'
    value_gap_source_title: Steering Graph Neural Networks with Pinning Control
    value_gap_source_is_current_paper: false
    value_gap: 0.16699999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.6412
    sort_std: null
    global_rank: 409
    paper_rank: 585
    rank_delta: 176
    rank_delta_abs: 176
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Steering Graph Neural Networks with Pinning Control
    comparison_source_arxiv: '2303.01265'
    is_best: false
    is_std_outlier: false
  - model: Homophily
    model_key: homophily
    model_plain: Homophily
    value: 0.003
    std: null
    paper_value: 0.003
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification accuracy on heterophily datasets.
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.003
    true_std: null
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.003
    sort_std: null
    global_rank: 657
    paper_rank: 657
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
  dataset: MUTAG
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.991
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
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.991
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ID-GNN+BEC
    model_key: id-gnn+bec
    model_plain: ID-GNN+BEC
    value: 0.983
    std: 0.036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_display: Mar 2025
    date_iso: '2025-03-03'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SupCosine
    model_key: supcosine
    model_plain: SupCosine
    value: 0.983
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.07691'
    title: Supervised Contrastive Learning with Structure Inference for Graph Classification
    date: Mar 15, 2022
    date_display: Mar 2022
    date_iso: '2022-03-15'
    venue: IEEE Transactions on Network Science and Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.894
    std: 0.056
    paper_value: 0.894
    paper_std: 0.056
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: reported as mean accuracy and standard deviation
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.933
    at_pub_std: 0.029
    at_pub_source_arxiv: '2112.00911'
    at_pub_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    at_pub_source_date_iso: '2021-12-02'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-12-02'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.039000000000000035
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.933
    true_std: 0.029
    value_gap_source_arxiv: '2112.00911'
    value_gap_source_title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.039000000000000035
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.029
    global_rank: 43
    paper_rank: 254
    rank_delta: 211
    rank_delta_abs: 211
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PatchySan
    model_key: patchysan
    model_plain: PatchySan
    value: 0.926
    std: 0.042
    paper_value: 0.926
    paper_std: 0.042
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: reported as mean accuracy and standard deviation
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.926
    at_pub_std: 0.042
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.926
    true_std: 0.042
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.926
    sort_std: 0.042
    global_rank: 61
    paper_rank: 61
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
    value: 0.856
    std: 0.058
    paper_value: 0.856
    paper_std: 0.058
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: reported as mean accuracy and standard deviation
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.922
    at_pub_std: 0.044
    at_pub_source_arxiv: '2503.01079'
    at_pub_source_title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery
      Curvature
    at_pub_source_date_iso: '2025-03-03'
    at_pub_source_date_label: KDD 2025
    value_gap_source_date_iso: '2025-03-03'
    value_gap_source_date_label: KDD 2025
    gap_vs_at_pub: 0.06600000000000006
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.922
    true_std: 0.044
    value_gap_source_arxiv: '2503.01079'
    value_gap_source_title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery
      Curvature
    value_gap_source_is_current_paper: false
    value_gap: 0.06600000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.922
    sort_std: 0.044
    global_rank: 71
    paper_rank: 465
    rank_delta: 394
    rank_delta_abs: 394
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RF-GCN
    model_key: rf-gcn
    model_plain: RF-GCN
    value: 0.915
    std: 0.049
    paper_value: 0.915
    paper_std: 0.049
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: reported as mean accuracy and standard deviation
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.915
    true_std: 0.049
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.915
    sort_std: 0.049
    global_rank: 103
    paper_rank: 103
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
    value: 0.904
    std: 0.078
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2205.12245'
    title: Asynchronous Neural Networks for Learning in Graphs
    date: May 24, 2022
    date_display: May 2022
    date_iso: '2022-05-24'
    venue: arXiv.org
    codebase_url: https://github.com/beabevi/ESAN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 170
    sort_value: 0.904
    sort_std: 0.078
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCKM
    model_key: gckm
    model_plain: GCKM
    value: 0.887
    std: 0.076
    paper_value: 0.887
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: reported as mean accuracy and standard deviation
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.887
    true_std: 0.076
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.887
    sort_std: 0.076
    global_rank: 319
    paper_rank: 319
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AWL
    model_key: awl
    model_plain: AWL
    value: 0.879
    std: 0.098
    paper_value: 0.879
    paper_std: 0.098
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: reported as mean accuracy and standard deviation
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.879
    at_pub_std: 0.098
    at_pub_source_arxiv: '1810.00826'
    at_pub_source_title: How Powerful are Graph Neural Networks?
    at_pub_source_date_iso: '2018-10-01'
    at_pub_source_date_label: ICLR 2018
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.879
    true_std: 0.098
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.879
    sort_std: 0.098
    global_rank: 356
    paper_rank: 356
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
    value: 0.84
    std: 0.061
    paper_value: 0.84
    paper_std: 0.061
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: reported as mean accuracy and standard deviation
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.866
    at_pub_std: 0.0495
    at_pub_source_arxiv: '2106.04319'
    at_pub_source_title: Breaking the Limits of Message Passing Graph Neural Networks
    at_pub_source_date_iso: '2021-06-08'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2021-06-08'
    value_gap_source_date_label: ICML 2021
    gap_vs_at_pub: 0.026000000000000023
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.866
    true_std: 0.0495
    value_gap_source_arxiv: '2106.04319'
    value_gap_source_title: Breaking the Limits of Message Passing Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.026000000000000023
    has_value_note: false
    value_note: ''
    sort_value: 0.866
    sort_std: 0.0495
    global_rank: 430
    paper_rank: 533
    rank_delta: 103
    rank_delta_abs: 103
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.858
    std: null
    paper_value: 0.858
    paper_std: null
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: reported as mean accuracy and standard deviation
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8583
    at_pub_std: null
    at_pub_source_arxiv: '1901.08296'
    at_pub_source_title: 'Deep Learning on Attributed Graphs: A Journey from Graphs
      to Their Embeddings and Back'
    at_pub_source_date_iso: '2018-12-14'
    at_pub_source_date_label: '2018'
    value_gap_source_date_iso: '2024-12-20'
    value_gap_source_date_label: AAAI 2024
    gap_vs_at_pub: 0.00029999999999996696
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8583
    true_std: 0.0116
    value_gap_source_arxiv: '2412.17856'
    value_gap_source_title: Graph Structure Refinement with Energy-based Contrastive
      Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.00029999999999996696
    has_value_note: false
    value_note: ''
    sort_value: 0.8583
    sort_std: 0.0116
    global_rank: 455
    paper_rank: 455
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Deep Learning on Attributed Graphs: A Journey from Graphs
      to Their Embeddings and Back'
    comparison_source_arxiv: '1901.08296'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: PROTEINS
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.941
    std: 0.033
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.941
    sort_std: 0.033
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GRDL
    model_key: grdl
    model_plain: GRDL
    value: 0.826
    std: 0.012
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2408.11370'
    title: 'Graph Classification via Reference Distribution Learning: Theory and Practice'
    date: Aug 21, 2024
    date_display: Aug 2024
    date_iso: '2024-08-21'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.826
    sort_std: 0.012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.8225
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2002.09518'
    title: Memory-Based Graph Networks
    date: Feb 21, 2020
    date_display: Feb 2020
    date_iso: '2020-02-21'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/amirkhas/GraphMemoryNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8225
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.762
    std: 0.032
    paper_value: 0.762
    paper_std: 0.032
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.788
    at_pub_std: 0.041
    at_pub_source_arxiv: '2312.08671'
    at_pub_source_title: 'Permutation-Invariant graph partitioning: How graph neural
      networks capture structural interactions?'
    at_pub_source_date_iso: '2023-12-14'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2023-12-14'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.026000000000000023
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.788
    true_std: 0.041
    value_gap_source_arxiv: '2312.08671'
    value_gap_source_title: 'Permutation-Invariant graph partitioning: How graph neural
      networks capture structural interactions?'
    value_gap_source_is_current_paper: false
    value_gap: 0.026000000000000023
    has_value_note: false
    value_note: ''
    sort_value: 0.788
    sort_std: 0.041
    global_rank: 38
    paper_rank: 157
    rank_delta: 119
    rank_delta_abs: 119
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RF-GCN
    model_key: rf-gcn
    model_plain: RF-GCN
    value: 0.786
    std: 0.024
    paper_value: 0.786
    paper_std: 0.024
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.786
    true_std: 0.024
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.786
    sort_std: 0.024
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.7726
    std: 0.0228
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2206.05416'
    title: Semi-Supervised Hierarchical Graph Classification
    date: Jun 11, 2022
    date_display: Jun 2022
    date_iso: '2022-06-11'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 80
    sort_value: 0.7726
    sort_std: 0.0228
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.759
    std: 0.032
    paper_value: 0.759
    paper_std: 0.032
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7667
    at_pub_std: 0.0305
    at_pub_source_arxiv: '2402.16346'
    at_pub_source_title: Boosting Graph Pooling with Persistent Homology
    at_pub_source_date_iso: '2024-02-26'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-02-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.00770000000000004
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7667
    true_std: 0.0305
    value_gap_source_arxiv: '2402.16346'
    value_gap_source_title: Boosting Graph Pooling with Persistent Homology
    value_gap_source_is_current_paper: false
    value_gap: 0.00770000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.7667
    sort_std: 0.0305
    global_rank: 113
    paper_rank: 176
    rank_delta: 63
    rank_delta_abs: 63
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.76
    std: 0.032
    paper_value: 0.76
    paper_std: 0.032
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7665
    at_pub_std: 0.0314
    at_pub_source_arxiv: '2402.16346'
    at_pub_source_title: Boosting Graph Pooling with Persistent Homology
    at_pub_source_date_iso: '2024-02-26'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-02-26'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: 0.00649999999999995
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7665
    true_std: 0.0314
    value_gap_source_arxiv: '2402.16346'
    value_gap_source_title: Boosting Graph Pooling with Persistent Homology
    value_gap_source_is_current_paper: false
    value_gap: 0.00649999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.7665
    sort_std: 0.0314
    global_rank: 114
    paper_rank: 168
    rank_delta: 54
    rank_delta_abs: 54
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DGCNN
    model_key: dgcnn
    model_plain: DGCNN
    value: 0.755
    std: null
    paper_value: 0.755
    paper_std: null
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7626
    at_pub_std: null
    at_pub_source_arxiv: '2109.11338'
    at_pub_source_title: Orthogonal Graph Neural Networks
    at_pub_source_date_iso: '2021-09-23'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-09-23'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.00759999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7626
    true_std: null
    value_gap_source_arxiv: '2109.11338'
    value_gap_source_title: Orthogonal Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.00759999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.7626
    sort_std: null
    global_rank: 154
    paper_rank: 215
    rank_delta: 61
    rank_delta_abs: 61
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Orthogonal Graph Neural Networks
    comparison_source_arxiv: '2109.11338'
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.76
    std: 0.032
    paper_value: 0.76
    paper_std: 0.032
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.75823
    at_pub_std: 0.02915
    at_pub_source_arxiv: '2003.00982'
    at_pub_source_title: GNNBenchmark
    at_pub_source_date_iso: '2023-01-01'
    at_pub_source_date_label: JMLR 2023
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.0017700000000000493
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.76
    true_std: 0.032
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.76
    sort_std: 0.032
    global_rank: 170
    paper_rank: 170
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PatchySan
    model_key: patchysan
    model_plain: PatchySan
    value: 0.759
    std: 0.028
    paper_value: 0.759
    paper_std: 0.028
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.759
    at_pub_std: 0.028
    at_pub_source_arxiv: '2202.00529'
    at_pub_source_title: Molecular Representation Learning via Heterogeneous Motif
      Graph Neural Networks
    at_pub_source_date_iso: '2022-02-01'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.759
    true_std: 0.028
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.759
    sort_std: 0.028
    global_rank: 177
    paper_rank: 177
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCKM
    model_key: gckm
    model_plain: GCKM
    value: 0.745
    std: 0.039
    paper_value: 0.745
    paper_std: 0.039
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy reported in table
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-04-18'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.745
    true_std: 0.039
    value_gap_source_arxiv: '2504.13426'
    value_gap_source_title: Simplifying Graph Convolutional Networks with Redundancy-Free
      Neighbors
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.745
    sort_std: 0.039
    global_rank: 325
    paper_rank: 325
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
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: TU Dortmund
  datasets:
  - *id001
  - *id002
  - *id003
- benchmark: Heterophilic Graphs
  datasets:
  - *id004
  - *id005
- benchmark: Heterogeneous Graph Benchmarks
  datasets:
  - *id006
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Cornell
      dataset_slug: cornell
    - dataset: Actor
      dataset_slug: actor
  - benchmark: Heterogeneous Graph Benchmarks
    benchmark_slug: heterogeneous-graph-benchmarks
    datasets:
    - dataset: ACM
      dataset_slug: acm
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
    - dataset: PROTEINS
      dataset_slug: proteins
    - dataset: COLLAB
      dataset_slug: collab
main_figure: /figures/2504.13426/main_figure.jpegoptim.jpg
---

