---
title: GNN Explanations that do not Explain and How to find Them
arxiv_id: '2601.20815'
source_url: ''
authors:
- name: Steve Azzolin
  orcid: null
  s2_author_id: '2165224662'
  s2_url: null
- name: Stefano Teso
  orcid: null
  s2_author_id: '2580338'
  s2_url: null
- name: Bruno Lepri
  orcid: null
  s2_author_id: '2291065942'
  s2_url: null
- name: Andrea Passerini
  orcid: null
  s2_author_id: '2259941595'
  s2_url: null
- name: Sagar Malhotra
  orcid: null
  s2_author_id: '2305683691'
  s2_url: null
published_date: Jan 28, 2026
published_date_iso: '2026-01-28'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Explanations provided by Self-explainable Graph Neural Networks (SE-GNNs)
  are fundamental for understanding the model''s inner workings and for identifying
  potential misuse of sensitive attributes. Although recent works have highlighted
  that these explanations can be suboptimal and potentially misleading, a characterization
  of their failure cases is unavailable. In this work, we identify a critical failure
  of SE-GNN explanations: explanations can be unambiguously unrelated to how the SE-GNNs
  infer labels. We show that, on the one hand, many SE-GNNs can achieve optimal true
  risk while producing these degenerate explanations, and on the other, most faithfulness
  metrics can fail to identify these failure modes. Our empirical analysis reveals
  that degenerate explanations can be maliciously planted (allowing an attacker to
  hide the use of sensitive attributes) and can also emerge naturally, highlighting
  the need for reliable auditing. To address this, we introduce a novel faithfulness
  metric that reliably marks degenerate explanations as unfaithful, in both malicious
  and natural settings.'
codebase_url: https://github.com/steveazzolin/gnn_deg_expl
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- TU Dortmund
- GNNBenchmark
benchmark_coverage:
- benchmark: TU Dortmund
  benchmark_slug: tu-dortmund
  evaluated: 1
  total: 11
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 1
  total: 6
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id002
  dataset: MNIST
  rows:
  - model: Tango_GPS
    model_key: schrödinger gnn
    model_plain: Tango_GPS
    value: 0.9913
    std: 0.0004
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9913
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: cnn
    model_plain: Tango_GPS
    value: 0.9907
    std: 0.0007
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.9907
    sort_std: 0.0007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Tango_GPS
    model_key: mpnn
    model_plain: Tango_GPS
    value: 0.9895
    std: 0.0006
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.13383'
    title: 'Beyond Oversquashing: Understanding Signal Propagation in GNNs Via Observables'
    date: May 13, 2026
    date_display: May 2026
    date_iso: '2026-05-13'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9895
    sort_std: 0.0006
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSAT
    model_key: gsat
    model_plain: GSAT
    value: 0.947
    std: 0.004
    paper_value: 0.947
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for well-performing models.
    date: Jan 28, 2026
    date_display: Jan 2026
    date_iso: '2026-01-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.947
    true_std: 0.004
    value_gap_source_arxiv: '2601.20815'
    value_gap_source_title: GNN Explanations that do not Explain and How to find Them
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.947
    sort_std: 0.004
    global_rank: 125
    paper_rank: 125
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SMGNN
    model_key: smgnn
    model_plain: SMGNN
    value: 0.868
    std: 0.08
    paper_value: 0.868
    paper_std: 0.08
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for well-performing models.
    date: Jan 28, 2026
    date_display: Jan 2026
    date_iso: '2026-01-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-01-28'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.868
    true_std: 0.08
    value_gap_source_arxiv: '2601.20815'
    value_gap_source_title: GNN Explanations that do not Explain and How to find Them
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.868
    sort_std: 0.08
    global_rank: 140
    paper_rank: 140
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: true
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
  dataset: MUTAG
  rows:
  - model: ECC
    model_key: msh-gnn
    model_plain: ECC
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
    input_feature_source: null
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
  - model: ECC
    model_key: supcosine
    model_plain: ECC
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
    global_rank: 2
    sort_value: 0.983
    sort_std: 0.025
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: ECC
    model_key: cauemo
    model_plain: ECC
    value: 0.9692
    std: 0.0136
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2505.06283'
    title: 'Soft causal learning for generalized molecule property prediction: An
      environment modeling perspective'
    date: May 7, 2025
    date_display: May 2025
    date_iso: '2025-05-07'
    venue: Knowledge and Information Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.9692
    sort_std: 0.0136
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GSAT
    model_key: gsat
    model_plain: GSAT
    value: 0.806
    std: 0.03
    paper_value: 0.806
    paper_std: 0.03
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for well-performing models.
    date: Jan 28, 2026
    date_display: Jan 2026
    date_iso: '2026-01-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.9637
    at_pub_std: 0.0215
    at_pub_source_arxiv: '2505.06283'
    at_pub_source_title: 'Soft causal learning for generalized molecule property prediction:
      An environment modeling perspective'
    at_pub_source_date_iso: '2025-05-07'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-05-07'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.15769999999999995
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.9637
    true_std: 0.0215
    value_gap_source_arxiv: '2505.06283'
    value_gap_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.15769999999999995
    has_value_note: false
    value_note: ''
    sort_value: 0.9637
    sort_std: 0.0215
    global_rank: 6
    paper_rank: 604
    rank_delta: 598
    rank_delta_abs: 598
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Soft causal learning for generalized molecule property
      prediction: An environment modeling perspective'
    comparison_source_arxiv: '2505.06283'
    is_best: false
    is_std_outlier: false
  - model: SMGNN
    model_key: smgnn
    model_plain: SMGNN
    value: 0.779
    std: 0.024
    paper_value: 0.779
    paper_std: 0.024
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test accuracy reported for well-performing models.
    date: Jan 28, 2026
    date_display: Jan 2026
    date_iso: '2026-01-28'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.79
    at_pub_std: 0.02
    at_pub_source_arxiv: '2502.02719'
    at_pub_source_title: 'Beyond Topological Self-Explainable GNNs: A Formal Explainability
      Perspective'
    at_pub_source_date_iso: '2025-02-04'
    at_pub_source_date_label: ICML 2025
    value_gap_source_date_iso: '2025-02-04'
    value_gap_source_date_label: ICML 2025
    gap_vs_at_pub: 0.01100000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.79
    true_std: 0.02
    value_gap_source_arxiv: '2502.02719'
    value_gap_source_title: 'Beyond Topological Self-Explainable GNNs: A Formal Explainability
      Perspective'
    value_gap_source_is_current_paper: false
    value_gap: 0.01100000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.79
    sort_std: 0.02
    global_rank: 656
    paper_rank: 673
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
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
- benchmark: GNNBenchmark
  datasets:
  - *id002
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: TU Dortmund
    benchmark_slug: tu-dortmund
    datasets:
    - dataset: MUTAG
      dataset_slug: mutag
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: MNIST
      dataset_slug: mnist
main_figure: /figures/2601.20815/main_figure.jpegoptim.jpg
---

