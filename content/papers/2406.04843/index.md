---
title: Variational Flow Matching for Graph Generation
arxiv_id: '2406.04843'
source_url: ''
authors:
- name: Floor Eijkelboom
  orcid: null
  s2_author_id: '2208907804'
  s2_url: null
- name: G. Bartosh
  orcid: null
  s2_author_id: '2205312481'
  s2_url: null
- name: C. A. Naesseth
  orcid: null
  s2_author_id: '2328322'
  s2_url: null
- name: Max Welling
  orcid: null
  s2_author_id: '2293173625'
  s2_url: null
- name: Jan-Willem van de Meent
  orcid: null
  s2_author_id: '2086966519'
  s2_url: null
published_date: Jun 7, 2024
published_date_iso: '2024-06-07'
published_venue: NeurIPS 2024
published_conference: NeurIPS 2024
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: We present a formulation of flow matching as variational inference, which
  we refer to as variational flow matching (VFM). Based on this formulation we develop
  CatFlow, a flow matching method for categorical data. CatFlow is easy to implement,
  computationally efficient, and achieves strong results on graph generation tasks.
  The key observation in VFM is that we can parameterize the vector field of the flow
  in terms of a variational approximation of the posterior probability path, which
  is the distribution over possible end points of a trajectory. We show that this
  variational interpretation admits both the CatFlow objective and the original flow
  matching objective as special cases. We also relate VFM to score-based models, in
  which the dynamics are stochastic rather than deterministic, and derive a bound
  on the model likelihood based on a reweighted VFM objective. We evaluate CatFlow
  on one abstract graph generation task and two molecular generation tasks. In all
  cases, CatFlow exceeds or matches performance of the current state-of-the-art.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- CatFlow
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
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
  dataset: ENZYMES
  is_multi_metric: true
  rows:
  - model: CatFlow
    model_key: catflow
    model_plain: CatFlow
    metric_values:
    - null
    - 0.013
    - 0.062
    - 0.008
    metric_stds:
    - null
    - 0.012
    - 0.011
    - 0.007
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.013
    sort_std: 0.012
    true_value: 0.013
    true_std: 0.012
    paper_value: 0.013
    paper_std: 0.012
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2406.04843'
    value_gap_source_title: Variational Flow Matching for Graph Generation
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-06-07'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2024
    date: Jun 7, 2024
    date_display: Jun 2024
    date_iso: '2024-06-07'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
    global_rank: 1
  metrics:
  - Accuracy
  - Degree
  - Clustering
  - Orbit
  primary_metric: Accuracy
  rank_metric: Degree
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Degree
  - Clustering
  - Orbit
  metric: Degree
  uses_non_primary_metric: true
  paper_has_primary_metric: false
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
    - dataset: ENZYMES
      dataset_slug: enzymes
single_proposed_model: CatFlow
---

