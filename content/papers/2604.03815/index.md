---
title: k-Maximum Inner Product Attention for Graph Transformers and the Expressive
  Power of GraphGPS
arxiv_id: '2604.03815'
source_url: ''
authors:
- name: Jonas De Schouwer
  orcid: null
  s2_author_id: '2428252455'
  s2_url: null
- name: H. Borde
  orcid: null
  s2_author_id: '2117030133'
  s2_url: null
- name: Xiaowen Dong
  orcid: null
  s2_author_id: '2239060705'
  s2_url: null
published_date: Apr 4, 2026
published_date_iso: '2026-04-04'
published_venue: ICLR 2026
published_conference: ICLR 2026
published_conference_short: ICLR
published_conference_slug: iclr
abstract: 'Graph transformers have shown promise in overcoming limitations of traditional
  graph neural networks, such as oversquashing and difficulties in modeling long-range
  dependencies. However, their application to large-scale graphs is hindered by the
  quadratic memory and computational complexity of the all-to-all attention mechanism.
  Although alternatives such as linearized attention and restricted attention patterns
  have been proposed, these often degrade performance or limit expressive power. To
  better balance efficiency and effectiveness, we introduce k-Maximum Inner Product
  (k-MIP) attention for graph transformers. k-MIP attention selects the most relevant
  key nodes per query via a top-k operation, yielding a sparse yet flexible attention
  pattern. Combined with an attention score computation based on symbolic matrices,
  this results in linear memory complexity and practical speedups of up to an order
  of magnitude compared to all-to-all attention, enabling the processing of graphs
  with over 500k nodes on a single A100 GPU. We provide a theoretical analysis of
  expressive power, showing that k-MIP attention does not compromise the expressiveness
  of graph transformers: specifically, we prove that k-MIP transformers can approximate
  any full-attention transformer to arbitrary precision. In addition, we analyze the
  expressive power of the GraphGPS framework, in which we integrate our attention
  mechanism, and establish an upper bound on its graph distinguishing capability in
  terms of the S-SEG-WL test. Finally, we validate our approach on the Long Range
  Graph Benchmark, the City-Networks benchmark, and two custom large-scale inductive
  point cloud datasets, consistently ranking among the top-performing scalable graph
  transformers.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GPS + k-MIP
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- Other Graph Benchmarks
- City-Networks
benchmark_coverage:
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 4
- benchmark: City-Networks
  benchmark_slug: city-networks
  evaluated: 3
  total: 4
task_categories:
- node_classification
experiment_scopes:
- node-level
results:
- &id004
  dataset: London
  rows:
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.6147
    std: 0.0014
    paper_value: 0.6147
    paper_std: 0.0014
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6147
    sort_std: 0.0014
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GINE
    model_key: gine
    model_plain: GINE
    value: 0.576
    std: 0.002
    paper_value: 0.576
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.576
    sort_std: 0.002
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS + k-MIP
    model_key: gps + k-mip
    model_plain: GPS + k-MIP
    value: 0.5605
    std: null
    paper_value: 0.5605
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.5605
    sort_std: null
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: graphsage
    model_plain: SGFormer
    value: 0.554
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_display: Mar 2025
    date_iso: '2025-03-12'
    venue: Published as a conference paper at ICLR 2026
    codebase_url: https://github.com/LeonResearch/City-Networks
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: nodes represent road junctions with features like longitude,
      latitude, land use, etc.
    is_global_top: true
    global_rank: 1
    sort_value: 0.554
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: chebnet
    model_plain: SGFormer
    value: 0.547
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_display: Mar 2025
    date_iso: '2025-03-12'
    venue: Published as a conference paper at ICLR 2026
    codebase_url: https://github.com/LeonResearch/City-Networks
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: nodes represent road junctions with features like longitude,
      latitude, land use, etc.
    is_global_top: true
    global_rank: 2
    sort_value: 0.547
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS + Performer
    model_key: gps + performer
    model_plain: GPS + Performer
    value: 0.532
    std: null
    paper_value: 0.532
    paper_std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.532
    sort_std: null
    global_rank: 3
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.5719
    std: 0.0109
    paper_value: 0.5719
    paper_std: 0.0109
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.52
    at_pub_std: 0.003
    at_pub_source_arxiv: '2503.09008'
    at_pub_source_title: City-Networks
    at_pub_source_date_iso: '2025-03-12'
    at_pub_source_date_label: ICLR 2025
    value_gap_source_date_iso: '2025-03-12'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.051899999999999946
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.52
    true_std: 0.003
    value_gap_source_arxiv: '2503.09008'
    value_gap_source_title: City-Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.051899999999999946
    has_value_note: false
    value_note: ''
    sort_value: 0.52
    sort_std: 0.003
    global_rank: 3
    paper_rank: 1
    rank_delta: -2
    rank_delta_abs: 2
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: City-Networks
    comparison_source_arxiv: '2503.09008'
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5525
    std: 0.0006
    paper_value: 0.5525
    paper_std: 0.0006
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.501
    at_pub_std: 0.007
    at_pub_source_arxiv: '2503.09008'
    at_pub_source_title: City-Networks
    at_pub_source_date_iso: '2025-03-12'
    at_pub_source_date_label: ICLR 2025
    value_gap_source_date_iso: '2025-03-12'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.05149999999999999
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.501
    true_std: 0.007
    value_gap_source_arxiv: '2503.09008'
    value_gap_source_title: City-Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.05149999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.501
    sort_std: 0.007
    global_rank: 4
    paper_rank: 2
    rank_delta: -2
    rank_delta_abs: 2
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: City-Networks
    comparison_source_arxiv: '2503.09008'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id002
  dataset: Paris
  rows:
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.514
    std: 0.0008
    paper_value: 0.514
    paper_std: 0.0008
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.551
    at_pub_std: 0.008
    at_pub_source_arxiv: '2503.09008'
    at_pub_source_title: City-Networks
    at_pub_source_date_iso: '2025-03-12'
    at_pub_source_date_label: ICLR 2025
    value_gap_source_date_iso: '2025-03-12'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.03700000000000003
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.551
    true_std: 0.008
    value_gap_source_arxiv: '2503.09008'
    value_gap_source_title: City-Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.03700000000000003
    has_value_note: false
    value_note: ''
    sort_value: 0.551
    sort_std: 0.008
    global_rank: 1
    paper_rank: 6
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: City-Networks
    comparison_source_arxiv: '2503.09008'
    is_best: true
    is_std_outlier: false
  - model: SGFormer
    model_key: graphsage
    model_plain: SGFormer
    value: 0.546
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_display: Mar 2025
    date_iso: '2025-03-12'
    venue: Published as a conference paper at ICLR 2026
    codebase_url: https://github.com/LeonResearch/City-Networks
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: node features such as geographical coordinates, land
      use, etc.
    is_global_top: true
    global_rank: 2
    sort_value: 0.546
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: SGFormer
    model_key: chebnet
    model_plain: SGFormer
    value: 0.541
    std: 0.002
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_display: Mar 2025
    date_iso: '2025-03-12'
    venue: Published as a conference paper at ICLR 2026
    codebase_url: https://github.com/LeonResearch/City-Networks
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: node features such as geographical coordinates, land
      use, etc.
    is_global_top: true
    global_rank: 3
    sort_value: 0.541
    sort_std: 0.002
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS + Performer
    model_key: gps + performer
    model_plain: GPS + Performer
    value: 0.5406
    std: 0.0027
    paper_value: 0.5406
    paper_std: 0.0027
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.5406
    sort_std: 0.0027
    global_rank: 4
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS + k-MIP
    model_key: gps + k-mip
    model_plain: GPS + k-MIP
    value: 0.5362
    std: 0.0022
    paper_value: 0.5362
    paper_std: 0.0022
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.5362
    sort_std: 0.0022
    global_rank: 4
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS + BigBird
    model_key: gps + bigbird
    model_plain: GPS + BigBird
    value: 0.5353
    std: 0.0037
    paper_value: 0.5353
    paper_std: 0.0037
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.5353
    sort_std: 0.0037
    global_rank: 4
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GINE
    model_key: gine
    model_plain: GINE
    value: 0.5336
    std: 0.0023
    paper_value: 0.5336
    paper_std: 0.0023
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.5336
    sort_std: 0.0023
    global_rank: 4
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.5327
    std: 0.001
    paper_value: 0.5327
    paper_std: 0.001
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.5327
    sort_std: 0.001
    global_rank: 4
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5293
    std: 0.0006
    paper_value: 0.5293
    paper_std: 0.0006
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.532
    at_pub_std: 0.003
    at_pub_source_arxiv: '2503.09008'
    at_pub_source_title: City-Networks
    at_pub_source_date_iso: '2025-03-12'
    at_pub_source_date_label: ICLR 2025
    value_gap_source_date_iso: '2025-03-12'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.0027000000000000357
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: 0.532
    true_std: 0.003
    value_gap_source_arxiv: '2503.09008'
    value_gap_source_title: City-Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.0027000000000000357
    has_value_note: false
    value_note: ''
    sort_value: 0.532
    sort_std: 0.003
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.5583
    std: 0.0042
    paper_value: 0.5583
    paper_std: 0.0042
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.511
    at_pub_std: 0.003
    at_pub_source_arxiv: '2503.09008'
    at_pub_source_title: City-Networks
    at_pub_source_date_iso: '2025-03-12'
    at_pub_source_date_label: ICLR 2025
    value_gap_source_date_iso: '2025-03-12'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.04730000000000001
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.511
    true_std: 0.003
    value_gap_source_arxiv: '2503.09008'
    value_gap_source_title: City-Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.04730000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.511
    sort_std: 0.003
    global_rank: 8
    paper_rank: 1
    rank_delta: -7
    rank_delta_abs: 7
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: City-Networks
    comparison_source_arxiv: '2503.09008'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: Shanghai
  rows:
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.6233
    std: 0.0016
    paper_value: 0.6233
    paper_std: 0.0016
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.702
    at_pub_std: 0.004
    at_pub_source_arxiv: '2503.09008'
    at_pub_source_title: City-Networks
    at_pub_source_date_iso: '2025-03-12'
    at_pub_source_date_label: ICLR 2025
    value_gap_source_date_iso: '2025-03-12'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.07869999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.702
    true_std: 0.004
    value_gap_source_arxiv: '2503.09008'
    value_gap_source_title: City-Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.07869999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.702
    sort_std: 0.004
    global_rank: 1
    paper_rank: 6
    rank_delta: 5
    rank_delta_abs: 5
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: City-Networks
    comparison_source_arxiv: '2503.09008'
    is_best: true
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.688
    std: 0.0021
    paper_value: 0.688
    paper_std: 0.0021
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.688
    sort_std: 0.0021
    global_rank: 2
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SGFormer
    model_key: graphsage
    model_plain: SGFormer
    value: 0.683
    std: 0.005
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2503.09008'
    title: City-Networks
    date: Mar 12, 2025
    date_display: Mar 2025
    date_iso: '2025-03-12'
    venue: Published as a conference paper at ICLR 2026
    codebase_url: https://github.com/LeonResearch/City-Networks
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: node features such as geographical coordinates, land
      use, etc.
    is_global_top: true
    global_rank: 2
    sort_value: 0.683
    sort_std: 0.005
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.7253
    std: 0.0023
    paper_value: 0.7253
    paper_std: 0.0023
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.68
    at_pub_std: 0.005
    at_pub_source_arxiv: '2503.09008'
    at_pub_source_title: City-Networks
    at_pub_source_date_iso: '2025-03-12'
    at_pub_source_date_label: ICLR 2025
    value_gap_source_date_iso: '2025-03-12'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.045299999999999896
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.68
    true_std: 0.005
    value_gap_source_arxiv: '2503.09008'
    value_gap_source_title: City-Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.045299999999999896
    has_value_note: false
    value_note: ''
    sort_value: 0.68
    sort_std: 0.005
    global_rank: 3
    paper_rank: 1
    rank_delta: -2
    rank_delta_abs: 2
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: City-Networks
    comparison_source_arxiv: '2503.09008'
    is_best: false
    is_std_outlier: false
  - model: GPS + Performer
    model_key: gps + performer
    model_plain: GPS + Performer
    value: 0.6727
    std: 0.0017
    paper_value: 0.6727
    paper_std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6727
    sort_std: 0.0017
    global_rank: 4
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS + k-MIP
    model_key: gps + k-mip
    model_plain: GPS + k-MIP
    value: 0.6694
    std: 0.0044
    paper_value: 0.6694
    paper_std: 0.0044
    metric: Accuracy
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6694
    sort_std: 0.0044
    global_rank: 4
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS + BigBird
    model_key: gps + bigbird
    model_plain: GPS + BigBird
    value: 0.6524
    std: 0.0017
    paper_value: 0.6524
    paper_std: 0.0017
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6524
    sort_std: 0.0017
    global_rank: 5
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GINE
    model_key: gine
    model_plain: GINE
    value: 0.6335
    std: 0.002
    paper_value: 0.6335
    paper_std: 0.002
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6335
    sort_std: 0.002
    global_rank: 6
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.5775
    std: 0.0024
    paper_value: 0.5775
    paper_std: 0.0024
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: 0.621
    at_pub_std: 0.002
    at_pub_source_arxiv: '2503.09008'
    at_pub_source_title: City-Networks
    at_pub_source_date_iso: '2025-03-12'
    at_pub_source_date_label: ICLR 2025
    value_gap_source_date_iso: '2025-03-12'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: 0.04349999999999998
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.621
    true_std: 0.002
    value_gap_source_arxiv: '2503.09008'
    value_gap_source_title: City-Networks
    value_gap_source_is_current_paper: false
    value_gap: 0.04349999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.621
    sort_std: 0.002
    global_rank: 7
    paper_rank: 9
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: City-Networks
    comparison_source_arxiv: '2503.09008'
    is_best: false
    is_std_outlier: false
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: node-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: ShapeNet-Part
  rows:
  - model: GPS + k-MIP
    model_key: gps + k-mip
    model_plain: GPS + k-MIP
    value: 0.8268
    std: 0.0064
    paper_value: 0.8268
    paper_std: 0.0064
    metric: F1
    higher_is_better: true
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8268
    sort_std: 0.0064
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: Exphormer
    model_key: exphormer
    model_plain: Exphormer
    value: 0.8262
    std: 0.0031
    paper_value: 0.8262
    paper_std: 0.0031
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.8262
    sort_std: 0.0031
    global_rank: 1
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: AC-DGCNN
    model_key: vn-dgcnn
    model_plain: AC-DGCNN
    value: 0.814
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: Sep 29, 2025
    date_display: Sep 2025
    date_iso: '2025-09-29'
    venue: arXiv.org
    codebase_url: https://github.com/ywelld/_ac
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.814
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AC-DGCNN
    model_key: ac-dgcnn
    model_plain: AC-DGCNN
    value: 0.809
    std: 0.007
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: Sep 29, 2025
    date_display: Sep 2025
    date_iso: '2025-09-29'
    venue: arXiv.org
    codebase_url: https://github.com/ywelld/_ac
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 0.809
    sort_std: 0.007
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS + BigBird
    model_key: gps + bigbird
    model_plain: GPS + BigBird
    value: 0.7965
    std: 0.0098
    paper_value: 0.7965
    paper_std: 0.0098
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.7965
    sort_std: 0.0098
    global_rank: 3
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: AC-DGCNN
    model_key: dgcnn
    model_plain: AC-DGCNN
    value: 0.786
    std: null
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2509.24886'
    title: Adaptive Canonicalization with Application to Invariant Anisotropic Geometric
      Networks
    date: Sep 29, 2025
    date_display: Sep 2025
    date_iso: '2025-09-29'
    venue: arXiv.org
    codebase_url: https://github.com/ywelld/_ac
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 0.786
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS + Performer
    model_key: gps + performer
    model_plain: GPS + Performer
    value: 0.7736
    std: 0.0123
    paper_value: 0.7736
    paper_std: 0.0123
    metric: F1
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.7736
    sort_std: 0.0123
    global_rank: 5
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: 0.762
    std: 0.0032
    paper_value: 0.762
    paper_std: 0.0032
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.762
    sort_std: 0.0032
    global_rank: 5
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GINE
    model_key: gine
    model_plain: GINE
    value: 0.6457
    std: 0.0035
    paper_value: 0.6457
    paper_std: 0.0035
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6457
    sort_std: 0.0035
    global_rank: 8
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GAT
    model_key: gat
    model_plain: GAT
    value: 0.6301
    std: 0.0017
    paper_value: 0.6301
    paper_std: 0.0017
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6301
    sort_std: 0.0017
    global_rank: 8
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 0.6018
    std: 0.0004
    paper_value: 0.6018
    paper_std: 0.0004
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Apr 4, 2026
    date_display: Apr 2026
    date_iso: '2026-04-04'
    published_venue: ICLR 2026
    published_conference: ICLR 2026
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: ''
    value_gap_source_date_label: ''
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    sort_value: 0.6018
    sort_std: 0.0004
    global_rank: 9
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_note: ''
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    rank_delta_direction: null
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
- benchmark: Other Graph Benchmarks
  datasets:
  - *id001
- benchmark: City-Networks
  datasets:
  - *id002
  - *id003
  - *id004
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: ShapeNet-Part
      dataset_slug: shapenet-part
  - benchmark: City-Networks
    benchmark_slug: city-networks
    datasets:
    - dataset: Paris
      dataset_slug: paris
    - dataset: Shanghai
      dataset_slug: shanghai
    - dataset: London
      dataset_slug: london
single_proposed_model: GPS + k-MIP
---

