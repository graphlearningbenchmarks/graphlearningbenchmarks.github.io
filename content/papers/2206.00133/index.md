---
title: Pre-training via Denoising for Molecular Property Prediction
arxiv_id: '2206.00133'
source_url: ''
authors:
- name: Sheheryar Zaidi
  orcid: null
  s2_author_id: '1749331444'
  s2_url: null
- name: Michael Schaarschmidt
  orcid: null
  s2_author_id: '1759544'
  s2_url: null
- name: James Martens
  orcid: null
  s2_author_id: '145704247'
  s2_url: null
- name: Hyunjik Kim
  orcid: null
  s2_author_id: '3407176'
  s2_url: null
- name: Y. Teh
  orcid: null
  s2_author_id: '1725303'
  s2_url: null
- name: Alvaro Sanchez-Gonzalez
  orcid: null
  s2_author_id: '1398105826'
  s2_url: null
- name: P. Battaglia
  orcid: null
  s2_author_id: '2019153'
  s2_url: null
- name: Razvan Pascanu
  orcid: null
  s2_author_id: '1996134'
  s2_url: null
- name: Jonathan Godwin
  orcid: null
  s2_author_id: '2069002234'
  s2_url: null
published_date: May 31, 2022
published_date_iso: '2022-05-31'
published_venue: ICLR 2022
published_conference: ICLR 2022
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Many important problems involving molecular property prediction from 3D
  structures have limited data, posing a generalization challenge for neural networks.
  In this paper, we describe a pre-training technique based on denoising that achieves
  a new state-of-the-art in molecular property prediction by utilizing large datasets
  of 3D molecular structures at equilibrium to learn meaningful representations for
  downstream tasks. Relying on the well-known link between denoising autoencoders
  and score-matching, we show that the denoising objective corresponds to learning
  a molecular force field -- arising from approximating the Boltzmann distribution
  with a mixture of Gaussians -- directly from equilibrium structures. Our experiments
  demonstrate that using this pre-training objective significantly improves performance
  on multiple benchmarks, achieving a new state-of-the-art on the majority of targets
  in the widely used QM9 dataset. Our analysis then provides practical insights into
  the effects of different factors -- dataset sizes, model size and architecture,
  and the choice of upstream and downstream datasets -- on pre-training.
codebase_url: https://github.com/shehzaidi/pre-training-via-denoising
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
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
  - model: TorchMD-NET + Pre-training
    model_key: egt-large
    model_plain: TorchMD-NET + Pre-training
    value: 0.0872
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 110.8
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_display: Jan 2022
    date_iso: '2022-01-30'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.0872
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: TorchMD-NET + Pre-training
    model_key: grpe-standard
    model_plain: TorchMD-NET + Pre-training
    value: 0.0898
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 46.2
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2201.12787'
    title: 'GRPE: Relative Positional Encoding for Graph Transformer'
    date: Jan 30, 2022
    date_display: Jan 2022
    date_iso: '2022-01-30'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.0898
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TorchMD-NET + Pre-training
    model_key: advsyngnn
    model_plain: TorchMD-NET + Pre-training
    value: 0.108
    std: 0.002
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2602.17071'
    title: 'AdvSynGNN: Structure-Adaptive Graph Neural Nets via Adversarial Synthesis
      and Self-Corrective Propagation'
    date: Feb 19, 2026
    date_display: Feb 2026
    date_iso: '2026-02-19'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.108
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TorchMD-NET + Pre-training
    model_key: torchmd-net + pre-training
    model_plain: TorchMD-NET + Pre-training
    value: 15.6
    std: 0.1
    paper_value: 15.6
    paper_std: 0.1
    metric: MAE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Evaluation on HOMO target using standard split/protocol for PCQM4Mv2
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 15.6
    true_std: 0.1
    value_gap_source_arxiv: '2206.00133'
    value_gap_source_title: Pre-training via Denoising for Molecular Property Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 15.6
    sort_std: 0.1
    global_rank: 22
    paper_rank: 22
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TorchMD-NET + Noisy Nodes
    model_key: torchmd-net + noisy nodes
    model_plain: TorchMD-NET + Noisy Nodes
    value: 18.1
    std: 0.1
    paper_value: 18.1
    paper_std: 0.1
    metric: MAE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Evaluation on HOMO target using standard split/protocol for PCQM4Mv2
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 18.1
    true_std: 0.1
    value_gap_source_arxiv: '2206.00133'
    value_gap_source_title: Pre-training via Denoising for Molecular Property Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 18.1
    sort_std: 0.1
    global_rank: 23
    paper_rank: 23
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TorchMD-Net
    model_key: torchmd-net
    model_plain: TorchMD-Net
    value: 22.0
    std: 0.6
    paper_value: 22.0
    paper_std: 0.6
    metric: MAE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Evaluation on HOMO target using standard split/protocol for PCQM4Mv2
    date: May 31, 2022
    date_display: May 2022
    date_iso: '2022-05-31'
    published_venue: ICLR 2022
    published_conference: ICLR 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-05-31'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 22.0
    true_std: 0.6
    value_gap_source_arxiv: '2206.00133'
    value_gap_source_title: Pre-training via Denoising for Molecular Property Prediction
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 22.0
    sort_std: 0.6
    global_rank: 24
    paper_rank: 24
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
main_figure: /figures/2206.00133/main_figure.jpegoptim.jpg
---

