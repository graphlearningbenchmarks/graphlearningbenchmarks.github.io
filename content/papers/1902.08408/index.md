---
title: 'PhysNet: A Neural Network for Predicting Energies, Forces, Dipole Moments
  and Partial Charges'
arxiv_id: '1902.08408'
source_url: ''
authors:
- name: Oliver T. Unke
  orcid: null
  s2_author_id: '9914431'
  s2_url: null
- name: M. Meuwly
  orcid: null
  s2_author_id: '2609300'
  s2_url: null
published_date: Feb 22, 2019
published_date_iso: '2019-02-22'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'In recent years, machine learning (ML) methods have become increasingly
  popular in computational chemistry. After being trained on appropriate ab initio
  reference data, these methods allow to accurately predict the properties of chemical
  systems, circumventing the need for explicitly solving the electronic Schr\"odinger
  equation. Because of their computational efficiency and scalability to large datasets,
  deep neural networks (DNNs) are a particularly promising ML algorithm for chemical
  applications. This work introduces, a DNN architecture designed for predicting energies,
  forces and dipole moments of chemical systems. \ achieves state-of-the-art performance
  on the QM9, MD17 and ISO17 benchmarks. Further, two new datasets are generated in
  order to probe the performance of ML models for describing chemical reactions, long-range
  interactions, and condensed phase systems. It is shown that explicitly including
  electrostatics in energy predictions is crucial for a qualitatively correct description
  of the asymptotic regions of a potential energy surface (PES). \ models trained
  on a systematically constructed set of small peptide fragments (at most eight heavy
  atoms) are able to generalize to considerably larger proteins like deca-alanine
  (Ala$_10$): The optimized geometry of helical Ala$_10$ predicted by \ is virtually
  identical to ab initio results ($RMSD=0.21$). By running unbiased molecular dynamics
  (MD) simulations of Ala$_10$ on the -PES in gas phase, it is found that instead
  of a helical structure, Ala$_10$ folds into a ``wreath-shaped'''' configuration,
  which is more stable than the helical form by $0.46$ kcal mol$^-1$ according to
  the reference ab initio calculations.'
codebase_url: https://github.com/MeuwlyGroup/PhysNet
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- PhysNet
- PhysNet-ens5
mrr: 0.0139
adjusted_mrr: 0.0046
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
  - model: SliDe
    model_key: qhnet
    model_plain: SliDe
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
  - model: SliDe
    model_key: qhnetv2
    model_plain: SliDe
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
  - model: SliDe
    model_key: phisnet
    model_plain: SliDe
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
  - model: PhysNet-ens5
    model_key: physnet-ens5
    model_plain: PhysNet-ens5
    value: 0.02
    std: null
    paper_value: 0.02
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 22, 2019
    date_display: Feb 2019
    date_iso: '2019-02-22'
    published_venue: ''
    published_conference: ''
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
    sort_value: 0.02
    sort_std: null
    global_rank: 14
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
  - model: DTNN
    model_key: dtnn
    model_plain: DTNN
    value: 0.04
    std: null
    paper_value: 0.04
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
    source_ref: schutt2017quantum
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 22, 2019
    date_display: Feb 2019
    date_iso: '2019-02-22'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.04
    at_pub_std: null
    at_pub_source_arxiv: '1712.06113'
    at_pub_source_title: SchNet -- a deep learning architecture for molecules and
      materials
    at_pub_source_date_iso: '2017-12-17'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2017-12-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.04
    true_std: null
    value_gap_source_arxiv: '1712.06113'
    value_gap_source_title: SchNet -- a deep learning architecture for molecules and
      materials
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.04
    sort_std: null
    global_rank: 21
    paper_rank: 21
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: HIP-NN
    model_key: hip-nn
    model_plain: HIP-NN
    value: 0.06
    std: null
    paper_value: 0.06
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
    source_ref: lubbers2018hierarchical
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 22, 2019
    date_display: Feb 2019
    date_iso: '2019-02-22'
    published_venue: ''
    published_conference: ''
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
    sort_value: 0.06
    sort_std: null
    global_rank: 41
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
  - model: GDML
    model_key: gdml
    model_plain: GDML
    value: 0.02
    std: null
    paper_value: 0.02
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: svm_kernel
    architecture_label: SVM
    architecture_title: SVM / kernel method
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: chmiela2017machine
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 22, 2019
    date_display: Feb 2019
    date_iso: '2019-02-22'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.07
    at_pub_std: null
    at_pub_source_arxiv: '1712.06113'
    at_pub_source_title: SchNet -- a deep learning architecture for molecules and
      materials
    at_pub_source_date_iso: '2017-12-17'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2017-12-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: 0.05
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.07
    true_std: null
    value_gap_source_arxiv: '1712.06113'
    value_gap_source_title: SchNet -- a deep learning architecture for molecules and
      materials
    value_gap_source_is_current_paper: false
    value_gap: 0.05
    has_value_note: false
    value_note: ''
    sort_value: 0.07
    sort_std: null
    global_rank: 43
    paper_rank: 14
    rank_delta: -29
    rank_delta_abs: 29
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: SchNet -- a deep learning architecture for molecules
      and materials
    comparison_source_arxiv: '1712.06113'
    is_best: false
    is_std_outlier: false
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    value: 0.05
    std: null
    paper_value: 0.05
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
    source_ref: schutt2017schnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 22, 2019
    date_display: Feb 2019
    date_iso: '2019-02-22'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.08
    at_pub_std: null
    at_pub_source_arxiv: '1712.06113'
    at_pub_source_title: SchNet -- a deep learning architecture for molecules and
      materials
    at_pub_source_date_iso: '2017-12-17'
    at_pub_source_date_label: '2017'
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.03
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.08
    true_std: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: false
    value_gap: 0.03
    has_value_note: false
    value_note: ''
    sort_value: 0.08
    sort_std: null
    global_rank: 46
    paper_rank: 28
    rank_delta: -18
    rank_delta_abs: 18
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: SchNet -- a deep learning architecture for molecules
      and materials
    comparison_source_arxiv: '1712.06113'
    is_best: false
    is_std_outlier: false
  - model: PhysNet
    model_key: physnet
    model_plain: PhysNet
    value: 0.03
    std: null
    paper_value: 0.03
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Feb 22, 2019
    date_display: Feb 2019
    date_iso: '2019-02-22'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-01-01'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.23
    true_std: null
    value_gap_source_arxiv: '2202.02541'
    value_gap_source_title: 'TorchMD-NET: Equivariant Transformers for Neural Network
      based Molecular Potentials'
    value_gap_source_is_current_paper: false
    value_gap: 0.2
    has_value_note: false
    value_note: ''
    sort_value: 0.23
    sort_std: null
    global_rank: 72
    paper_rank: 15
    rank_delta: -57
    rank_delta_abs: 57
    rank_delta_direction: better
    has_value_gap: true
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
main_figure: /figures/1902.08408/main_figure.jpegoptim.jpg
---

