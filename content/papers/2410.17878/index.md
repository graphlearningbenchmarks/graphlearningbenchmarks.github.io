---
title: Relaxed Equivariance via Multitask Learning
arxiv_id: '2410.17878'
source_url: ''
authors:
- name: Ahmed A. A. Elhag
  orcid: null
  s2_author_id: '83724577'
  s2_url: null
- name: T. Konstantin Rusch
  orcid: null
  s2_author_id: '67164720'
  s2_url: null
- name: Francesco Di Giovanni
  orcid: null
  s2_author_id: '94290272'
  s2_url: null
- name: Michael M. Bronstein
  orcid: null
  s2_author_id: '2256977580'
  s2_url: null
published_date: Oct 23, 2024
published_date_iso: '2024-10-23'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Incorporating equivariance as an inductive bias into deep learning architectures
  to take advantage of the data symmetry has been successful in multiple applications,
  such as chemistry and dynamical systems. In particular, roto-translations are crucial
  for effectively modeling geometric graphs and molecules, where understanding the
  3D structures enhances generalization. However, strictly equivariant models often
  pose challenges due to their higher computational complexity. In this paper, we
  introduce REMUL, a training procedure that learns approximate equivariance for unconstrained
  networks via multitask learning. By formulating equivariance as a tunable objective
  alongside the primary task loss, REMUL offers a principled way to control the degree
  of approximate symmetry, relaxing the rigid constraints of traditional equivariant
  architectures. We show that unconstrained models (which do not build equivariance
  into the architecture) can learn approximate symmetries by minimizing an additional
  simple equivariance loss. This enables quantitative control over the trade-off between
  enforcing equivariance constraints and optimizing for task-specific performance.
  Our method achieves competitive performance compared to equivariant baselines while
  being significantly faster (up to 10$ $ at inference and 2.5$ $ at training), offering
  a practical and adaptable approach to leveraging symmetry in unconstrained architectures.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- REMUL-GNN
mrr: 0.0556
adjusted_mrr: 0.0185
mrr_dataset_count: 1
benchmark_categories:
- Quantum Chemistry
benchmark_coverage:
- benchmark: Quantum Chemistry
  benchmark_slug: quantum-chemistry
  evaluated: 1
  total: 1
task_categories:
- graph_regression
experiment_scopes:
- graph-level
results:
- &id001
  dataset: MD17
  rows:
  - model: QHNet
    model_key: qhnet
    model_plain: QHNet
    value: 1.036e-05
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    venue: arXiv.org
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 1
    sort_value: 1.036e-05
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: true
    is_std_outlier: false
  - model: QHNetV2
    model_key: qhnetv2
    model_plain: QHNetV2
    value: 1.038e-05
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    venue: arXiv.org
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 2
    sort_value: 1.038e-05
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PhiSNet
    model_key: phisnet
    model_plain: PhiSNet
    value: 1.759e-05
    std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    arxiv_id: '2506.09398'
    title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2)
      Local Frames
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    venue: arXiv.org
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    input_feature_source: null
    feature_source_evidence: ''
    is_global_top: true
    global_rank: 3
    sort_value: 1.759e-05
    sort_std: null
    comparison_type: global_top
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: EGNO
    model_key: egno
    model_plain: EGNO
    value: 0.0037
    std: 0.0001
    paper_value: 0.0037
    paper_std: 0.0001
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task; values scaled by 10^-2 in table
    date: Oct 23, 2024
    date_display: Oct 2024
    date_iso: '2024-10-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-23'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0037
    true_std: 0.0001
    value_gap_source_arxiv: '2410.17878'
    value_gap_source_title: Relaxed Equivariance via Multitask Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0037
    sort_std: 0.0001
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
  - model: HEGNN
    model_key: hegnn
    model_plain: HEGNN
    value: 0.0037
    std: 0.0002
    paper_value: 0.0037
    paper_std: 0.0002
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task; values scaled by 10^-2 in table
    date: Oct 23, 2024
    date_display: Oct 2024
    date_iso: '2024-10-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-23'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0037
    true_std: 0.0002
    value_gap_source_arxiv: '2410.17878'
    value_gap_source_title: Relaxed Equivariance via Multitask Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0037
    sort_std: 0.0002
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
  - model: GMN
    model_key: gmn
    model_plain: GMN
    value: 0.004
    std: 0.0001
    paper_value: 0.004
    paper_std: 0.0001
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task; values scaled by 10^-2 in table
    date: Oct 23, 2024
    date_display: Oct 2024
    date_iso: '2024-10-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.004
    at_pub_std: 0.0001
    at_pub_source_arxiv: '2410.11443'
    at_pub_source_title: Are High-Degree Representations Really Unnecessary in Equivariant
      Graph Neural Networks?
    at_pub_source_date_iso: '2024-10-15'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-10-23'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.004
    true_std: 0.0001
    value_gap_source_arxiv: '2410.17878'
    value_gap_source_title: Relaxed Equivariance via Multitask Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.004
    sort_std: 0.0001
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
  - model: EGNN
    model_key: egnn
    model_plain: EGNN
    value: 0.0047
    std: 0.0002
    paper_value: 0.0047
    paper_std: 0.0002
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task; values scaled by 10^-2 in table
    date: Oct 23, 2024
    date_display: Oct 2024
    date_iso: '2024-10-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.0047
    at_pub_std: 0.0002
    at_pub_source_arxiv: '2410.11443'
    at_pub_source_title: Are High-Degree Representations Really Unnecessary in Equivariant
      Graph Neural Networks?
    at_pub_source_date_iso: '2024-10-15'
    at_pub_source_date_label: NeurIPS 2024
    value_gap_source_date_iso: '2024-10-23'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0047
    true_std: 0.0002
    value_gap_source_arxiv: '2410.17878'
    value_gap_source_title: Relaxed Equivariance via Multitask Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0047
    sort_std: 0.0002
    global_rank: 15
    paper_rank: 15
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: REMUL-GNN
    model_key: remul-gnn
    model_plain: REMUL-GNN
    value: 0.0054
    std: 1.0e-05
    paper_value: 0.0054
    paper_std: 1.0e-05
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task; values scaled by 10^-2 in table
    date: Oct 23, 2024
    date_display: Oct 2024
    date_iso: '2024-10-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-23'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0054
    true_std: 1.0e-05
    value_gap_source_arxiv: '2410.17878'
    value_gap_source_title: Relaxed Equivariance via Multitask Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0054
    sort_std: 1.0e-05
    global_rank: 18
    paper_rank: 18
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GNN
    model_key: gnn
    model_plain: GNN
    value: 0.0054
    std: 1.0e-05
    paper_value: 0.0054
    paper_std: 1.0e-05
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task; values scaled by 10^-2 in table
    date: Oct 23, 2024
    date_display: Oct 2024
    date_iso: '2024-10-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-23'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0054
    true_std: 1.0e-05
    value_gap_source_arxiv: '2410.17878'
    value_gap_source_title: Relaxed Equivariance via Multitask Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0054
    sort_std: 1.0e-05
    global_rank: 17
    paper_rank: 17
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DA-GNN
    model_key: da-gnn
    model_plain: DA-GNN
    value: 0.0069
    std: 1.0e-05
    paper_value: 0.0069
    paper_std: 1.0e-05
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
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 regression task; values scaled by 10^-2 in table
    date: Oct 23, 2024
    date_display: Oct 2024
    date_iso: '2024-10-23'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-10-23'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.0069
    true_std: 1.0e-05
    value_gap_source_arxiv: '2410.17878'
    value_gap_source_title: Relaxed Equivariance via Multitask Learning
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.0069
    sort_std: 1.0e-05
    global_rank: 20
    paper_rank: 20
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
single_proposed_model: REMUL-GNN
main_figure: /figures/2410.17878/main_figure.jpegoptim.jpg
---

