---
title: Large-scale graph representation learning with very deep GNNs and self-supervision
arxiv_id: '2107.09422'
source_url: ''
authors:
- name: Ravichandra Addanki
  orcid: null
  s2_author_id: '104000494'
  s2_url: null
- name: P. Battaglia
  orcid: null
  s2_author_id: '2019153'
  s2_url: null
- name: D. Budden
  orcid: null
  s2_author_id: '2508525'
  s2_url: null
- name: Andreea Deac
  orcid: null
  s2_author_id: '48860334'
  s2_url: null
- name: Jonathan Godwin
  orcid: null
  s2_author_id: '2069002234'
  s2_url: null
- name: T. Keck
  orcid: null
  s2_author_id: '143926707'
  s2_url: null
- name: Wai Lok Sibon Li
  orcid: null
  s2_author_id: '2154686884'
  s2_url: null
- name: Alvaro Sanchez-Gonzalez
  orcid: null
  s2_author_id: '1398105826'
  s2_url: null
- name: Jacklynn Stott
  orcid: null
  s2_author_id: '2114860628'
  s2_url: null
- name: S. Thakoor
  orcid: null
  s2_author_id: '41037204'
  s2_url: null
- name: Petar Velivckovi'c
  orcid: null
  s2_author_id: '1742197495'
  s2_url: null
published_date: Jul 20, 2021
published_date_iso: '2021-07-20'
published_venue: KDD 2021
published_conference: KDD 2021
published_conference_short: KDD
published_conference_slug: kdd
abstract: 'Effectively and efficiently deploying graph neural networks (GNNs) at scale
  remains one of the most challenging aspects of graph representation learning. Many
  powerful solutions have only ever been validated on comparatively small datasets,
  often with counter-intuitive outcomes---a barrier which has been broken by the Open
  Graph Benchmark Large-Scale Challenge (OGB-LSC). We entered the OGB-LSC with two
  large-scale GNNs: a deep transductive node classifier powered by bootstrapping,
  and a very deep (up to 50-layer) inductive graph regressor regularised by denoising
  objectives. Our models achieved an award-level (top-3) performance on both the MAG240M
  and PCQM4M benchmarks. In doing so, we demonstrate evidence of scalable self-supervised
  graph representation learning, and utility of very deep GNNs---both very important
  open issues. Our code is publicly available at:.'
codebase_url: https://github.com/deepmind/deepmind-research
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- ILSVRC
mrr: 0.0147
adjusted_mrr: 0.0049
mrr_dataset_count: 1
benchmark_categories:
- OGB
benchmark_coverage:
- benchmark: OGB
  benchmark_slug: ogb
  evaluated: 1
  total: 16
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: PCQM4Mv2
  rows:
  - model: DeMol
    model_key: demol
    model_plain: DeMol
    value: 0.0603
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 186.0
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    venue: Accepted to ICLR 2026
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.0603
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TGT-At
    model_key: tgt-at
    model_plain: TGT-At
    value: 0.0671
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 203.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    venue: Accepted to ICLR 2026
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.0671
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TGT-At (+RDKit)
    model_key: tgt-at (+rdkit)
    model_plain: TGT-At (+RDKit)
    value: 0.0683
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 203.0
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.04538'
    title: 'Triplet Interaction Improves Graph Transformers: Accurate Molecular Graph
      Learning with Triplet Graph Transformers'
    date: Feb 7, 2024
    date_display: Feb 2024
    date_iso: '2024-02-07'
    venue: International Conference on Machine Learning
    codebase_url: https://github.com/shamim-hussain/tgt
    uses_external_data: true
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.0683
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.1195
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 3.8
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2603.00568'
    title: Enhancing Molecular Property Predictions by Learning from Bond Modelling
      and Interactions
    date: Feb 28, 2026
    date_display: Feb 2026
    date_iso: '2026-02-28'
    venue: Accepted to ICLR 2026
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 66
    sort_value: 0.1195
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: ILSVRC
    model_key: ilsvrc
    model_plain: ILSVRC
    value: 0.1205
    std: null
    paper_value: 0.1205
    paper_std: null
    metric: MAE
    higher_is_better: false
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
    table_ref: ''
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to pcqm4mv2 (score=86)'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Inductive graph regression on PCQM4M-LSC using the standard 80:10:10
      split based on PubChem ID.
    date: Jul 20, 2021
    date_display: Jul 2021
    date_iso: '2021-07-20'
    published_venue: KDD 2021
    published_conference: KDD 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-07-20'
    value_gap_source_date_label: KDD 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1205
    true_std: null
    value_gap_source_arxiv: '2107.09422'
    value_gap_source_title: Large-scale graph representation learning with very deep
      GNNs and self-supervision
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1205
    sort_std: null
    global_rank: 68
    paper_rank: 68
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  metric: MAE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
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
    - dataset: PCQM4Mv2
      dataset_slug: pcqm4mv2
single_proposed_model: ILSVRC
main_figure: /figures/2107.09422/main_figure.jpegoptim.jpg
---

