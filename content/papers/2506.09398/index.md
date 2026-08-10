---
title: Efficient Prediction of SO(3)-Equivariant Hamiltonian Matrices via SO(2) Local
  Frames
arxiv_id: '2506.09398'
source_url: ''
authors:
- name: Haiyang Yu
  orcid: null
  s2_author_id: '2321143504'
  s2_url: null
- name: Yu-Ching Lin
  orcid: null
  s2_author_id: '2107966079'
  s2_url: null
- name: Xuan Zhang
  orcid: null
  s2_author_id: '2293765617'
  s2_url: null
- name: Xiaofeng Qian
  orcid: null
  s2_author_id: '2268839992'
  s2_url: null
- name: Shuiwang Ji
  orcid: null
  s2_author_id: '2265639861'
  s2_url: null
published_date: Jun 11, 2025
published_date_iso: '2025-06-11'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: We consider the task of predicting Hamiltonian matrices to accelerate electronic
  structure calculations, which plays an important role in physics, chemistry, and
  materials science. Motivated by the inherent relationship between the off-diagonal
  blocks of the Hamiltonian matrix and the SO(2) local frame, we propose a novel and
  efficient network, called QHNetV2, that achieves global SO(3) equivariance without
  the costly SO(3) Clebsch-Gordan tensor products. This is achieved by introducing
  a set of new efficient and powerful SO(2)-equivariant operations and performing
  all off-diagonal feature updates and message passing within SO(2) local frames,
  thereby eliminating the need of SO(3) tensor products. Moreover, a continuous SO(2)
  tensor product is performed within the SO(2) local frame at each node to fuse node
  features, mimicking the symmetric contraction operation. Extensive experiments on
  the large QH9 and MD17 datasets demonstrate that our model achieves superior performance
  across a wide range of molecular structures and trajectories, highlighting its strong
  generalization capability. The proposed SO(2) operations on SO(2) local frames offer
  a promising direction for scalable and symmetry-aware learning of electronic structures.
  Our code will be released as part of the AIRS library https://github.com/divelab/AIRS.
codebase_url: https://github.com/divelab/AIRS
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- QHNetV2
mrr: 0.5
adjusted_mrr: 0.1667
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
    paper_value: 1.036e-05
    paper_std: null
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
    protocol_note: MAE on Hamiltonian H for Water molecule
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: 8.312e-05
    at_pub_std: null
    at_pub_source_arxiv: '2306.09549'
    at_pub_source_title: 'QH9: A Quantum Hamiltonian Prediction Benchmark for QM9
      Molecules'
    at_pub_source_date_iso: '2023-06-15'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2025-06-11'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 7.276e-05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.036e-05
    true_std: null
    value_gap_source_arxiv: '2506.09398'
    value_gap_source_title: Efficient Prediction of SO(3)-Equivariant Hamiltonian
      Matrices via SO(2) Local Frames
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.036e-05
    sort_std: null
    global_rank: 1
    paper_rank: 1
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'QH9: A Quantum Hamiltonian Prediction Benchmark for
      QM9 Molecules'
    comparison_source_arxiv: '2306.09549'
    is_best: true
    is_std_outlier: false
  - model: QHNetV2
    model_key: qhnetv2
    model_plain: QHNetV2
    value: 1.038e-05
    std: null
    paper_value: 1.038e-05
    paper_std: null
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
    protocol_note: MAE on Hamiltonian H for Uracil molecule
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-11'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.038e-05
    true_std: null
    value_gap_source_arxiv: '2506.09398'
    value_gap_source_title: Efficient Prediction of SO(3)-Equivariant Hamiltonian
      Matrices via SO(2) Local Frames
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.038e-05
    sort_std: null
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
  - model: PhiSNet
    model_key: phisnet
    model_plain: PhiSNet
    value: 1.759e-05
    std: null
    paper_value: 1.759e-05
    paper_std: null
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
    protocol_note: MAE on Hamiltonian H for Water molecule
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-11'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.759e-05
    true_std: null
    value_gap_source_arxiv: '2506.09398'
    value_gap_source_title: Efficient Prediction of SO(3)-Equivariant Hamiltonian
      Matrices via SO(2) Local Frames
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.759e-05
    sort_std: null
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
  - model: SPHNet
    model_key: sphnet
    model_plain: SPHNet
    value: 1.936e-05
    std: null
    paper_value: 1.936e-05
    paper_std: null
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
    protocol_note: MAE on Hamiltonian H for Uracil molecule
    date: Jun 11, 2025
    date_display: Jun 2025
    date_iso: '2025-06-11'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-06-11'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 1.936e-05
    true_std: null
    value_gap_source_arxiv: '2506.09398'
    value_gap_source_title: Efficient Prediction of SO(3)-Equivariant Hamiltonian
      Matrices via SO(2) Local Frames
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 1.936e-05
    sort_std: null
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
single_proposed_model: QHNetV2
main_figure: /figures/2506.09398/main_figure.jpegoptim.jpg
---

