---
title: A Piece-wise Polynomial Filtering Approach for Graph Neural Networks
arxiv_id: '2112.03499'
source_url: ''
authors:
- name: Vijay Lingam
  orcid: null
  s2_author_id: '41074153'
  s2_url: null
- name: C. Ekbote
  orcid: null
  s2_author_id: '1491548557'
  s2_url: null
- name: Manan Sharma
  orcid: null
  s2_author_id: '2110202022'
  s2_url: null
- name: Rahul Ragesh
  orcid: null
  s2_author_id: '2066060363'
  s2_url: null
- name: Arun Shankar Iyer
  orcid: null
  s2_author_id: '2397529'
  s2_url: null
- name: Sundararajan Sellamanickam
  orcid: null
  s2_author_id: '1779926'
  s2_url: null
published_date: Dec 7, 2021
published_date_iso: '2021-12-07'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Neural Networks (GNNs) exploit signals from node features and the
  input graph topology to improve node classification task performance. However, these
  models tend to perform poorly on heterophilic graphs, where connected nodes have
  different labels. Recently proposed GNNs work across graphs having varying levels
  of homophily. Among these, models relying on polynomial graph filters have shown
  promise. We observe that solutions to these polynomial graph filter models are also
  solutions to an overdetermined system of equations. It suggests that in some instances,
  the model needs to learn a reasonably high order polynomial. On investigation, we
  find the proposed models ineffective at learning such polynomials due to their designs.
  To mitigate this issue, we perform an eigendecomposition of the graph and propose
  to learn multiple adaptive polynomial filters acting on different subsets of the
  spectrum. We theoretically and empirically show that our proposed model learns a
  better filter, thereby improving classification accuracy. We study various aspects
  of our proposed model including, dependency on the number of eigencomponents utilized,
  latent polynomial filters learned, and performance of the individual polynomials
  on the node classification task. We further show that our model is scalable by evaluating
  over large graphs. Our model achieves performance gains of up to 10\
codebase_url: https://github.com/yushundong/AdaGNN
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- PP-GNN
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
- Heterophilic Graphs
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
- benchmark: Heterophilic Graphs
  benchmark_slug: heterophilic-graphs
  evaluated: 2
  total: 6
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: Amazon-Computers
  rows:
  - model: C (orthogonal)
    model_key: graphtarif
    model_plain: C (orthogonal)
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
    value: 0.825
    std: 0.0123
    paper_value: 0.825
    paper_std: 0.0123
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
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
    gap_vs_at_pub: 0.05349999999999999
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
    value_gap: 0.11620000000000008
    has_value_note: false
    value_note: ''
    sort_value: 0.9412
    sort_std: 0.0008
    global_rank: 2
    paper_rank: 426
    rank_delta: 424
    rank_delta_abs: 424
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Learning on Attribute-Missing Graphs
    comparison_source_arxiv: '2011.01623'
    is_best: false
    is_std_outlier: false
  - model: C (orthogonal)
    model_key: gat
    model_plain: C (orthogonal)
    value: 0.9398
    std: 0.0022
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
    global_rank: 3
    sort_value: 0.9398
    sort_std: 0.0022
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.8203
    std: 0.0204
    paper_value: 0.8203
    paper_std: 0.0204
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
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
    gap_vs_at_pub: 0.009599999999999942
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.08899999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.9093
    sort_std: 0.0018
    global_rank: 84
    paper_rank: 438
    rank_delta: 354
    rank_delta_abs: 354
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.8216
    std: 0.0148
    paper_value: 0.8216
    paper_std: 0.0148
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8968
    true_std: 0.0097
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07520000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.8968
    sort_std: 0.0097
    global_rank: 158
    paper_rank: 434
    rank_delta: 276
    rank_delta_abs: 276
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8238
    std: 0.016
    paper_value: 0.8238
    paper_std: 0.016
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-06-13'
    value_gap_source_date_label: ICML 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8763
    true_std: 0.0048
    value_gap_source_arxiv: '2306.07608'
    value_gap_source_title: 'Finding the Missing-half: Graph Complementary Learning
      for Homophily-prone and Heterophily-prone Graphs'
    value_gap_source_is_current_paper: false
    value_gap: 0.05249999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.8763
    sort_std: 0.0048
    global_rank: 281
    paper_rank: 432
    rank_delta: 151
    rank_delta_abs: 151
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PP-GNN
    model_key: pp-gnn
    model_plain: PP-GNN
    value: 0.8523
    std: 0.0136
    paper_value: 0.8523
    paper_std: 0.0136
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8523
    sort_std: 0.0136
    global_rank: 348
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.6496
    std: 0.0357
    paper_value: 0.6496
    paper_std: 0.0357
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.678
    at_pub_std: 0.0106
    at_pub_source_arxiv: '2110.08727'
    at_pub_source_title: 'Graph-less Neural Networks: Teaching Old MLPs New Tricks
      via Distillation'
    at_pub_source_date_iso: '2021-10-17'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2024-07-16'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: 0.028400000000000092
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8463
    true_std: null
    value_gap_source_arxiv: '2407.11907'
    value_gap_source_title: 'GraphFM: A generalist graph transformer that learns transferable
      representations across diverse domains'
    value_gap_source_is_current_paper: false
    value_gap: 0.1967000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.8463
    sort_std: null
    global_rank: 359
    paper_rank: 516
    rank_delta: 157
    rank_delta_abs: 157
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TDGNN
    model_key: tdgnn
    model_plain: TDGNN
    value: 0.8452
    std: 0.0092
    paper_value: 0.8452
    paper_std: 0.0092
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8452
    sort_std: 0.0092
    global_rank: 362
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LGC
    model_key: lgc
    model_plain: LGC
    value: 0.8344
    std: 0.0177
    paper_value: 0.8344
    paper_std: 0.0177
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8344
    sort_std: 0.0177
    global_rank: 407
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SuperGAT
    model_key: supergat
    model_plain: SuperGAT
    value: 0.8304
    std: 0.0102
    paper_value: 0.8304
    paper_std: 0.0102
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8304
    sort_std: 0.0102
    global_rank: 418
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGCN
    model_key: sgcn
    model_plain: SGCN
    value: 0.8065
    std: 0.0278
    paper_value: 0.8065
    paper_std: 0.0278
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8065
    sort_std: 0.0278
    global_rank: 463
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LR
    model_key: lr
    model_plain: LR
    value: 0.6492
    std: 0.0259
    paper_value: 0.6492
    paper_std: 0.0259
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6492
    sort_std: 0.0259
    global_rank: 517
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
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
  dataset: Cornell
  rows:
  - model: R-SoftGraphAIN
    model_key: p^2gnn
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: acm-gcn
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: rf-gcn
    model_plain: R-SoftGraphAIN
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
  - model: APPNP
    model_key: appnp
    model_plain: APPNP
    value: 0.8189
    std: 0.0625
    paper_value: 0.8189
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.587
    at_pub_std: 0.04
    at_pub_source_arxiv: '2102.11391'
    at_pub_source_title: 'MagNet: A Neural Network for Directed Graphs'
    at_pub_source_date_iso: '2021-02-22'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2023-03-24'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.2319
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9181
    true_std: 0.0196
    value_gap_source_arxiv: '2303.13750'
    value_gap_source_title: 'LON-GNN: Spectral GNNs with Learnable Orthonormal Basis'
    value_gap_source_is_current_paper: false
    value_gap: 0.09920000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.9181
    sort_std: 0.0196
    global_rank: 20
    paper_rank: 171
    rank_delta: 151
    rank_delta_abs: 151
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'MagNet: A Neural Network for Directed Graphs'
    comparison_source_arxiv: '2102.11391'
    is_best: true
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.7811
    std: 0.0655
    paper_value: 0.7811
    paper_std: 0.0655
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-02-04'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9157
    true_std: 0.0196
    value_gap_source_arxiv: '2202.03580'
    value_gap_source_title: Convolutional Neural Networks on Graphs with Chebyshev
      Approximation, Revisited
    value_gap_source_is_current_paper: false
    value_gap: 0.13459999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.9157
    sort_std: 0.0196
    global_rank: 23
    paper_rank: 217
    rank_delta: 194
    rank_delta_abs: 194
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.8378
    std: 0.058
    paper_value: 0.8378
    paper_std: 0.058
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8486
    at_pub_std: 0.0604
    at_pub_source_arxiv: '2106.06134'
    at_pub_source_title: Is Homophily a Necessity for Graph Neural Networks?
    at_pub_source_date_iso: '2021-06-11'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.010800000000000032
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
    value_gap: 0.07579999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.9136
    sort_std: 0.007
    global_rank: 25
    paper_rank: 132
    rank_delta: 107
    rank_delta_abs: 107
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.7919
    std: 0.0979
    paper_value: 0.7919
    paper_std: 0.0979
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8852
    true_std: 0.0133
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.09329999999999994
    has_value_note: false
    value_note: ''
    sort_value: 0.8852
    sort_std: 0.0133
    global_rank: 50
    paper_rank: 201
    rank_delta: 151
    rank_delta_abs: 151
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.8216
    std: 0.048
    paper_value: 0.8216
    paper_std: 0.048
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8216
    at_pub_std: 0.048
    at_pub_source_arxiv: '2103.06064'
    at_pub_source_title: Graph Neural Networks Inspired by Classical Iterative Algorithms
    at_pub_source_date_iso: '2021-03-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2026-03-10'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8623
    true_std: 0.0471
    value_gap_source_arxiv: '2603.09195'
    value_gap_source_title: '$P^2$GNN: Two Prototype Sets to boost GNN Performance'
    value_gap_source_is_current_paper: false
    value_gap: 0.04069999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.8623
    sort_std: 0.0471
    global_rank: 82
    paper_rank: 163
    rank_delta: 81
    rank_delta_abs: 81
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LR
    model_key: lr
    model_plain: LR
    value: 0.8324
    std: 0.0564
    paper_value: 0.8324
    paper_std: 0.0564
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8324
    sort_std: 0.0564
    global_rank: 144
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TDGNN
    model_key: tdgnn
    model_plain: TDGNN
    value: 0.8292
    std: 0.0661
    paper_value: 0.8292
    paper_std: 0.0661
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8292
    sort_std: 0.0661
    global_rank: 149
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PP-GNN
    model_key: pp-gnn
    model_plain: PP-GNN
    value: 0.8243
    std: 0.0427
    paper_value: 0.8243
    paper_std: 0.0427
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8243
    sort_std: 0.0427
    global_rank: 159
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6297
    std: 0.0541
    paper_value: 0.6297
    paper_std: 0.0541
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.5935
    at_pub_std: 0.0419
    at_pub_source_arxiv: '2106.06134'
    at_pub_source_title: Is Homophily a Necessity for Graph Neural Networks?
    at_pub_source_date_iso: '2021-06-11'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2024-05-25'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03620000000000001
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8015
    true_std: 0.0037
    value_gap_source_arxiv: '2405.16185'
    value_gap_source_title: Differentiable Cluster Graph Neural Network
    value_gap_source_is_current_paper: false
    value_gap: 0.17179999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.8015
    sort_std: 0.0037
    global_rank: 190
    paper_rank: 372
    rank_delta: 182
    rank_delta_abs: 182
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LGC
    model_key: lgc
    model_plain: LGC
    value: 0.7459
    std: 0.0342
    paper_value: 0.7459
    paper_std: 0.0342
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.7459
    sort_std: 0.0342
    global_rank: 265
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6081
    at_pub_std: null
    at_pub_source_arxiv: '2103.06064'
    at_pub_source_title: Graph Neural Networks Inspired by Classical Iterative Algorithms
    at_pub_source_date_iso: '2021-03-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-03-02'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
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
    value_gap: 0.03310000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.6412
    sort_std: null
    global_rank: 359
    paper_rank: 385
    rank_delta: 26
    rank_delta_abs: 26
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGCN
    model_key: sgcn
    model_plain: SGCN
    value: 0.6243
    std: 0.049
    paper_value: 0.6243
    paper_std: 0.049
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-22'
    value_gap_source_date_label: IJCAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.6252
    true_std: 0.051
    value_gap_source_arxiv: '2305.13115'
    value_gap_source_title: 'Causal-Based Supervision of Attention in Graph Neural
      Network: A Better and Simpler Choice towards Powerful Attention'
    value_gap_source_is_current_paper: false
    value_gap: 0.0009000000000000119
    has_value_note: false
    value_note: ''
    sort_value: 0.6252
    sort_std: 0.051
    global_rank: 374
    paper_rank: 375
    rank_delta: 1
    rank_delta_abs: 1
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SuperGAT
    model_key: supergat
    model_plain: SuperGAT
    value: 0.573
    std: 0.0853
    paper_value: 0.573
    paper_std: 0.0853
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.573
    at_pub_std: 0.043
    at_pub_source_arxiv: '2110.08128'
    at_pub_source_title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    at_pub_source_date_iso: '2021-10-15'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-15'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.573
    true_std: 0.043
    value_gap_source_arxiv: '2110.08128'
    value_gap_source_title: Label-Wise Graph Convolutional Network for Heterophilic
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.573
    sort_std: 0.043
    global_rank: 440
    paper_rank: 440
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
  dataset: Texas
  rows:
  - model: R-SoftGraphAIN
    model_key: p^2gnn
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: dog
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: gpf-plus
    model_plain: R-SoftGraphAIN
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
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.8135
    std: 0.0532
    paper_value: 0.8135
    paper_std: 0.0532
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-29'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9295
    true_std: 0.0131
    value_gap_source_arxiv: '2505.23014'
    value_gap_source_title: 'Hyperbolic-PDE GNN: Spectral Graph Neural Networks in
      the Perspective of A System of Hyperbolic Partial Differential Equations'
    value_gap_source_is_current_paper: false
    value_gap: 0.11599999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.9295
    sort_std: 0.0131
    global_rank: 36
    paper_rank: 252
    rank_delta: 216
    rank_delta_abs: 216
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
    value: 0.8124
    std: 0.0635
    paper_value: 0.8124
    paper_std: 0.0635
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.833
    at_pub_std: 0.0454
    at_pub_source_arxiv: '2106.06134'
    at_pub_source_title: Is Homophily a Necessity for Graph Neural Networks?
    at_pub_source_date_iso: '2021-06-11'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2024-01-26'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.02059999999999995
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.923
    true_std: 0.007
    value_gap_source_arxiv: '2401.14580'
    value_gap_source_title: 'Design your own universe: a physics-informed agnostic
      method for enhancing graph neural networks'
    value_gap_source_is_current_paper: false
    value_gap: 0.11060000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.923
    sort_std: 0.007
    global_rank: 43
    paper_rank: 259
    rank_delta: 216
    rank_delta_abs: 216
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
    value: 0.8189
    std: 0.0585
    paper_value: 0.8189
    paper_std: 0.0585
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6068
    at_pub_std: 0.045
    at_pub_source_arxiv: '2108.10521'
    at_pub_source_title: 'Bag of Tricks for Training Deeper Graph Neural Networks:
      A Comprehensive Benchmark Study'
    at_pub_source_date_iso: '2021-08-24'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-10-18'
    value_gap_source_date_label: WWW 2023
    gap_vs_at_pub: 0.21209999999999996
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9131
    true_std: 0.0197
    value_gap_source_arxiv: '2310.11762'
    value_gap_source_title: A Quasi-Wasserstein Loss for Learning Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.09420000000000006
    has_value_note: false
    value_note: ''
    sort_value: 0.9131
    sort_std: 0.0197
    global_rank: 55
    paper_rank: 239
    rank_delta: 184
    rank_delta_abs: 184
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Bag of Tricks for Training Deeper Graph Neural Networks:
      A Comprehensive Benchmark Study'
    comparison_source_arxiv: '2108.10521'
    is_best: false
    is_std_outlier: false
  - model: PP-GNN
    model_key: pp-gnn
    model_plain: PP-GNN
    value: 0.8973
    std: 0.049
    paper_value: 0.8973
    paper_std: 0.049
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8973
    sort_std: 0.049
    global_rank: 74
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: FAGCN
    model_key: fagcn
    model_plain: FAGCN
    value: 0.8243
    std: 0.0689
    paper_value: 0.8243
    paper_std: 0.0689
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.795
    at_pub_std: 0.048
    at_pub_source_arxiv: '2110.08128'
    at_pub_source_title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    at_pub_source_date_iso: '2021-10-15'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-12-07'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: 0.029299999999999993
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.8961
    true_std: 0.0152
    value_gap_source_arxiv: '2212.03654'
    value_gap_source_title: Node-oriented Spectral Filtering for Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07179999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.8961
    sort_std: 0.0152
    global_rank: 75
    paper_rank: 221
    rank_delta: 146
    rank_delta_abs: 146
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: H2GCN
    model_key: h2gcn
    model_plain: H2GCN
    value: 0.8486
    std: 0.0677
    paper_value: 0.8486
    paper_std: 0.0677
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.8486
    at_pub_std: 0.0677
    at_pub_source_arxiv: '2103.06064'
    at_pub_source_title: Graph Neural Networks Inspired by Classical Iterative Algorithms
    at_pub_source_date_iso: '2021-03-10'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2024-06-01'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.8765
    true_std: null
    value_gap_source_arxiv: '2406.10863'
    value_gap_source_title: Global-Local Graph Neural Networks for Node-Classification
    value_gap_source_is_current_paper: false
    value_gap: 0.027899999999999925
    has_value_note: false
    value_note: ''
    sort_value: 0.8765
    sort_std: null
    global_rank: 101
    paper_rank: 172
    rank_delta: 71
    rank_delta_abs: 71
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TDGNN
    model_key: tdgnn
    model_plain: TDGNN
    value: 0.83
    std: 0.045
    paper_value: 0.83
    paper_std: 0.045
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.83
    sort_std: 0.045
    global_rank: 213
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LR
    model_key: lr
    model_plain: LR
    value: 0.8135
    std: 0.0633
    paper_value: 0.8135
    paper_std: 0.0633
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8135
    sort_std: 0.0633
    global_rank: 255
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: LGC
    model_key: lgc
    model_plain: LGC
    value: 0.802
    std: 0.0428
    paper_value: 0.802
    paper_std: 0.0428
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.802
    sort_std: 0.0428
    global_rank: 282
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6162
    std: 0.0614
    paper_value: 0.6162
    paper_std: 0.0614
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.6381
    at_pub_std: 0.0527
    at_pub_source_arxiv: '2106.06134'
    at_pub_source_title: Is Homophily a Necessity for Graph Neural Networks?
    at_pub_source_date_iso: '2021-06-11'
    at_pub_source_date_label: ICLR 2021
    value_gap_source_date_iso: '2025-04-22'
    value_gap_source_date_label: WWW 2025
    gap_vs_at_pub: 0.02190000000000003
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
    value_gap: 0.17710000000000004
    has_value_note: false
    value_note: ''
    sort_value: 0.7933
    sort_std: 0.0447
    global_rank: 299
    paper_rank: 515
    rank_delta: 216
    rank_delta_abs: 216
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Geom-GCN
    model_key: geom-gcn
    model_plain: Geom-GCN
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.676
    at_pub_std: null
    at_pub_source_arxiv: '2005.14612'
    at_pub_source_title: Non-Local Graph Neural Networks
    at_pub_source_date_iso: '2020-05-29'
    at_pub_source_date_label: '2020'
    value_gap_source_date_iso: '2020-05-29'
    value_gap_source_date_label: '2020'
    gap_vs_at_pub: 0.000300000000000078
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.676
    true_std: null
    value_gap_source_arxiv: '2005.14612'
    value_gap_source_title: Non-Local Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.000300000000000078
    has_value_note: false
    value_note: ''
    sort_value: 0.676
    sort_std: null
    global_rank: 443
    paper_rank: 443
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Non-Local Graph Neural Networks
    comparison_source_arxiv: '2005.14612'
    is_best: false
    is_std_outlier: false
  - model: SuperGAT
    model_key: supergat
    model_plain: SuperGAT
    value: 0.6108
    std: 0.0497
    paper_value: 0.6108
    paper_std: 0.0497
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.586
    at_pub_std: 0.077
    at_pub_source_arxiv: '2110.08128'
    at_pub_source_title: Label-Wise Graph Convolutional Network for Heterophilic Graphs
    at_pub_source_date_iso: '2021-10-15'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-10-15'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: 0.024800000000000044
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.586
    true_std: 0.077
    value_gap_source_arxiv: '2110.08128'
    value_gap_source_title: Label-Wise Graph Convolutional Network for Heterophilic
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.024800000000000044
    has_value_note: false
    value_note: ''
    sort_value: 0.586
    sort_std: 0.077
    global_rank: 559
    paper_rank: 525
    rank_delta: -34
    rank_delta_abs: 34
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGCN
    model_key: sgcn
    model_plain: SGCN
    value: 0.6243
    std: 0.0443
    paper_value: 0.6243
    paper_std: 0.0443
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 7, 2021
    date_display: Dec 2021
    date_iso: '2021-12-07'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-05-22'
    value_gap_source_date_label: IJCAI 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.5641
    true_std: 0.0429
    value_gap_source_arxiv: '2305.13115'
    value_gap_source_title: 'Causal-Based Supervision of Attention in Graph Neural
      Network: A Better and Simpler Choice towards Powerful Attention'
    value_gap_source_is_current_paper: false
    value_gap: 0.06019999999999992
    has_value_note: false
    value_note: ''
    sort_value: 0.5641
    sort_std: 0.0429
    global_rank: 589
    paper_rank: 506
    rank_delta: -83
    rank_delta_abs: 83
    rank_delta_direction: better
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
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
- benchmark: Heterophilic Graphs
  datasets:
  - *id002
  - *id003
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
  - benchmark: Heterophilic Graphs
    benchmark_slug: heterophilic-graphs
    datasets:
    - dataset: Texas
      dataset_slug: texas
    - dataset: Cornell
      dataset_slug: cornell
single_proposed_model: PP-GNN
main_figure: /figures/2112.03499/main_figure.jpegoptim.jpg
---

