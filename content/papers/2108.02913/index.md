---
title: 'NewtonNet: A Newtonian message passing network for deep learning of interatomic
  potentials and forces'
arxiv_id: '2108.02913'
source_url: ''
authors:
- name: Mojtaba Haghighatlari
  orcid: null
  s2_author_id: '88814594'
  s2_url: null
- name: Jie Li
  orcid: null
  s2_author_id: '2155869393'
  s2_url: null
- name: Xingyi Guan
  orcid: null
  s2_author_id: '1828814882'
  s2_url: null
- name: Oufan Zhang
  orcid: null
  s2_author_id: '2122909086'
  s2_url: null
- name: A. Das
  orcid: null
  s2_author_id: '2382730459'
  s2_url: null
- name: Christopher J. Stein
  orcid: null
  s2_author_id: '40396671'
  s2_url: null
- name: Farnaz Heidar‐Zadeh
  orcid: null
  s2_author_id: '103130132'
  s2_url: null
- name: Meili Liu
  orcid: null
  s2_author_id: '2004646077'
  s2_url: null
- name: M. Head‐Gordon
  orcid: null
  s2_author_id: '1401513374'
  s2_url: null
- name: Luke W. Bertels
  orcid: null
  s2_author_id: '35700705'
  s2_url: null
- name: Hongxia Hao
  orcid: null
  s2_author_id: '2147326378'
  s2_url: null
- name: I. Leven
  orcid: null
  s2_author_id: '113423567'
  s2_url: null
- name: T. Head‐Gordon
  orcid: null
  s2_author_id: '1396506620'
  s2_url: null
published_date: Aug 6, 2021
published_date_iso: '2021-08-06'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: We report a new deep learning message passing network that takes inspiration
  from Newton's equations of motion to learn interatomic potentials and forces. With
  the advantage of directional information from trainable latent force vectors, and
  physics-infused operators that are inspired by the Newtonian physics, the entire
  model remains rotationally equivariant, and many-body interactions are inferred
  by more interpretable physical features. We test NewtonNet on the prediction of
  several reactive and non-reactive high quality ab initio data sets including single
  small molecule dynamics, a large set of chemically diverse molecules, and methane
  and hydrogen combustion reactions, achieving state-of-the-art test performance on
  energies and forces with far greater data and computational efficiency than other
  deep learning models.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- NewtonNet
mrr: 0.0156
adjusted_mrr: 0.0052
mrr_dataset_count: 1
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
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    value: 0.159
    std: null
    paper_value: 0.159
    paper_std: null
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
    protocol_note: Averaged over four random splits for MD17 energy prediction
    date: Aug 6, 2021
    date_display: Aug 2021
    date_iso: '2021-08-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.159
    at_pub_std: null
    at_pub_source_arxiv: '2105.00304'
    at_pub_source_title: 'SpookyNet: Learning force fields with electronic degrees
      of freedom and nonlocal effects'
    at_pub_source_date_iso: '2021-05-01'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-06-15'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.01
    true_std: null
    value_gap_source_arxiv: '2306.09375'
    value_gap_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    value_gap_source_is_current_paper: false
    value_gap: 0.149
    has_value_note: false
    value_note: ''
    sort_value: 0.01
    sort_std: null
    global_rank: 22
    paper_rank: 98
    rank_delta: 76
    rank_delta_abs: 76
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PhysNet
    model_key: physnet
    model_plain: PhysNet
    value: 0.23
    std: null
    paper_value: 0.23
    paper_std: null
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
    protocol_note: Averaged over four random splits for MD17 energy prediction
    date: Aug 6, 2021
    date_display: Aug 2021
    date_iso: '2021-08-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.03
    at_pub_std: null
    at_pub_source_arxiv: '1902.08408'
    at_pub_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    at_pub_source_date_iso: '2019-02-22'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-02-22'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.2
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.03
    true_std: null
    value_gap_source_arxiv: '1902.08408'
    value_gap_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    value_gap_source_is_current_paper: false
    value_gap: 0.2
    has_value_note: false
    value_note: ''
    sort_value: 0.03
    sort_std: null
    global_rank: 29
    paper_rank: 101
    rank_delta: 72
    rank_delta_abs: 72
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    comparison_source_arxiv: '1902.08408'
    is_best: false
    is_std_outlier: false
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    value: 0.37
    std: null
    paper_value: 0.37
    paper_std: null
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
    protocol_note: Averaged over four random splits for MD17 energy prediction
    date: Aug 6, 2021
    date_display: Aug 2021
    date_iso: '2021-08-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.05
    at_pub_std: null
    at_pub_source_arxiv: '1902.08408'
    at_pub_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    at_pub_source_date_iso: '2019-02-22'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2019-02-22'
    value_gap_source_date_label: '2019'
    gap_vs_at_pub: 0.32
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.05
    true_std: null
    value_gap_source_arxiv: '1902.08408'
    value_gap_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    value_gap_source_is_current_paper: false
    value_gap: 0.32
    has_value_note: false
    value_note: ''
    sort_value: 0.05
    sort_std: null
    global_rank: 46
    paper_rank: 109
    rank_delta: 63
    rank_delta_abs: 63
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    comparison_source_arxiv: '1902.08408'
    is_best: false
    is_std_outlier: false
  - model: sGDML
    model_key: sgdml
    model_plain: sGDML
    value: 0.19
    std: null
    paper_value: 0.19
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Averaged over four random splits for MD17 energy prediction
    date: Aug 6, 2021
    date_display: Aug 2021
    date_iso: '2021-08-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.06
    at_pub_std: null
    at_pub_source_arxiv: '2003.03123'
    at_pub_source_title: Directional Message Passing for Molecular Graphs
    at_pub_source_date_iso: '2020-03-06'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2020-03-06'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: 0.13
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.06
    true_std: null
    value_gap_source_arxiv: '2003.03123'
    value_gap_source_title: Directional Message Passing for Molecular Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.13
    has_value_note: false
    value_note: ''
    sort_value: 0.06
    sort_std: null
    global_rank: 62
    paper_rank: 100
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Directional Message Passing for Molecular Graphs
    comparison_source_arxiv: '2003.03123'
    is_best: false
    is_std_outlier: false
  - model: NewtonNet
    model_key: newtonnet
    model_plain: NewtonNet
    value: 0.061
    std: 0.009
    paper_value: 0.061
    paper_std: 0.009
    metric: MAE
    higher_is_better: false
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
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Averaged over four random splits for MD17 energy prediction
    date: Aug 6, 2021
    date_display: Aug 2021
    date_iso: '2021-08-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.6
    at_pub_std: null
    at_pub_source_arxiv: '2101.03164'
    at_pub_source_title: E(3)-Equivariant Graph Neural Networks for Data-Efficient
      and Accurate Interatomic Potentials
    at_pub_source_date_iso: '2021-01-08'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 2.539
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.061
    true_std: null
    value_gap_source_arxiv: '2205.14276'
    value_gap_source_title: 'So3krates: Equivariant attention for interactions on
      arbitrary length-scales in molecular systems'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.061
    sort_std: null
    global_rank: 64
    paper_rank: 64
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: E(3)-Equivariant Graph Neural Networks for Data-Efficient
      and Accurate Interatomic Potentials
    comparison_source_arxiv: '2101.03164'
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 0.204
    std: null
    paper_value: 0.204
    paper_std: null
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
    protocol_note: Averaged over four random splits for MD17 energy prediction
    date: Aug 6, 2021
    date_display: Aug 2021
    date_iso: '2021-08-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.064
    at_pub_std: null
    at_pub_source_arxiv: '2003.03123'
    at_pub_source_title: Directional Message Passing for Molecular Graphs
    at_pub_source_date_iso: '2020-03-06'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.13999999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.064
    true_std: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: false
    value_gap: 0.13999999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.064
    sort_std: null
    global_rank: 65
    paper_rank: 100
    rank_delta: 35
    rank_delta_abs: 35
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Directional Message Passing for Molecular Graphs
    comparison_source_arxiv: '2003.03123'
    is_best: false
    is_std_outlier: false
  - model: FCHL19
    model_key: fchl19
    model_plain: FCHL19
    value: 0.182
    std: null
    paper_value: 0.182
    paper_std: null
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
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Averaged over four random splits for MD17 energy prediction
    date: Aug 6, 2021
    date_display: Aug 2021
    date_iso: '2021-08-06'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.182
    at_pub_std: null
    at_pub_source_arxiv: '2105.00304'
    at_pub_source_title: 'SpookyNet: Learning force fields with electronic degrees
      of freedom and nonlocal effects'
    at_pub_source_date_iso: '2021-05-01'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-08-06'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.182
    true_std: null
    value_gap_source_arxiv: '2108.02913'
    value_gap_source_title: 'NewtonNet: A Newtonian message passing network for deep
      learning of interatomic potentials and forces'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.182
    sort_std: null
    global_rank: 100
    paper_rank: 100
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
single_proposed_model: NewtonNet
main_figure: /figures/2108.02913/main_figure.jpegoptim.jpg
---

