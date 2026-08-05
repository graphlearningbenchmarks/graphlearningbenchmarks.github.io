---
title: Graph Distillation with Eigenbasis Matching
arxiv_id: '2310.09202'
source_url: ''
authors:
- name: Yang Liu
  orcid: null
  s2_author_id: '2258560015'
  s2_url: null
- name: Deyu Bo
  orcid: null
  s2_author_id: '1491450638'
  s2_url: null
- name: Chuan Shi
  orcid: null
  s2_author_id: '2257131498'
  s2_url: null
published_date: Oct 13, 2023
published_date_iso: '2023-10-13'
published_venue: ICML 2023
published_conference: ICML 2023
published_conference_short: ICML
published_conference_slug: icml
abstract: The increasing amount of graph data places requirements on the efficient
  training of graph neural networks (GNNs). The emerging graph distillation (GD) tackles
  this challenge by distilling a small synthetic graph to replace the real large graph,
  ensuring GNNs trained on real and synthetic graphs exhibit comparable performance.
  However, existing methods rely on GNN-related information as supervision, including
  gradients, representations, and trajectories, which have two limitations. First,
  GNNs can affect the spectrum (i.e., eigenvalues) of the real graph, causing spectrum
  bias in the synthetic graph. Second, the variety of GNN architectures leads to the
  creation of different synthetic graphs, requiring traversal to obtain optimal performance.
  To tackle these issues, we propose Graph Distillation with Eigenbasis Matching (GDEM),
  which aligns the eigenbasis and node features of real and synthetic graphs. Meanwhile,
  it directly replicates the spectrum of the real graph and thus prevents the influence
  of GNNs. Moreover, we design a discrimination constraint to balance the effectiveness
  and generalization of GDEM. Theoretically, the synthetic graphs distilled by GDEM
  are restricted spectral approximations of the real graphs. Extensive experiments
  demonstrate that GDEM outperforms state-of-the-art GD methods with powerful cross-architecture
  generalization ability and significant distillation efficiency. Our code is available
  at https://github.com/liuyang-tian/GDEM.
codebase_url: https://github.com/liuyang-tian/GDEM
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GDEM
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
  - model: TinyGraph
    model_key: ne-asgcn
    model_plain: TinyGraph
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
    global_rank: 1
    sort_value: 0.9758
    sort_std: 0.0027
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TinyGraph
    model_key: hsgt
    model_plain: TinyGraph
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
    global_rank: 2
    sort_value: 0.973
    sort_std: 0.0024
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TinyGraph
    model_key: gcmae
    model_plain: TinyGraph
    value: 0.9713
    std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2310.15523'
    title: Generative and Contrastive Paradigms Are Complementary for Graph Self-Supervised
      Learning
    date: Oct 24, 2023
    date_display: Oct 2023
    date_iso: '2023-10-24'
    venue: IEEE International Conference on Data Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9713
    sort_std: 0.0017
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GDEM
    model_key: gdem
    model_plain: GDEM
    value: 0.932
    std: 0.004
    paper_value: 0.932
    paper_std: 0.004
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Reddit with 0.50% ratio split using Accuracy
    date: Oct 13, 2023
    date_display: Oct 2023
    date_iso: '2023-10-13'
    published_venue: ICML 2023
    published_conference: ICML 2023
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
    true_value: 0.932
    true_std: 0.004
    value_gap_source_arxiv: '2310.09202'
    value_gap_source_title: Graph Distillation with Eigenbasis Matching
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.932
    sort_std: 0.004
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
  - model: SGDD
    model_key: sgdd
    model_plain: SGDD
    value: 0.918
    std: 0.019
    paper_value: 0.918
    paper_std: 0.019
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Reddit with 0.05% ratio split using Accuracy
    date: Oct 13, 2023
    date_display: Oct 2023
    date_iso: '2023-10-13'
    published_venue: ICML 2023
    published_conference: ICML 2023
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
    true_value: 0.918
    true_std: 0.019
    value_gap_source_arxiv: '2310.09202'
    value_gap_source_title: Graph Distillation with Eigenbasis Matching
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.918
    sort_std: 0.019
    global_rank: 97
    paper_rank: 97
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Reddit with 0.05% ratio split using Accuracy
    date: Oct 13, 2023
    date_display: Oct 2023
    date_iso: '2023-10-13'
    published_venue: ICML 2023
    published_conference: ICML 2023
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
    global_rank: 106
    paper_rank: 153
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Reddit with 0.05% ratio split using Accuracy
    date: Oct 13, 2023
    date_display: Oct 2023
    date_iso: '2023-10-13'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.8963
    at_pub_std: 0.0025
    at_pub_source_arxiv: '2307.15967'
    at_pub_source_title: Graph Condensation for Inductive Node Representation Learning
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-07-10'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.01629999999999998
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
    global_rank: 111
    paper_rank: 125
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SFGC
    model_key: sfgc
    model_plain: SFGC
    value: 0.897
    std: 0.002
    paper_value: 0.897
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
    protocol_note: Node classification on Reddit with 0.05% ratio split using Accuracy
    date: Oct 13, 2023
    date_display: Oct 2023
    date_iso: '2023-10-13'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.9
    at_pub_std: 0.003
    at_pub_source_arxiv: '2306.02664'
    at_pub_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    at_pub_source_date_iso: '2023-06-05'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-06-05'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.0030000000000000027
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.9
    true_std: 0.003
    value_gap_source_arxiv: '2306.02664'
    value_gap_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    value_gap_source_is_current_paper: false
    value_gap: 0.0030000000000000027
    has_value_note: false
    value_note: ''
    sort_value: 0.9
    sort_std: 0.003
    global_rank: 114
    paper_rank: 114
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Reddit with 0.05% ratio split using Accuracy
    date: Oct 13, 2023
    date_display: Oct 2023
    date_iso: '2023-10-13'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.5586
    at_pub_std: 0.0179
    at_pub_source_arxiv: '2307.15967'
    at_pub_source_title: Graph Condensation for Inductive Node Representation Learning
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-01-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: 0.027599999999999958
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.714
    true_std: 0.016
    value_gap_source_arxiv: '2401.12231'
    value_gap_source_title: Disentangled Condensation for Large-scale Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.18299999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.714
    sort_std: 0.016
    global_rank: 141
    paper_rank: 151
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Reddit with 0.05% ratio split using Accuracy
    date: Oct 13, 2023
    date_display: Oct 2023
    date_iso: '2023-10-13'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.5536
    at_pub_std: 0.0178
    at_pub_source_arxiv: '2307.15967'
    at_pub_source_title: Graph Condensation for Inductive Node Representation Learning
    at_pub_source_date_iso: '2023-07-29'
    at_pub_source_date_label: '2023'
    value_gap_source_date_iso: '2024-01-18'
    value_gap_source_date_label: WWW 2024
    gap_vs_at_pub: 0.08759999999999996
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.574
    true_std: 0.018
    value_gap_source_arxiv: '2401.12231'
    value_gap_source_title: Disentangled Condensation for Large-scale Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.10799999999999993
    has_value_note: false
    value_note: ''
    sort_value: 0.574
    sort_std: 0.018
    global_rank: 148
    paper_rank: 152
    rank_delta: 4
    rank_delta_abs: 4
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Graph Condensation for Inductive Node Representation
      Learning
    comparison_source_arxiv: '2307.15967'
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Node classification on Reddit with 0.05% ratio split using Accuracy
    date: Oct 13, 2023
    date_display: Oct 2023
    date_iso: '2023-10-13'
    published_venue: ICML 2023
    published_conference: ICML 2023
    at_pub_value: 0.409
    at_pub_std: 0.005
    at_pub_source_arxiv: '2306.02664'
    at_pub_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    at_pub_source_date_iso: '2023-06-05'
    at_pub_source_date_label: NeurIPS 2023
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
    true_value: 0.409
    true_std: 0.005
    value_gap_source_arxiv: '2306.02664'
    value_gap_source_title: 'Structure-free Graph Condensation: From Large-scale Graphs
      to Condensed Graph-free Data'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.409
    sort_std: 0.005
    global_rank: 155
    paper_rank: 155
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
single_proposed_model: GDEM
main_figure: /figures/2310.09202/main_figure.jpegoptim.jpg
---

