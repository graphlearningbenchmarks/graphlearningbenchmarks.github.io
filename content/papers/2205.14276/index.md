---
title: 'So3krates: Equivariant attention for interactions on arbitrary length-scales
  in molecular systems'
arxiv_id: '2205.14276'
source_url: ''
authors:
- name: Thorben Frank
  orcid: null
  s2_author_id: '2107032645'
  s2_url: null
- name: Klaus-Robert Müller
  orcid: null
  s2_author_id: '2113612432'
  s2_url: null
- name: Oliver T. Unke
  orcid: null
  s2_author_id: '9914431'
  s2_url: null
published_date: May 28, 2022
published_date_iso: '2022-05-28'
published_venue: NeurIPS 2022
published_conference: NeurIPS 2022
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: The application of machine learning methods in quantum chemistry has enabled
  the study of numerous chemical phenomena, which are computationally intractable
  with traditional ab-initio methods. However, some quantum mechanical properties
  of molecules and materials depend on non-local electronic effects, which are often
  neglected due to the difficulty of modeling them efficiently. This work proposes
  a modified attention mechanism adapted to the underlying physics, which allows to
  recover the relevant non-local effects. Namely, we introduce spherical harmonic
  coordinates (SPHCs) to reflect higher-order geometric information for each atom
  in a molecule, enabling a non-local formulation of attention in the SPHC space.
  Our proposed model So3krates -- a self-attention based message passing neural network
  -- uncouples geometric information from atomic features, making them independently
  amenable to attention mechanisms. Thereby we construct spherical filters, which
  extend the concept of continuous filters in Euclidean space to SPHC space and serve
  as foundation for a spherical self-attention mechanism. We show that in contrast
  to other published methods, So3krates is able to describe non-local quantum mechanical
  effects over arbitrary length scales. Further, we find evidence that the inclusion
  of higher-order geometric correlations increases data efficiency and improves generalization.
  So3krates matches or exceeds state-of-the-art performance on popular benchmarks,
  notably, requiring a significantly lower number of parameters (0.25--0.4x) while
  at the same time giving a substantial speedup (6--14x for training and 2--11x for
  inference) compared to other models.
codebase_url: https://github.com/thorben-frank/mlff
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- So3krates
mrr: 0.0154
adjusted_mrr: 0.0051
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
  - model: GemNetQ
    model_key: gemnetq
    model_plain: GemNetQ
    value: 0.051
    std: null
    paper_value: 0.051
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 2.2
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: klicpera2021gemnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 28, 2022
    date_display: May 2022
    date_iso: '2022-05-28'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
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
    sort_value: 0.051
    sort_std: null
    global_rank: 30
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
  - model: SpookyNet
    model_key: spookynet
    model_plain: SpookyNet
    value: 0.052
    std: null
    paper_value: 0.052
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 3.0
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: unke2021spookynet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 28, 2022
    date_display: May 2022
    date_iso: '2022-05-28'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.052
    at_pub_std: 0.001
    at_pub_source_arxiv: '2105.00304'
    at_pub_source_title: 'SpookyNet: Learning force fields with electronic degrees
      of freedom and nonlocal effects'
    at_pub_source_date_iso: '2021-05-01'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2021-05-01'
    value_gap_source_date_label: '2021'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.052
    true_std: 0.001
    value_gap_source_arxiv: '2105.00304'
    value_gap_source_title: 'SpookyNet: Learning force fields with electronic degrees
      of freedom and nonlocal effects'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.052
    sort_std: 0.001
    global_rank: 32
    paper_rank: 32
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: NequIP
    model_key: nequip
    model_plain: NequIP
    value: 0.04
    std: null
    paper_value: 0.04
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 3.0
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: batzner2021se
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 28, 2022
    date_display: May 2022
    date_iso: '2022-05-28'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.348
    at_pub_std: null
    at_pub_source_arxiv: '2202.02541'
    at_pub_source_title: 'TorchMD-NET: Equivariant Transformers for Neural Network
      based Molecular Potentials'
    at_pub_source_date_iso: '2022-01-01'
    at_pub_source_date_label: '2022'
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: 0.308
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.053
    true_std: null
    value_gap_source_arxiv: '2402.04836'
    value_gap_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    value_gap_source_is_current_paper: false
    value_gap: 0.012999999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 34
    paper_rank: 22
    rank_delta: -12
    rank_delta_abs: 12
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'TorchMD-NET: Equivariant Transformers for Neural Network
      based Molecular Potentials'
    comparison_source_arxiv: '2202.02541'
    is_best: false
    is_std_outlier: false
  - model: NewtonNet
    model_key: newtonnet
    model_plain: NewtonNet
    value: 0.061
    std: null
    paper_value: 0.061
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.5
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: haghighatlari2021newtonnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 28, 2022
    date_display: May 2022
    date_iso: '2022-05-28'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.061
    at_pub_std: 0.009
    at_pub_source_arxiv: '2108.02913'
    at_pub_source_title: 'NewtonNet: A Newtonian message passing network for deep
      learning of interatomic potentials and forces'
    at_pub_source_date_iso: '2021-08-06'
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
    true_value: 0.061
    true_std: 0.009
    value_gap_source_arxiv: '2108.02913'
    value_gap_source_title: 'NewtonNet: A Newtonian message passing network for deep
      learning of interatomic potentials and forces'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.061
    sort_std: 0.009
    global_rank: 41
    paper_rank: 41
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 0.064
    std: null
    paper_value: 0.064
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 1.9
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: klicpera2020directional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 28, 2022
    date_display: May 2022
    date_iso: '2022-05-28'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.064
    at_pub_std: null
    at_pub_source_arxiv: '2003.03123'
    at_pub_source_title: Directional Message Passing for Molecular Graphs
    at_pub_source_date_iso: '2020-03-06'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.064
    true_std: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.064
    sort_std: null
    global_rank: 42
    paper_rank: 42
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    value: 0.063
    std: null
    paper_value: 0.063
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: true
    is_overridden: false
    override_reason: ''
    params_millions: 0.6
    architecture_type: gnn
    architecture_label: GNN
    architecture_title: Message-passing GNN
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: schutt2021equivariant
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: May 28, 2022
    date_display: May 2022
    date_iso: '2022-05-28'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: 0.159
    at_pub_std: null
    at_pub_source_arxiv: '2105.00304'
    at_pub_source_title: 'SpookyNet: Learning force fields with electronic degrees
      of freedom and nonlocal effects'
    at_pub_source_date_iso: '2021-05-01'
    at_pub_source_date_label: '2021'
    value_gap_source_date_iso: '2023-11-03'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.096
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.077
    true_std: null
    value_gap_source_arxiv: '2311.02124'
    value_gap_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    value_gap_source_is_current_paper: false
    value_gap: 0.013999999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.077
    sort_std: null
    global_rank: 45
    paper_rank: 42
    rank_delta: -3
    rank_delta_abs: 3
    rank_delta_direction: better
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'SpookyNet: Learning force fields with electronic degrees
      of freedom and nonlocal effects'
    comparison_source_arxiv: '2105.00304'
    is_best: false
    is_std_outlier: false
  - model: So3krates
    model_key: so3krates
    model_plain: So3krates
    value: 0.052
    std: null
    paper_value: 0.052
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: 0.7
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
    date: May 28, 2022
    date_display: May 2022
    date_iso: '2022-05-28'
    published_venue: NeurIPS 2022
    published_conference: NeurIPS 2022
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2022-10-29'
    value_gap_source_date_label: '2022'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: true
    today_delta_significant: true
    true_value: 0.139
    true_std: null
    value_gap_source_arxiv: '2210.16518'
    value_gap_source_title: 'ViSNet: an equivariant geometry-enhanced graph neural
      network with vector-scalar interactive message passing for molecules'
    value_gap_source_is_current_paper: false
    value_gap: 0.08700000000000002
    has_value_note: false
    value_note: ''
    sort_value: 0.139
    sort_std: null
    global_rank: 65
    paper_rank: 33
    rank_delta: -32
    rank_delta_abs: 32
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
single_proposed_model: So3krates
main_figure: /figures/2205.14276/main_figure.jpegoptim.jpg
---

