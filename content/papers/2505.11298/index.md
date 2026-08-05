---
title: 'Graph Representational Learning: When Does More Expressivity Hurt Generalization?'
arxiv_id: '2505.11298'
source_url: ''
authors:
- name: Sohir Maskey
  orcid: null
  s2_author_id: '2127602704'
  s2_url: null
- name: Raffaele Paolino
  orcid: null
  s2_author_id: '2187930583'
  s2_url: null
- name: Fabian Jogl
  orcid: null
  s2_author_id: '2091417275'
  s2_url: null
- name: Gitta Kutyniok
  orcid: null
  s2_author_id: '3125779'
  s2_url: null
- name: J. Lutzeyer
  orcid: null
  s2_author_id: '89948093'
  s2_url: null
published_date: May 16, 2025
published_date_iso: '2025-05-16'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Neural Networks (GNNs) are powerful tools for learning on structured
  data, yet the relationship between their expressivity and predictive performance
  remains unclear. We introduce a family of pseudometrics that capture different degrees
  of structural similarity between graphs and relate these similarities to generalization,
  and consequently, the performance of expressive GNNs. By considering a setting where
  graph labels are correlated with structural features, we derive generalization bounds
  that depend on the distance between training and test graphs, model complexity,
  and training set size. These bounds reveal that more expressive GNNs may generalize
  worse unless their increased complexity is balanced by a sufficiently large training
  set or reduced distance between training and test graphs. Our findings relate expressivity
  and generalization, offering theoretical insights supported by empirical results.
  Our code is available on GitHub.
codebase_url: https://github.com/RPaolino/GenVsExp
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- GraphBench
benchmark_coverage:
- benchmark: GraphBench
  benchmark_slug: graphbench
  evaluated: 3
  total: 8
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: BA graph
  rows:
  - model: F4-MPNN
    model_key: f4-mpnn
    model_plain: F4-MPNN
    value: 0.9793
    std: 0.0068
    paper_value: 0.9793
    paper_std: 0.0068
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
    protocol_note: Test accuracy on synthetic BA graphs using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9793
    true_std: 0.0068
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9793
    sort_std: 0.0068
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: F7-MPNN
    model_key: f7-mpnn
    model_plain: F7-MPNN
    value: 0.966
    std: 0.0065
    paper_value: 0.966
    paper_std: 0.0065
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
    protocol_note: Test accuracy on synthetic BA graphs using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.966
    true_std: 0.0065
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: 0.0065
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: F3-MPNN
    model_key: f3-mpnn
    model_plain: F3-MPNN
    value: 0.8657
    std: 0.0085
    paper_value: 0.8657
    paper_std: 0.0085
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
    protocol_note: Test accuracy on synthetic BA graphs using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8657
    true_std: 0.0085
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8657
    sort_std: 0.0085
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Sub-G
    model_key: sub-g
    model_plain: Sub-G
    value: 0.8623
    std: 0.0058
    paper_value: 0.8623
    paper_std: 0.0058
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
    protocol_note: Test accuracy on synthetic BA graphs using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8623
    true_std: 0.0058
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8623
    sort_std: 0.0058
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: L-G
    model_key: l-g
    model_plain: L-G
    value: 0.8543
    std: 0.0063
    paper_value: 0.8543
    paper_std: 0.0063
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
    protocol_note: Test accuracy on synthetic BA graphs using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8543
    true_std: 0.0063
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8543
    sort_std: 0.0063
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    value: 0.849
    std: 0.0045
    paper_value: 0.849
    paper_std: 0.0045
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
    protocol_note: Test accuracy on synthetic BA graphs using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.849
    true_std: 0.0045
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.849
    sort_std: 0.0045
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
  - model: LF-G
    model_key: lf-g
    model_plain: LF-G
    value: 0.845
    std: 0.0135
    paper_value: 0.845
    paper_std: 0.0135
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
    protocol_note: Test accuracy on synthetic BA graphs using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.845
    true_std: 0.0135
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.845
    sort_std: 0.0135
    global_rank: 7
    paper_rank: 7
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
  dataset: ER graph
  rows:
  - model: F_4-MPNN
    model_key: f_4-mpnn
    model_plain: F_4-MPNN
    value: 0.9793
    std: 0.0068
    paper_value: 0.9793
    paper_std: 0.0068
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
    protocol_note: 10-fold cross-validation on Erdős–Rényi graphs for Task 1 (Median-Based
      Labeling with Cycle Counts).
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9793
    true_std: 0.0068
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9793
    sort_std: 0.0068
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: F_7-MPNN
    model_key: f_7-mpnn
    model_plain: F_7-MPNN
    value: 0.966
    std: 0.0065
    paper_value: 0.966
    paper_std: 0.0065
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
    protocol_note: 10-fold cross-validation on Erdős–Rényi graphs for Task 1 (Median-Based
      Labeling with Cycle Counts).
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.966
    true_std: 0.0065
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: 0.0065
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GraphWiz-DPO (LLaMA 2-7B)
    model_key: graphwiz (llama 2-13b)
    model_plain: GraphWiz-DPO (LLaMA 2-7B)
    value: 0.9475
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: llm
    architecture_label: LLM
    architecture_title: LLM applied to graphs
    arxiv_id: '2402.16029'
    title: 'GraphWiz: An Instruction-Following Language Model for Graph Computational
      Problems'
    date: Feb 25, 2024
    date_display: Feb 2024
    date_iso: '2024-02-25'
    venue: null
    codebase_url: https://github.com/nuochenpku/Graph-Reasoning-LLM
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9475
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: F_3-MPNN
    model_key: f_3-mpnn
    model_plain: F_3-MPNN
    value: 0.8657
    std: 0.0085
    paper_value: 0.8657
    paper_std: 0.0085
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
    protocol_note: 10-fold cross-validation on Erdős–Rényi graphs for Task 1 (Median-Based
      Labeling with Cycle Counts).
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8657
    true_std: 0.0085
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8657
    sort_std: 0.0085
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Sub-G
    model_key: sub-g
    model_plain: Sub-G
    value: 0.8623
    std: 0.0058
    paper_value: 0.8623
    paper_std: 0.0058
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
    protocol_note: 10-fold cross-validation on Erdős–Rényi graphs for Task 1 (Median-Based
      Labeling with Cycle Counts).
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8623
    true_std: 0.0058
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8623
    sort_std: 0.0058
    global_rank: 8
    paper_rank: 8
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: L-G
    model_key: l-g
    model_plain: L-G
    value: 0.8543
    std: 0.0063
    paper_value: 0.8543
    paper_std: 0.0063
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
    protocol_note: 10-fold cross-validation on Erdős–Rényi graphs for Task 1 (Median-Based
      Labeling with Cycle Counts).
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8543
    true_std: 0.0063
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8543
    sort_std: 0.0063
    global_rank: 9
    paper_rank: 9
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    value: 0.849
    std: 0.0045
    paper_value: 0.849
    paper_std: 0.0045
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
    protocol_note: 10-fold cross-validation on Erdős–Rényi graphs for Task 1 (Median-Based
      Labeling with Cycle Counts).
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.849
    true_std: 0.0045
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.849
    sort_std: 0.0045
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
  - model: LF-G
    model_key: lf-g
    model_plain: LF-G
    value: 0.845
    std: 0.0135
    paper_value: 0.845
    paper_std: 0.0135
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
    protocol_note: 10-fold cross-validation on Erdős–Rényi graphs for Task 1 (Median-Based
      Labeling with Cycle Counts).
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.845
    true_std: 0.0135
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.845
    sort_std: 0.0135
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
  dataset: RB graph
  rows:
  - model: F_4-MPNN
    model_key: f_4-mpnn
    model_plain: F_4-MPNN
    value: 0.9793
    std: 0.0068
    paper_value: 0.9793
    paper_std: 0.0068
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
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=82)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Erdős–Rényi graphs for Task 1 using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9793
    true_std: 0.0068
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9793
    sort_std: 0.0068
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: F_7-MPNN
    model_key: f_7-mpnn
    model_plain: F_7-MPNN
    value: 0.966
    std: 0.0065
    paper_value: 0.966
    paper_std: 0.0065
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
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=82)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Erdős–Rényi graphs for Task 1 using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.966
    true_std: 0.0065
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.966
    sort_std: 0.0065
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: F_3-MPNN
    model_key: f_3-mpnn
    model_plain: F_3-MPNN
    value: 0.8657
    std: 0.0085
    paper_value: 0.8657
    paper_std: 0.0085
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
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=82)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Erdős–Rényi graphs for Task 1 using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8657
    true_std: 0.0085
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8657
    sort_std: 0.0085
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Sub-G
    model_key: sub-g
    model_plain: Sub-G
    value: 0.8623
    std: 0.0058
    paper_value: 0.8623
    paper_std: 0.0058
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
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=82)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Erdős–Rényi graphs for Task 1 using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8623
    true_std: 0.0058
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8623
    sort_std: 0.0058
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: L-G
    model_key: l-g
    model_plain: L-G
    value: 0.8543
    std: 0.0063
    paper_value: 0.8543
    paper_std: 0.0063
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
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=82)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Erdős–Rényi graphs for Task 1 using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.8543
    true_std: 0.0063
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.8543
    sort_std: 0.0063
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    value: 0.849
    std: 0.0045
    paper_value: 0.849
    paper_std: 0.0045
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
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=82)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Erdős–Rényi graphs for Task 1 using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.849
    true_std: 0.0045
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.849
    sort_std: 0.0045
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
  - model: LF-G
    model_key: lf-g
    model_plain: LF-G
    value: 0.845
    std: 0.0135
    paper_value: 0.845
    paper_std: 0.0135
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
    variant_inference_reason: 'dataset: fuzzy match to rb graph (score=82)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy on Erdős–Rényi graphs for Task 1 using 10-fold cross-validation.
    date: May 16, 2025
    date_display: May 2025
    date_iso: '2025-05-16'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-16'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.845
    true_std: 0.0135
    value_gap_source_arxiv: '2505.11298'
    value_gap_source_title: 'Graph Representational Learning: When Does More Expressivity
      Hurt Generalization?'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.845
    sort_std: 0.0135
    global_rank: 7
    paper_rank: 7
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
- benchmark: GraphBench
  datasets:
  - *id001
  - *id002
  - *id003
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: GraphBench
    benchmark_slug: graphbench
    datasets:
    - dataset: ER graph
      dataset_slug: er-graph
    - dataset: BA graph
      dataset_slug: ba-graph
    - dataset: RB graph
      dataset_slug: rb-graph
main_figure: /figures/2505.11298/main_figure.jpegoptim.jpg
---

