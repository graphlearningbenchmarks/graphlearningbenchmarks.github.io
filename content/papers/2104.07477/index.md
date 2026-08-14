---
title: Lorentzian Graph Convolutional Networks
arxiv_id: '2104.07477'
source_url: ''
authors:
- name: Yiding Zhang
  orcid: null
  s2_author_id: '93506381'
  s2_url: null
- name: Xiao Wang
  orcid: null
  s2_author_id: '2118449003'
  s2_url: null
- name: C. Shi
  orcid: null
  s2_author_id: '144123161'
  s2_url: null
- name: Nian Liu
  orcid: null
  s2_author_id: '2087010708'
  s2_url: null
- name: Guojie Song
  orcid: null
  s2_author_id: '2090871'
  s2_url: null
published_date: Apr 15, 2021
published_date_iso: '2021-04-15'
published_venue: WWW 2021
published_conference: WWW 2021
published_conference_short: WWW
published_conference_slug: www
abstract: Graph convolutional networks (GCNs) have received considerable research
  attention recently. Most GCNs learn the node representations in Euclidean geometry,
  but that could have a high distortion in the case of embedding graphs with scale-free
  or hierarchical structure. Recently, some GCNs are proposed to deal with this problem
  in non-Euclidean geometry, e.g., hyperbolic geometry. Although hyperbolic GCNs achieve
  promising performance, existing hyperbolic graph operations actually cannot rigorously
  follow the hyperbolic geometry, which may limit the ability of hyperbolic geometry
  and thus hurt the performance of hyperbolic GCNs. In this paper, we propose a novel
  hyperbolic GCN named Lorentzian graph convolutional network (LGCN), which rigorously
  guarantees the learned node features follow the hyperbolic geometry. Specifically,
  we rebuild the graph operations of hyperbolic GCNs with Lorentzian version, e.g.,
  the feature transformation and non-linear activation. Also, an elegant neighborhood
  aggregation method is designed based on the centroid of Lorentzian distance. Moreover,
  we prove some proposed graph operations are equivalent in different types of hyperbolic
  geometry, which fundamentally indicates their correctness. Experiments on six datasets
  show that LGCN performs better than the state-of-the-art methods. LGCN has lower
  distortion to learn the representation of tree-likeness graphs compared with existing
  hyperbolic GCNs. We also find that the performance of some hyperbolic GCNs can be
  improved by simply replacing the graph operations with those we defined in this
  paper.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- LGCN
mrr: 0.0022
adjusted_mrr: 0.0022
mrr_dataset_count: 3
benchmark_categories:
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Amazon2M
  rows:
  - model: GFD
    model_key: gfd
    model_plain: GFD
    value: 0.9757
    std: 0.0012
    metric: AUC
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2412.00020'
    title: Partitioning Message Passing for Graph Fraud Detection
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Xtra-Computing/PMP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9757
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: BWGNN
    model_key: bwgnn
    model_plain: BWGNN
    value: 0.9742
    std: 0.0048
    metric: AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.00020'
    title: Partitioning Message Passing for Graph Fraud Detection
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Xtra-Computing/PMP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9742
    sort_std: 0.0048
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GDN
    model_key: gdn
    model_plain: GDN
    value: 0.9709
    std: 0.0016
    metric: AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2412.00020'
    title: Partitioning Message Passing for Graph Fraud Detection
    date: Nov 16, 2024
    date_display: Nov 2024
    date_iso: '2024-11-16'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/Xtra-Computing/PMP
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9709
    sort_std: 0.0016
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LGCN
    model_key: lgcn
    model_plain: LGCN
    value: 0.964
    std: 0.011
    paper_value: 0.964
    paper_std: 0.011
    metric: AUC
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 15, 2021
    date_display: Apr 2021
    date_iso: '2021-04-15'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-15'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.964
    true_std: 0.011
    value_gap_source_arxiv: '2104.07477'
    value_gap_source_title: Lorentzian Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.964
    sort_std: 0.011
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DeepWalk
    model_key: deepwalk
    model_plain: DeepWalk
    value: 0.961
    std: 0.0
    paper_value: 0.961
    paper_std: 0.0
    metric: AUC
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
    variant_inference_reason: 'dataset: fuzzy match to amazon2m (score=86)'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 15, 2021
    date_display: Apr 2021
    date_iso: '2021-04-15'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-15'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.961
    true_std: 0.0
    value_gap_source_arxiv: '2104.07477'
    value_gap_source_title: Lorentzian Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.961
    sort_std: 0.0
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
  - model: HAT
    model_key: hat
    model_plain: HAT
    value: 0.948
    std: 0.008
    paper_value: 0.948
    paper_std: 0.008
    metric: AUC
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 15, 2021
    date_display: Apr 2021
    date_iso: '2021-04-15'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-15'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.948
    true_std: 0.008
    value_gap_source_arxiv: '2104.07477'
    value_gap_source_title: Lorentzian Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.948
    sort_std: 0.008
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGCN
    model_key: hgcn
    model_plain: HGCN
    value: 0.935
    std: 0.006
    paper_value: 0.935
    paper_std: 0.006
    metric: AUC
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 15, 2021
    date_display: Apr 2021
    date_iso: '2021-04-15'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-15'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.935
    true_std: 0.006
    value_gap_source_arxiv: '2104.07477'
    value_gap_source_title: Lorentzian Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.935
    sort_std: 0.006
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
  - model: GraphSAGE
    model_key: graphsage
    model_plain: GraphSAGE
    value: 0.904
    std: 0.003
    paper_value: 0.904
    paper_std: 0.003
    metric: AUC
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 15, 2021
    date_display: Apr 2021
    date_iso: '2021-04-15'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.7527
    at_pub_std: null
    at_pub_source_arxiv: '2008.08692'
    at_pub_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    at_pub_source_date_iso: '2020-08-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2024-11-16'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.1513
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9316
    true_std: 0.0087
    value_gap_source_arxiv: '2412.00020'
    value_gap_source_title: Partitioning Message Passing for Graph Fraud Detection
    value_gap_source_is_current_paper: false
    value_gap: 0.027599999999999958
    has_value_note: false
    value_note: ''
    sort_value: 0.9316
    sort_std: 0.0087
    global_rank: 13
    paper_rank: 16
    rank_delta: 3
    rank_delta_abs: 3
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Enhancing Graph Neural Network-based Fraud Detectors
      against Camouflaged Fraudsters
    comparison_source_arxiv: '2008.08692'
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.913
    std: 0.006
    paper_value: 0.913
    paper_std: 0.006
    metric: AUC
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 15, 2021
    date_display: Apr 2021
    date_iso: '2021-04-15'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.7516
    at_pub_std: null
    at_pub_source_arxiv: '2008.08692'
    at_pub_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    at_pub_source_date_iso: '2020-08-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2021-04-15'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: 0.1614
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.913
    true_std: 0.006
    value_gap_source_arxiv: '2104.07477'
    value_gap_source_title: Lorentzian Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.913
    sort_std: 0.006
    global_rank: 14
    paper_rank: 14
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Enhancing Graph Neural Network-based Fraud Detectors
      against Camouflaged Fraudsters
    comparison_source_arxiv: '2008.08692'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.911
    std: 0.006
    paper_value: 0.911
    paper_std: 0.006
    metric: AUC
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 15, 2021
    date_display: Apr 2021
    date_iso: '2021-04-15'
    published_venue: WWW 2021
    published_conference: WWW 2021
    at_pub_value: 0.7525
    at_pub_std: null
    at_pub_source_arxiv: '2008.08692'
    at_pub_source_title: Enhancing Graph Neural Network-based Fraud Detectors against
      Camouflaged Fraudsters
    at_pub_source_date_iso: '2020-08-19'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2021-04-15'
    value_gap_source_date_label: WWW 2021
    gap_vs_at_pub: 0.15850000000000009
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.911
    true_std: 0.006
    value_gap_source_arxiv: '2104.07477'
    value_gap_source_title: Lorentzian Graph Convolutional Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.911
    sort_std: 0.006
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Enhancing Graph Neural Network-based Fraud Detectors
      against Camouflaged Fraudsters
    comparison_source_arxiv: '2008.08692'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.7535
    std: null
    metric: AUC
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2401.14155'
    title: Alleviating Structural Distribution Shift in Graph Anomaly Detection
    date: Feb 27, 2023
    date_display: Feb 2023
    date_iso: '2023-02-27'
    venue: Web Search and Data Mining
    codebase_url: https://github.com/blacksingular/wsdm_GDN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 26
    sort_value: 0.7535
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AUC
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - AUC
  metric: AUC
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Other Graph Benchmarks
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: Amazon2M
      dataset_slug: amazon2m
single_proposed_model: LGCN
main_figure: /figures/2104.07477/main_figure.jpegoptim.jpg
---

