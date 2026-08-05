---
title: Motif-driven Subgraph Structure Learning for Graph Classification
arxiv_id: '2406.08897'
source_url: ''
authors:
- name: Zhiyao Zhou
  orcid: null
  s2_author_id: '151481855'
  s2_url: null
- name: Sheng Zhou
  orcid: null
  s2_author_id: '2115867010'
  s2_url: null
- name: Bochao Mao
  orcid: null
  s2_author_id: '2179479629'
  s2_url: null
- name: Jiawei Chen
  orcid: null
  s2_author_id: '2115448385'
  s2_url: null
- name: Qingyun Sun
  orcid: null
  s2_author_id: '2287980208'
  s2_url: null
- name: Yan Feng
  orcid: null
  s2_author_id: '1692947908'
  s2_url: null
- name: Chun Chen
  orcid: null
  s2_author_id: '2109525713'
  s2_url: null
- name: Can Wang
  orcid: null
  s2_author_id: '2279089364'
  s2_url: null
published_date: Jun 13, 2024
published_date_iso: '2024-06-13'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: To mitigate the suboptimal nature of graph structure, Graph Structure Learning
  (GSL) has emerged as a promising approach to improve graph structure and boost performance
  in downstream tasks. Despite the proposal of numerous GSL methods, the progresses
  in this field mostly concentrated on node-level tasks, while graph-level tasks (e.g.,
  graph classification) remain largely unexplored. Notably, applying node-level GSL
  to graph classification is non-trivial due to the lack of find-grained guidance
  for intricate structure learning. Inspired by the vital role of subgraph in graph
  classification, in this paper we explore the potential of subgraph structure learning
  for graph classification by tackling the challenges of key subgraph selection and
  structure optimization. We propose a novel Motif-driven Subgraph Structure Learning
  method for Graph Classification (MOSGSL). Specifically, MOSGSL incorporates a subgraph
  structure learning module which can adaptively select important subgraphs. A motif-driven
  structure guidance module is further introduced to capture key subgraph-level structural
  patterns (motifs) and facilitate personalized structure learning. Extensive experiments
  demonstrate a significant and consistent improvement over baselines, as well as
  its flexibility and generalizability for various backbones and learning procedures.
  The code is available in the.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 3
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: ENZYMES
  rows:
  - model: WL
    model_key: bgnn(m)-cs
    model_plain: WL
    value: 0.8068
    std: 0.0149
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.8068
    sort_std: 0.0149
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: WL
    model_key: bgnn
    model_plain: WL
    value: 0.7936
    std: 0.0281
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.7936
    sort_std: 0.0281
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: WL
    model_key: bgnn(m)-sc
    model_plain: WL
    value: 0.7889
    std: 0.0079
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2210.05920'
    title: Boosting Graph Neural Networks via Adaptive Knowledge Distillation
    date: Oct 12, 2022
    date_display: Oct 2022
    date_iso: '2022-10-12'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7889
    sort_std: 0.0079
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.54
    std: 0.0517
    paper_value: 0.54
    paper_std: 0.0517
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.762
    at_pub_std: 0.028
    at_pub_source_arxiv: '2305.06102'
    at_pub_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    at_pub_source_date_iso: '2023-05-10'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.22199999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.762
    true_std: 0.028
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: 0.22199999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.762
    sort_std: 0.028
    global_rank: 8
    paper_rank: 163
    rank_delta: 155
    rank_delta_abs: 155
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    comparison_source_arxiv: '2305.06102'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.4867
    std: 0.0571
    paper_value: 0.4867
    paper_std: 0.0571
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.665
    at_pub_std: 0.0691
    at_pub_source_arxiv: '2012.08734'
    at_pub_source_title: Hierarchical Graph Capsule Network
    at_pub_source_date_iso: '2020-12-16'
    at_pub_source_date_label: AAAI 2020
    value_gap_source_date_iso: '2020-12-16'
    value_gap_source_date_label: AAAI 2020
    gap_vs_at_pub: 0.17830000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.665
    true_std: 0.0691
    value_gap_source_arxiv: '2012.08734'
    value_gap_source_title: Hierarchical Graph Capsule Network
    value_gap_source_is_current_paper: false
    value_gap: 0.17830000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.665
    sort_std: 0.0691
    global_rank: 48
    paper_rank: 183
    rank_delta: 135
    rank_delta_abs: 135
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Hierarchical Graph Capsule Network
    comparison_source_arxiv: '2012.08734'
    is_best: false
    is_std_outlier: false
  - model: GMT
    model_key: gmt
    model_plain: GMT
    value: 0.6033
    std: 0.0661
    paper_value: 0.6033
    paper_std: 0.0661
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6033
    true_std: 0.0661
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6033
    sort_std: 0.0661
    global_rank: 112
    paper_rank: 112
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NeuralSparse
    model_key: neuralsparse
    model_plain: NeuralSparse
    value: 0.5967
    std: 0.0515
    paper_value: 0.5967
    paper_std: 0.0515
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy (SAGE backbone)
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5967
    true_std: 0.0515
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5967
    sort_std: 0.0515
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
  - model: VIBGSL
    model_key: vibgsl
    model_plain: VIBGSL
    value: 0.5833
    std: 0.0405
    paper_value: 0.5833
    paper_std: 0.0405
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy (SAGE backbone)
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5833
    true_std: 0.0405
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5833
    sort_std: 0.0405
    global_rank: 131
    paper_rank: 131
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGP-SL
    model_key: hgp-sl
    model_plain: HGP-SL
    value: 0.5583
    std: 0.0746
    paper_value: 0.5583
    paper_std: 0.0746
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy (GIN backbone)
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5583
    true_std: 0.0746
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5583
    sort_std: 0.0746
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
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.555
    std: 0.0511
    paper_value: 0.555
    paper_std: 0.0511
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.3799
    at_pub_std: 0.037
    at_pub_source_arxiv: '2406.01249'
    at_pub_source_title: Equivariant Machine Learning on Graphs with Nonlinear Spectral
      Filters
    at_pub_source_date_iso: '2024-06-03'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.17510000000000003
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.555
    true_std: 0.0511
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.555
    sort_std: 0.0511
    global_rank: 147
    paper_rank: 147
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Equivariant Machine Learning on Graphs with Nonlinear
      Spectral Filters
    comparison_source_arxiv: '2406.01249'
    is_best: false
    is_std_outlier: false
  - model: EdgePool
    model_key: edgepool
    model_plain: EdgePool
    value: 0.5517
    std: 0.0926
    paper_value: 0.5517
    paper_std: 0.0926
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5517
    true_std: 0.0926
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5517
    sort_std: 0.0926
    global_rank: 151
    paper_rank: 151
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TopKPool
    model_key: topkpool
    model_plain: TopKPool
    value: 0.5267
    std: 0.0754
    paper_value: 0.5267
    paper_std: 0.0754
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5267
    true_std: 0.0754
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5267
    sort_std: 0.0754
    global_rank: 169
    paper_rank: 169
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAUG
    model_key: gaug
    model_plain: GAUG
    value: 0.5233
    std: 0.0902
    paper_value: 0.5233
    paper_std: 0.0902
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy (SAGE backbone)
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5233
    true_std: 0.0902
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5233
    sort_std: 0.0902
    global_rank: 172
    paper_rank: 172
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRCN
    model_key: grcn
    model_plain: GRCN
    value: 0.4817
    std: 0.0558
    paper_value: 0.4817
    paper_std: 0.0558
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV accuracy (SAGE backbone)
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.4817
    true_std: 0.0558
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.4817
    sort_std: 0.0558
    global_rank: 189
    paper_rank: 189
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
- &id001
  dataset: PROTEINS
  rows:
  - model: Graphormer-SPIS
    model_key: gmn
    model_plain: Graphormer-SPIS
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
    global_rank: 1
    sort_value: 0.8225
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: ci-gnn
    model_plain: Graphormer-SPIS
    value: 0.82
    std: 0.02
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2301.01642'
    title: 'CI-GNN: A Granger Causality-Inspired Graph Neural Network for Interpretable
      Brain Network-Based Psychiatric Diagnosis'
    date: Jan 4, 2023
    date_display: Jan 2023
    date_iso: '2023-01-04'
    venue: Neural Networks
    codebase_url: https://github.com/ZKZ-Brain/CI-GNN
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.82
    sort_std: 0.02
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: diffpool+gpl
    model_plain: Graphormer-SPIS
    value: 0.8196
    std: 0.0286
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.11361'
    title: 'Graph Structure Prompt Learning: A Novel Methodology to Improve Performance
      of Graph Neural Networks'
    date: Jul 16, 2024
    date_display: Jul 2024
    date_iso: '2024-07-16'
    venue: Applied intelligence (Boston)
    codebase_url: https://github.com/PreckLi/graph_prompt_learning
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.8196
    sort_std: 0.0286
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.6918
    std: 0.0285
    paper_value: 0.6918
    paper_std: 0.0285
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV (mean of 10 runs) on PROTEINS
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
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
    gap_vs_at_pub: 0.09620000000000006
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.788
    true_std: 0.041
    value_gap_source_arxiv: '2312.08671'
    value_gap_source_title: 'Permutation-Invariant graph partitioning: How graph neural
      networks capture structural interactions?'
    value_gap_source_is_current_paper: false
    value_gap: 0.09620000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.788
    sort_std: 0.041
    global_rank: 27
    paper_rank: 463
    rank_delta: 436
    rank_delta_abs: 436
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Permutation-Invariant graph partitioning: How graph
      neural networks capture structural interactions?'
    comparison_source_arxiv: '2312.08671'
    is_best: true
    is_std_outlier: false
  - model: TopKPool
    model_key: topkpool
    model_plain: TopKPool
    value: 0.7133
    std: 0.0656
    paper_value: 0.7133
    paper_std: 0.0656
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV (mean of 10 runs) on PROTEINS
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7768
    at_pub_std: null
    at_pub_source_arxiv: '2002.09518'
    at_pub_source_title: Memory-Based Graph Networks
    at_pub_source_date_iso: '2020-02-21'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2020-02-21'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: 0.0635
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7768
    true_std: null
    value_gap_source_arxiv: '2002.09518'
    value_gap_source_title: Memory-Based Graph Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0635
    has_value_note: false
    value_note: ''
    sort_value: 0.7768
    sort_std: null
    global_rank: 52
    paper_rank: 431
    rank_delta: 379
    rank_delta_abs: 379
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.6856
    std: 0.0493
    paper_value: 0.6856
    paper_std: 0.0493
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV (mean of 10 runs) on PROTEINS
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7726
    at_pub_std: 0.0228
    at_pub_source_arxiv: '1904.05003'
    at_pub_source_title: 'Semi-Supervised Graph Classification: A Hierarchical Graph
      Perspective'
    at_pub_source_date_iso: '2019-04-10'
    at_pub_source_date_label: WWW 2019
    value_gap_source_date_iso: '2019-04-10'
    value_gap_source_date_label: WWW 2019
    gap_vs_at_pub: 0.08699999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7726
    true_std: 0.0228
    value_gap_source_arxiv: '1904.05003'
    value_gap_source_title: 'Semi-Supervised Graph Classification: A Hierarchical
      Graph Perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.08699999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.7726
    sort_std: 0.0228
    global_rank: 63
    paper_rank: 465
    rank_delta: 402
    rank_delta_abs: 402
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Semi-Supervised Graph Classification: A Hierarchical
      Graph Perspective'
    comparison_source_arxiv: '1904.05003'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6649
    std: 0.0458
    paper_value: 0.6649
    paper_std: 0.0458
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV (mean of 10 runs) on PROTEINS
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
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
    gap_vs_at_pub: 0.10159999999999991
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7665
    true_std: 0.0314
    value_gap_source_arxiv: '2402.16346'
    value_gap_source_title: Boosting Graph Pooling with Persistent Homology
    value_gap_source_is_current_paper: false
    value_gap: 0.10159999999999991
    has_value_note: false
    value_note: ''
    sort_value: 0.7665
    sort_std: 0.0314
    global_rank: 94
    paper_rank: 477
    rank_delta: 383
    rank_delta_abs: 383
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Boosting Graph Pooling with Persistent Homology
    comparison_source_arxiv: '2402.16346'
    is_best: false
    is_std_outlier: false
  - model: EdgePool
    model_key: edgepool
    model_plain: EdgePool
    value: 0.7134
    std: 0.0455
    paper_value: 0.7134
    paper_std: 0.0455
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV (mean of 10 runs) on PROTEINS
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.756
    at_pub_std: 0.024
    at_pub_source_arxiv: '2205.15068'
    at_pub_source_title: Embedding Graphs on Grassmann Manifold
    at_pub_source_date_iso: '2022-05-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2022-05-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.04259999999999997
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.756
    true_std: 0.024
    value_gap_source_arxiv: '2205.15068'
    value_gap_source_title: Embedding Graphs on Grassmann Manifold
    value_gap_source_is_current_paper: false
    value_gap: 0.04259999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.756
    sort_std: 0.024
    global_rank: 193
    paper_rank: 431
    rank_delta: 238
    rank_delta_abs: 238
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMT
    model_key: gmt
    model_plain: GMT
    value: 0.7377
    std: 0.0569
    paper_value: 0.7377
    paper_std: 0.0569
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV (mean of 10 runs) on PROTEINS
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.7509
    at_pub_std: 0.0059
    at_pub_source_arxiv: '2206.13510'
    at_pub_source_title: Structural Entropy Guided Graph Hierarchical Pooling
    at_pub_source_date_iso: '2022-06-26'
    at_pub_source_date_label: ICML 2022
    value_gap_source_date_iso: '2022-06-26'
    value_gap_source_date_label: ICML 2022
    gap_vs_at_pub: 0.01319999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.7509
    true_std: 0.0059
    value_gap_source_arxiv: '2206.13510'
    value_gap_source_title: Structural Entropy Guided Graph Hierarchical Pooling
    value_gap_source_is_current_paper: false
    value_gap: 0.01319999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.7509
    sort_std: 0.0059
    global_rank: 251
    paper_rank: 337
    rank_delta: 86
    rank_delta_abs: 86
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HGP-SL
    model_key: hgp-sl
    model_plain: HGP-SL
    value: 0.7188
    std: 0.0435
    paper_value: 0.7188
    paper_std: 0.0435
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV (mean of 10 runs) on PROTEINS
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7188
    true_std: 0.0435
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7188
    sort_std: 0.0435
    global_rank: 418
    paper_rank: 418
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VIBGSL
    model_key: vibgsl
    model_plain: VIBGSL
    value: 0.7161
    std: 0.0457
    paper_value: 0.7161
    paper_std: 0.0457
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV (mean of 10 runs) on PROTEINS
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7161
    true_std: 0.0457
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7161
    sort_std: 0.0457
    global_rank: 429
    paper_rank: 429
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NeuralSparse
    model_key: neuralsparse
    model_plain: NeuralSparse
    value: 0.6847
    std: 0.0385
    paper_value: 0.6847
    paper_std: 0.0385
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV (mean of 10 runs) on PROTEINS
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6847
    true_std: 0.0385
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6847
    sort_std: 0.0385
    global_rank: 467
    paper_rank: 467
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GRCN
    model_key: grcn
    model_plain: GRCN
    value: 0.6069
    std: 0.0229
    paper_value: 0.6069
    paper_std: 0.0229
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV (mean of 10 runs) on PROTEINS
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6069
    true_std: 0.0229
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6069
    sort_std: 0.0229
    global_rank: 512
    paper_rank: 512
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAUG
    model_key: gaug
    model_plain: GAUG
    value: 0.5957
    std: 0.07
    paper_value: 0.5957
    paper_std: 0.07
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV (mean of 10 runs) on PROTEINS
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5957
    true_std: 0.07
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5957
    sort_std: 0.07
    global_rank: 515
    paper_rank: 515
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
- &id003
  dataset: RDT-B
  rows:
  - model: CIN
    model_key: oepg
    model_plain: CIN
    value: 0.963
    std: 0.009
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2205.15746'
    title: Omni-Granular Ego-Semantic Propagation for Self-Supervised Graph Representation
      Learning
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.963
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CIN
    model_key: msh-gnn
    model_plain: CIN
    value: 0.958
    std: 0.009
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
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.958
    sort_std: 0.009
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: CIN
    model_key: gnn-ak+
    model_plain: CIN
    value: 0.948
    std: 0.008
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2110.03753'
    title: 'From Stars to Subgraphs: Uplifting Any GNN with Local Structure Awareness'
    date: Oct 7, 2021
    date_display: Oct 2021
    date_iso: '2021-10-07'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/LingxiaoShawn/GNNAsKernel
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.948
    sort_std: 0.008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.755
    std: 0.024
    paper_value: 0.755
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV, Accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.924
    at_pub_std: null
    at_pub_source_arxiv: '2103.00111'
    at_pub_source_title: 'Graph Self-Supervised Learning: A Survey'
    at_pub_source_date_iso: '2021-02-27'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-05-10'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: 0.16900000000000004
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.924
    true_std: 0.025
    value_gap_source_arxiv: '2305.06102'
    value_gap_source_title: Towards Better Graph Representation Learning with Parameterized
      Decomposition & Filtering
    value_gap_source_is_current_paper: false
    value_gap: 0.16900000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.924
    sort_std: 0.025
    global_rank: 12
    paper_rank: 68
    rank_delta: 56
    rank_delta_abs: 56
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Graph Self-Supervised Learning: A Survey'
    comparison_source_arxiv: '2103.00111'
    is_best: false
    is_std_outlier: false
  - model: TopKPool
    model_key: topkpool
    model_plain: TopKPool
    value: 0.848
    std: 0.0625
    paper_value: 0.848
    paper_std: 0.0625
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV, Accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.848
    true_std: 0.0625
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.848
    sort_std: 0.0625
    global_rank: 54
    paper_rank: 54
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GMT
    model_key: gmt
    model_plain: GMT
    value: 0.8415
    std: 0.0247
    paper_value: 0.8415
    paper_std: 0.0247
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV, Accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8415
    true_std: 0.0247
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8415
    sort_std: 0.0247
    global_rank: 56
    paper_rank: 56
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NeuralSparse
    model_key: neuralsparse
    model_plain: NeuralSparse
    value: 0.8125
    std: 0.0223
    paper_value: 0.8125
    paper_std: 0.0223
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV, Accuracy (GIN backbone)
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8125
    true_std: 0.0223
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8125
    sort_std: 0.0223
    global_rank: 58
    paper_rank: 58
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EdgePool
    model_key: edgepool
    model_plain: EdgePool
    value: 0.8115
    std: 0.0356
    paper_value: 0.8115
    paper_std: 0.0356
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV, Accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8115
    true_std: 0.0356
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8115
    sort_std: 0.0356
    global_rank: 59
    paper_rank: 59
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: VIBGSL
    model_key: vibgsl
    model_plain: VIBGSL
    value: 0.7645
    std: 0.0297
    paper_value: 0.7645
    paper_std: 0.0297
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV, Accuracy (GIN backbone)
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.7645
    true_std: 0.0297
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.7645
    sort_std: 0.0297
    global_rank: 67
    paper_rank: 67
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
    value: 0.706
    std: 0.0369
    paper_value: 0.706
    paper_std: 0.0369
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV, Accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5
    at_pub_std: 0.0
    at_pub_source_arxiv: '2106.09645'
    at_pub_source_title: Prototypical Graph Contrastive Learning
    at_pub_source_date_iso: '2021-06-17'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.20599999999999996
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.706
    true_std: 0.0369
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.706
    sort_std: 0.0369
    global_rank: 73
    paper_rank: 73
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Prototypical Graph Contrastive Learning
    comparison_source_arxiv: '2106.09645'
    is_best: false
    is_std_outlier: false
  - model: SAGE
    model_key: sage
    model_plain: SAGE
    value: 0.678
    std: 0.0424
    paper_value: 0.678
    paper_std: 0.0424
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: 10-fold CV, Accuracy
    date: Jun 13, 2024
    date_display: Jun 2024
    date_iso: '2024-06-13'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-13'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.678
    true_std: 0.0424
    value_gap_source_arxiv: '2406.08897'
    value_gap_source_title: Motif-driven Subgraph Structure Learning for Graph Classification
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.678
    sort_std: 0.0424
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
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: PROTEINS
      dataset_slug: proteins
    - dataset: ENZYMES
      dataset_slug: enzymes
    - dataset: RDT-B
      dataset_slug: rdt-b
main_figure: /figures/2406.08897/main_figure.jpegoptim.jpg
---

