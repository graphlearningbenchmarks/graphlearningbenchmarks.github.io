---
title: 'Weisfeiler and Leman Go Loopy: A New Hierarchy for Graph Representational
  Learning'
arxiv_id: '2403.13749'
source_url: ''
authors:
- name: Raffaele Paolino
  orcid: null
  s2_author_id: '2187930583'
  s2_url: null
- name: Sohir Maskey
  orcid: null
  s2_author_id: '2127602704'
  s2_url: null
- name: Pascal Welke
  orcid: null
  s2_author_id: '2305682691'
  s2_url: null
- name: Gitta Kutyniok
  orcid: null
  s2_author_id: '3125779'
  s2_url: null
published_date: Mar 20, 2024
published_date_iso: '2024-03-20'
published_venue: NeurIPS 2024
published_conference: NeurIPS 2024
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: We introduce $r$-loopy Weisfeiler-Leman ($r$-$ $WL), a novel hierarchy of
  graph isomorphism tests and a corresponding GNN framework, $r$-$ $MPNN, that can
  count cycles up to length $r+2$. Most notably, we show that $r$-$ $WL can count
  homomorphisms of cactus graphs. This extends 1-WL, which can only count homomorphisms
  of trees and, in fact, we prove that $r$-$ $WL is incomparable to $k$-WL for any
  fixed $k$. We empirically validate the expressive and counting power of $r$-$ $MPNN
  on several synthetic datasets and demonstrate the scalability and strong performance
  on various real-world datasets, particularly on sparse graphs. Our code is available.
codebase_url: https://github.com/RPaolino/loopy
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GIN
mrr: 0.0345
adjusted_mrr: 0.0115
mrr_dataset_count: 1
benchmark_categories:
- LRGB
benchmark_coverage:
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 1
  total: 5
task_categories:
- graph_classification
experiment_scopes:
- graph-level
results:
- &id001
  dataset: Peptides-func
  rows:
  - model: S^2GCN
    model_key: s^2gcn
    model_plain: S^2GCN
    value: 0.7311
    std: 0.0066
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2411.12732'
    title: Benchmarking Positional Encodings for GNNs and Graph Transformers
    date: Nov 19, 2024
    date_display: Nov 2024
    date_iso: '2024-11-19'
    venue: Knowledge Discovery and Data Mining
    codebase_url: https://github.com/ETH-DISCO/Benchmarking-PEs
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.7311
    sort_std: 0.0066
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: S^2 GCN + PE
    model_key: s^2 gcn + pe
    model_plain: S^2 GCN + PE
    value: 0.7311
    std: 0.0066
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2405.19121'
    title: Spatio-Spectral Graph Neural Networks
    date: May 29, 2024
    date_display: May 2024
    date_iso: '2024-05-29'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: PE is described as stable positional encodings almost
      free of cost for S2GNNs.
    is_global_top: true
    global_rank: 2
    sort_value: 0.7311
    sort_std: 0.0066
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: S4G
    model_key: s4g
    model_plain: S4G
    value: 0.7293
    std: 0.0004
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2402.08678'
    title: 'Graph Mamba: Towards Learning on Graphs with State Space Models'
    date: Feb 13, 2024
    date_display: Feb 2024
    date_iso: '2024-02-13'
    venue: Knowledge Discovery and Data Mining
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.7293
    sort_std: 0.0004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.593
    std: 0.0023
    paper_value: 0.593
    paper_std: 0.0023
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 12
    source_ref: Kipf & Welling 2017
    variant_inference_reason: 'dataset: fuzzy match to peptides-func (score=76)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set results for FUNC task (AP)
    date: Mar 20, 2024
    date_display: Mar 2024
    date_iso: '2024-03-20'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.686
    at_pub_std: 0.005
    at_pub_source_arxiv: '2309.00367'
    at_pub_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph Benchmark
    at_pub_source_date_iso: '2023-09-01'
    at_pub_source_date_label: TMLR 2023
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.09300000000000008
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7261
    true_std: 0.0011
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.1331
    has_value_note: false
    value_note: ''
    sort_value: 0.7261
    sort_std: 0.0011
    global_rank: 5
    paper_rank: 146
    rank_delta: 141
    rank_delta_abs: 141
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Where Did the Gap Go? Reassessing the Long-Range Graph
      Benchmark
    comparison_source_arxiv: '2309.00367'
    is_best: true
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: 0.593
    std: 0.0023
    paper_value: 0.593
    paper_std: 0.0023
    metric: AP
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 12
    source_ref: Hu* 2020
    variant_inference_reason: 'dataset: fuzzy match to peptides-func (score=76)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set results for FUNC task (AP)
    date: Mar 20, 2024
    date_display: Mar 2024
    date_iso: '2024-03-20'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: 0.5498
    at_pub_std: 0.0079
    at_pub_source_arxiv: '2402.08678'
    at_pub_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    at_pub_source_date_iso: '2024-02-13'
    at_pub_source_date_label: KDD 2024
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.043200000000000016
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.7059
    true_std: 0.0089
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.1129
    has_value_note: false
    value_note: ''
    sort_value: 0.7059
    sort_std: 0.0089
    global_rank: 29
    paper_rank: 146
    rank_delta: 117
    rank_delta_abs: 117
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Graph Mamba: Towards Learning on Graphs with State Space
      Models'
    comparison_source_arxiv: '2402.08678'
    is_best: false
    is_std_outlier: false
  - model: 7-ℓGIN
    model_key: 7-ℓgin
    model_plain: 7-ℓGIN
    value: 0.657
    std: 0.006
    paper_value: 0.657
    paper_std: 0.006
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 12
    source_ref: this paper
    variant_inference_reason: 'dataset: fuzzy match to peptides-func (score=76)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set results for FUNC task (AP)
    date: Mar 20, 2024
    date_display: Mar 2024
    date_iso: '2024-03-20'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-20'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.657
    true_std: 0.006
    value_gap_source_arxiv: '2403.13749'
    value_gap_source_title: 'Weisfeiler and Leman Go Loopy: A New Hierarchy for Graph
      Representational Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.657
    sort_std: 0.006
    global_rank: 91
    paper_rank: 91
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPR-GNN
    model_key: gpr-gnn
    model_plain: GPR-GNN
    value: 0.5864
    std: 0.0077
    paper_value: 0.5864
    paper_std: 0.0077
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 12
    source_ref: Bresson et al. 2017
    variant_inference_reason: 'dataset: fuzzy match to peptides-func (score=76)'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Test set results for FUNC task (AP)
    date: Mar 20, 2024
    date_display: Mar 2024
    date_iso: '2024-03-20'
    published_venue: NeurIPS 2024
    published_conference: NeurIPS 2024
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-03-20'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.5864
    true_std: 0.0077
    value_gap_source_arxiv: '2403.13749'
    value_gap_source_title: 'Weisfeiler and Leman Go Loopy: A New Hierarchy for Graph
      Representational Learning'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.5864
    sort_std: 0.0077
    global_rank: 154
    paper_rank: 154
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MLP
    model_key: mlp
    model_plain: MLP
    value: 0.406
    std: 0.0021
    metric: AP
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2306.03561'
    title: 'CIN++: Enhancing Topological Message Passing'
    date: Jun 6, 2023
    date_display: Jun 2023
    date_iso: '2023-06-06'
    venue: arXiv.org
    codebase_url: https://github.com/twitter-research/cwn
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: For both datasets, we did not employ any feature augmentation
      such as positional encoding.
    is_global_top: true
    global_rank: 186
    sort_value: 0.406
    sort_std: 0.0021
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: AP
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: AP
  paper_metrics:
  - AP
  metric: AP
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: LRGB
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: Peptides-func
      dataset_slug: peptides-func
single_proposed_model: GIN
main_figure: /figures/2403.13749/main_figure.jpegoptim.jpg
---

