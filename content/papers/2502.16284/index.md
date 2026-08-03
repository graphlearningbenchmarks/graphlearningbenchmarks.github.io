---
title: 'MolSpectra: Pre-training 3D Molecular Representation with Multi-modal Energy
  Spectra'
arxiv_id: '2502.16284'
source_url: ''
authors:
- name: Liang Wang
  orcid: null
  s2_author_id: '2258184369'
  s2_url: null
- name: Shaozhen Liu
  orcid: null
  s2_author_id: '2329233363'
  s2_url: null
- name: Yu Rong
  orcid: null
  s2_author_id: '2345187236'
  s2_url: null
- name: Deli Zhao
  orcid: null
  s2_author_id: '2344957479'
  s2_url: null
- name: Q. Liu
  orcid: null
  s2_author_id: '48873756'
  s2_url: null
- name: Shu Wu
  orcid: null
  s2_author_id: '50425438'
  s2_url: null
published_date: Feb 22, 2025
published_date_iso: '2025-02-22'
published_venue: ICLR 2025
published_conference: ICLR 2025
published_conference_short: ICLR
published_conference_slug: iclr
abstract: Establishing the relationship between 3D structures and the energy states
  of molecular systems has proven to be a promising approach for learning 3D molecular
  representations. However, existing methods are limited to modeling the molecular
  energy states from classical mechanics. This limitation results in a significant
  oversight of quantum mechanical effects, such as quantized (discrete) energy level
  structures, which offer a more accurate estimation of molecular energy and can be
  experimentally measured through energy spectra. In this paper, we propose to utilize
  the energy spectra to enhance the pre-training of 3D molecular representations (MolSpectra),
  thereby infusing the knowledge of quantum mechanics into the molecular representations.
  Specifically, we propose SpecFormer, a multi-spectrum encoder for encoding molecular
  spectra via masked patch reconstruction. By further aligning outputs from the 3D
  encoder and spectrum encoder using a contrastive objective, we enhance the 3D encoder's
  understanding of molecules. Evaluations on public benchmarks reveal that our pre-trained
  representations surpass existing methods in predicting molecular properties and
  modeling dynamics. 1
codebase_url: https://github.com/AzureLeon1/MolSpectra
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MolSpectra
mrr: 0.0385
adjusted_mrr: 0.0128
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
  - model: TorchMD-Net
    model_key: torchmd-net
    model_plain: TorchMD-Net
    value: 0.059
    std: null
    paper_value: 0.059
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
    protocol_note: Force prediction on MD17 molecules
    date: Feb 22, 2025
    date_display: Feb 2025
    date_iso: '2025-02-22'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 2.3
    at_pub_std: null
    at_pub_source_arxiv: '2502.08209'
    at_pub_source_title: Equivariant Masked position prediction for efficient molecular
      representation
    at_pub_source_date_iso: '2025-02-12'
    at_pub_source_date_label: ICLR 2025
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 2.2409999999999997
    worse_than_at_pub: false
    surpassed_since_pub: true
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: true
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.039
    true_std: null
    value_gap_source_arxiv: '2510.16780'
    value_gap_source_title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective
      Re-mask Decoding'
    value_gap_source_is_current_paper: false
    value_gap: 0.019999999999999997
    has_value_note: false
    value_note: ''
    sort_value: 0.039
    sort_std: null
    global_rank: 16
    paper_rank: 33
    rank_delta: 17
    rank_delta_abs: 17
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: Equivariant Masked position prediction for efficient
      molecular representation
    comparison_source_arxiv: '2502.08209'
    is_best: false
    is_std_outlier: false
  - model: MolSpectra
    model_key: molspectra
    model_plain: MolSpectra
    value: 0.052
    std: null
    paper_value: 0.052
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: hybrid
    architecture_label: Hyb
    architecture_title: Hybrid MPNN + transformer
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: Force prediction on MD17 molecules; uses spectral pre-training
    date: Feb 22, 2025
    date_display: Feb 2025
    date_iso: '2025-02-22'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-02-22'
    value_gap_source_date_label: ICLR 2025
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.052
    true_std: null
    value_gap_source_arxiv: '2502.16284'
    value_gap_source_title: 'MolSpectra: Pre-training 3D Molecular Representation
      with Multi-modal Energy Spectra'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.052
    sort_std: null
    global_rank: 26
    paper_rank: 26
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Coord
    model_key: coord
    model_plain: Coord
    value: 0.053
    std: null
    paper_value: 0.053
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
    protocol_note: Force prediction on MD17 molecules
    date: Feb 22, 2025
    date_display: Feb 2025
    date_iso: '2025-02-22'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.0529
    at_pub_std: null
    at_pub_source_arxiv: '2311.02124'
    at_pub_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    at_pub_source_date_iso: '2023-11-03'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2023-11-03'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 9.999999999999593e-05
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0529
    true_std: null
    value_gap_source_arxiv: '2311.02124'
    value_gap_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    value_gap_source_is_current_paper: false
    value_gap: 9.999999999999593e-05
    has_value_note: false
    value_note: ''
    sort_value: 0.0529
    sort_std: null
    global_rank: 28
    paper_rank: 28
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    comparison_source_arxiv: '2311.02124'
    is_best: false
    is_std_outlier: false
  - model: DimeNet++
    model_key: dimenet++
    model_plain: DimeNet++
    value: 0.187
    std: null
    paper_value: 0.187
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
    protocol_note: Force prediction on MD17 molecules
    date: Feb 22, 2025
    date_display: Feb 2025
    date_iso: '2025-02-22'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.0061
    at_pub_std: null
    at_pub_source_arxiv: '2402.04836'
    at_pub_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    at_pub_source_date_iso: '2024-02-07'
    at_pub_source_date_label: ICLR 2024
    value_gap_source_date_iso: '2020-03-06'
    value_gap_source_date_label: ICLR 2020
    gap_vs_at_pub: 0.1809
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.064
    true_std: null
    value_gap_source_arxiv: '2003.03123'
    value_gap_source_title: Directional Message Passing for Molecular Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.123
    has_value_note: false
    value_note: ''
    sort_value: 0.064
    sort_std: null
    global_rank: 36
    paper_rank: 50
    rank_delta: 14
    rank_delta_abs: 14
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: On the Completeness of Invariant Geometric Deep Learning
      Models
    comparison_source_arxiv: '2402.04836'
    is_best: false
    is_std_outlier: false
  - model: PaiNN
    model_key: painn
    model_plain: PaiNN
    value: 0.077
    std: null
    paper_value: 0.077
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
    protocol_note: Force prediction on MD17 molecules
    date: Feb 22, 2025
    date_display: Feb 2025
    date_iso: '2025-02-22'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.01
    at_pub_std: null
    at_pub_source_arxiv: '2306.09375'
    at_pub_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    at_pub_source_date_iso: '2023-06-15'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-11-03'
    value_gap_source_date_label: ICLR 2023
    gap_vs_at_pub: 0.067
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.077
    true_std: null
    value_gap_source_arxiv: '2311.02124'
    value_gap_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.077
    sort_std: null
    global_rank: 39
    paper_rank: 39
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    comparison_source_arxiv: '2306.09375'
    is_best: false
    is_std_outlier: false
  - model: SchNet
    model_key: schnet
    model_plain: SchNet
    value: 0.31
    std: null
    paper_value: 0.31
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
    protocol_note: Force prediction on MD17 molecules
    date: Feb 22, 2025
    date_display: Feb 2025
    date_iso: '2025-02-22'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.05
    at_pub_std: null
    at_pub_source_arxiv: '1902.08408'
    at_pub_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    at_pub_source_date_iso: '2019-02-22'
    at_pub_source_date_label: '2019'
    value_gap_source_date_iso: '2017-12-17'
    value_gap_source_date_label: '2017'
    gap_vs_at_pub: 0.26
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.08
    true_std: null
    value_gap_source_arxiv: '1712.06113'
    value_gap_source_title: SchNet -- a deep learning architecture for molecules and
      materials
    value_gap_source_is_current_paper: false
    value_gap: 0.22999999999999998
    has_value_note: false
    value_note: ''
    sort_value: 0.08
    sort_std: null
    global_rank: 40
    paper_rank: 58
    rank_delta: 18
    rank_delta_abs: 18
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: 'PhysNet: A Neural Network for Predicting Energies, Forces,
      Dipole Moments and Partial Charges'
    comparison_source_arxiv: '1902.08408'
    is_best: false
    is_std_outlier: false
  - model: SE(3)-DDM
    model_key: se(3)-ddm
    model_plain: SE(3)-DDM
    value: 0.122
    std: null
    paper_value: 0.122
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
    protocol_note: Force prediction on MD17 molecules
    date: Feb 22, 2025
    date_display: Feb 2025
    date_iso: '2025-02-22'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.122
    at_pub_std: null
    at_pub_source_arxiv: '2311.02124'
    at_pub_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    at_pub_source_date_iso: '2023-11-03'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2024-05-15'
    value_gap_source_date_label: ICML 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.122
    true_std: null
    value_gap_source_arxiv: '2405.10343'
    value_gap_source_title: 'UniCorn: A Unified Contrastive Learning Approach for
      Multi-view Molecular Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.122
    sort_std: null
    global_rank: 44
    paper_rank: 44
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: SphereNet
    model_key: spherenet
    model_plain: SphereNet
    value: 0.155
    std: null
    paper_value: 0.155
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
    protocol_note: Force prediction on MD17 molecules
    date: Feb 22, 2025
    date_display: Feb 2025
    date_iso: '2025-02-22'
    published_venue: ICLR 2025
    published_conference: ICLR 2025
    at_pub_value: 0.052
    at_pub_std: null
    at_pub_source_arxiv: '2306.09375'
    at_pub_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    at_pub_source_date_iso: '2023-06-15'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-04-07'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.10300000000000001
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.008000000000000007
    has_value_note: false
    value_note: ''
    sort_value: 0.147
    sort_std: null
    global_rank: 49
    paper_rank: 49
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    comparison_source_arxiv: '2306.09375'
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
single_proposed_model: MolSpectra
---

