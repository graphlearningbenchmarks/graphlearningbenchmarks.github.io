---
title: Spherical Message Passing for 3D Molecular Graphs
arxiv_id: '2102.05013'
source_url: ''
authors:
- name: Yi Liu
  orcid: null
  s2_author_id: '2153630672'
  s2_url: null
- name: Limei Wang
  orcid: null
  s2_author_id: '2109120459'
  s2_url: null
- name: Meng Liu
  orcid: null
  s2_author_id: '38813990'
  s2_url: null
- name: Xuan Zhang
  orcid: null
  s2_author_id: '2108232316'
  s2_url: null
- name: Bora Oztekin
  orcid: null
  s2_author_id: '1734808354'
  s2_url: null
- name: Shuiwang Ji
  orcid: null
  s2_author_id: '1743600'
  s2_url: null
published_date: Feb 9, 2021
published_date_iso: '2021-02-09'
published_venue: ICLR 2021
published_conference: ICLR 2021
published_conference_short: ICLR
published_conference_slug: iclr
abstract: We consider representation learning of 3D molecular graphs in which each
  atom is associated with a spatial position in 3D. This is an under-explored area
  of research, and a principled message passing framework is currently lacking. In
  this work, we conduct analyses in the spherical coordinate system (SCS) for the
  complete identification of 3D graph structures. Based on such observations, we propose
  the spherical message passing (SMP) as a novel and powerful scheme for 3D molecular
  learning. SMP dramatically reduces training complexity, enabling it to perform efficiently
  on large-scale molecules. In addition, SMP is capable of distinguishing almost all
  molecular structures, and the uncovered cases may not exist in practice. Based on
  meaningful physically-based representations of 3D information, we further propose
  the SphereNet for 3D molecular learning. Experimental results demonstrate that the
  use of meaningful 3D information in SphereNet leads to significant performance improvements
  in prediction tasks. Our results also demonstrate the advantages of SphereNet in
  terms of capability, efficiency, and scalability. Our code is publicly available
  as part of the DIG library.
codebase_url: https://github.com/divelab/DIG
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- SphereNet
mrr: 0.0147
adjusted_mrr: 0.0049
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
  - model: NequIP
    model_key: nequip
    model_plain: NequIP
    value: 0.353
    std: null
    paper_value: 0.353
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
    table_ref: Table 2
    source_ref: batzner2021se
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE of forces on MD17 molecules with WoFE=100
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2024-02-07'
    value_gap_source_date_label: ICLR 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
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
    value_gap: 0.3
    has_value_note: false
    value_note: ''
    sort_value: 0.053
    sort_std: null
    global_rank: 34
    paper_rank: 79
    rank_delta: 45
    rank_delta_abs: 45
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: sGDML
    model_key: sgdml
    model_plain: sGDML
    value: 0.68
    std: null
    paper_value: 0.68
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
    table_ref: Table 2
    source_ref: chmiela2018towards
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE of forces on MD17 molecules with WoFE=100
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.06
    at_pub_std: null
    at_pub_source_arxiv: '2003.03123'
    at_pub_source_title: Directional Message Passing for Molecular Graphs
    at_pub_source_date_iso: '2020-03-06'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2020-03-06'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: 0.6200000000000001
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
    value_gap: 0.6200000000000001
    has_value_note: false
    value_note: ''
    sort_value: 0.06
    sort_std: null
    global_rank: 40
    paper_rank: 80
    rank_delta: 40
    rank_delta_abs: 40
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Directional Message Passing for Molecular Graphs
    comparison_source_arxiv: '2003.03123'
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 0.499
    std: null
    paper_value: 0.499
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
    table_ref: Table 2
    source_ref: klicpera_dimenet_2020
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE of forces on MD17 molecules with WoFE=100
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.064
    at_pub_std: null
    at_pub_source_arxiv: '2003.03123'
    at_pub_source_title: Directional Message Passing for Molecular Graphs
    at_pub_source_date_iso: '2020-03-06'
    at_pub_source_date_label: ICLR 2020
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 0.435
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
    value_gap: 0.435
    has_value_note: false
    value_note: ''
    sort_value: 0.064
    sort_std: null
    global_rank: 42
    paper_rank: 80
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Directional Message Passing for Molecular Graphs
    comparison_source_arxiv: '2003.03123'
    is_best: false
    is_std_outlier: false
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    value: 1.35
    std: null
    paper_value: 1.35
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
    table_ref: Table 2
    source_ref: schutt2017schnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE of forces on MD17 molecules with WoFE=100
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: 0.05
    at_pub_std: null
    at_pub_source_arxiv: '1902.08408'
    at_pub_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    at_pub_source_date_iso: '2019-02-22'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2024-06-19'
    value_gap_source_date_label: '2024'
    gap_vs_at_pub: 1.3
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.08
    true_std: null
    value_gap_source_arxiv: '2406.13265'
    value_gap_source_title: Molecule Graph Networks with Many-body Equivariant Interactions
    value_gap_source_is_current_paper: false
    value_gap: 1.27
    has_value_note: false
    value_note: ''
    sort_value: 0.08
    sort_std: null
    global_rank: 46
    paper_rank: 83
    rank_delta: 37
    rank_delta_abs: 37
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    comparison_source_arxiv: '1902.08408'
    is_best: false
    is_std_outlier: false
  - model: GemNet-T
    model_key: gemnet-t
    model_plain: GemNet-T
    value: 0.22
    std: null
    paper_value: 0.22
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
    table_ref: Table 2
    source_ref: klicpera2021gemnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE of forces on MD17 molecules with WoFE=100
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-09-27'
    value_gap_source_date_label: '2023'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.101
    true_std: null
    value_gap_source_arxiv: '2309.15718'
    value_gap_source_title: Geometry-enhanced pretraining on interatomic potentials
    value_gap_source_is_current_paper: false
    value_gap: 0.119
    has_value_note: false
    value_note: ''
    sort_value: 0.101
    sort_std: null
    global_rank: 54
    paper_rank: 71
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    value: 0.209
    std: null
    paper_value: 0.209
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
    table_ref: Table 2
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE of forces on MD17 molecules with WoFE=1000
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-04-07'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.147
    true_std: null
    value_gap_source_arxiv: '2304.04757'
    value_gap_source_title: A new perspective on building efficient and expressive
      3D equivariant graph neural networks
    value_gap_source_is_current_paper: false
    value_gap: 0.062
    has_value_note: false
    value_note: ''
    sort_value: 0.147
    sort_std: null
    global_rank: 68
    paper_rank: 70
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GemNet-Q
    model_key: gemnet-q
    model_plain: GemNet-Q
    value: 0.217
    std: null
    paper_value: 0.217
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
    table_ref: Table 2
    source_ref: klicpera2021gemnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MAE of forces on MD17 molecules with WoFE=100
    date: Feb 9, 2021
    date_display: Feb 2021
    date_iso: '2021-02-09'
    published_venue: ICLR 2021
    published_conference: ICLR 2021
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2021-02-09'
    value_gap_source_date_label: ICLR 2021
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.217
    true_std: null
    value_gap_source_arxiv: '2102.05013'
    value_gap_source_title: Spherical Message Passing for 3D Molecular Graphs
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.217
    sort_std: null
    global_rank: 71
    paper_rank: 71
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
single_proposed_model: SphereNet
main_figure: /figures/2102.05013/main_figure.jpegoptim.jpg
---

