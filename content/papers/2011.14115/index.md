---
title: Fast and Uncertainty-Aware Directional Message Passing for Non-Equilibrium
  Molecules
arxiv_id: '2011.14115'
source_url: ''
authors:
- name: Johannes Klicpera
  orcid: null
  s2_author_id: '51516539'
  s2_url: null
- name: S. Giri
  orcid: null
  s2_author_id: '48972811'
  s2_url: null
- name: Johannes T. Margraf
  orcid: null
  s2_author_id: '39203264'
  s2_url: null
- name: Stephan Gunnemann
  orcid: null
  s2_author_id: '51249380'
  s2_url: null
published_date: Nov 28, 2020
published_date_iso: '2020-11-28'
published_venue: NeurIPS 2020
published_conference: NeurIPS 2020
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Many important tasks in chemistry revolve around molecules during reactions.
  This requires predictions far from the equilibrium, while most recent work in machine
  learning for molecules has been focused on equilibrium or near-equilibrium states.
  In this paper we aim to extend this scope in three ways. First, we propose the DimeNet$^++$
  model, which is 8x faster and more accurate than the original DimeNet on the QM9
  benchmark of equilibrium molecules. Second, we validate DimeNet$^++$ on highly reactive
  molecules by developing the challenging COLL dataset, which contains distorted configurations
  of small molecules during collisions. Finally, we investigate ensembling and mean-variance
  estimation for uncertainty quantification with the goal of accelerating the exploration
  of the vast space of non-equilibrium structures. Our DimeNet$^++$ implementation
  as well as the COLL dataset are available online.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DimeNet++
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Quantum Chemistry
benchmark_coverage:
- benchmark: Quantum Chemistry
  benchmark_slug: quantum-chemistry
  evaluated: 1
  total: 3
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: QM9
  is_multi_metric: true
  rows:
  - model: Graphormer-SPIS
    model_key: equiformer v2
    model_plain: Graphormer-SPIS
    metric_values:
    - 0.01
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.23086'
    title: Equivariant Spherical Transformer for Efficient Molecular Modeling
    published_venue: ''
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.01
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: eqgat
    model_plain: Graphormer-SPIS
    metric_values:
    - 0.011
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.23086'
    title: Equivariant Spherical Transformer for Efficient Molecular Modeling
    published_venue: ''
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.011
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: Graphormer-SPIS
    model_key: equiformer
    model_plain: Graphormer-SPIS
    metric_values:
    - 0.011
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.23086'
    title: Equivariant Spherical Transformer for Efficient Molecular Modeling
    published_venue: ''
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.011
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    metric_values:
    - null
    - 0.0286
    - 0.0435
    - 6.32
    - 6.53
    - 7.56
    - 0.023
    - 24.6
    - 19.5
    - 6.28
    - 1.21
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.019
    sort_std: 0.001
    true_value: 0.019
    true_std: 0.001
    paper_value: 0.0286
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.009600000000000001
    value_gap_source_arxiv: '2401.17752'
    value_gap_source_title: 'PF-GNN: Differentiable particle filtering based approximation
      of universal graph representations'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-01-31'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: NeurIPS 2020
    date: Nov 28, 2020
    date_display: Nov 2020
    date_iso: '2020-11-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  - model: DeepMoleNet
    model_key: deepmolenet
    model_plain: DeepMoleNet
    metric_values:
    - null
    - 0.0253
    - 0.0681
    - 7.7
    - 7.8
    - 8.6
    - 0.029
    - 23.9
    - 22.7
    - 7.8
    - 1.9
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.0253
    sort_std: null
    true_value: 0.0253
    true_std: null
    paper_value: 0.0253
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2011.14115'
    value_gap_source_title: Fast and Uncertainty-Aware Directional Message Passing
      for Non-Equilibrium Molecules
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2020-11-28'
    value_gap_source_date_label: NeurIPS 2020
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
    published_venue: NeurIPS 2020
    date: Nov 28, 2020
    date_display: Nov 2020
    date_iso: '2020-11-28'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 13
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    metric_values:
    - null
    - 0.033
    - 0.235
    - 14.0
    - 14.0
    - 14.0
    - 0.033
    - 41.0
    - 34.0
    - 19.0
    - 1.7
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.033
    sort_std: null
    true_value: 0.033
    true_std: null
    paper_value: 0.033
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.01191'
    value_gap_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-04'
    value_gap_source_date_label: AAAI 2021
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
    published_venue: NeurIPS 2020
    date: Nov 28, 2020
    date_display: Nov 2020
    date_iso: '2020-11-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 23
  - model: MGCN
    model_key: mgcn
    model_plain: MGCN
    metric_values:
    - null
    - 0.056
    - 0.03
    - 12.9
    - 14.6
    - 16.2
    - 0.038
    - 42.1
    - 57.4
    - 14.4
    - 1.12
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.056
    sort_std: null
    true_value: 0.056
    true_std: null
    paper_value: 0.056
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2110.01191'
    value_gap_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-10-04'
    value_gap_source_date_label: AAAI 2021
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
    published_venue: NeurIPS 2020
    date: Nov 28, 2020
    date_display: Nov 2020
    date_iso: '2020-11-28'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 32
  metrics:
  - gap
  - mu
  - alpha
  - U0
  - H
  - G
  - Cv
  - HOMO
  - LUMO
  - U
  - zpve
  primary_metric: gap
  rank_metric: mu
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: gap
  paper_metrics:
  - mu
  - alpha
  - U0
  - H
  - G
  - Cv
  - HOMO
  - LUMO
  - U
  - zpve
  metric: mu
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Quantum Chemistry
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Quantum Chemistry
    benchmark_slug: quantum-chemistry
    datasets:
    - dataset: QM9
      dataset_slug: qm9
single_proposed_model: DimeNet++
main_figure: /figures/2011.14115/main_figure.jpegoptim.jpg
---

