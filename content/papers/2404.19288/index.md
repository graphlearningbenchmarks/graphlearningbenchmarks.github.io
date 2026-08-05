---
title: Training-free Graph Neural Networks and the Power of Labels as Features
arxiv_id: '2404.19288'
source_url: ''
authors:
- name: Ryoma Sato
  orcid: null
  s2_author_id: '2330247302'
  s2_url: null
published_date: Apr 30, 2024
published_date_iso: '2024-04-30'
published_venue: TMLR 2024
published_conference: TMLR 2024
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: We propose training-free graph neural networks (TFGNNs), which can be used
  without training and can also be improved with optional training, for transductive
  node classification. We first advocate labels as features (LaF), which is an admissible
  but not explored technique. We show that LaF provably enhances the expressive power
  of graph neural networks. We design TFGNNs based on this analysis. In the experiments,
  we confirm that TFGNNs outperform existing GNNs in the training-free setting and
  converge with much fewer training iterations than traditional GNNs.
codebase_url: https://github.com/joisino/laf
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- TFGNNs + random initialization
- TFGNNs
mrr: 0.0022
adjusted_mrr: 0.0022
mrr_dataset_count: 6
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 6
  total: 12
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id004
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
  - model: C (orthogonal)
    model_key: gcn
    model_plain: C (orthogonal)
    value: 0.9412
    std: 0.0008
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
    global_rank: 2
    sort_value: 0.9412
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
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
  - model: TFGNNs
    model_key: tfgnns
    model_plain: TFGNNs
    value: 0.73
    std: null
    paper_value: 0.73
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.73
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.73
    sort_std: null
    global_rank: 495
    paper_rank: 495
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGNNs + random initialization
    model_key: tfgnns + random initialization
    model_plain: TFGNNs + random initialization
    value: 0.158
    std: null
    paper_value: 0.158
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.158
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.158
    sort_std: null
    global_rank: 543
    paper_rank: 543
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNs + LaF
    model_key: gcns + laf
    model_plain: GCNs + LaF
    value: 0.061
    std: null
    paper_value: 0.061
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.061
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.061
    sort_std: null
    global_rank: 547
    paper_rank: 547
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs
    model_key: gats
    model_plain: GATs
    value: 0.058
    std: null
    paper_value: 0.058
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.058
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.058
    sort_std: null
    global_rank: 548
    paper_rank: 548
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs + LaF
    model_key: gats + laf
    model_plain: GATs + LaF
    value: 0.025
    std: null
    paper_value: 0.025
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.025
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.025
    sort_std: null
    global_rank: 549
    paper_rank: 549
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNs
    model_key: gcns
    model_plain: GCNs
    value: 0.023
    std: null
    paper_value: 0.023
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-computers (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.023
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.023
    sort_std: null
    global_rank: 550
    paper_rank: 550
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
  dataset: Amazon-Photo
  rows:
  - model: C (orthogonal)
    model_key: msh-gnn
    model_plain: C (orthogonal)
    value: 0.9766
    std: 0.005
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
    global_rank: 1
    sort_value: 0.9766
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: C (orthogonal)
    model_key: geomancer
    model_plain: C (orthogonal)
    value: 0.9705
    std: 0.0013
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9705
    sort_std: 0.0013
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: C (orthogonal)
    model_key: graphtarif
    model_plain: C (orthogonal)
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
    global_rank: 3
    sort_value: 0.9703
    sort_std: 0.0019
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TFGNNs
    model_key: tfgnns
    model_plain: TFGNNs
    value: 0.637
    std: null
    paper_value: 0.637
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting.
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.637
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.637
    sort_std: null
    global_rank: 531
    paper_rank: 531
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNs + LaF
    model_key: gcns + laf
    model_plain: GCNs + LaF
    value: 0.142
    std: null
    paper_value: 0.142
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting using
      Labels as Features (LaF).
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.142
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.142
    sort_std: null
    global_rank: 587
    paper_rank: 587
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs
    model_key: gats
    model_plain: GATs
    value: 0.122
    std: null
    paper_value: 0.122
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting.
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.122
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.122
    sort_std: null
    global_rank: 588
    paper_rank: 588
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNs
    model_key: gcns
    model_plain: GCNs
    value: 0.119
    std: null
    paper_value: 0.119
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting.
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.119
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.119
    sort_std: null
    global_rank: 589
    paper_rank: 589
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGNNs + random initialization
    model_key: tfgnns + random initialization
    model_plain: TFGNNs + random initialization
    value: 0.09
    std: null
    paper_value: 0.09
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
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting with
      random initialization.
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.09
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.09
    sort_std: null
    global_rank: 590
    paper_rank: 590
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs + LaF
    model_key: gats + laf
    model_plain: GATs + LaF
    value: 0.044
    std: null
    paper_value: 0.044
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to amazon-photo (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Transductive node classification in the training-free setting using
      Labels as Features (LaF).
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.044
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.044
    sort_std: null
    global_rank: 591
    paper_rank: 591
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
  dataset: CiteSeer
  rows:
  - model: SGC+TSC
    model_key: cna
    model_plain: SGC+TSC
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
  - model: SGC+TSC
    model_key: is-gib
    model_plain: SGC+TSC
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
    input_feature_source: null
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
  - model: SGC+TSC
    model_key: eerm
    model_plain: SGC+TSC
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
    input_feature_source: null
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
  - model: GCNs
    model_key: gcns
    model_plain: GCNs
    value: 0.167
    std: null
    paper_value: 0.167
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, rest for testing (Yang et al. 2016).'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.7122
    at_pub_std: 0.0047
    at_pub_source_arxiv: '2108.06280'
    at_pub_source_title: Understanding Structural Vulnerability in Graph Convolutional
      Networks
    at_pub_source_date_iso: '2021-08-01'
    at_pub_source_date_label: IJCAI 2021
    value_gap_source_date_iso: '2021-08-01'
    value_gap_source_date_label: IJCAI 2021
    gap_vs_at_pub: 0.5452
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7122
    true_std: 0.0047
    value_gap_source_arxiv: '2108.06280'
    value_gap_source_title: Understanding Structural Vulnerability in Graph Convolutional
      Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.5452
    has_value_note: false
    value_note: ''
    sort_value: 0.7122
    sort_std: 0.0047
    global_rank: 596
    paper_rank: 980
    rank_delta: 384
    rank_delta_abs: 384
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Understanding Structural Vulnerability in Graph Convolutional
      Networks
    comparison_source_arxiv: '2108.06280'
    is_best: false
    is_std_outlier: false
  - model: TFGNNs
    model_key: tfgnns
    model_plain: TFGNNs
    value: 0.362
    std: null
    paper_value: 0.362
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, rest for testing (Yang et al. 2016).'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.362
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.362
    sort_std: null
    global_rank: 960
    paper_rank: 960
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs
    model_key: gats
    model_plain: GATs
    value: 0.229
    std: null
    paper_value: 0.229
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, rest for testing (Yang et al. 2016).'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.229
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.229
    sort_std: null
    global_rank: 972
    paper_rank: 972
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGNNs + random initialization
    model_key: tfgnns + random initialization
    model_plain: TFGNNs + random initialization
    value: 0.177
    std: null
    paper_value: 0.177
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, rest for testing (Yang et al. 2016).'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.177
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.177
    sort_std: null
    global_rank: 979
    paper_rank: 979
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNs + LaF
    model_key: gcns + laf
    model_plain: GCNs + LaF
    value: 0.159
    std: null
    paper_value: 0.159
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, rest for testing (Yang et al. 2016).'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.159
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.159
    sort_std: null
    global_rank: 981
    paper_rank: 981
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs + LaF
    model_key: gats + laf
    model_plain: GATs + LaF
    value: 0.077
    std: null
    paper_value: 0.077
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, rest for testing (Yang et al. 2016).'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.077
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.077
    sort_std: null
    global_rank: 983
    paper_rank: 983
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
- &id006
  dataset: Coauthor-CS
  rows:
  - model: DGI (PPR)
    model_key: dog
    model_plain: DGI (PPR)
    value: 0.969
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
    arxiv_id: '2503.12563'
    title: 'Diffusion on Graph: Augmentation of Graph Structure for Node Classification'
    date: Mar 16, 2025
    date_display: Mar 2025
    date_iso: '2025-03-16'
    venue: Trans. Mach. Learn. Res.
    codebase_url: https://github.com/Statistical-Deep-Learning/DoG
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: synthetic graph structures added to the training set
    is_global_top: true
    global_rank: 1
    sort_value: 0.969
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DGI (PPR)
    model_key: gwn-fa
    model_plain: DGI (PPR)
    value: 0.9667
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9667
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: DGI (PPR)
    model_key: gwn-sym
    model_plain: DGI (PPR)
    value: 0.9666
    std: 0.0026
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.20034'
    title: Graph Wave Networks
    date: Apr 22, 2025
    date_display: Apr 2025
    date_iso: '2025-04-22'
    venue: The Web Conference
    codebase_url: https://github.com/YueAWu/Graph-Wave-Networks
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9666
    sort_std: 0.0026
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCNs
    model_key: gcns
    model_plain: GCNs
    value: 0.079
    std: null
    paper_value: 0.079
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: 0.928
    at_pub_std: 0.009
    at_pub_source_arxiv: '2007.09296'
    at_pub_source_title: Towards Deeper Graph Neural Networks
    at_pub_source_date_iso: '2020-07-06'
    at_pub_source_date_label: KDD 2020
    value_gap_source_date_iso: '2020-07-06'
    value_gap_source_date_label: KDD 2020
    gap_vs_at_pub: 0.8490000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.928
    true_std: 0.009
    value_gap_source_arxiv: '2007.09296'
    value_gap_source_title: Towards Deeper Graph Neural Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.8490000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.928
    sort_std: 0.009
    global_rank: 110
    paper_rank: 266
    rank_delta: 156
    rank_delta_abs: 156
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Towards Deeper Graph Neural Networks
    comparison_source_arxiv: '2007.09296'
    is_best: false
    is_std_outlier: false
  - model: TFGNNs
    model_key: tfgnns
    model_plain: TFGNNs
    value: 0.601
    std: null
    paper_value: 0.601
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.601
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.601
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
  - model: GCNs + LaF
    model_key: gcns + laf
    model_plain: GCNs + LaF
    value: 0.08
    std: null
    paper_value: 0.08
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.08
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.08
    sort_std: null
    global_rank: 266
    paper_rank: 266
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs + LaF
    model_key: gats + laf
    model_plain: GATs + LaF
    value: 0.076
    std: null
    paper_value: 0.076
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.076
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.076
    sort_std: null
    global_rank: 267
    paper_rank: 267
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs
    model_key: gats
    model_plain: GATs
    value: 0.04
    std: null
    paper_value: 0.04
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.04
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.04
    sort_std: null
    global_rank: 268
    paper_rank: 268
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGNNs + random initialization
    model_key: tfgnns + random initialization
    model_plain: TFGNNs + random initialization
    value: 0.023
    std: null
    paper_value: 0.023
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-cs (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.023
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.023
    sort_std: null
    global_rank: 269
    paper_rank: 269
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
- &id005
  dataset: Coauthor-Physics
  rows:
  - model: SelfGNN LDP
    model_key: geomancer
    model_plain: SelfGNN LDP
    value: 0.9878
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
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9878
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SelfGNN LDP
    model_key: lgd
    model_plain: SelfGNN LDP
    value: 0.9855
    std: 0.0012
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2510.04522'
    title: 'Toward a Unified Geometry Understanding: Riemannian Diffusion Framework
      for Graph Generation and Prediction'
    date: Oct 6, 2025
    date_display: Oct 2025
    date_iso: '2025-10-06'
    venue: Accepted by NeurIPS 2025
    codebase_url: https://github.com/RingBDStack/GeoMancer
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9855
    sort_std: 0.0012
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SelfGNN LDP
    model_key: msh-gnn
    model_plain: SelfGNN LDP
    value: 0.9837
    std: 0.0008
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
    global_rank: 3
    sort_value: 0.9837
    sort_std: 0.0008
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGNNs
    model_key: tfgnns
    model_plain: TFGNNs
    value: 0.717
    std: null
    paper_value: 0.717
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.717
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.717
    sort_std: null
    global_rank: 257
    paper_rank: 257
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGNNs + random initialization
    model_key: tfgnns + random initialization
    model_plain: TFGNNs + random initialization
    value: 0.166
    std: null
    paper_value: 0.166
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.166
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.166
    sort_std: null
    global_rank: 270
    paper_rank: 270
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs
    model_key: gats
    model_plain: GATs
    value: 0.163
    std: null
    paper_value: 0.163
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.163
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.163
    sort_std: null
    global_rank: 271
    paper_rank: 271
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNs + LaF
    model_key: gcns + laf
    model_plain: GCNs + LaF
    value: 0.146
    std: null
    paper_value: 0.146
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.146
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.146
    sort_std: null
    global_rank: 272
    paper_rank: 272
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNs
    model_key: gcns
    model_plain: GCNs
    value: 0.101
    std: null
    paper_value: 0.101
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.101
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.101
    sort_std: null
    global_rank: 273
    paper_rank: 273
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs + LaF
    model_key: gats + laf
    model_plain: GATs + LaF
    value: 0.079
    std: null
    paper_value: 0.079
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
    variant_inference_reason: 'dataset: fuzzy match to coauthor-physics (score=100)'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: transductive node classification in the training-free setting
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.079
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.079
    sort_std: null
    global_rank: 274
    paper_rank: 274
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
  dataset: PubMed
  rows:
  - model: R-SoftGraphAIN
    model_key: lgtl
    model_plain: R-SoftGraphAIN
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
  - model: R-SoftGraphAIN
    model_key: sagn
    model_plain: R-SoftGraphAIN
    value: 0.9517
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
    arxiv_id: '2605.24867'
    title: 'Clustering as Reasoning: A $k$-Means Interpretation of Chain-of-Thought
      Graph Learning'
    date: May 24, 2026
    date_display: May 2026
    date_iso: '2026-05-24'
    venue: Accepted by ICML 2026
    codebase_url: https://github.com/Uncnbb/KCoT
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9517
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: R-SoftGraphAIN
    model_key: mixhop (lo)
    model_plain: R-SoftGraphAIN
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
    global_rank: 3
    sort_value: 0.9513
    sort_std: 0.0038
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TFGNNs
    model_key: tfgnns
    model_plain: TFGNNs
    value: 0.413
    std: null
    paper_value: 0.413
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, and the rest for testing.'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.413
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.413
    sort_std: null
    global_rank: 920
    paper_rank: 920
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNs + LaF
    model_key: gcns + laf
    model_plain: GCNs + LaF
    value: 0.407
    std: null
    paper_value: 0.407
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, and the rest for testing.'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.407
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.407
    sort_std: null
    global_rank: 925
    paper_rank: 925
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TFGNNs + random initialization
    model_key: tfgnns + random initialization
    model_plain: TFGNNs + random initialization
    value: 0.18
    std: null
    paper_value: 0.18
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, and the rest for testing.'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.18
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.18
    sort_std: null
    global_rank: 936
    paper_rank: 936
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNs
    model_key: gcns
    model_plain: GCNs
    value: 0.18
    std: null
    paper_value: 0.18
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, and the rest for testing.'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.18
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.18
    sort_std: null
    global_rank: 933
    paper_rank: 933
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs
    model_key: gats
    model_plain: GATs
    value: 0.18
    std: null
    paper_value: 0.18
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
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, and the rest for testing.'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.18
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.18
    sort_std: null
    global_rank: 934
    paper_rank: 934
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GATs + LaF
    model_key: gats + laf
    model_plain: GATs + LaF
    value: 0.18
    std: null
    paper_value: 0.18
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
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: 'Planetoid split: 20 nodes per class for training, 500 nodes for
      validation, and the rest for testing.'
    date: Apr 30, 2024
    date_display: Apr 2024
    date_iso: '2024-04-30'
    published_venue: TMLR 2024
    published_conference: TMLR 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-04-30'
    value_gap_source_date_label: TMLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.18
    true_std: null
    value_gap_source_arxiv: '2404.19288'
    value_gap_source_title: Training-free Graph Neural Networks and the Power of Labels
      as Features
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.18
    sort_std: null
    global_rank: 935
    paper_rank: 935
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
  - *id003
  - *id004
  - *id005
  - *id006
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: CiteSeer
      dataset_slug: citeseer
    - dataset: PubMed
      dataset_slug: pubmed
    - dataset: Amazon-Photo
      dataset_slug: amazon-photo
    - dataset: Amazon-Computers
      dataset_slug: amazon-computers
    - dataset: Coauthor-Physics
      dataset_slug: coauthor-physics
    - dataset: Coauthor-CS
      dataset_slug: coauthor-cs
main_figure: /figures/2404.19288/main_figure.jpegoptim.jpg
---

