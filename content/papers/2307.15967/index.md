---
title: Graph Condensation for Inductive Node Representation Learning
arxiv_id: '2307.15967'
source_url: ''
authors:
- name: Xin Gao
  orcid: null
  s2_author_id: '2192083394'
  s2_url: null
- name: Tong Chen
  orcid: null
  s2_author_id: '1490931831'
  s2_url: null
- name: Yilong Zang
  orcid: null
  s2_author_id: '2183027408'
  s2_url: null
- name: Wentao Zhang
  orcid: null
  s2_author_id: '2136776515'
  s2_url: null
- name: Q. Nguyen
  orcid: null
  s2_author_id: '144133815'
  s2_url: null
- name: Kai Zheng
  orcid: null
  s2_author_id: '145487536'
  s2_url: null
- name: Hongzhi Yin
  orcid: null
  s2_author_id: '2416851'
  s2_url: null
published_date: Jul 29, 2023
published_date_iso: '2023-07-29'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph neural networks (GNNs) encounter significant computational challenges
  when handling large-scale graphs, which severely restricts their efficacy across
  diverse applications. To address this limitation, graph condensation has emerged
  as a promising technique, which constructs a small synthetic graph for efficiently
  training GNNs while retaining performance. However, due to the topology structure
  among nodes, graph condensation is limited to condensing only the observed training
  nodes and their corresponding structure, thus lacking the ability to effectively
  handle the unseen data. Consequently, the original large graph is still required
  in the inference stage to perform message passing to inductive nodes, resulting
  in substantial computational demands. To overcome this issue, we propose mapping-aware
  graph condensation (MCond), explicitly learning the one-to-many node mapping from
  original nodes to synthetic nodes to seamlessly integrate new nodes into the synthetic
  graph for inductive representation learning. This enables direct information propagation
  on the synthetic graph, which is much more efficient than on the original large
  graph. Specifically, MCond employs an alternating optimization scheme with innovative
  loss terms from transductive and inductive perspectives, facilitating the mutual
  promotion between graph condensation and node mapping learning. Extensive experiments
  demonstrate the efficacy of our approach in inductive inference. On the Reddit dataset,
  MCond achieves up to $121.5 $ inference speedup and $55.9 $ reduction in storage
  requirements compared with counterparts based on the original graph.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MCond_OS
- MCond_SO
- MCond_SS
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 2
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
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
    value: 0.9296
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
    global_rank: 19
    sort_value: 0.9296
    sort_std: 0.0015
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.869
    std: 0.0074
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2310.00183'
    title: On the Equivalence of Graph Convolution and Mixup
    date: Sep 29, 2023
    date_display: Sep 2023
    date_iso: '2023-09-29'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/ahxt/GraphConv_is_Mixup
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 243
    sort_value: 0.869
    sort_std: 0.0074
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Whole
    model_key: whole
    model_plain: Whole
    value: 0.7903
    std: 0.0009
    paper_value: 0.7903
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
    protocol_note: Planetoid split (fixed split) for node classification
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7903
    true_std: 0.0009
    value_gap_source_arxiv: '2307.15967'
    value_gap_source_title: Graph Condensation for Inductive Node Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7903
    sort_std: 0.0009
    global_rank: 641
    paper_rank: 641
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
- &id002
  dataset: Reddit
  rows:
  - model: GAP-EDP
    model_key: gap-edp
    model_plain: GAP-EDP
    value: 0.987
    std: 0.0003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2203.00949'
    title: 'GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation'
    date: Mar 2, 2022
    date_display: Mar 2022
    date_iso: '2022-03-02'
    venue: USENIX Security Symposium
    codebase_url: https://github.com/sisaman/GAP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.987
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: NE-ASGCN
    model_key: ne-asgcn
    model_plain: NE-ASGCN
    value: 0.9758
    std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.16097'
    title: Neighbor Enhanced Graph Convolutional Networks for Node Classification
      and Recommendation
    date: Mar 1, 2022
    date_display: Mar 2022
    date_iso: '2022-03-01'
    venue: Knowledge-Based Systems
    codebase_url: ''
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9758
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HSGT
    model_key: hsgt
    model_plain: HSGT
    value: 0.973
    std: 0.0024
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2305.02866'
    title: Hierarchical Transformer for Scalable Graph Learning
    date: May 4, 2023
    date_display: May 2023
    date_iso: '2023-05-04'
    venue: International Joint Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.973
    sort_std: 0.0024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.8889
    std: 0.0021
    paper_value: 0.8889
    paper_std: 0.0021
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
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%)
      using GraphSAGE architecture.
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9653
    at_pub_std: 0.0011
    at_pub_source_arxiv: '2305.02866'
    at_pub_source_title: Hierarchical Transformer for Scalable Graph Learning
    at_pub_source_date_iso: '2023-05-04'
    at_pub_source_date_label: IJCAI 2023
    value_gap_source_date_iso: '2023-05-04'
    value_gap_source_date_label: IJCAI 2023
    gap_vs_at_pub: 0.07640000000000002
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9653
    true_std: 0.0011
    value_gap_source_arxiv: '2305.02866'
    value_gap_source_title: Hierarchical Transformer for Scalable Graph Learning
    value_gap_source_is_current_paper: false
    value_gap: 0.07640000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.9653
    sort_std: 0.0011
    global_rank: 20
    paper_rank: 126
    rank_delta: 106
    rank_delta_abs: 106
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hierarchical Transformer for Scalable Graph Learning
    comparison_source_arxiv: '2305.02866'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.965
    std: 0.0003
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2406.12059'
    title: A Scalable and Effective Alternative to Graph Transformers
    date: Jun 17, 2024
    date_display: Jun 2024
    date_iso: '2024-06-17'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 22
    sort_value: 0.965
    sort_std: 0.0003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.8712
    std: 0.0013
    paper_value: 0.8712
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
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%)
      using APPNP architecture.
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.95
    at_pub_std: null
    at_pub_source_arxiv: '2102.10739'
    at_pub_source_title: Dissecting the Diffusion Process in Linear Graph Convolutional
      Networks
    at_pub_source_date_iso: '2021-02-22'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2021-02-22'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.07879999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.95
    true_std: null
    value_gap_source_arxiv: '2102.10739'
    value_gap_source_title: Dissecting the Diffusion Process in Linear Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07879999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.95
    sort_std: null
    global_rank: 68
    paper_rank: 134
    rank_delta: 66
    rank_delta_abs: 66
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Dissecting the Diffusion Process in Linear Graph Convolutional
      Networks
    comparison_source_arxiv: '2102.10739'
    is_best: false
    is_std_outlier: false
  - model: Whole
    model_key: whole
    model_plain: Whole
    value: 0.94
    std: 0.0002
    paper_value: 0.94
    paper_std: 0.0002
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
    protocol_note: Test accuracy on original graph (Whole) for Reddit node classification.
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.94
    true_std: 0.0002
    value_gap_source_arxiv: '2307.15967'
    value_gap_source_title: Graph Condensation for Inductive Node Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.94
    sort_std: 0.0002
    global_rank: 75
    paper_rank: 75
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MCond_OS
    model_key: mcond_os
    model_plain: MCond_OS
    value: 0.9153
    std: 0.0012
    paper_value: 0.9153
    paper_std: 0.0012
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%).
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9153
    true_std: 0.0012
    value_gap_source_arxiv: '2307.15967'
    value_gap_source_title: Graph Condensation for Inductive Node Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9153
    sort_std: 0.0012
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
  - model: Degree
    model_key: degree
    model_plain: Degree
    value: 0.5587
    std: 0.0142
    paper_value: 0.5587
    paper_std: 0.0142
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
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%).
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.914
    at_pub_std: null
    at_pub_source_arxiv: '2108.00219'
    at_pub_source_title: 'Grain: Improving Data Efficiency of Graph Neural Networks
      via Diversified Influence Maximization'
    at_pub_source_date_iso: '2021-07-01'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-07-01'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.35530000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.914
    true_std: null
    value_gap_source_arxiv: '2108.00219'
    value_gap_source_title: 'Grain: Improving Data Efficiency of Graph Neural Networks
      via Diversified Influence Maximization'
    value_gap_source_is_current_paper: false
    value_gap: 0.35530000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.914
    sort_std: null
    global_rank: 107
    paper_rank: 159
    rank_delta: 52
    rank_delta_abs: 52
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Grain: Improving Data Efficiency of Graph Neural Networks
      via Diversified Influence Maximization'
    comparison_source_arxiv: '2108.00219'
    is_best: false
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.5577
    std: 0.0176
    paper_value: 0.5577
    paper_std: 0.0176
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
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%).
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.911
    at_pub_std: null
    at_pub_source_arxiv: '2108.00219'
    at_pub_source_title: 'Grain: Improving Data Efficiency of Graph Neural Networks
      via Diversified Influence Maximization'
    at_pub_source_date_iso: '2021-07-01'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-07-01'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.35330000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.911
    true_std: null
    value_gap_source_arxiv: '2108.00219'
    value_gap_source_title: 'Grain: Improving Data Efficiency of Graph Neural Networks
      via Diversified Influence Maximization'
    value_gap_source_is_current_paper: false
    value_gap: 0.35330000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.911
    sort_std: null
    global_rank: 112
    paper_rank: 159
    rank_delta: 47
    rank_delta_abs: 47
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Grain: Improving Data Efficiency of Graph Neural Networks
      via Diversified Influence Maximization'
    comparison_source_arxiv: '2108.00219'
    is_best: false
    is_std_outlier: false
  - model: GCond
    model_key: gcond
    model_plain: GCond
    value: 0.8963
    std: 0.0025
    paper_value: 0.8963
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
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%).
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.88
    at_pub_std: 0.018
    at_pub_source_arxiv: '2306.02664'
    at_pub_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    at_pub_source_date_iso: '2023-06-05'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-07-10'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.01629999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.903
    true_std: 0.031
    value_gap_source_arxiv: '2407.08064'
    value_gap_source_title: 'TinyGraph: Joint Feature and Node Condensation for Graph
      Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.006700000000000039
    has_value_note: false
    value_note: ''
    sort_value: 0.903
    sort_std: 0.031
    global_rank: 117
    paper_rank: 121
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: MCond_SO
    model_key: mcond_so
    model_plain: MCond_SO
    value: 0.9006
    std: 0.0023
    paper_value: 0.9006
    paper_std: 0.0023
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
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%).
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9006
    true_std: 0.0023
    value_gap_source_arxiv: '2307.15967'
    value_gap_source_title: Graph Condensation for Inductive Node Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9006
    sort_std: 0.0023
    global_rank: 119
    paper_rank: 119
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MCond_SS
    model_key: mcond_ss
    model_plain: MCond_SS
    value: 0.8877
    std: 0.0044
    paper_value: 0.8877
    paper_std: 0.0044
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
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%).
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8877
    true_std: 0.0044
    value_gap_source_arxiv: '2307.15967'
    value_gap_source_title: Graph Condensation for Inductive Node Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8877
    sort_std: 0.0044
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
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.824
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
    arxiv_id: '2203.00949'
    title: 'GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation'
    date: Mar 2, 2022
    date_display: Mar 2022
    date_iso: '2022-03-02'
    venue: USENIX Security Symposium
    codebase_url: https://github.com/sisaman/GAP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 143
    sort_value: 0.824
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VNG
    model_key: vng
    model_plain: VNG
    value: 0.7942
    std: 0.0113
    paper_value: 0.7942
    paper_std: 0.0113
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
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%).
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7942
    true_std: 0.0113
    value_gap_source_arxiv: '2307.15967'
    value_gap_source_title: Graph Condensation for Inductive Node Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7942
    sort_std: 0.0113
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
  - model: Cheby
    model_key: cheby
    model_plain: Cheby
    value: 0.753
    std: 0.0002
    paper_value: 0.753
    paper_std: 0.0002
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
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%)
      using Cheby architecture.
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-07-29'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.753
    true_std: 0.0002
    value_gap_source_arxiv: '2307.15967'
    value_gap_source_title: Graph Condensation for Inductive Node Representation Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.753
    sort_std: 0.0002
    global_rank: 146
    paper_rank: 146
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Herding
    model_key: herding
    model_plain: Herding
    value: 0.5586
    std: 0.0179
    paper_value: 0.5586
    paper_std: 0.0179
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
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%).
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.531
    at_pub_std: 0.025
    at_pub_source_arxiv: '2306.02664'
    at_pub_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    at_pub_source_date_iso: '2023-06-05'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-03-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.027599999999999958
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.714
    true_std: 0.016
    value_gap_source_arxiv: '2403.14951'
    value_gap_source_title: Simple Graph Condensation
    value_gap_source_is_current_paper: false
    value_gap: 0.15539999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.714
    sort_std: 0.016
    global_rank: 149
    paper_rank: 159
    rank_delta: 10
    rank_delta_abs: 10
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: K-Center
    model_key: k-center
    model_plain: K-Center
    value: 0.5536
    std: 0.0178
    paper_value: 0.5536
    paper_std: 0.0178
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
    table_ref: Table 41
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test accuracy for Reddit node classification (Graph batch, r=0.10%).
    date: Jul 29, 2023
    date_display: Jul 2023
    date_iso: '2023-07-29'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.466
    at_pub_std: 0.023
    at_pub_source_arxiv: '2306.02664'
    at_pub_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    at_pub_source_date_iso: '2023-06-05'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2024-03-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.08759999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.574
    true_std: 0.018
    value_gap_source_arxiv: '2403.14951'
    value_gap_source_title: Simple Graph Condensation
    value_gap_source_is_current_paper: false
    value_gap: 0.020399999999999974
    has_value_note: false
    value_note: ''
    sort_value: 0.574
    sort_std: 0.018
    global_rank: 157
    paper_rank: 159
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Structure-free Graph Condensation: From Large-scale
      Graphs to Condensed Graph-free Data'
    comparison_source_arxiv: '2306.02664'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: Reddit
      dataset_slug: reddit
main_figure: /figures/2307.15967/main_figure.jpegoptim.jpg
---

