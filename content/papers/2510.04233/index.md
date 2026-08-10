---
title: 'PAINET: A Principled Efficient Transformer for 3D Dynamics Modeling'
arxiv_id: '2510.04233'
source_url: ''
authors:
- name: Kai Yang
  orcid: null
  s2_author_id: '2321352062'
  s2_url: null
- name: Yuqi Huang
  orcid: null
  s2_author_id: '2320344314'
  s2_url: null
- name: J.-Q. Tao
  orcid: null
  s2_author_id: '2164463389'
  s2_url: null
- name: Wanyu Wang
  orcid: null
  s2_author_id: '2211473272'
  s2_url: null
- name: Qitian Wu
  orcid: null
  s2_author_id: '51171144'
  s2_url: null
published_date: Oct 5, 2025
published_date_iso: '2025-10-05'
published_venue: ICLR 2025
published_conference: ICLR 2025
published_conference_short: ICLR
published_conference_slug: iclr
abstract: 'Modeling 3D dynamics is a fundamental problem in multi-body systems across
  scientific and engineering domains and has important practical implications in object
  trajectory prediction and simulation. While recent GNN-based approaches have achieved
  strong performance by enforcing geometric symmetries, encoding high-order features
  or incorporating neural-ODE mechanics, they typically depend on explicitly observed
  structures and inherently fail to capture the unobserved interactions that are crucial
  to complex physical behaviors and dynamics mechanism. In this paper, we propose
  PAINET, a principled $SE(3)$-equivariant transformer for learning all-pair interactions
  in multi-body systems. The model comprises: (1) a novel physics-inspired attention
  network derived from the minimization trajectory of an energy function, and (2)
  a parallel decoder that preserves equivariance while enabling efficient inference.
  Empirical results on diverse real-world benchmarks, including human motion capture,
  molecular dynamics, and large-scale protein simulations, show that PAINET consistently
  outperforms recently proposed models, yielding 4.7\'
codebase_url: https://github.com/Icarus1411/PAINET
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- PAINET
mrr: 0.1
adjusted_mrr: 0.0333
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
  is_multi_metric: true
  rows:
  - model: QHNet
    model_key: qhnet
    model_plain: QHNet
    metric_values:
    - 1.036e-05
    - null
    metric_stds:
    - null
    - null
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
    published_venue: ''
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    is_global_top: true
    global_rank: 1
    is_best: true
    sort_value: 1.036e-05
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
  - model: QHNetV2
    model_key: qhnetv2
    model_plain: QHNetV2
    metric_values:
    - 1.038e-05
    - null
    metric_stds:
    - null
    - null
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
    published_venue: ''
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    is_global_top: true
    global_rank: 2
    is_best: false
    sort_value: 1.038e-05
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
  - model: PhiSNet
    model_key: phisnet
    model_plain: PhiSNet
    metric_values:
    - 1.759e-05
    - null
    metric_stds:
    - null
    - null
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
    published_venue: ''
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    codebase_url: https://github.com/divelab/AIRS
    uses_external_data: false
    is_global_top: true
    global_rank: 3
    is_best: false
    sort_value: 1.759e-05
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
  - model: PAINET
    model_key: painet
    model_plain: PAINET
    metric_values:
    - 0.00324
    - 0.00183
    metric_stds:
    - 0.000119
    - 8.0e-06
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    sort_value: 0.00324
    sort_std: 0.000119
    true_value: 0.00324
    true_std: 0.000119
    paper_value: 0.00324
    paper_std: 0.000119
    has_value_gap: false
    has_value_note: false
    value_gap: null
    value_gap_source_arxiv: '2510.04233'
    value_gap_source_title: 'PAINET: A Principled Efficient Transformer for 3D Dynamics
      Modeling'
    value_note: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-05'
    value_gap_source_date_label: ICLR 2025
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
    published_venue: ICLR 2025
    date: Oct 5, 2025
    date_display: Oct 2025
    date_iso: '2025-10-05'
    codebase_url: ''
    uses_external_data: 0
    input_feature_source: raw_features
    feature_source_evidence: ''
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
    global_rank: 10
  metrics:
  - MAE
  - RMSD
  primary_metric: MAE
  rank_metric: MAE
  higher_is_better: false
  experiment_scope: graph-level
  dataset_primary_metric: MAE
  paper_metrics:
  - MAE
  - RMSD
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
single_proposed_model: PAINET
main_figure: /figures/2510.04233/main_figure.jpegoptim.jpg
---

