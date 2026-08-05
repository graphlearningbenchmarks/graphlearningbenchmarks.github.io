---
title: 'Self-Attention in Colors: Another Take on Encoding Graph Structure in Transformers'
arxiv_id: '2304.10933'
source_url: ''
authors:
- name: Romain Menegaux
  orcid: null
  s2_author_id: '2364586368'
  s2_url: null
- name: Emmanuel Jehanno
  orcid: null
  s2_author_id: '91393750'
  s2_url: null
- name: Margot Selosse
  orcid: null
  s2_author_id: '66643494'
  s2_url: null
- name: J. Mairal
  orcid: null
  s2_author_id: '2599292'
  s2_url: null
published_date: Apr 21, 2023
published_date_iso: '2023-04-21'
published_venue: TMLR 2023
published_conference: TMLR 2023
published_conference_short: TMLR
published_conference_slug: tmlr
abstract: We introduce a novel self-attention mechanism, which we call CSA (Chromatic
  Self-Attention), which extends the notion of attention scores to attention _filters_,
  independently modulating the feature channels. We showcase CSA in a fully-attentional
  graph Transformer CGT (Chromatic Graph Transformer) which integrates both graph
  structural information and edge features, completely bypassing the need for local
  message-passing components. Our method flexibly encodes graph structure through
  node-node interactions, by enriching the original edge features with a relative
  positional encoding scheme. We propose a new scheme based on random walks that encodes
  both structural and positional information, and show how to incorporate higher-order
  topological information, such as rings in molecular graphs. Our approach achieves
  state-of-the-art results on the ZINC benchmark dataset, while providing a flexible
  framework for encoding graph structure and incorporating higher-order topology.
codebase_url: https://github.com/inria-thoth/csa
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
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
  - model: CSA-rings
    model_key: csa-rings
    model_plain: CSA-rings
    value: 0.056
    std: 0.002
    paper_value: 0.056
    paper_std: 0.002
    metric: MAE
    higher_is_better: false
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'zinc: mae fallback <= 0.06'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 21, 2023
    date_display: Apr 2023
    date_iso: '2023-04-21'
    published_venue: TMLR 2023
    published_conference: TMLR 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-21'
    value_gap_source_date_label: TMLR 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.056
    true_std: 0.002
    value_gap_source_arxiv: '2304.10933'
    value_gap_source_title: 'Self-Attention in Colors: Another Take on Encoding Graph
      Structure in Transformers'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.056
    sort_std: 0.002
    global_rank: 63
    paper_rank: 63
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
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
main_figure: /figures/2304.10933/main_figure.jpegoptim.jpg
---

