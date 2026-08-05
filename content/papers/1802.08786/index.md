---
title: Syntax-Directed Variational Autoencoder for Structured Data
arxiv_id: '1802.08786'
source_url: ''
authors:
- name: H. Dai
  orcid: null
  s2_author_id: '2791430'
  s2_url: null
- name: Yingtao Tian
  orcid: null
  s2_author_id: '48391641'
  s2_url: null
- name: Bo Dai
  orcid: null
  s2_author_id: '144445933'
  s2_url: null
- name: S. Skiena
  orcid: null
  s2_author_id: '1721948'
  s2_url: null
- name: Le Song
  orcid: null
  s2_author_id: '1779453'
  s2_url: null
published_date: Feb 15, 2018
published_date_iso: '2018-02-15'
published_venue: ICLR 2018
published_conference: ICLR 2018
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Deep generative models have been enjoying success in modeling continuous
  data. However it remains challenging to capture the representations for discrete
  structures with formal grammars and semantics,, computer programs and molecular
  structures. How to generate both syntactically and semantically correct data still
  remains largely an open problem. Inspired by the theory of compiler where the syntax
  and semantics check is done via syntax-directed translation (SDT), we propose a
  novel syntax-directed variational autoencoder (SD-VAE) by introducing stochastic
  lazy attributes. This approach converts the offline SDT check into on-the-fly generated
  guidance for constraining the decoder. Comparing to the state-of-the-art methods,
  our approach enforces constraints on the output space so that the output will be
  not only syntactically valid, but also semantically reasonable. We evaluate the
  proposed model with applications in programming language and molecules, including
  reconstruction and program/molecule optimization. The results demonstrate the effectiveness
  in incorporating syntactic and semantic constraints in discrete generative models,
  which is significantly better than current state-of-the-art approaches.
codebase_url: https://github.com/Hanjun-Dai/sdvae
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SD-VAE
mrr: 0.0088
adjusted_mrr: 0.0029
mrr_dataset_count: 1
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
  rows:
  - model: TIGT
    model_key: tigt
    model_plain: TIGT
    value: 0.014
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2402.02005'
    title: Topology-Informed Graph Transformer
    date: Feb 3, 2024
    date_display: Feb 2024
    date_iso: '2024-02-03'
    venue: GRaM
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.014
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: FloydNet
    model_key: floydnet
    model_plain: FloydNet
    value: 0.016
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2601.19094'
    title: 'FloydNet: A Learning Paradigm for Global Relational Reasoning'
    date: Jan 27, 2026
    date_display: Jan 2026
    date_iso: '2026-01-27'
    venue: arXiv.org
    codebase_url: https://github.com/ocx-lab/FloydNet
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.016
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PST
    model_key: pst
    model_plain: PST
    value: 0.018
    std: 0.001
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2405.02795'
    title: Graph as Point Set
    date: May 5, 2024
    date_display: May 2024
    date_iso: '2024-05-05'
    venue: International Conference on Machine Learning
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.018
    sort_std: 0.001
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.088
    std: 0.002
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2502.02479'
    title: Using Random Noise Equivariantly to Boost Graph Neural Networks Universally
    date: Feb 4, 2025
    date_display: Feb 2025
    date_iso: '2025-02-04'
    venue: arXiv.org
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 74
    sort_value: 0.088
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SD-VAE
    model_key: sd-vae
    model_plain: SD-VAE
    value: 1.366
    std: 0.023
    paper_value: 1.366
    paper_std: 0.023
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test RMSE/LL reported for Zinc regression task using encoded mean
      latent vector.
    date: Feb 15, 2018
    date_display: Feb 2018
    date_iso: '2018-02-15'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-02-15'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.366
    true_std: 0.023
    value_gap_source_arxiv: '1802.08786'
    value_gap_source_title: Syntax-Directed Variational Autoencoder for Structured
      Data
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.366
    sort_std: 0.023
    global_rank: 114
    paper_rank: 114
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GVAE
    model_key: gvae
    model_plain: GVAE
    value: 1.404
    std: 0.006
    paper_value: 1.404
    paper_std: 0.006
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
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test RMSE/LL reported for Zinc regression task using encoded mean
      latent vector.
    date: Feb 15, 2018
    date_display: Feb 2018
    date_iso: '2018-02-15'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-02-15'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.404
    true_std: 0.006
    value_gap_source_arxiv: '1802.08786'
    value_gap_source_title: Syntax-Directed Variational Autoencoder for Structured
      Data
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.404
    sort_std: 0.006
    global_rank: 115
    paper_rank: 115
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: CVAE
    model_key: cvae
    model_plain: CVAE
    value: 1.504
    std: 0.006
    paper_value: 1.504
    paper_std: 0.006
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
    variant_inference_reason: 'zinc: paper text matched full'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test RMSE/LL reported for Zinc regression task using encoded mean
      latent vector.
    date: Feb 15, 2018
    date_display: Feb 2018
    date_iso: '2018-02-15'
    published_venue: ICLR 2018
    published_conference: ICLR 2018
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2018-02-15'
    value_gap_source_date_label: ICLR 2018
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.504
    true_std: 0.006
    value_gap_source_arxiv: '1802.08786'
    value_gap_source_title: Syntax-Directed Variational Autoencoder for Structured
      Data
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.504
    sort_std: 0.006
    global_rank: 117
    paper_rank: 117
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
single_proposed_model: SD-VAE
main_figure: /figures/1802.08786/main_figure.jpegoptim.jpg
---

