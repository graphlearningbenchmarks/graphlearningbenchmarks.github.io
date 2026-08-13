---
title: ECHO Benchmark
arxiv_id: '2512.17762'
source_url: ''
authors:
- name: Luca Miglior
  orcid: null
  s2_author_id: '2292617786'
  s2_url: null
- name: Matteo Tolloso
  orcid: null
  s2_author_id: '2371068009'
  s2_url: null
- name: Alessio Gravina
  orcid: null
  s2_author_id: '2042289369'
  s2_url: null
- name: Davide Bacciu
  orcid: null
  s2_author_id: '2371068121'
  s2_url: null
published_date: Dec 19, 2025
published_date_iso: '2025-12-19'
published_venue: ICLR 2025
published_conference: ICLR 2025
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Effectively capturing long-range interactions remains a fundamental yet
  unresolved challenge in graph neural network (GNN) research, critical for applications
  across diverse fields of science. To systematically address this, we introduce ECHO
  (Evaluating Communication over long HOps), a novel benchmark specifically designed
  to rigorously assess the capabilities of GNNs in handling very long-range graph
  propagation. ECHO includes three synthetic graph tasks, namely single-source shortest
  paths, node eccentricity, and graph diameter, each constructed over diverse and
  structurally challenging topologies intentionally designed to introduce significant
  information bottlenecks. ECHO also includes two real-world datasets, ECHO-Charge
  and ECHO-Energy, which define chemically grounded benchmarks for predicting atomic
  partial charges and molecular total energies, respectively, with reference computations
  obtained at the density functional theory (DFT) level. Both tasks inherently depend
  on capturing complex long-range molecular interactions. Our extensive benchmarking
  of popular GNN architectures reveals clear performance gaps, emphasizing the difficulty
  of true long-range propagation and highlighting design choices capable of overcoming
  inherent limitations. ECHO thereby sets a new standard for evaluating long-range
  information propagation, also providing a compelling example for its need in AI
  for science.
codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: dataset
proposed_models: []
mrr: null
adjusted_mrr: null
mrr_dataset_count: 0
benchmark_categories:
- ECHO Benchmark
benchmark_coverage:
- benchmark: ECHO Benchmark
  benchmark_slug: echo-benchmark
  evaluated: 1
  total: 1
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: ECHO-Synth
  rows:
  - model: GHR
    model_key: ghr
    model_plain: GHR
    value: 0.035
    std: 0.004
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2605.18387'
    title: Graph Hierarchical Recurrence for Long-Range Generalization
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: The model uses node and edge attributes projected into
      latent space via learnable linear maps.
    is_global_top: true
    global_rank: 1
    sort_value: 0.035
    sort_std: 0.004
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GRIT
    model_key: grit
    model_plain: GRIT
    value: 0.121
    std: 0.013
    paper_value: 0.121
    paper_std: 0.013
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for synthetic tasks diam, ecc, and sssp
    date: Dec 19, 2025
    date_display: Dec 2025
    date_iso: '2025-12-19'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.121
    true_std: 0.013
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.121
    sort_std: 0.013
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GHR-GINE
    model_key: ghr-gine
    model_plain: GHR-GINE
    value: 0.379
    std: 0.191
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.18387'
    title: Graph Hierarchical Recurrence for Long-Range Generalization
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: The model uses node and edge attributes projected into
      latent space via learnable linear maps.
    is_global_top: true
    global_rank: 3
    sort_value: 0.379
    sort_std: 0.191
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GPS
    model_key: gps
    model_plain: GPS
    value: 0.472
    std: 0.05
    paper_value: 0.472
    paper_std: 0.05
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for synthetic tasks diam, ecc, and sssp
    date: Dec 19, 2025
    date_display: Dec 2025
    date_iso: '2025-12-19'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.472
    true_std: 0.05
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.472
    sort_std: 0.05
    global_rank: 4
    paper_rank: 4
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SWAN
    model_key: swan
    model_plain: SWAN
    value: 0.896
    std: 0.232
    paper_value: 0.896
    paper_std: 0.232
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for synthetic tasks diam, ecc, and sssp
    date: Dec 19, 2025
    date_display: Dec 2025
    date_iso: '2025-12-19'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.896
    true_std: 0.232
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.896
    sort_std: 0.232
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: A-DGN
    model_key: a-dgn
    model_plain: A-DGN
    value: 1.151
    std: 0.038
    paper_value: 1.151
    paper_std: 0.038
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for synthetic tasks diam, ecc, and sssp
    date: Dec 19, 2025
    date_display: Dec 2025
    date_iso: '2025-12-19'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.151
    true_std: 0.038
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.151
    sort_std: 0.038
    global_rank: 6
    paper_rank: 6
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DRew
    model_key: drew
    model_plain: DRew
    value: 1.243
    std: 0.047
    paper_value: 1.243
    paper_std: 0.047
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    uses_external_data: 1
    input_feature_source: other_external_features
    feature_source_evidence: DRew’s reported runtime does not include the pre-processing
      step, which involves computing the Floyd–Warshall algorithm
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for synthetic tasks diam, ecc, and sssp
    date: Dec 19, 2025
    date_display: Dec 2025
    date_iso: '2025-12-19'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.243
    true_std: 0.047
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.243
    sort_std: 0.047
    global_rank: 7
    paper_rank: 7
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PH-DGN
    model_key: ph-dgn
    model_plain: PH-DGN
    value: 1.323
    std: 0.485
    paper_value: 1.323
    paper_std: 0.485
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for synthetic tasks diam, ecc, and sssp
    date: Dec 19, 2025
    date_display: Dec 2025
    date_iso: '2025-12-19'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.323
    true_std: 0.485
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.323
    sort_std: 0.485
    global_rank: 8
    paper_rank: 8
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
    value: 1.63
    std: 0.161
    paper_value: 1.63
    paper_std: 0.161
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for synthetic tasks diam, ecc, and sssp
    date: Dec 19, 2025
    date_display: Dec 2025
    date_iso: '2025-12-19'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-12-19'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.63
    true_std: 0.161
    value_gap_source_arxiv: '2512.17762'
    value_gap_source_title: ECHO Benchmark
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.63
    sort_std: 0.161
    global_rank: 10
    paper_rank: 10
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCNII
    model_key: gcnii
    model_plain: GCNII
    value: 2.005
    std: 0.093
    paper_value: 2.005
    paper_std: 0.093
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for synthetic tasks diam, ecc, and sssp
    date: Dec 19, 2025
    date_display: Dec 2025
    date_iso: '2025-12-19'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.005
    true_std: 0.093
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.005
    sort_std: 0.093
    global_rank: 11
    paper_rank: 11
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GCN
    model_key: gcn
    model_plain: GCN
    value: 2.102
    std: 0.094
    paper_value: 2.102
    paper_std: 0.094
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for synthetic tasks diam, ecc, and sssp
    date: Dec 19, 2025
    date_display: Dec 2025
    date_iso: '2025-12-19'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.102
    true_std: 0.094
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.102
    sort_std: 0.094
    global_rank: 12
    paper_rank: 12
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GraphCON
    model_key: graphcon
    model_plain: GraphCON
    value: 2.969
    std: 0.189
    paper_value: 2.969
    paper_std: 0.189
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
    input_feature_source: raw_features
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Test split for synthetic tasks diam, ecc, and sssp
    date: Dec 19, 2025
    date_display: Dec 2025
    date_iso: '2025-12-19'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 2.969
    true_std: 0.189
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 2.969
    sort_std: 0.189
    global_rank: 13
    paper_rank: 13
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
- benchmark: ECHO Benchmark
  datasets:
  - *id001
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: ECHO Benchmark
    benchmark_slug: echo-benchmark
    datasets:
    - dataset: ECHO-Synth
      dataset_slug: echo-synth
main_figure: /figures/2512.17762/main_figure.jpegoptim.jpg
---

