---
title: 'Message Passing on the Edge: Towards Scalable and Expressive GNNs'
arxiv_id: '2510.13615'
source_url: ''
authors:
- name: P. Barcel'o
  orcid: null
  s2_author_id: '2385786481'
  s2_url: null
- name: Fabian Jogl
  orcid: null
  s2_author_id: '2091417275'
  s2_url: null
- name: A. Kozachinskiy
  orcid: null
  s2_author_id: '1699029'
  s2_url: null
- name: Matthias Lanzinger
  orcid: null
  s2_author_id: '2249532932'
  s2_url: null
- name: S. Neumann
  orcid: null
  s2_author_id: '48815534'
  s2_url: null
- name: Cristóbal Rojas
  orcid: null
  s2_author_id: '2282963745'
  s2_url: null
published_date: Oct 15, 2025
published_date_iso: '2025-10-15'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Graph neural networks (GNNs) are widely used in graph learning and most
  architectures propagate information by passing messages between vertices. In this
  work, we shift our attention to GNNs that perform message passing on edges and introduce
  EB-1WL, an edge-based color-refinement test, and a corresponding architecture, EB-GNN.
  Our EB-GNN architecture is inspired by the classic triangle-counting algorithm of
  Chiba and Nishizeki and passes messages along edges and triangles. Our contributions
  are as follows: (1) Theoretically, we show that EB-1WL is significantly more expressive
  than 1WL. We provide a complete logical characterization of EB-1WL in first-order
  logic, along with distinguishability results via homomorphism counting. To the best
  of our knowledge, EB-GNN has the strongest theoretical expressivity guarantees among
  edge-based message-passing GNNs in the literature. (2) Unlike many GNN architectures
  that are more expressive than 1WL, we prove that EB-1WL and EB-GNN admit near-linear
  time and memory usage on practical graph learning workloads. (3) We show in experiments
  that EB-GNN is a highly efficient general-purpose architecture: it substantially
  outperforms simple MPNNs and remains competitive with task-specialized state-of-the-art
  GNNs at substantially lower computational cost.'
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- EB-GNN
mrr: 0.0172
adjusted_mrr: 0.0057
mrr_dataset_count: 1
benchmark_categories:
- Quantum Chemistry
- GNNBenchmark
- Other Graph Benchmarks
benchmark_coverage:
- benchmark: Quantum Chemistry
  benchmark_slug: quantum-chemistry
  evaluated: 1
  total: 3
- benchmark: GNNBenchmark
  benchmark_slug: gnnbenchmark
  evaluated: 1
  total: 6
- benchmark: Other Graph Benchmarks
  benchmark_slug: other-graph-benchmarks
  evaluated: 1
  total: 4
task_categories:
- graph_classification
- graph_regression
experiment_scopes:
- graph-level
results:
- &id002
  dataset: CSL
  rows:
  - model: GatedGCN (Abs(EigVecs))
    model_key: ppgn
    model_plain: GatedGCN (Abs(EigVecs))
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GatedGCN (Abs(EigVecs))
    model_key: rw-agentnet
    model_plain: GatedGCN (Abs(EigVecs))
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: walk
    architecture_label: Walk
    architecture_title: Random-walk graph embedding
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GatedGCN (Abs(EigVecs))
    model_key: agentnet
    model_plain: GatedGCN (Abs(EigVecs))
    value: 1.0
    std: null
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: other_traditional
    architecture_label: Trad
    architecture_title: Traditional / classical method
    arxiv_id: '2407.01214'
    title: Revisiting Random Walks for Learning on Graphs
    date: Jul 1, 2024
    date_display: Jul 2024
    date_iso: '2024-07-01'
    venue: International Conference on Learning Representations
    codebase_url: https://github.com/jw9730/random-walk
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 1.0
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: "4-\ell-GIN"
    model_key: "4-\ell-gin"
    model_plain: "4-\ell-GIN"
    value: 0.6
    std: null
    paper_value: 0.6
    paper_std: null
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Expressivity task on synthetic CSL dataset
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.6
    true_std: null
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.6
    sort_std: null
    global_rank: 47
    paper_rank: 47
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EB-GNN
    model_key: eb-gnn
    model_plain: EB-GNN
    value: 0.2
    std: null
    paper_value: 0.2
    paper_std: null
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Expressivity task on synthetic CSL dataset
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2
    true_std: null
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2
    sort_std: null
    global_rank: 58
    paper_rank: 58
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPNN + C_3
    model_key: mpnn + c_3
    model_plain: MPNN + C_3
    value: 0.2
    std: null
    paper_value: 0.2
    paper_std: null
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Expressivity task on synthetic CSL dataset
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2
    true_std: null
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2
    sort_std: null
    global_rank: 56
    paper_rank: 56
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NC-GNN
    model_key: nc-gnn
    model_plain: NC-GNN
    value: 0.2
    std: null
    paper_value: 0.2
    paper_std: null
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Expressivity task on synthetic CSL dataset
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.2
    true_std: null
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.2
    sort_std: null
    global_rank: 57
    paper_rank: 57
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    value: 0.1
    std: null
    paper_value: 0.1
    paper_std: null
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Expressivity task on synthetic CSL dataset
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.1
    at_pub_std: null
    at_pub_source_arxiv: '2303.10576'
    at_pub_source_title: An Efficient Subgraph GNN with Provable Substructure Counting
      Power
    at_pub_source_date_iso: '2023-03-19'
    at_pub_source_date_label: KDD 2023
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.1
    true_std: null
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.1
    sort_std: null
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id003
  dataset: MalNet-Tiny
  rows:
  - model: EB-GNN
    model_key: dag+graphgps
    model_plain: EB-GNN
    value: 0.9345
    std: 0.0041
    metric: Accuracy
    higher_is_better: true
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    arxiv_id: '2210.13148'
    title: Transformers over Directed Acyclic Graphs
    date: Oct 24, 2022
    date_display: Oct 2022
    date_iso: '2022-10-24'
    venue: Neural Information Processing Systems
    codebase_url: ''
    uses_external_data: false
    input_feature_source: raw_features
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 0.9345
    sort_std: 0.0041
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: EB-GNN
    model_key: eb-gnn
    model_plain: EB-GNN
    value: 0.933
    std: 0.0066
    paper_value: 0.933
    paper_std: 0.0066
    metric: Accuracy
    higher_is_better: true
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard accuracy on MalNet-Tiny graph classification task.
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.933
    true_std: 0.0066
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.933
    sort_std: 0.0066
    global_rank: 2
    paper_rank: 2
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: HyMN
    model_key: hymn
    model_plain: HyMN
    value: 0.9284
    std: 0.0052
    paper_value: 0.9284
    paper_std: 0.0052
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
    source_ref: HyMN
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard accuracy on MalNet-Tiny graph classification task.
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9284
    true_std: 0.0052
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9284
    sort_std: 0.0052
    global_rank: 3
    paper_rank: 3
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: NC-GNN
    model_key: nc-gnn
    model_plain: NC-GNN
    value: 0.925
    std: 0.0056
    paper_value: 0.925
    paper_std: 0.0056
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard accuracy on MalNet-Tiny graph classification task.
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.925
    true_std: 0.0056
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.925
    sort_std: 0.0056
    global_rank: 5
    paper_rank: 5
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: GPS (Perf.)
    model_key: gps (perf.)
    model_plain: GPS (Perf.)
    value: 0.9214
    std: 0.0024
    paper_value: 0.9214
    paper_std: 0.0024
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard accuracy on MalNet-Tiny graph classification task.
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.9214
    true_std: 0.0024
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.9214
    sort_std: 0.0024
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
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    value: 0.911
    std: 0.0098
    paper_value: 0.911
    paper_std: 0.0098
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
    evaluation_task: graph_classification
    protocol_decision: standard
    protocol_note: Standard accuracy on MalNet-Tiny graph classification task.
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.911
    true_std: 0.0098
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.911
    sort_std: 0.0098
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
  rank_metric: Accuracy
  higher_is_better: true
  experiment_scope: graph-level
  dataset_primary_metric: Accuracy
  paper_metrics:
  - Accuracy
  metric: Accuracy
  uses_non_primary_metric: false
  paper_has_primary_metric: true
- &id001
  dataset: QM9
  is_multi_metric: true
  rows:
  - model: DimeNet++
    model_key: equiformer v2
    model_plain: DimeNet++
    metric_values:
    - 0.01
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.23086'
    title: Equivariant Spherical Transformer for Efficient Molecular Modeling
    published_venue: ''
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 0.01
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DimeNet++
    model_key: eqgat
    model_plain: DimeNet++
    metric_values:
    - 0.011
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: graph_transformer
    architecture_label: GT
    architecture_title: Graph transformer
    arxiv_id: '2505.23086'
    title: Equivariant Spherical Transformer for Efficient Molecular Modeling
    published_venue: ''
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 0.011
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: DimeNet++
    model_key: equiformer
    model_plain: DimeNet++
    metric_values:
    - 0.011
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2505.23086'
    title: Equivariant Spherical Transformer for Efficient Molecular Modeling
    published_venue: ''
    date: May 29, 2025
    date_display: May 2025
    date_iso: '2025-05-29'
    codebase_url: ''
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 0.011
    sort_std: null
    has_value_gap: false
    has_value_note: false
    paper_rank: null
    rank_delta: null
    rank_delta_abs: null
    value_note: ''
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_std_outlier: false
  - model: MPNN
    model_key: mpnn
    model_plain: MPNN
    metric_values:
    - null
    - 0.493
    - 0.78
    - 2.32
    - 2.23
    - 1.94
    - 0.27
    - 0.00321
    - 0.00355
    - 2.08
    - 0.00124
    - 34.1
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.03
    sort_std: null
    true_value: 0.03
    true_std: null
    paper_value: 0.493
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.46299999999999997
    value_gap_source_arxiv: '2110.01191'
    value_gap_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    value_note: ''
    at_pub_value: 0.03
    at_pub_std: null
    at_pub_source_arxiv: '2110.01191'
    at_pub_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous Molecular
      Graphs'
    at_pub_source_date_iso: '2021-10-04'
    at_pub_source_date_label: AAAI 2021
    value_gap_source_date_iso: '2021-10-04'
    value_gap_source_date_label: AAAI 2021
    gap_vs_at_pub: 0.46299999999999997
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'Molformer: Motif-based Transformer on 3D Heterogeneous
      Molecular Graphs'
    comparison_source_arxiv: '2110.01191'
    is_best: false
    is_std_outlier: false
    global_rank: 20
  - model: DTNN
    model_key: dtnn
    model_plain: DTNN
    metric_values:
    - null
    - 0.244
    - 0.95
    - 2.43
    - 2.43
    - 2.43
    - 2.43
    - 0.00388
    - 0.00512
    - 2.43
    - 0.00172
    - 17.0
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.244
    sort_std: null
    true_value: 0.244
    true_std: null
    paper_value: 0.244
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2305.04963'
    value_gap_source_title: 'From Relational Pooling to Subgraph GNNs: A Universal
      Framework for More Expressive Graph Neural Networks'
    value_note: ''
    at_pub_value: 0.244
    at_pub_std: null
    at_pub_source_arxiv: '2305.04963'
    at_pub_source_title: 'From Relational Pooling to Subgraph GNNs: A Universal Framework
      for More Expressive Graph Neural Networks'
    at_pub_source_date_iso: '2023-05-08'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2023-05-08'
    value_gap_source_date_label: ICML 2023
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
    published_venue: ''
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 44
  - model: EB-GNN
    model_key: eb-gnn
    model_plain: EB-GNN
    metric_values:
    - null
    - 0.315
    - 0.208
    - 0.063
    - 0.0564
    - 0.076
    - 0.092
    - 0.00218
    - 0.00217
    - 0.078
    - 0.0126
    - 13.83
    metric_stds:
    - null
    - 0.02
    - 0.03
    - 0.002
    - 0.0075
    - 0.006
    - 0.001
    - 0.0001
    - 0.0002
    - 0.008
    - 0.0001
    - 0.0012
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.315
    sort_std: 0.02
    true_value: 0.315
    true_std: 0.02
    paper_value: 0.315
    paper_std: 0.02
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
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
    published_venue: ''
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 46
  - model: DRFWL
    model_key: drfwl
    model_plain: DRFWL
    metric_values:
    - null
    - 0.346
    - 0.222
    - 0.156
    - 0.145
    - 0.156
    - 0.0901
    - 0.00226
    - 0.00225
    - 0.156
    - 0.017
    - 15.04
    metric_stds:
    - null
    - null
    - 0.25
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.346
    sort_std: null
    true_value: 0.346
    true_std: null
    paper_value: 0.346
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
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
    published_venue: ''
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 49
  - model: 5-ℓGIN
    model_key: 5-ℓgin
    model_plain: 5-ℓGIN
    metric_values:
    - null
    - 0.35
    - 0.217
    - 0.0418
    - 0.0352
    - 0.0118
    - 0.0702
    - 0.00205
    - 0.00216
    - 0.0418
    - 0.0127
    - 13.21
    metric_stds:
    - null
    - 0.11
    - 0.25
    - 0.052
    - 0.0304
    - 0.0015
    - 0.0024
    - null
    - 0.0004
    - 0.052
    - 0.0003
    - 0.0019
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.35
    sort_std: 0.11
    true_value: 0.35
    true_std: 0.11
    paper_value: 0.35
    paper_std: 0.11
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
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
    published_venue: ''
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 50
  - model: NestedGNN
    model_key: nestedgnn
    model_plain: NestedGNN
    metric_values:
    - null
    - 0.428
    - 0.29
    - 0.295
    - 0.305
    - 0.489
    - 0.174
    - 0.00265
    - 0.00297
    - 0.361
    - 0.002
    - 20.5
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.428
    sort_std: null
    true_value: 0.428
    true_std: null
    paper_value: 0.428
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
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
    published_venue: ''
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 70
  - model: I2-GNN
    model_key: i2-gnn
    model_plain: I2-GNN
    metric_values:
    - null
    - 0.428
    - 0.23
    - 0.211
    - 0.269
    - 0.261
    - 0.073
    - 0.00261
    - 0.00267
    - 0.206
    - 0.014
    - 18.64
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.428
    sort_std: null
    true_value: 0.428
    true_std: null
    paper_value: 0.428
    paper_std: null
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2510.13615'
    value_gap_source_title: 'Message Passing on the Edge: Towards Scalable and Expressive
      GNNs'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-15'
    value_gap_source_date_label: '2025'
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
    published_venue: ''
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 71
  - model: 1-2-3 GNN
    model_key: 1-2-3 gnn
    model_plain: 1-2-3 GNN
    metric_values:
    - null
    - 0.476
    - 0.27
    - 0.0427
    - 0.0419
    - 0.0469
    - 0.0944
    - 0.00337
    - 0.00351
    - 0.111
    - 0.0019
    - 22.9
    metric_stds:
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    - null
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.473
    sort_std: null
    true_value: 0.473
    true_std: null
    paper_value: 0.476
    paper_std: null
    has_value_gap: true
    has_value_note: false
    value_gap: 0.0030000000000000027
    value_gap_source_arxiv: '2111.06283'
    value_gap_source_title: 'DropGNN: Random Dropouts Increase the Expressiveness
      of Graph Neural Networks'
    value_note: ''
    at_pub_value: 0.473
    at_pub_std: null
    at_pub_source_arxiv: '2111.06283'
    at_pub_source_title: 'DropGNN: Random Dropouts Increase the Expressiveness of
      Graph Neural Networks'
    at_pub_source_date_iso: '2021-11-11'
    at_pub_source_date_label: NeurIPS 2021
    value_gap_source_date_iso: '2021-11-11'
    value_gap_source_date_label: NeurIPS 2021
    gap_vs_at_pub: 0.0030000000000000027
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    arxiv_id: ''
    title: ''
    published_venue: ''
    date: Oct 15, 2025
    date_display: Oct 2025
    date_iso: '2025-10-15'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    comparison_type: behind
    comparison_source_title: 'DropGNN: Random Dropouts Increase the Expressiveness
      of Graph Neural Networks'
    comparison_source_arxiv: '2111.06283'
    is_best: false
    is_std_outlier: false
    global_rank: 77
  metrics:
  - gap
  - mu
  - alpha
  - U0
  - H
  - G
  - Cv
  - HOMO
  - LUMO
  - U
  - zpve
  - R2
  primary_metric: gap
  rank_metric: mu
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: gap
  paper_metrics:
  - mu
  - alpha
  - U0
  - H
  - G
  - Cv
  - HOMO
  - LUMO
  - U
  - zpve
  - R2
  metric: mu
  uses_non_primary_metric: true
  paper_has_primary_metric: false
results_grouped:
- benchmark: Quantum Chemistry
  datasets:
  - *id001
- benchmark: GNNBenchmark
  datasets:
  - *id002
- benchmark: Other Graph Benchmarks
  datasets:
  - *id003
datasets_by_scope:
- scope: graph-level
  label: Graph-level
  benchmarks:
  - benchmark: Quantum Chemistry
    benchmark_slug: quantum-chemistry
    datasets:
    - dataset: QM9
      dataset_slug: qm9
  - benchmark: GNNBenchmark
    benchmark_slug: gnnbenchmark
    datasets:
    - dataset: CSL
      dataset_slug: csl
  - benchmark: Other Graph Benchmarks
    benchmark_slug: other-graph-benchmarks
    datasets:
    - dataset: MalNet-Tiny
      dataset_slug: malnet-tiny
single_proposed_model: EB-GNN
---

