---
title: AdS-GNN - a Conformally Equivariant Graph Neural Network
arxiv_id: '2505.12880'
source_url: ''
authors:
- name: Maksim Zhdanov
  orcid: null
  s2_author_id: '2284990639'
  s2_url: null
- name: Nabil Iqbal
  orcid: null
  s2_author_id: '2293286794'
  s2_url: null
- name: Erik Bekkers
  orcid: null
  s2_author_id: '2357335645'
  s2_url: null
- name: Patrick Forr'e
  orcid: null
  s2_author_id: '51131843'
  s2_url: null
published_date: May 19, 2025
published_date_iso: '2025-05-19'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Conformal symmetries, i.e.\ coordinate transformations that preserve angles,
  play a key role in many fields, including physics, mathematics, computer vision
  and (geometric) machine learning. Here we build a neural network that is equivariant
  under general conformal transformations. To achieve this, we lift data from flat
  Euclidean space to Anti de Sitter (AdS) space. This allows us to exploit a known
  correspondence between conformal transformations of flat space and isometric transformations
  on the AdS space. We then build upon the fact that such isometric transformations
  have been extensively studied on general geometries in the geometric deep learning
  literature. We employ message-passing layers conditioned on the proper distance,
  yielding a computationally efficient framework. We validate our model on tasks from
  computer vision and statistical physics, demonstrating strong performance, improved
  generalization capacities, and the ability to extract conformal data such as scaling
  dimensions from the trained network.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- AdS-GNN
mrr: 0.0145
adjusted_mrr: 0.0048
mrr_dataset_count: 1
benchmark_categories:
- LRGB
benchmark_coverage:
- benchmark: LRGB
  benchmark_slug: lrgb
  evaluated: 1
  total: 5
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id001
  dataset: PascalVOC-SP
  rows:
  - model: SAN+RWSE
    model_key: gcn
    model_plain: SAN+RWSE
    value: 0.78
    std: 0.31
    metric: F1
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
    sort_value: 0.78
    sort_std: 0.31
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SAN+RWSE
    model_key: crawl
    model_plain: SAN+RWSE
    value: 0.4588
    std: 0.79
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
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
    global_rank: 2
    sort_value: 0.4588
    sort_std: 0.79
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SAN+RWSE
    model_key: graphgps
    model_plain: SAN+RWSE
    value: 0.4538
    std: 0.83
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
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
    global_rank: 3
    sort_value: 0.4538
    sort_std: 0.83
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AdS-GNN
    model_key: ads-gnn
    model_plain: AdS-GNN
    value: 0.2807
    std: 0.0057
    paper_value: 0.2807
    paper_std: 0.0057
    metric: F1
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test set evaluation on PascalVOC-SP
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2807
    true_std: 0.0057
    value_gap_source_arxiv: '2505.12880'
    value_gap_source_title: AdS-GNN - a Conformally Equivariant Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2807
    sort_std: 0.0057
    global_rank: 69
    paper_rank: 69
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EGNN
    model_key: egnn
    model_plain: EGNN
    value: 0.278
    std: 0.0074
    paper_value: 0.278
    paper_std: 0.0074
    metric: F1
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_classification
    protocol_decision: standard
    protocol_note: Test set evaluation on PascalVOC-SP
    date: May 19, 2025
    date_display: May 2025
    date_iso: '2025-05-19'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-05-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.278
    true_std: 0.0074
    value_gap_source_arxiv: '2505.12880'
    value_gap_source_title: AdS-GNN - a Conformally Equivariant Graph Neural Network
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.278
    sort_std: 0.0074
    global_rank: 70
    paper_rank: 70
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: F1
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: F1
  paper_metrics:
  - F1
  metric: F1
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: LRGB
  datasets:
  - *id001
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: LRGB
    benchmark_slug: lrgb
    datasets:
    - dataset: PascalVOC-SP
      dataset_slug: pascalvoc-sp
single_proposed_model: AdS-GNN
---

