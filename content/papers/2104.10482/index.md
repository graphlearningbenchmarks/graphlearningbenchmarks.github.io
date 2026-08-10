---
title: 'GraphSVX: Shapley Value Explanations for Graph Neural Networks'
arxiv_id: '2104.10482'
source_url: ''
authors:
- name: Alexandre Duval
  orcid: null
  s2_author_id: '2256990809'
  s2_url: null
- name: Fragkiskos D. Malliaros
  orcid: null
  s2_author_id: '2817467'
  s2_url: null
published_date: Apr 18, 2021
published_date_iso: '2021-04-18'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Neural Networks (GNNs) achieve significant performance for various
  learning tasks on geometric data due to the incorporation of graph structure into
  the learning of node representations, which renders their comprehension challenging.
  In this paper, we first propose a unified framework satisfied by most existing GNN
  explainers. Then, we introduce GraphSVX, a post hoc local model-agnostic explanation
  method specifically designed for GNNs. GraphSVX is a decomposition technique that
  captures the ``fair'' contribution of each feature and node towards the explained
  prediction by constructing a surrogate model on a perturbed dataset. It extends
  to graphs and ultimately provides as explanation the Shapley Values from game theory.
  Experiments on real-world and synthetic datasets demonstrate that GraphSVX achieves
  state-of-the-art performance compared to baseline models while presenting core theoretical
  and human-centric properties.
codebase_url: https://github.com/AlexDuvalinho/GraphSVX
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GraphSVX
mrr: 0.0013
adjusted_mrr: 0.0004
mrr_dataset_count: 1
benchmark_categories:
- TU Dortmund
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: MUTAG
  rows:
  - model: MSH-GNN
    model_key: msh-gnn
    model_plain: MSH-GNN
    value: 0.991
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
    arxiv_id: '2505.15015'
    title: Multi-Scale Harmonic Encoding for Feature-Wise Graph Message Passing
    date: May 21, 2025
    date_display: May 2025
    date_iso: '2025-05-21'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.991
    sort_std: 0.003
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ID-GNN+BEC
    model_key: id-gnn+bec
    model_plain: ID-GNN+BEC
    value: 0.983
    std: 0.036
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2503.01079'
    title: Depth-Adaptive Graph Neural Networks via Learnable Bakry-Émery Curvature
    date: Mar 3, 2025
    date_display: Mar 2025
    date_iso: '2025-03-03'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.036
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SupCosine
    model_key: supcosine
    model_plain: SupCosine
    value: 0.983
    std: 0.025
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2203.07691'
    title: Supervised Contrastive Learning with Structure Inference for Graph Classification
    date: Mar 15, 2022
    date_display: Mar 2022
    date_iso: '2022-03-15'
    venue: IEEE Transactions on Network Science and Engineering
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.933
    std: 0.029
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2112.00911'
    title: 'ProtGNN: Towards Self-Explaining Graph Neural Networks'
    date: Dec 2, 2021
    date_display: Dec 2021
    date_iso: '2021-12-02'
    venue: AAAI Conference on Artificial Intelligence
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 43
    sort_value: 0.933
    sort_std: 0.029
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNNExplainer
    model_key: gnnexplainer
    model_plain: GNNExplainer
    value: 0.65
    std: null
    paper_value: 0.65
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluation of explanation accuracy on the MUTAG graph classification
      dataset.
    date: Apr 18, 2021
    date_display: Apr 2021
    date_iso: '2021-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.809
    at_pub_std: null
    at_pub_source_arxiv: '2104.06643'
    at_pub_source_title: Generative Causal Explanations for Graph Neural Networks
    at_pub_source_date_iso: '2021-04-14'
    at_pub_source_date_label: ICML 2021
    value_gap_source_date_iso: '2023-01-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: 0.15900000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.88
    true_std: 0.03
    value_gap_source_arxiv: '2301.01642'
    value_gap_source_title: 'CI-GNN: A Granger Causality-Inspired Graph Neural Network
      for Interpretable Brain Network-Based Psychiatric Diagnosis'
    value_gap_source_is_current_paper: false
    value_gap: 0.22999999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.88
    sort_std: 0.03
    global_rank: 351
    paper_rank: 857
    rank_delta: 506
    rank_delta_abs: 506
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Generative Causal Explanations for Graph Neural Networks
    comparison_source_arxiv: '2104.06643'
    is_best: false
    is_std_outlier: false
  - model: PGExplainer
    model_key: pgexplainer
    model_plain: PGExplainer
    value: 0.79
    std: null
    paper_value: 0.79
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluation of explanation accuracy on the MUTAG graph classification
      dataset.
    date: Apr 18, 2021
    date_display: Apr 2021
    date_iso: '2021-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-01-04'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.87
    true_std: 0.03
    value_gap_source_arxiv: '2301.01642'
    value_gap_source_title: 'CI-GNN: A Granger Causality-Inspired Graph Neural Network
      for Interpretable Brain Network-Based Psychiatric Diagnosis'
    value_gap_source_is_current_paper: false
    value_gap: 0.07999999999999996
    has_value_note: false
    value_note: ''
    sort_value: 0.87
    sort_std: 0.03
    global_rank: 417
    paper_rank: 714
    rank_delta: 297
    rank_delta_abs: 297
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
    value: 0.866
    std: 0.0495
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2106.04319'
    title: Breaking the Limits of Message Passing Graph Neural Networks
    date: Jun 8, 2021
    date_display: Jun 2021
    date_iso: '2021-06-08'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/balcilar/gnn-matlang
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 430
    sort_value: 0.866
    sort_std: 0.0495
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphSVX
    model_key: graphsvx
    model_plain: GraphSVX
    value: 0.77
    std: null
    paper_value: 0.77
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluation of explanation accuracy on the MUTAG graph classification
      dataset.
    date: Apr 18, 2021
    date_display: Apr 2021
    date_iso: '2021-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-18'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.77
    true_std: null
    value_gap_source_arxiv: '2104.10482'
    value_gap_source_title: 'GraphSVX: Shapley Value Explanations for Graph Neural
      Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.77
    sort_std: null
    global_rank: 754
    paper_rank: 754
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PGM-Explainer
    model_key: pgm-explainer
    model_plain: PGM-Explainer
    value: 0.72
    std: null
    paper_value: 0.72
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Evaluation of explanation accuracy on the MUTAG graph classification
      dataset.
    date: Apr 18, 2021
    date_display: Apr 2021
    date_iso: '2021-04-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-04-18'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.72
    true_std: null
    value_gap_source_arxiv: '2104.10482'
    value_gap_source_title: 'GraphSVX: Shapley Value Explanations for Graph Neural
      Networks'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.72
    sort_std: null
    global_rank: 825
    paper_rank: 825
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
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
single_proposed_model: GraphSVX
main_figure: /figures/2104.10482/main_figure.jpegoptim.jpg
---

