---
title: 'SpookyNet: Learning force fields with electronic degrees of freedom and nonlocal
  effects'
arxiv_id: '2105.00304'
source_url: ''
authors:
- name: Oliver T. Unke
  orcid: null
  s2_author_id: '9914431'
  s2_url: null
- name: Stefan Chmiela
  orcid: null
  s2_author_id: '7631063'
  s2_url: null
- name: Michael Gastegger
  orcid: null
  s2_author_id: '5742764'
  s2_url: null
- name: Kristof T. Sch\"utt
  orcid: null
  s2_author_id: '33075217'
  s2_url: null
- name: Huziel E.\ Sauceda
  orcid: null
  s2_author_id: '10667063'
  s2_url: null
- name: Klaus-Robert M\"uller
  orcid: null
  s2_author_id: '145034054'
  s2_url: null
published_date: May 1, 2021
published_date_iso: '2021-05-01'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: Machine-learned force fields combine the accuracy of ab initio methods with
  the efficiency of conventional force fields. However, current machine-learned force
  fields typically ignore electronic degrees of freedom, such as the total charge
  or spin state, and assume chemical locality, which is problematic when molecules
  have inconsistent electronic states, or when nonlocal effects play a significant
  role. This work introduces SpookyNet, a deep neural network for constructing machine-learned
  force fields with explicit treatment of electronic degrees of freedom and nonlocality,
  modeled via self-attention in a transformer architecture. Chemically meaningful
  inductive biases and analytical corrections built into the network architecture
  allow it to properly model physical limits. SpookyNet improves upon the current
  state-of-the-art (or achieves similar performance) on popular quantum chemistry
  data sets. Notably, it is able to generalize across chemical and conformational
  space and can leverage the learned chemical insights, e.g. by predicting unknown
  spin states, thus helping to close a further important remaining gap for today’s
  machine learning models in quantum chemistry. Current machine-learned force fields
  typically ignore electronic degrees of freedom. SpookyNet is a deep neural network
  that explicitly treats electronic degrees of freedom, closing an important remaining
  gap for models in quantum chemistry.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SpookyNet
mrr: 0.0196
adjusted_mrr: 0.0065
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
    source_ref: schutt2021equivariant
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin energy prediction
    date: May 1, 2021
    date_display: May 2021
    date_iso: '2021-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.7
    at_pub_std: null
    at_pub_source_arxiv: '2101.03164'
    at_pub_source_title: E(3)-Equivariant Graph Neural Networks for Data-Efficient
      and Accurate Interatomic Potentials
    at_pub_source_date_iso: '2021-01-08'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-06-15'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 2.5410000000000004
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
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
    paper_rank: 96
    rank_delta: 74
    rank_delta_abs: 74
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: E(3)-Equivariant Graph Neural Networks for Data-Efficient
      and Accurate Interatomic Potentials
    comparison_source_arxiv: '2101.03164'
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
    source_ref: unke2019physnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin energy prediction
    date: May 1, 2021
    date_display: May 2021
    date_iso: '2021-05-01'
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
    paper_rank: 99
    rank_delta: 70
    rank_delta_abs: 70
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
    source_ref: schutt2018schnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin energy prediction
    date: May 1, 2021
    date_display: May 2021
    date_iso: '2021-05-01'
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
    paper_rank: 107
    rank_delta: 61
    rank_delta_abs: 61
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    comparison_source_arxiv: '1902.08408'
    is_best: false
    is_std_outlier: false
  - model: SpookyNet
    model_key: spookynet
    model_plain: SpookyNet
    value: 0.052
    std: 0.001
    paper_value: 0.052
    paper_std: 0.001
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
    protocol_note: Ethanol energy prediction; averaged over ten random splits
    date: May 1, 2021
    date_display: May 2021
    date_iso: '2021-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: 2.3
    at_pub_std: null
    at_pub_source_arxiv: '2101.03164'
    at_pub_source_title: E(3)-Equivariant Graph Neural Networks for Data-Efficient
      and Accurate Interatomic Potentials
    at_pub_source_date_iso: '2021-01-08'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2022-05-28'
    value_gap_source_date_label: NeurIPS 2022
    gap_vs_at_pub: 2.2479999999999998
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.052
    true_std: null
    value_gap_source_arxiv: '2205.14276'
    value_gap_source_title: 'So3krates: Equivariant attention for interactions on
      arbitrary length-scales in molecular systems'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.052
    sort_std: null
    global_rank: 51
    paper_rank: 51
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
    source_ref: chmiela2019sgdml
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin energy prediction
    date: May 1, 2021
    date_display: May 2021
    date_iso: '2021-05-01'
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
    global_rank: 61
    paper_rank: 98
    rank_delta: 37
    rank_delta_abs: 37
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
    source_ref: christensen2020fchl
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Aspirin energy prediction
    date: May 1, 2021
    date_display: May 2021
    date_iso: '2021-05-01'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.182
    sort_std: null
    global_rank: 98
    paper_rank: 98
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
single_proposed_model: SpookyNet
main_figure: /figures/2105.00304/main_figure.jpegoptim.jpg
---

