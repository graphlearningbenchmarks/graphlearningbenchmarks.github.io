---
title: Equivariant 3D-Conditional Diffusion Models for Molecular Linker Design
arxiv_id: '2210.05274'
source_url: ''
authors:
- name: Ilia Igashov
  orcid: null
  s2_author_id: '1677188150'
  s2_url: null
- name: Hannes Stärk
  orcid: null
  s2_author_id: '2278629180'
  s2_url: null
- name: Clément Vignac
  orcid: null
  s2_author_id: '1404062244'
  s2_url: null
- name: Arne Schneuing
  orcid: null
  s2_author_id: '89961757'
  s2_url: null
- name: Victor Garcia Satorras
  orcid: null
  s2_author_id: '73240341'
  s2_url: null
- name: Pascal Frossard
  orcid: null
  s2_author_id: '2312038635'
  s2_url: null
- name: Max Welling
  orcid: null
  s2_author_id: '2286919637'
  s2_url: null
- name: Michael M. Bronstein
  orcid: null
  s2_author_id: '2266904063'
  s2_url: null
- name: Bruno E. Correia
  orcid: null
  s2_author_id: '2266904604'
  s2_url: null
published_date: Oct 11, 2022
published_date_iso: '2022-10-11'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Fragment-based drug discovery has been an effective paradigm in early-stage
  drug development. An open challenge in this area is designing linkers between disconnected
  molecular fragments of interest to obtain chemically-relevant candidate drug molecules.
  In this work, we propose DiffLinker, an E(3)-equivariant 3D-conditional diffusion
  model for molecular linker design. Given a set of disconnected fragments, our model
  places missing atoms in between and designs a molecule incorporating all the initial
  fragments. Unlike previous approaches that are only able to connect pairs of molecular
  fragments, our method can link an arbitrary number of fragments. Additionally, the
  model automatically determines the number of atoms in the linker and its attachment
  points to the input fragments. We demonstrate that DiffLinker outperforms other
  methods on the standard datasets generating more diverse and synthetically-accessible
  molecules. Besides, we experimentally test our method in real-world applications,
  showing that it can successfully generate valid linkers conditioned on target protein
  pockets.
codebase_url: https://github.com/igashov/DiffLinker
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- DiffLinker
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Classic
benchmark_coverage:
- benchmark: Classic
  benchmark_slug: classic
  evaluated: 1
  total: 12
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ZINC
  is_multi_metric: true
  rows:
  - model: DiffLinker
    model_key: difflinker
    model_plain: DiffLinker
    metric_values:
    - null
    - 0.68
    - 3.01
    - 0.872
    - 0.32
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    sort_value: 0.68
    sort_std: null
    true_value: 0.68
    true_std: null
    paper_value: 0.68
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2210.05274'
    value_gap_source_title: Equivariant 3D-Conditional Diffusion Models for Molecular
      Linker Design
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-11'
    value_gap_source_date_label: '2022'
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
    published_venue: ''
    date: Oct 11, 2022
    date_display: Oct 2022
    date_iso: '2022-10-11'
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
  - model: 3DLinker (given anchors)
    model_key: 3dlinker (given anchors)
    model_plain: 3DLinker (given anchors)
    metric_values:
    - null
    - 0.65
    - 3.11
    - 0.94
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.65
    sort_std: null
    true_value: 0.65
    true_std: null
    paper_value: 0.65
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2210.05274'
    value_gap_source_title: Equivariant 3D-Conditional Diffusion Models for Molecular
      Linker Design
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-11'
    value_gap_source_date_label: '2022'
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
    published_venue: ''
    date: Oct 11, 2022
    date_display: Oct 2022
    date_iso: '2022-10-11'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 2
  - model: DeLinker + ConfVAE + MMFF
    model_key: delinker + confvae + mmff
    model_plain: DeLinker + ConfVAE + MMFF
    metric_values:
    - null
    - 0.64
    - 3.11
    - 0.802
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    sort_value: 0.64
    sort_std: null
    true_value: 0.64
    true_std: null
    paper_value: 0.64
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2210.05274'
    value_gap_source_title: Equivariant 3D-Conditional Diffusion Models for Molecular
      Linker Design
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-11'
    value_gap_source_date_label: '2022'
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
    published_venue: ''
    date: Oct 11, 2022
    date_display: Oct 2022
    date_iso: '2022-10-11'
    codebase_url: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 3
  metrics:
  - MAE
  - QED
  - SA
  - Recovery
  - RMSD
  primary_metric: MAE
  rank_metric: QED
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - QED
  - SA
  - Recovery
  - RMSD
  metric: QED
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Classic
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Classic
    benchmark_slug: classic
    datasets:
    - dataset: ZINC
      dataset_slug: zinc
single_proposed_model: DiffLinker
main_figure: /figures/2210.05274/main_figure.jpegoptim.jpg
---

