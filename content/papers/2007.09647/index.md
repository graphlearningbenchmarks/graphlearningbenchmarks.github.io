---
title: Adversarial Immunization for Certifiable Robustness on Graphs
arxiv_id: '2007.09647'
source_url: ''
authors:
- name: Shuchang Tao
  orcid: null
  s2_author_id: '32504908'
  s2_url: null
- name: Huawei Shen
  orcid: null
  s2_author_id: '2476503'
  s2_url: null
- name: Qi Cao
  orcid: null
  s2_author_id: '2057766936'
  s2_url: null
- name: Liang Hou
  orcid: null
  s2_author_id: '2055765400'
  s2_url: null
- name: Xueqi Cheng
  orcid: null
  s2_author_id: '1717004'
  s2_url: null
published_date: Jul 19, 2020
published_date_iso: '2020-07-19'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Despite achieving strong performance in semi-supervised node classification
  task, graph neural networks (GNNs) are vulnerable to adversarial attacks, similar
  to other deep learning models. Existing researches focus on developing either robust
  GNN models or attack detection methods against adversarial attacks on graphs. However,
  little research attention is paid to the potential and practice of immunization
  to adversarial attacks on graphs. In this paper, we propose and formulate the graph
  adversarial immunization problem, i.e., vaccinating an affordable fraction of node
  pairs, connected or unconnected, to improve the certifiable robustness of graph
  against any admissible adversarial attack. We further propose an effective algorithm,
  called AdvImmune, which optimizes with meta-gradient in a discrete way to circumvent
  the computationally expensive combinatorial optimization when solving the adversarial
  immunization problem. Experiments are conducted on two citation networks and one
  social network. Experimental results demonstrate that the proposed AdvImmune method
  remarkably improves the ratio of robust nodes by 12$\
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- AdvImmune
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
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
  - model: AdvImmune
    model_key: advimmune
    model_plain: AdvImmune
    value: 0.90453
    std: null
    paper_value: 0.90453
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy of node classification by GNN model on clean graph
    date: Jul 19, 2020
    date_display: Jul 2020
    date_iso: '2020-07-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.90453
    true_std: null
    value_gap_source_arxiv: '2007.09647'
    value_gap_source_title: Adversarial Immunization for Certifiable Robustness on
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.90453
    sort_std: null
    global_rank: 115
    paper_rank: 115
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: No defense
    model_key: no defense
    model_plain: No defense
    value: 0.90453
    std: null
    paper_value: 0.90453
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy of node classification by GNN model on clean graph
    date: Jul 19, 2020
    date_display: Jul 2020
    date_iso: '2020-07-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.90453
    true_std: null
    value_gap_source_arxiv: '2007.09647'
    value_gap_source_title: Adversarial Immunization for Certifiable Robustness on
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.90453
    sort_std: null
    global_rank: 114
    paper_rank: 114
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: RCE
    model_key: rce
    model_plain: RCE
    value: 0.86706
    std: null
    paper_value: 0.86706
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy of node classification by GNN model under Surrogate attack
    date: Jul 19, 2020
    date_display: Jul 2020
    date_iso: '2020-07-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86706
    true_std: null
    value_gap_source_arxiv: '2007.09647'
    value_gap_source_title: Adversarial Immunization for Certifiable Robustness on
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86706
    sort_std: null
    global_rank: 136
    paper_rank: 136
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CEM
    model_key: cem
    model_plain: CEM
    value: 0.86347
    std: null
    paper_value: 0.86347
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
    table_ref: Table 3
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Accuracy of node classification by GNN model under Surrogate attack
    date: Jul 19, 2020
    date_display: Jul 2020
    date_iso: '2020-07-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-07-19'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.86347
    true_std: null
    value_gap_source_arxiv: '2007.09647'
    value_gap_source_title: Adversarial Immunization for Certifiable Robustness on
      Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.86347
    sort_std: null
    global_rank: 138
    paper_rank: 138
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
single_proposed_model: AdvImmune
main_figure: /figures/2007.09647/main_figure.jpegoptim.jpg
---

