---
title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised Classification'
arxiv_id: '2012.03476'
source_url: ''
authors:
- name: Rui Yang
  orcid: null
  s2_author_id: '2115430809'
  s2_url: null
- name: Wenrui Dai
  orcid: null
  s2_author_id: '3207464'
  s2_url: null
- name: Chenglin Li
  orcid: null
  s2_author_id: '144535686'
  s2_url: null
- name: Junni Zou
  orcid: null
  s2_author_id: '38871632'
  s2_url: null
- name: H. Xiong
  orcid: null
  s2_author_id: '144045763'
  s2_url: null
published_date: Dec 7, 2020
published_date_iso: '2020-12-07'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Message passing has evolved as an effective tool for designing Graph Neural
  Networks (GNNs). However, most existing methods for message passing simply sum or
  average all the neighboring features to update node representations. They are restricted
  by two problems, i.e., (i) lack of interpretability to identify node features significant
  to the prediction of GNNs, and (ii) feature over-mixing that leads to the over-smoothing
  issue in capturing long-range dependencies and inability to handle graphs under
  heterophily or low homophily. In this paper, we propose a Node-level Capsule Graph
  Neural Network (NCGNN) to address these problems with an improved message passing
  scheme. Specifically, NCGNN represents nodes as groups of node-level capsules, in
  which each capsule extracts distinctive features of its corresponding node. For
  each node-level capsule, a novel dynamic routing procedure is developed to adaptively
  select appropriate capsules for aggregation from a subgraph identified by the designed
  graph filter. NCGNN aggregates only the advantageous capsules and restrains irrelevant
  messages to avoid over-mixing features of interacting nodes. Therefore, it can relieve
  the over-smoothing issue and learn effective node representations over graphs with
  homophily or heterophily. Furthermore, our proposed message passing scheme is inherently
  interpretable and exempt from complex post-hoc explanations, as the graph filter
  and the dynamic routing procedure identify a subset of node features that are most
  significant to the model prediction from the extracted subgraph. Extensive experiments
  on synthetic as well as real-world graphs demonstrate that NCGNN can well address
  the over-smoothing issue and produce better node representations for semisupervised
  node classification. It outperforms the state of the arts under both homophily and
  heterophily.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- NCGNN-D
- NCGNN-A
- NCGNN
mrr: 0.005
adjusted_mrr: 0.005
mrr_dataset_count: 4
benchmark_categories:
- Classic
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 3
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
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
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.3385
    std: null
    paper_value: 0.3385
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
    table_ref: Table 5
    source_ref: gcnii
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4082
    true_std: 0.0179
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.06969999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.4082
    sort_std: 0.0179
    global_rank: 48
    paper_rank: 324
    rank_delta: 276
    rank_delta_abs: 276
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.3576
    std: null
    paper_value: 0.3576
    paper_std: null
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.351
    at_pub_std: 0.008
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-02-07'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.006599999999999995
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.4026
    true_std: 0.0108
    value_gap_source_arxiv: '2302.03228'
    value_gap_source_title: Heterophily-Aware Graph Attention Network
    value_gap_source_is_current_paper: false
    value_gap: 0.04500000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.4026
    sort_std: 0.0108
    global_rank: 55
    paper_rank: 235
    rank_delta: 180
    rank_delta_abs: 180
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
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
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.3026
    std: null
    paper_value: 0.3026
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
    table_ref: Table 5
    source_ref: gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.303
    at_pub_std: 0.016
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2021-01-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.00040000000000001146
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.369
    true_std: null
    value_gap_source_arxiv: '2101.00797'
    value_gap_source_title: Beyond Low-frequency Information in Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.06640000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.369
    sort_std: null
    global_rank: 166
    paper_rank: 398
    rank_delta: 232
    rank_delta_abs: 232
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NCGNN
    model_key: ncgnn
    model_plain: NCGNN
    value: 0.3684
    std: null
    paper_value: 0.3684
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3684
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3684
    sort_std: null
    global_rank: 171
    paper_rank: 171
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
    value: 0.2628
    std: null
    paper_value: 0.2628
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
    table_ref: Table 5
    source_ref: gat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.294
    at_pub_std: 0.012
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-10-08'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 0.031200000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3605
    true_std: 0.0035
    value_gap_source_arxiv: '2210.03930'
    value_gap_source_title: Hierarchical Graph Transformer with Adaptive Node Sampling
    value_gap_source_is_current_paper: false
    value_gap: 0.09770000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.3605
    sort_std: 0.0035
    global_rank: 218
    paper_rank: 473
    rank_delta: 255
    rank_delta_abs: 255
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Non-Local Graph Neural Networks
    comparison_source_arxiv: '2005.14612'
    is_best: false
    is_std_outlier: false
  - model: H2GCN-1
    model_key: h2gcn-1
    model_plain: H2GCN-1
    value: 0.3586
    std: null
    paper_value: 0.3586
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
    table_ref: Table 5
    source_ref: beyond
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-02'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.3594
    true_std: 0.013
    value_gap_source_arxiv: '2303.01265'
    value_gap_source_title: Steering Graph Neural Networks with Pinning Control
    value_gap_source_is_current_paper: false
    value_gap: 0.0008000000000000229
    has_value_note: false
    value_note: ''
    sort_value: 0.3594
    sort_std: 0.013
    global_rank: 227
    paper_rank: 231
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN-2
    model_key: h2gcn-2
    model_plain: H2GCN-2
    value: 0.3562
    std: null
    paper_value: 0.3562
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
    table_ref: Table 5
    source_ref: beyond
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-02-23'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.3562
    true_std: 0.013
    value_gap_source_arxiv: '2302.12357'
    value_gap_source_title: 'Auto-HeG: Automated Graph Neural Network on Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.3562
    sort_std: 0.013
    global_rank: 246
    paper_rank: 246
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.3368
    std: null
    paper_value: 0.3368
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
    table_ref: Table 5
    source_ref: dagnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3551
    true_std: 0.011
    value_gap_source_arxiv: '2211.11761'
    value_gap_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.01830000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.3551
    sort_std: 0.011
    global_rank: 254
    paper_rank: 328
    rank_delta: 74
    rank_delta_abs: 74
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN-S
    model_key: geom-gcn-s
    model_plain: Geom-GCN-S
    value: 0.2983
    std: null
    paper_value: 0.2983
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
    table_ref: Table 5
    source_ref: geomgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.346
    at_pub_std: null
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-05-29'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.047699999999999965
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.346
    true_std: null
    value_gap_source_arxiv: '2005.14612'
    value_gap_source_title: Non-Local Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.047699999999999965
    has_value_note: false
    value_note: ''
    sort_value: 0.346
    sort_std: null
    global_rank: 295
    paper_rank: 413
    rank_delta: 118
    rank_delta_abs: 118
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Non-Local Graph Neural Networks
    comparison_source_arxiv: '2005.14612'
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN-P
    model_key: geom-gcn-p
    model_plain: Geom-GCN-P
    value: 0.3128
    std: null
    paper_value: 0.3128
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
    table_ref: Table 5
    source_ref: geomgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3163
    at_pub_std: null
    at_pub_source_arxiv: '2002.05287'
    at_pub_source_title: Heterophilic Graphs
    at_pub_source_date_iso: '2020-02-13'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2023-10-01'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.003500000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.3163
    true_std: null
    value_gap_source_arxiv: '2310.00697'
    value_gap_source_title: Learning How to Propagate Messages in Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.003500000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.3163
    sort_std: null
    global_rank: 360
    paper_rank: 371
    rank_delta: 11
    rank_delta_abs: 11
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterophilic Graphs
    comparison_source_arxiv: '2002.05287'
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN-I
    model_key: geom-gcn-i
    model_plain: Geom-GCN-I
    value: 0.2865
    std: null
    paper_value: 0.2865
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
    table_ref: Table 5
    source_ref: geomgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.2909
    at_pub_std: null
    at_pub_source_arxiv: '2002.05287'
    at_pub_source_title: Heterophilic Graphs
    at_pub_source_date_iso: '2020-02-13'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2023-10-01'
    value_gap_source_date_label: KDD 2023
    gap_vs_at_pub: 0.004400000000000015
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.2909
    true_std: null
    value_gap_source_arxiv: '2310.00697'
    value_gap_source_title: Learning How to Propagate Messages in Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.004400000000000015
    has_value_note: false
    value_note: ''
    sort_value: 0.2909
    sort_std: null
    global_rank: 430
    paper_rank: 442
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Heterophilic Graphs
    comparison_source_arxiv: '2002.05287'
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
  dataset: Amazon-Computers
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9461
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9461
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.8245
    std: null
    paper_value: 0.8245
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
    table_ref: Table 4
    source_ref: gcn
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8785
    at_pub_std: null
    at_pub_source_arxiv: '2011.01623'
    at_pub_source_title: Learning on Attribute-Missing Graphs
    at_pub_source_date_iso: '2020-10-01'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.05399999999999994
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9412
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.11670000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9412
    sort_std: 0.0008
    global_rank: 2
    paper_rank: 440
    rank_delta: 438
    rank_delta_abs: 438
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning on Attribute-Missing Graphs
    comparison_source_arxiv: '2011.01623'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.828
    std: null
    paper_value: 0.828
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
    table_ref: Table 4
    source_ref: gat
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8693
    at_pub_std: 0.29
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0413
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9398
    true_std: 0.0022
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.11180000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.9398
    sort_std: 0.0022
    global_rank: 3
    paper_rank: 436
    rank_delta: 433
    rank_delta_abs: 433
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9351
    std: 0.0006
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 8
    sort_value: 0.9351
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.8113
    std: null
    paper_value: 0.8113
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
    table_ref: Table 4
    source_ref: gcnii
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9104
    true_std: 0.0041
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: 0.09909999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9104
    sort_std: 0.0041
    global_rank: 75
    paper_rank: 470
    rank_delta: 395
    rank_delta_abs: 395
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.8139
    std: null
    paper_value: 0.8139
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
    table_ref: Table 4
    source_ref: pagerank
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8299
    at_pub_std: 0.016
    at_pub_source_arxiv: '2010.01777'
    at_pub_source_title: A Unified View on Graph Neural Networks as Graph Signal Denoising
    at_pub_source_date_iso: '2020-10-05'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.016000000000000014
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9093
    true_std: 0.0018
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.09540000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.9093
    sort_std: 0.0018
    global_rank: 86
    paper_rank: 464
    rank_delta: 378
    rank_delta_abs: 378
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: A Unified View on Graph Neural Networks as Graph Signal
      Denoising
    comparison_source_arxiv: '2010.01777'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.8338
    std: null
    paper_value: 0.8338
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
    table_ref: Table 4
    source_ref: sgc
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.818
    at_pub_std: 0.023
    at_pub_source_arxiv: '1911.07123'
    at_pub_source_title: Graph-Revised Convolutional Network
    at_pub_source_date_iso: '2019-11-17'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.015800000000000036
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9022
    true_std: 0.0021
    value_gap_source_arxiv: '2310.11025'
    value_gap_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.06840000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9022
    sort_std: 0.0021
    global_rank: 113
    paper_rank: 421
    rank_delta: 308
    rank_delta_abs: 308
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Scattering GCN
    model_key: scattering gcn
    model_plain: Scattering GCN
    value: 0.6869
    std: null
    paper_value: 0.6869
    paper_std: null
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
    table_ref: Table 4
    source_ref: scattering
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8883
    true_std: 0.0044
    value_gap_source_arxiv: '2405.13806'
    value_gap_source_title: A General Graph Spectral Wavelet Convolution via Chebyshev
      Order Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.20140000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8883
    sort_std: 0.0044
    global_rank: 209
    paper_rank: 541
    rank_delta: 332
    rank_delta_abs: 332
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NCGNN-A
    model_key: ncgnn-a
    model_plain: NCGNN-A
    value: 0.8812
    std: null
    paper_value: 0.8812
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8812
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8812
    sort_std: null
    global_rank: 246
    paper_rank: 246
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NCGNN-D
    model_key: ncgnn-d
    model_plain: NCGNN-D
    value: 0.8811
    std: null
    paper_value: 0.8811
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8811
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8811
    sort_std: null
    global_rank: 248
    paper_rank: 248
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
    value: 0.8463
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.11907'
    title: 'GraphFM: A generalist graph transformer that learns transferable representations
      across diverse domains'
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/nerdslab/GraphFM
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 365
    sort_value: 0.8463
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.8278
    std: null
    paper_value: 0.8278
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
    table_ref: Table 4
    source_ref: dagnn
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.845
    at_pub_std: 0.012
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2024-12-09'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.017199999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.845
    true_std: 0.012
    value_gap_source_arxiv: '2412.06173'
    value_gap_source_title: Revisiting the Necessity of Graph Learning and Common
      Graph Benchmarks
    value_gap_source_is_current_paper: false
    value_gap: 0.017199999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.845
    sort_std: 0.012
    global_rank: 369
    paper_rank: 436
    rank_delta: 67
    rank_delta_abs: 67
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Deeper Graph Neural Networks
    comparison_source_arxiv: '2007.09296'
    is_best: false
    is_std_outlier: false
  - model: DropEdge
    model_key: dropedge
    model_plain: DropEdge
    value: 0.823
    std: null
    paper_value: 0.823
    paper_std: null
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
    table_ref: Table 4
    source_ref: dropedge
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.823
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.823
    sort_std: null
    global_rank: 447
    paper_rank: 447
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AdaEdge
    model_key: adaedge
    model_plain: AdaEdge
    value: 0.8218
    std: null
    paper_value: 0.8218
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
    table_ref: Table 4
    source_ref: measuring
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8218
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8218
    sort_std: null
    global_rank: 448
    paper_rank: 448
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: JK-Net
    model_key: jk-net
    model_plain: JK-Net
    value: 0.7993
    std: null
    paper_value: 0.7993
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
    table_ref: Table 4
    source_ref: jknet
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.82
    true_std: 0.006
    value_gap_source_arxiv: '2506.13083'
    value_gap_source_title: 'Uncertainty-Aware Graph Neural Networks: A Multi-Hop
      Evidence Fusion Approach'
    value_gap_source_is_current_paper: false
    value_gap: 0.02069999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.82
    sort_std: 0.006
    global_rank: 454
    paper_rank: 483
    rank_delta: 29
    rank_delta_abs: 29
    rank_delta_direction: worse
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
  dataset: Amazon-Photo
  rows:
  - model: GraphTARIF
    model_key: graphtarif
    model_plain: GraphTARIF
    value: 0.9703
    std: 0.0019
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9703
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.8936
    std: null
    paper_value: 0.8936
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
    table_ref: Table 4
    source_ref: gat
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9256
    at_pub_std: 0.0035
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.03200000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9669
    true_std: 0.0014
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.07330000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.9669
    sort_std: 0.0014
    global_rank: 2
    paper_rank: 512
    rank_delta: 510
    rank_delta_abs: 510
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Contrastive Learning with Adaptive Augmentation
    comparison_source_arxiv: '2010.14945'
    is_best: false
    is_std_outlier: false
  - model: DAM-GT
    model_key: dam-gt
    model_plain: DAM-GT
    value: 0.9666
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.17660'
    title: 'DAM-GT: Dual Positional Encoding-Based Attention Masking Graph Transformer
      for Node Classification'
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.9643
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.20248'
    title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions in Node
      Classification'
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: https://github.com/transductive-sharpening/tunedGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 8
    sort_value: 0.9643
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.9221
    std: null
    paper_value: 0.9221
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
    table_ref: Table 4
    source_ref: gcn
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9242
    at_pub_std: 0.0022
    at_pub_source_arxiv: '2010.14945'
    at_pub_source_title: Graph Contrastive Learning with Adaptive Augmentation
    at_pub_source_date_iso: '2020-10-27'
    at_pub_source_date_label: WWW 2020
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.0020999999999999908
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9632
    true_std: 0.0008
    value_gap_source_arxiv: '2605.20248'
    value_gap_source_title: 'Graph Transductive Sharpening: Leveraging Unlabeled Predictions
      in Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.041099999999999914
    has_value_note: false
    value_note: ''
    sort_value: 0.9632
    sort_std: 0.0008
    global_rank: 9
    paper_rank: 355
    rank_delta: 346
    rank_delta_abs: 346
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.9196
    std: null
    paper_value: 0.9196
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
    table_ref: Table 4
    source_ref: pagerank
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.918
    at_pub_std: null
    at_pub_source_arxiv: '2003.07450'
    at_pub_source_title: Spectral Graph Attention Network with Fast Eigen-approximation
    at_pub_source_date_iso: '2020-03-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-06-27'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.0015999999999999348
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9573
    true_std: 0.0012
    value_gap_source_arxiv: '2406.19249'
    value_gap_source_title: 'NTFormer: A Composite Node Tokenized Graph Transformer
      for Node Classification'
    value_gap_source_is_current_paper: false
    value_gap: 0.03770000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.9573
    sort_std: 0.0012
    global_rank: 23
    paper_rank: 376
    rank_delta: 353
    rank_delta_abs: 353
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Spectral Graph Attention Network with Fast Eigen-approximation
    comparison_source_arxiv: '2003.07450'
    is_best: false
    is_std_outlier: false
  - model: SGC
    model_key: sgc
    model_plain: SGC
    value: 0.9049
    std: null
    paper_value: 0.9049
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
    table_ref: Table 4
    source_ref: sgc
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.901
    at_pub_std: null
    at_pub_source_arxiv: '2003.07450'
    at_pub_source_title: Spectral Graph Attention Network with Fast Eigen-approximation
    at_pub_source_date_iso: '2020-03-17'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2023-10-17'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.0039000000000000146
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9511
    true_std: 0.0009
    value_gap_source_arxiv: '2310.11025'
    value_gap_source_title: 'SignGT: Signed Attention-based Graph Transformer for
      Graph Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: 0.04619999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.9511
    sort_std: 0.0009
    global_rank: 62
    paper_rank: 470
    rank_delta: 408
    rank_delta_abs: 408
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Spectral Graph Attention Network with Fast Eigen-approximation
    comparison_source_arxiv: '2003.07450'
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.8988
    std: null
    paper_value: 0.8988
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
    table_ref: Table 4
    source_ref: gcnii
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-02'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.943
    true_std: 0.002
    value_gap_source_arxiv: '2403.01232'
    value_gap_source_title: 'Polynormer: Polynomial-Expressive Graph Transformer in
      Linear Time'
    value_gap_source_is_current_paper: false
    value_gap: 0.044199999999999906
    has_value_note: false
    value_note: ''
    sort_value: 0.943
    sort_std: 0.002
    global_rank: 112
    paper_rank: 497
    rank_delta: 385
    rank_delta_abs: 385
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NCGNN-A
    model_key: ncgnn-a
    model_plain: NCGNN-A
    value: 0.9308
    std: null
    paper_value: 0.9308
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9308
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9308
    sort_std: null
    global_rank: 240
    paper_rank: 240
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Scattering GCN
    model_key: scattering gcn
    model_plain: Scattering GCN
    value: 0.8151
    std: null
    paper_value: 0.8151
    paper_std: null
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
    table_ref: Table 4
    source_ref: scattering
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-05-22'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9307
    true_std: 0.0042
    value_gap_source_arxiv: '2405.13806'
    value_gap_source_title: A General Graph Spectral Wavelet Convolution via Chebyshev
      Order Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.11559999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.9307
    sort_std: 0.0042
    global_rank: 241
    paper_rank: 579
    rank_delta: 338
    rank_delta_abs: 338
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NCGNN-D
    model_key: ncgnn-d
    model_plain: NCGNN-D
    value: 0.9286
    std: null
    paper_value: 0.9286
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 4
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9286
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9286
    sort_std: null
    global_rank: 261
    paper_rank: 261
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.9269
    std: null
    paper_value: 0.9269
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
    table_ref: Table 4
    source_ref: dagnn
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.92
    at_pub_std: 0.008
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.006899999999999906
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9269
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9269
    sort_std: null
    global_rank: 290
    paper_rank: 290
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AdaEdge
    model_key: adaedge
    model_plain: AdaEdge
    value: 0.9222
    std: null
    paper_value: 0.9222
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
    table_ref: Table 4
    source_ref: measuring
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9222
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9222
    sort_std: null
    global_rank: 354
    paper_rank: 354
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DropEdge
    model_key: dropedge
    model_plain: DropEdge
    value: 0.9221
    std: null
    paper_value: 0.9221
    paper_std: null
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
    table_ref: Table 4
    source_ref: dropedge
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9221
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9221
    sort_std: null
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
  - model: JK-Net
    model_key: jk-net
    model_plain: JK-Net
    value: 0.9176
    std: null
    paper_value: 0.9176
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
    table_ref: Table 4
    source_ref: jknet
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.919
    true_std: 0.007
    value_gap_source_arxiv: '2506.13083'
    value_gap_source_title: 'Uncertainty-Aware Graph Neural Networks: A Multi-Hop
      Evidence Fusion Approach'
    value_gap_source_is_current_paper: false
    value_gap: 0.0014000000000000679
    has_value_note: false
    value_note: ''
    sort_value: 0.919
    sort_std: 0.007
    global_rank: 382
    paper_rank: 394
    rank_delta: 12
    rank_delta_abs: 12
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.9128
    std: 0.0063
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2306.02285'
    title: Clarify Confused Nodes via Separated Learning
    date: Jun 4, 2023
    date_display: Jun 2023
    date_iso: '2023-06-04'
    venue: IEEE Transactions on Pattern Analysis and Machine Intelligence
    codebase_url: https://github.com/GISec-Team/NCGNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 426
    sort_value: 0.9128
    sort_std: 0.0063
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: BBGDC
    model_key: bbgdc
    model_plain: BBGDC
    value: 0.9059
    std: null
    paper_value: 0.9059
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
    table_ref: Table 4
    source_ref: bbgdc
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on Amazon Co-purchase graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9059
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9059
    sort_std: null
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
    value: 0.948
    std: 0.038
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2504.19785'
    title: Heterophily-informed Message Passing
    date: Apr 28, 2025
    date_display: Apr 2025
    date_iso: '2025-04-28'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/AaltoML/heterophily-imp
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.948
    sort_std: 0.038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: RF-GCN
    model_key: rf-gcn
    model_plain: RF-GCN
    value: 0.9429
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
    arxiv_id: '2504.13426'
    title: Simplifying Graph Convolutional Networks with Redundancy-Free Neighbors
    date: Apr 18, 2025
    date_display: Apr 2025
    date_iso: '2025-04-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9429
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8108
    std: null
    paper_value: 0.8108
    paper_std: null
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.816
    at_pub_std: 0.063
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.005199999999999982
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9136
    true_std: 0.007
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1028
    has_value_note: false
    value_note: ''
    sort_value: 0.9136
    sort_std: 0.007
    global_rank: 25
    paper_rank: 199
    rank_delta: 174
    rank_delta_abs: 174
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.7811
    std: null
    paper_value: 0.7811
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
    table_ref: Table 5
    source_ref: gcnii/2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8918
    true_std: 0.0396
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.11070000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.8918
    sort_std: 0.0396
    global_rank: 39
    paper_rank: 241
    rank_delta: 202
    rank_delta_abs: 202
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: NCGNN-A
    model_key: ncgnn-a
    model_plain: NCGNN-A
    value: 0.8379
    std: null
    paper_value: 0.8379
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8379
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8379
    sort_std: null
    global_rank: 141
    paper_rank: 141
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
  - model: H2GCN-1
    model_key: h2gcn-1
    model_plain: H2GCN-1
    value: 0.8216
    std: null
    paper_value: 0.8216
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
    table_ref: Table 5
    source_ref: beyond/2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-02'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8216
    true_std: 0.048
    value_gap_source_arxiv: '2303.01265'
    value_gap_source_title: Steering Graph Neural Networks with Pinning Control
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8216
    sort_std: 0.048
    global_rank: 182
    paper_rank: 182
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN-2
    model_key: h2gcn-2
    model_plain: H2GCN-2
    value: 0.8216
    std: null
    paper_value: 0.8216
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
    table_ref: Table 5
    source_ref: beyond/2021
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-02'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8216
    true_std: 0.06
    value_gap_source_arxiv: '2303.01265'
    value_gap_source_title: Steering Graph Neural Networks with Pinning Control
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8216
    sort_std: 0.06
    global_rank: 183
    paper_rank: 183
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
    value: 0.5892
    std: null
    paper_value: 0.5892
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
    table_ref: Table 5
    source_ref: gat/2018
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5432
    at_pub_std: null
    at_pub_source_arxiv: '2212.10822'
    at_pub_source_title: 'Complete the Missing Half: Augmenting Aggregation Filtering
      with Diversification for Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-08-20'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2022-06-06'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.04599999999999993
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.819
    true_std: 0.054
    value_gap_source_arxiv: '2206.02386'
    value_gap_source_title: Restructuring Graphs for Higher Homophily via Adaptive
      Spectral Clustering
    value_gap_source_is_current_paper: false
    value_gap: 0.2298
    has_value_note: false
    value_note: ''
    sort_value: 0.819
    sort_std: 0.054
    global_rank: 190
    paper_rank: 457
    rank_delta: 267
    rank_delta_abs: 267
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Complete the Missing Half: Augmenting Aggregation Filtering
      with Diversification for Graph Convolutional Networks'
    comparison_source_arxiv: '2212.10822'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5703
    std: null
    paper_value: 0.5703
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
    table_ref: Table 5
    source_ref: gcn/2017
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.527
    at_pub_std: null
    at_pub_source_arxiv: '2212.10822'
    at_pub_source_title: 'Complete the Missing Half: Augmenting Aggregation Filtering
      with Diversification for Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-08-20'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2025-07-01'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: 0.043300000000000005
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8082
    true_std: 0.036
    value_gap_source_arxiv: '2602.05358'
    value_gap_source_title: Bayesian Neighborhood Adaptation for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.2379
    has_value_note: false
    value_note: ''
    sort_value: 0.8082
    sort_std: 0.036
    global_rank: 203
    paper_rank: 493
    rank_delta: 290
    rank_delta_abs: 290
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Complete the Missing Half: Augmenting Aggregation Filtering
      with Diversification for Graph Convolutional Networks'
    comparison_source_arxiv: '2212.10822'
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN-S
    model_key: geom-gcn-s
    model_plain: Geom-GCN-S
    value: 0.5568
    std: null
    paper_value: 0.5568
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
    table_ref: Table 5
    source_ref: geomgcn/2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.754
    at_pub_std: null
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-05-29'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.19720000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.754
    true_std: null
    value_gap_source_arxiv: '2005.14612'
    value_gap_source_title: Non-Local Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.19720000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.754
    sort_std: null
    global_rank: 282
    paper_rank: 503
    rank_delta: 221
    rank_delta_abs: 221
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Non-Local Graph Neural Networks
    comparison_source_arxiv: '2005.14612'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.5989
    std: null
    paper_value: 0.5989
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
    table_ref: Table 5
    source_ref: dagnn/2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7351
    true_std: 0.0718
    value_gap_source_arxiv: '2211.11761'
    value_gap_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.1362
    has_value_note: false
    value_note: ''
    sort_value: 0.7351
    sort_std: 0.0718
    global_rank: 306
    paper_rank: 446
    rank_delta: 140
    rank_delta_abs: 140
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN-P
    model_key: geom-gcn-p
    model_plain: Geom-GCN-P
    value: 0.6081
    std: null
    paper_value: 0.6081
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
    table_ref: Table 5
    source_ref: geomgcn/2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6081
    at_pub_std: null
    at_pub_source_arxiv: '2212.10822'
    at_pub_source_title: 'Complete the Missing Half: Augmenting Aggregation Filtering
      with Diversification for Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-08-20'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-03-17'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6081
    true_std: null
    value_gap_source_arxiv: '2303.09778'
    value_gap_source_title: 'SE-GSL: A General and Effective Graph Structure Learning
      Framework through Structural Entropy Optimization'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6081
    sort_std: null
    global_rank: 437
    paper_rank: 437
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN-I
    model_key: geom-gcn-i
    model_plain: Geom-GCN-I
    value: 0.5676
    std: null
    paper_value: 0.5676
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
    table_ref: Table 5
    source_ref: geomgcn/2019
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5676
    at_pub_std: null
    at_pub_source_arxiv: '2212.10822'
    at_pub_source_title: 'Complete the Missing Half: Augmenting Aggregation Filtering
      with Diversification for Graph Convolutional Networks'
    at_pub_source_date_iso: '2020-08-20'
    at_pub_source_date_label: NeurIPS 2020
    value_gap_source_date_iso: '2023-02-23'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5676
    true_std: null
    value_gap_source_arxiv: '2302.12357'
    value_gap_source_title: 'Auto-HeG: Automated Graph Neural Network on Heterophilic
      Graphs'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5676
    sort_std: null
    global_rank: 496
    paper_rank: 496
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
  dataset: Texas
  rows:
  - model: P^2GNN
    model_key: p^2gnn
    model_plain: P^2GNN
    value: 0.9672
    std: 0.0147
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
    sort_value: 0.9672
    sort_std: 0.0147
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DoG
    model_key: dog
    model_plain: DoG
    value: 0.966
    std: 0.021
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
    uses_external_data: true
    input_feature_source: raw_features
    feature_source_evidence: DoG generates synthetic graph structures to boost the
      performance of GNNs.
    is_global_top: true
    global_rank: 2
    sort_value: 0.966
    sort_std: 0.021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPF-plus
    model_key: gpf-plus
    model_plain: GPF-plus
    value: 0.9583
    std: 0.0419
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.05346'
    title: 'ProG: A Graph Prompt Learning Benchmark'
    date: Jun 8, 2024
    date_display: Jun 2024
    date_iso: '2024-06-08'
    venue: Neural Information Processing Systems
    codebase_url: https://github.com/sheldonresearch/ProG
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9583
    sort_std: 0.0419
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8189
    std: null
    paper_value: 0.8189
    paper_std: null
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
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.813
    at_pub_std: 0.071
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-10-08'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.005900000000000016
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.923
    true_std: 0.007
    value_gap_source_arxiv: '2410.05593'
    value_gap_source_title: When Graph Neural Networks Meet Dynamic Mode Decomposition
    value_gap_source_is_current_paper: false
    value_gap: 0.10410000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.923
    sort_std: 0.007
    global_rank: 45
    paper_rank: 261
    rank_delta: 216
    rank_delta_abs: 216
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.9001
    std: 0.023
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
    global_rank: 73
    sort_value: 0.9001
    sort_std: 0.023
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 0.7546
    std: null
    paper_value: 0.7546
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
    table_ref: Table 5
    source_ref: gcnii
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: TMLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8918
    true_std: 0.0443
    value_gap_source_arxiv: '2505.04808'
    value_gap_source_title: Piecewise Constant Spectral Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.1372
    has_value_note: false
    value_note: ''
    sort_value: 0.8918
    sort_std: 0.0443
    global_rank: 91
    paper_rank: 387
    rank_delta: 296
    rank_delta_abs: 296
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN-1
    model_key: h2gcn-1
    model_plain: H2GCN-1
    value: 0.8486
    std: null
    paper_value: 0.8486
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
    table_ref: Table 5
    source_ref: beyond
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-02'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8486
    true_std: 0.067
    value_gap_source_arxiv: '2303.01265'
    value_gap_source_title: Steering Graph Neural Networks with Pinning Control
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8486
    sort_std: 0.067
    global_rank: 191
    paper_rank: 191
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NCGNN-A
    model_key: ncgnn-a
    model_plain: NCGNN-A
    value: 0.8443
    std: null
    paper_value: 0.8443
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 5
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-12-07'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8443
    true_std: null
    value_gap_source_arxiv: '2012.03476'
    value_gap_source_title: 'NCGNN: Node-Level Capsule Graph Neural Network for Semisupervised
      Classification'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8443
    sort_std: null
    global_rank: 207
    paper_rank: 207
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN-2
    model_key: h2gcn-2
    model_plain: H2GCN-2
    value: 0.8216
    std: null
    paper_value: 0.8216
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
    table_ref: Table 5
    source_ref: beyond
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-03-02'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8216
    true_std: 0.052
    value_gap_source_arxiv: '2303.01265'
    value_gap_source_title: Steering Graph Neural Networks with Pinning Control
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8216
    sort_std: 0.052
    global_rank: 254
    paper_rank: 254
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
    value: 0.5838
    std: null
    paper_value: 0.5838
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
    table_ref: Table 5
    source_ref: gat
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5838
    at_pub_std: null
    at_pub_source_arxiv: '2002.05287'
    at_pub_source_title: Heterophilic Graphs
    at_pub_source_date_iso: '2020-02-13'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2025-06-17'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8162
    true_std: 0.0645
    value_gap_source_arxiv: '2506.14291'
    value_gap_source_title: 'Equivariance Everywhere All At Once: A Recipe for Graph
      Foundation Models'
    value_gap_source_is_current_paper: false
    value_gap: 0.23240000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.8162
    sort_std: 0.0645
    global_rank: 266
    paper_rank: 624
    rank_delta: 358
    rank_delta_abs: 358
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
    value: 0.5946
    std: null
    paper_value: 0.5946
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
    table_ref: Table 5
    source_ref: gcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.611
    at_pub_std: 0.07
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.01639999999999997
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7933
    true_std: 0.0447
    value_gap_source_arxiv: '2505.20034'
    value_gap_source_title: Graph Wave Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.1987
    has_value_note: false
    value_note: ''
    sort_value: 0.7933
    sort_std: 0.0447
    global_rank: 323
    paper_rank: 602
    rank_delta: 279
    rank_delta_abs: 279
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN-S
    model_key: geom-gcn-s
    model_plain: Geom-GCN-S
    value: 0.5973
    std: null
    paper_value: 0.5973
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
    table_ref: Table 5
    source_ref: geomgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.735
    at_pub_std: null
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-05-29'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.13769999999999993
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.735
    true_std: null
    value_gap_source_arxiv: '2005.14612'
    value_gap_source_title: Non-Local Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.13769999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.735
    sort_std: null
    global_rank: 425
    paper_rank: 597
    rank_delta: 172
    rank_delta_abs: 172
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Non-Local Graph Neural Networks
    comparison_source_arxiv: '2005.14612'
    is_best: false
    is_std_outlier: false
  - model: DAGNN
    model_key: dagnn
    model_plain: DAGNN
    value: 0.5935
    std: null
    paper_value: 0.5935
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
    table_ref: Table 5
    source_ref: dagnn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-11-21'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7027
    true_std: 0.0493
    value_gap_source_arxiv: '2211.11761'
    value_gap_source_title: 'From Node Interaction to Hop Interaction: New Effective
      and Scalable Graph Learning Paradigm'
    value_gap_source_is_current_paper: false
    value_gap: 0.10919999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.7027
    sort_std: 0.0493
    global_rank: 462
    paper_rank: 606
    rank_delta: 144
    rank_delta_abs: 144
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN-P
    model_key: geom-gcn-p
    model_plain: Geom-GCN-P
    value: 0.6757
    std: null
    paper_value: 0.6757
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
    table_ref: Table 5
    source_ref: geomgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6757
    at_pub_std: null
    at_pub_source_arxiv: '2002.05287'
    at_pub_source_title: Heterophilic Graphs
    at_pub_source_date_iso: '2020-02-13'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2025-05-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6757
    true_std: null
    value_gap_source_arxiv: '2505.02020'
    value_gap_source_title: Wide & Deep Learning for Node Classification
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6757
    sort_std: null
    global_rank: 494
    paper_rank: 494
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN-I
    model_key: geom-gcn-i
    model_plain: Geom-GCN-I
    value: 0.5758
    std: null
    paper_value: 0.5758
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
    table_ref: Table 5
    source_ref: geomgcn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Average test accuracy on disassortative graphs
    date: Dec 7, 2020
    date_display: Dec 2020
    date_iso: '2020-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5758
    at_pub_std: null
    at_pub_source_arxiv: '2002.05287'
    at_pub_source_title: Heterophilic Graphs
    at_pub_source_date_iso: '2020-02-13'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2025-05-04'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5758
    true_std: null
    value_gap_source_arxiv: '2505.02020'
    value_gap_source_title: Wide & Deep Learning for Node Classification
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5758
    sort_std: null
    global_rank: 640
    paper_rank: 640
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
- benchmark: Heterophilic Graphs
  datasets:
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
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
    - dataset: Actor
      dataset_slug: actor
main_figure: /figures/2012.03476/main_figure.jpegoptim.jpg
---

