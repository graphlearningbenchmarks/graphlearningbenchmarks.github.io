---
title: Convexified Message-Passing Graph Neural Networks
arxiv_id: '2505.18289'
source_url: ''
authors:
- name: Saar Cohen
  orcid: null
  s2_author_id: '38511273'
  s2_url: null
- name: Noa Agmon
  orcid: null
  s2_author_id: '2273996768'
  s2_url: null
- name: Uri Shaham
  orcid: null
  s2_author_id: '2315333921'
  s2_url: null
published_date: May 23, 2025
published_date_iso: '2025-05-23'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Graph Neural Networks (GNNs) are key tools for graph representation learning,
  demonstrating strong results across diverse prediction tasks. In this paper, we
  present Convexified Message-Passing Graph Neural Networks (CGNNs), a novel and general
  framework that combines the power of message-passing GNNs with the tractability
  of convex optimization. By mapping their nonlinear filters into a reproducing kernel
  Hilbert space, CGNNs transform training into a convex optimization problem, which
  projected gradient methods can solve both efficiently and optimally. Convexity further
  allows CGNNs'statistical properties to be analyzed accurately and rigorously. For
  two-layer CGNNs, we establish rigorous generalization guarantees, showing convergence
  to the performance of an optimal GNN. To scale to deeper architectures, we adopt
  a principled layer-wise training strategy. Experiments on benchmark datasets show
  that CGNNs significantly exceed the performance of leading GNN models, obtaining
  10-40% higher accuracy in most cases, underscoring their promise as a powerful and
  principled method with strong theoretical foundations. In rare cases where improvements
  are not quantitatively substantial, the convex models either slightly exceed or
  match the baselines, stressing their robustness and wide applicability. Though over-parameterization
  is often used to enhance performance in non-convex models, we show that our CGNNs
  yield shallow convex models that can surpass non-convex ones in accuracy and model
  compactness.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MPNNs
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ogbg-molhiv
  rows:
  - model: MPNNs
    model_key: mpnns
    model_plain: MPNNs
    value: 0.98
    std: null
    paper_value: 0.98
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
    table_ref: Results and Analysis section
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: The text reports accuracy for the ogbg-molhiv dataset. Although
      the prompt asks for ROC-AUC, the provided text only contains accuracy values
      for this specific dataset.
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-23'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.98
    true_std: null
    value_gap_source_arxiv: '2505.18289'
    value_gap_source_title: Convexified Message-Passing Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.98
    sort_std: null
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
  - model: non-convex counterparts
    model_key: non-convex counterparts
    model_plain: non-convex counterparts
    value: 0.96
    std: null
    paper_value: 0.96
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Results and Analysis section
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: The text reports accuracy for the ogbg-molhiv dataset. Although
      the prompt asks for ROC-AUC, the provided text only contains accuracy values
      for this specific dataset.
    date: May 23, 2025
    date_display: May 2025
    date_iso: '2025-05-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-23'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.96
    true_std: null
    value_gap_source_arxiv: '2505.18289'
    value_gap_source_title: Convexified Message-Passing Graph Neural Networks
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.96
    sort_std: null
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: non-convex counterparts
    model_key: structposgssl-fa
    model_plain: non-convex counterparts
    value: 0.79
    std: 0.0243
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2502.16233'
    title: Graph Self-Supervised Learning with Learnable Structural and Positional
      Encodings
    date: Feb 22, 2025
    date_display: Feb 2025
    date_iso: '2025-02-22'
    venue: The Web Conference
    codebase_url: https://github.com/wokas36/StructPosGSSL
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.79
    sort_std: 0.0243
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: ROC-AUC
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: OGB
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: OGB
    benchmark_slug: ogb
    datasets:
    - dataset: ogbg-molhiv
      dataset_slug: ogbg-molhiv
single_proposed_model: MPNNs
---

