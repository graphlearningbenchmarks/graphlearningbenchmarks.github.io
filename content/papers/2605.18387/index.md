---
title: Graph Hierarchical Recurrence for Long-Range Generalization
arxiv_id: '2605.18387'
source_url: ''
authors:
- name: Stefano Carotti
  orcid: null
  s2_author_id: '2438630735'
  s2_url: null
- name: Marco Pacini
  orcid: null
  s2_author_id: '2279752716'
  s2_url: null
- name: Alessio Gravina
  orcid: null
  s2_author_id: '2283154256'
  s2_url: null
- name: Davide Bacciu
  orcid: null
  s2_author_id: '2292258601'
  s2_url: null
- name: Bruno Lepri
  orcid: null
  s2_author_id: '2257229710'
  s2_url: null
- name: Sebastiano Bontorin
  orcid: null
  s2_author_id: '1933077486'
  s2_url: null
published_date: May 18, 2026
published_date_iso: '2026-05-18'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph Neural Networks (GNNs) and Graph Transformers (GTs) are now a fundamental
  paradigm for graph learning, combining the representation-learning capabilities
  of deep models with the sample efficiency induced by their inductive biases. Despite
  their effectiveness, a large body of work has shown that these models still face
  fundamental limitations in tasks that require capturing correlations between distant
  regions of a graph. To address this issue, we introduce Graph Hierarchical Recurrence
  (GHR), a novel framework that operates jointly on the input graph and on a hierarchical
  abstraction obtained through pooling. We also show that the limitations of existing
  models are even more pronounced in out-of-range generalization, where test instances
  involve interactions over distances longer than those observed during training.
  By contrast, despite its simple design, GHR provides three key advantages: strong
  performance on long-range dependencies, improved out-of-range generalization, and
  high parameter efficiency. To corroborate these claims, we show that across a broad
  set of long-range benchmarks, GHR consistently outperforms existing graph models
  while using as little as 1% of the parameters of current state-of-the-art models.
  These results suggest a complementary direction to the current trend of scaling
  architectures to obtain graph foundation models, indicating that increased model
  capacity alone may not be sufficient for generalization.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- GHR
mrr: 0.0
adjusted_mrr: 0.0
mrr_dataset_count: 0
benchmark_categories:
- ECHO Benchmark
- LRIM Graph Benchmark
benchmark_coverage:
- benchmark: ECHO Benchmark
  benchmark_slug: echo-benchmark
  evaluated: 1
  total: 3
- benchmark: LRIM Graph Benchmark
  benchmark_slug: lrim-graph-benchmark
  evaluated: 1
  total: 1
task_categories:
- graph_regression
- node_regression
experiment_scopes:
- graph-level
- node-level
results:
- &id001
  dataset: ECHO-Synth
  rows:
  - model: GHR
    model_key: ghr
    model_plain: GHR
    value: 0.035
    std: 0.004
    paper_value: 0.035
    paper_std: 0.004
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The model uses node and edge attributes projected into
      latent space via learnable linear maps.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.035
    true_std: 0.004
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.035
    sort_std: 0.004
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
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
    feature_source_evidence: Baseline results from Miglior et al. 2025.
    table_ref: Table 1
    source_ref: miglior2025can
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.121
    at_pub_std: 0.013
    at_pub_source_arxiv: '2512.17762'
    at_pub_source_title: ECHO Benchmark
    at_pub_source_date_iso: '2025-12-19'
    at_pub_source_date_label: ICLR 2025
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
    value_gap_source_is_current_paper: true
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
    paper_value: 0.379
    paper_std: 0.191
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
    feature_source_evidence: The model uses node and edge attributes projected into
      latent space via learnable linear maps.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
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
    true_value: 0.379
    true_std: 0.191
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.379
    sort_std: 0.191
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
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
    feature_source_evidence: Baseline results from Miglior et al. 2025.
    table_ref: Table 1
    source_ref: miglior2025can
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.472
    at_pub_std: 0.05
    at_pub_source_arxiv: '2512.17762'
    at_pub_source_title: ECHO Benchmark
    at_pub_source_date_iso: '2025-12-19'
    at_pub_source_date_label: ICLR 2025
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
    value_gap_source_is_current_paper: true
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
    feature_source_evidence: Baseline results from Miglior et al. 2025.
    table_ref: Table 1
    source_ref: miglior2025can
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.896
    at_pub_std: 0.232
    at_pub_source_arxiv: '2512.17762'
    at_pub_source_title: ECHO Benchmark
    at_pub_source_date_iso: '2025-12-19'
    at_pub_source_date_label: ICLR 2025
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
    value_gap_source_is_current_paper: true
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
    feature_source_evidence: Baseline results from Miglior et al. 2025.
    table_ref: Table 1
    source_ref: miglior2025can
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.151
    at_pub_std: 0.038
    at_pub_source_arxiv: '2512.17762'
    at_pub_source_title: ECHO Benchmark
    at_pub_source_date_iso: '2025-12-19'
    at_pub_source_date_label: ICLR 2025
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
    value_gap_source_is_current_paper: true
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
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: Baseline results from Miglior et al. 2025.
    table_ref: Table 1
    source_ref: miglior2025can
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.243
    at_pub_std: 0.047
    at_pub_source_arxiv: '2512.17762'
    at_pub_source_title: ECHO Benchmark
    at_pub_source_date_iso: '2025-12-19'
    at_pub_source_date_label: ICLR 2025
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
    value_gap_source_is_current_paper: true
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
    feature_source_evidence: Baseline results from Miglior et al. 2025.
    table_ref: Table 1
    source_ref: miglior2025can
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 1.323
    at_pub_std: 0.485
    at_pub_source_arxiv: '2512.17762'
    at_pub_source_title: ECHO Benchmark
    at_pub_source_date_iso: '2025-12-19'
    at_pub_source_date_label: ICLR 2025
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
    value_gap_source_is_current_paper: true
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
  - model: GIN/GINE
    model_key: gin/gine
    model_plain: GIN/GINE
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
    feature_source_evidence: Baseline results from Miglior et al. 2025.
    table_ref: Table 1
    source_ref: miglior2025can
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
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
    true_value: 1.63
    true_std: 0.161
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.63
    sort_std: 0.161
    global_rank: 9
    paper_rank: 9
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
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2512.17762'
    title: ECHO Benchmark
    date: Dec 19, 2025
    date_display: Dec 2025
    date_iso: '2025-12-19'
    venue: Accepted at ICLR 2026 ( https://openreview.net/forum?id=DgkWFPZMPp )
    codebase_url: https://github.com/Graph-ECHO-Benchmark/ECHO
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 10
    sort_value: 1.63
    sort_std: 0.161
    comparison_type: global_top
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
    feature_source_evidence: Baseline results from Miglior et al. 2025.
    table_ref: Table 1
    source_ref: miglior2025can
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.005
    at_pub_std: 0.093
    at_pub_source_arxiv: '2512.17762'
    at_pub_source_title: ECHO Benchmark
    at_pub_source_date_iso: '2025-12-19'
    at_pub_source_date_label: ICLR 2025
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
    value_gap_source_is_current_paper: true
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
    feature_source_evidence: Baseline results from Miglior et al. 2025.
    table_ref: Table 1
    source_ref: miglior2025can
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.102
    at_pub_std: 0.094
    at_pub_source_arxiv: '2512.17762'
    at_pub_source_title: ECHO Benchmark
    at_pub_source_date_iso: '2025-12-19'
    at_pub_source_date_label: ICLR 2025
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
    value_gap_source_is_current_paper: true
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
    feature_source_evidence: Baseline results from Miglior et al. 2025.
    table_ref: Table 1
    source_ref: miglior2025can
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: ECHO-Synth tasks (sssp, ecc, diam) evaluated on standard split.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.969
    at_pub_std: 0.189
    at_pub_source_arxiv: '2512.17762'
    at_pub_source_title: ECHO Benchmark
    at_pub_source_date_iso: '2025-12-19'
    at_pub_source_date_label: ICLR 2025
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
    value_gap_source_is_current_paper: true
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
- &id002
  dataset: LRIM
  rows:
  - model: GPS-RWSE
    model_key: gps-rwse
    model_plain: GPS-RWSE
    value: -4.345
    std: 0.065
    metric: log-MSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_display: May 2026
    date_iso: '2026-05-12'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: -4.345
    sort_std: 0.065
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS-Base
    model_key: gps-base
    model_plain: GPS-Base
    value: -4.211
    std: 0.155
    paper_value: -4.211
    paper_std: 0.155
    metric: log-MSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: Standard Graph Transformer baseline.
    table_ref: Table 1
    source_ref: mathys2026lrim
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_regression
    protocol_decision: standard
    protocol_note: Evaluated on the 16x16 lattice (LRIM-16-hard) using the canonical
      log-MSE metric.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: -4.34
    at_pub_std: 0.101
    at_pub_source_arxiv: '2605.12358'
    at_pub_source_title: From Message-Passing to Linearized Graph Sequence Models
    at_pub_source_date_iso: '2026-05-12'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-12'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.12899999999999956
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: false
    true_value: -4.34
    true_std: 0.101
    value_gap_source_arxiv: '2605.12358'
    value_gap_source_title: From Message-Passing to Linearized Graph Sequence Models
    value_gap_source_is_current_paper: false
    value_gap: 0.12899999999999956
    has_value_note: false
    value_note: ''
    sort_value: -4.34
    sort_std: 0.101
    global_rank: 2
    paper_rank: 4
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS-LapPE
    model_key: gps-lappe
    model_plain: GPS-LapPE
    value: -4.334
    std: 0.065
    paper_value: -4.334
    paper_std: 0.065
    metric: log-MSE
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
    feature_source_evidence: LapPE is a positional encoding applied to the graph features.
    table_ref: Table 1
    source_ref: mathys2026lrim
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_regression
    protocol_decision: standard
    protocol_note: Evaluated on the 16x16 lattice (LRIM-16-hard) using the canonical
      log-MSE metric.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
    at_pub_value: -4.248
    at_pub_std: 0.11
    at_pub_source_arxiv: '2605.12358'
    at_pub_source_title: From Message-Passing to Linearized Graph Sequence Models
    at_pub_source_date_iso: '2026-05-12'
    at_pub_source_date_label: '2026'
    value_gap_source_date_iso: '2026-05-18'
    value_gap_source_date_label: '2026'
    gap_vs_at_pub: 0.08599999999999941
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: true
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: -4.334
    true_std: 0.065
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -4.334
    sort_std: 0.065
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GHR-GatedGCN
    model_key: ghr-gatedgcn
    model_plain: GHR-GatedGCN
    value: -4.195
    std: 0.061
    paper_value: -4.195
    paper_std: 0.061
    metric: log-MSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: The model uses GatedGCN as the message-passing operator
      on the original graph features.
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: node_regression
    protocol_decision: standard
    protocol_note: Evaluated on the 16x16 lattice (LRIM-16-hard) using the canonical
      log-MSE metric.
    date: May 18, 2026
    date_display: May 2026
    date_iso: '2026-05-18'
    published_venue: ''
    published_conference: ''
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
    true_value: -4.195
    true_std: 0.061
    value_gap_source_arxiv: '2605.18387'
    value_gap_source_title: Graph Hierarchical Recurrence for Long-Range Generalization
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: -4.195
    sort_std: 0.061
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
  - model: GatedGCN
    model_key: gatedgcn
    model_plain: GatedGCN
    value: -3.919
    std: 0.223
    metric: log-MSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_display: May 2026
    date_iso: '2026-05-12'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 6
    sort_value: -3.919
    sort_std: 0.223
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GIN
    model_key: gin
    model_plain: GIN
    value: -2.406
    std: 0.148
    metric: log-MSE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2605.12358'
    title: From Message-Passing to Linearized Graph Sequence Models
    date: May 12, 2026
    date_display: May 2026
    date_iso: '2026-05-12'
    venue: null
    codebase_url: ''
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 8
    sort_value: -2.406
    sort_std: 0.148
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  rank_metric: log-MSE
  higher_is_better: false
  experiment_scope: node-level
  dataset_primary_metric: log-MSE
  paper_metrics:
  - log-MSE
  metric: log-MSE
  uses_non_primary_metric: false
  paper_has_primary_metric: true
results_grouped:
- benchmark: ECHO Benchmark
  datasets:
  - *id001
- benchmark: LRIM Graph Benchmark
  datasets:
  - *id002
datasets_by_scope:
- scope: node-level
  label: Node-level
  benchmarks:
  - benchmark: LRIM Graph Benchmark
    benchmark_slug: lrim-graph-benchmark
    datasets:
    - dataset: LRIM
      dataset_slug: lrim
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: ECHO Benchmark
    benchmark_slug: echo-benchmark
    datasets:
    - dataset: ECHO-Synth
      dataset_slug: echo-synth
single_proposed_model: GHR
main_figure: /figures/2605.18387/main_figure.jpegoptim.jpg
---

