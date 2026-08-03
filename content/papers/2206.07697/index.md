---
title: 'MACE: Higher Order Equivariant Message Passing Neural Networks for Fast and
  Accurate Force Fields'
arxiv_id: '2206.07697'
source_url: ''
authors:
- name: Ilyes Batatia
  orcid: null
  s2_author_id: '2040711516'
  s2_url: null
- name: D. Kov'acs
  orcid: null
  s2_author_id: '2165311424'
  s2_url: null
- name: G. Simm
  orcid: null
  s2_author_id: '46338741'
  s2_url: null
- name: C. Ortner
  orcid: null
  s2_author_id: '2060586'
  s2_url: null
- name: Gábor Csányi
  orcid: null
  s2_author_id: '2559761'
  s2_url: null
published_date: Jun 15, 2022
published_date_iso: '2022-06-15'
published_venue: NeurIPS 2022
published_conference: NeurIPS 2022
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Creating fast and accurate force fields is a long-standing challenge in
  computational chemistry and materials science. Recently, several equivariant message
  passing neural networks (MPNNs) have been shown to outperform models built using
  other approaches in terms of accuracy. However, most MPNNs suffer from high computational
  cost and poor scalability. We propose that these limitations arise because MPNNs
  only pass two-body messages leading to a direct relationship between the number
  of layers and the expressivity of the network. In this work, we introduce MACE,
  a new equivariant MPNN model that uses higher body order messages. In particular,
  we show that using four-body messages reduces the required number of message passing
  iterations to just two, resulting in a fast and highly parallelizable model, reaching
  or exceeding state-of-the-art accuracy on the rMD17, 3BPA, and AcAc benchmark tasks.
  We also demonstrate that using higher order messages leads to an improved steepness
  of the learning curves.
codebase_url: https://github.com/ACEsuit/mace
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MACE
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
  dataset: MD17
  is_multi_metric: true
  rows:
  - model: MACE
    model_key: mace
    model_plain: MACE
    metric_values:
    - null
    - 0.4
    - 0.3
    metric_stds:
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
    sort_value: 0.4
    sort_std: null
    true_value: 0.4
    true_std: null
    paper_value: 0.4
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2206.07697'
    value_gap_source_title: 'MACE: Higher Order Equivariant Message Passing Neural
      Networks for Fast and Accurate Force Fields'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-06-15'
    value_gap_source_date_label: NeurIPS 2022
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
    published_venue: NeurIPS 2022
    date: Jun 15, 2022
    date_display: Jun 2022
    date_iso: '2022-06-15'
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
  - MAE
  - E
  - F
  primary_metric: MAE
  rank_metric: E
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - E
  - F
  metric: E
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
    - dataset: MD17
      dataset_slug: md17
single_proposed_model: MACE
---

