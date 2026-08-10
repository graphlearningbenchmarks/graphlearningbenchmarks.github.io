---
title: 'Structure-free Graph Condensation: From Large-scale Graphs to Condensed Graph-free
  Data'
arxiv_id: '2306.02664'
source_url: ''
authors:
- name: Xin Zheng
  orcid: null
  s2_author_id: '1430762233'
  s2_url: null
- name: Miao Zhang
  orcid: null
  s2_author_id: '2112175772'
  s2_url: null
- name: C. Chen
  orcid: null
  s2_author_id: '2143946417'
  s2_url: null
- name: Q. Nguyen
  orcid: null
  s2_author_id: '144133815'
  s2_url: null
- name: Xingquan Zhu
  orcid: null
  s2_author_id: '2145144616'
  s2_url: null
- name: Shirui Pan
  orcid: null
  s2_author_id: '2153326034'
  s2_url: null
published_date: Jun 5, 2023
published_date_iso: '2023-06-05'
published_venue: NeurIPS 2023
published_conference: NeurIPS 2023
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: 'Graph condensation, which reduces the size of a large-scale graph by synthesizing
  a small-scale condensed graph as its substitution, has immediate benefits for various
  graph learning tasks. However, existing graph condensation methods rely on the joint
  optimization of nodes and structures in the condensed graph, and overlook critical
  issues in effectiveness and generalization ability. In this paper, we advocate a
  new Structure-Free Graph Condensation paradigm, named SFGC, to distill a large-scale
  graph into a small-scale graph node set without explicit graph structures,, graph-free
  data. Our idea is to implicitly encode topology structure information into the node
  attributes in the synthesized graph-free data, whose topology is reduced to an identity
  matrix. Specifically, SFGC contains two collaborative components: (1) a training
  trajectory meta-matching scheme for effectively synthesizing small-scale graph-free
  data; (2) a graph neural feature score metric for dynamically evaluating the quality
  of the condensed data. Through training trajectory meta-matching, SFGC aligns the
  long-term GNN learning behaviors between the large-scale graph and the condensed
  small-scale graph-free data, ensuring comprehensive and compact transfer of informative
  knowledge to the graph-free data. Afterward, the underlying condensed graph-free
  data would be dynamically evaluated with the graph neural feature score, which is
  a closed-form metric for ensuring the excellent expressiveness of the condensed
  graph-free data. Extensive experiments verify the superiority of SFGC across different
  condensation ratios.'
codebase_url: https://github.com/Amanda-Zheng/SFGC
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SFGC
mrr: 0.0018
adjusted_mrr: 0.0012
mrr_dataset_count: 2
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
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
    value: 0.9653
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
    global_rank: 20
    sort_value: 0.9653
    sort_std: 0.0011
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Random
    model_key: random
    model_plain: Random
    value: 0.461
    std: 0.044
    paper_value: 0.461
    paper_std: 0.044
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
    source_ref: welling2009herding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive node classification using public splits
    date: Jun 5, 2023
    date_display: Jun 2023
    date_iso: '2023-06-05'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.911
    at_pub_std: null
    at_pub_source_arxiv: '2108.00219'
    at_pub_source_title: 'Grain: Improving Data Efficiency of Graph Neural Networks
      via Diversified Influence Maximization'
    at_pub_source_date_iso: '2021-07-01'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-07-01'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.45
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
    value_gap: 0.45
    has_value_note: false
    value_note: ''
    sort_value: 0.911
    sort_std: null
    global_rank: 112
    paper_rank: 162
    rank_delta: 50
    rank_delta_abs: 50
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Grain: Improving Data Efficiency of Graph Neural Networks
      via Diversified Influence Maximization'
    comparison_source_arxiv: '2108.00219'
    is_best: false
    is_std_outlier: true
  - model: GCond
    model_key: gcond
    model_plain: GCond
    value: 0.88
    std: 0.018
    paper_value: 0.88
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: jin2021Gcond
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive node classification using public splits
    date: Jun 5, 2023
    date_display: Jun 2023
    date_iso: '2023-06-05'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-07-10'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.903
    true_std: 0.031
    value_gap_source_arxiv: '2407.08064'
    value_gap_source_title: 'TinyGraph: Joint Feature and Node Condensation for Graph
      Neural Networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.02300000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.903
    sort_std: 0.031
    global_rank: 117
    paper_rank: 131
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
  - model: SFGC
    model_key: sfgc
    model_plain: SFGC
    value: 0.9
    std: 0.003
    paper_value: 0.9
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
    protocol_note: Inductive node classification using public splits
    date: Jun 5, 2023
    date_display: Jun 2023
    date_iso: '2023-06-05'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-05'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9
    true_std: 0.003
    value_gap_source_arxiv: '2306.02664'
    value_gap_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9
    sort_std: 0.003
    global_rank: 120
    paper_rank: 120
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCond-X
    model_key: gcond-x
    model_plain: GCond-X
    value: 0.884
    std: 0.004
    paper_value: 0.884
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
    source_ref: jin2021Gcond
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive node classification using public splits
    date: Jun 5, 2023
    date_display: Jun 2023
    date_iso: '2023-06-05'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-05'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.884
    true_std: 0.004
    value_gap_source_arxiv: '2306.02664'
    value_gap_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.884
    sort_std: 0.004
    global_rank: 129
    paper_rank: 129
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DC-Graph
    model_key: dc-graph
    model_plain: DC-Graph
    value: 0.882
    std: 0.002
    paper_value: 0.882
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
    source_ref: zhao2020DC-GM
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive node classification using public splits
    date: Jun 5, 2023
    date_display: Jun 2023
    date_iso: '2023-06-05'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-05'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.882
    true_std: 0.002
    value_gap_source_arxiv: '2306.02664'
    value_gap_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.882
    sort_std: 0.002
    global_rank: 130
    paper_rank: 130
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
  - model: Herding
    model_key: herding
    model_plain: Herding
    value: 0.531
    std: 0.025
    paper_value: 0.531
    paper_std: 0.025
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
    source_ref: welling2009herding
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive node classification using public splits
    date: Jun 5, 2023
    date_display: Jun 2023
    date_iso: '2023-06-05'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.714
    true_std: 0.016
    value_gap_source_arxiv: '2403.14951'
    value_gap_source_title: Simple Graph Condensation
    value_gap_source_is_current_paper: false
    value_gap: 0.18299999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.714
    sort_std: 0.016
    global_rank: 149
    paper_rank: 160
    rank_delta: 11
    rank_delta_abs: 11
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
    value: 0.466
    std: 0.023
    paper_value: 0.466
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: sener2018active
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive node classification using public splits
    date: Jun 5, 2023
    date_display: Jun 2023
    date_iso: '2023-06-05'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-22'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.574
    true_std: 0.018
    value_gap_source_arxiv: '2403.14951'
    value_gap_source_title: Simple Graph Condensation
    value_gap_source_is_current_paper: false
    value_gap: 0.10799999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.574
    sort_std: 0.018
    global_rank: 157
    paper_rank: 161
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Coarsening
    model_key: coarsening
    model_plain: Coarsening
    value: 0.409
    std: 0.005
    paper_value: 0.409
    paper_std: 0.005
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
    source_ref: huang2021scaling
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Inductive node classification using public splits
    date: Jun 5, 2023
    date_display: Jun 2023
    date_iso: '2023-06-05'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-10-13'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.409
    true_std: 0.005
    value_gap_source_arxiv: '2310.09202'
    value_gap_source_title: Graph Distillation with Eigenbasis Matching
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.409
    sort_std: 0.005
    global_rank: 164
    paper_rank: 164
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
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Reddit
      dataset_slug: reddit
single_proposed_model: SFGC
main_figure: /figures/2306.02664/main_figure.jpegoptim.jpg
---

