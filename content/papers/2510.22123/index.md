---
title: Learning 3D Anisotropic Noise Distributions Improves Molecular Force Field
  Modeling
arxiv_id: '2510.22123'
source_url: ''
authors:
- name: Xixian Liu
  orcid: null
  s2_author_id: '2300334072'
  s2_url: null
- name: Rui Jiao
  orcid: null
  s2_author_id: '2112690595'
  s2_url: null
- name: Zhiyuan Liu
  orcid: null
  s2_author_id: '2387879817'
  s2_url: null
- name: Yurou Liu
  orcid: null
  s2_author_id: '2370873045'
  s2_url: null
- name: Yang Liu
  orcid: null
  s2_author_id: '2319229208'
  s2_url: null
- name: Ziheng Lu
  orcid: null
  s2_author_id: '2387887824'
  s2_url: null
- name: Wenbing Huang
  orcid: null
  s2_author_id: '2279853791'
  s2_url: null
- name: Yang Zhang
  orcid: null
  s2_author_id: '2388904212'
  s2_url: null
- name: Yixin Cao
  orcid: null
  s2_author_id: '2267012059'
  s2_url: null
published_date: Oct 25, 2025
published_date_iso: '2025-10-25'
published_venue: ''
published_conference: ''
published_conference_short: ''
published_conference_slug: ''
abstract: 'Coordinate denoising has emerged as a promising method for 3D molecular
  pre-training due to its theoretical connection to learning a molecular force field.
  However, existing denoising methods rely on oversimplified molecular dynamics that
  assume atomic motions to be isotropic and homoscedastic. To address these limitations,
  we propose a novel denoising framework AniDS: sotropic Variational Autoencoder for
  3D Molecular enoi ing. AniDS introduces a structure-aware anisotropic noise generator
  that can produce atom-specific, full covariance matrices for Gaussian noise distributions
  to better reflect directional and structural variability in molecular systems. These
  covariances are derived from pairwise atomic interactions as anisotropic corrections
  to an isotropic base. Our design ensures that the resulting covariance matrices
  are symmetric, positive semi-definite, and SO(3)-equivariant, while providing greater
  capacity to model complex molecular dynamics. Extensive experiments show that AniDS
  outperforms prior isotropic and homoscedastic denoising models and other leading
  methods on the MD17 and OC22 benchmarks, achieving average relative improvements
  of 8.9\'
codebase_url: https://github.com/ZeroKnighting/AniDS
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- AniDS
mrr: 0.0312
adjusted_mrr: 0.0104
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
    source_ref: painn
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 test set split
    date: Oct 25, 2025
    date_display: Oct 2025
    date_iso: '2025-10-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.01
    at_pub_std: null
    at_pub_source_arxiv: '2306.09375'
    at_pub_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    at_pub_source_date_iso: '2023-06-15'
    at_pub_source_date_label: NeurIPS 2023
    value_gap_source_date_iso: '2023-06-15'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: 0.067
    worse_than_at_pub: true
    surpassed_since_pub: false
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
    value_gap: 0.067
    has_value_note: false
    value_note: ''
    sort_value: 0.01
    sort_std: null
    global_rank: 22
    paper_rank: 68
    rank_delta: 46
    rank_delta_abs: 46
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Symmetry-Informed Geometric Representation for Molecules,
      Proteins, and Crystalline Materials
    comparison_source_arxiv: '2306.09375'
    is_best: false
    is_std_outlier: false
  - model: AniDS
    model_key: anids
    model_plain: AniDS
    value: 0.036
    std: null
    paper_value: 0.036
    paper_std: null
    metric: MAE
    higher_is_better: false
    is_baseline: false
    is_overridden: false
    override_reason: ''
    params_millions: null
    architecture_type: null
    architecture_label: null
    architecture_title: ''
    uses_external_data: 1
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 test set split; pre-trained on PCQM4Mv2
    date: Oct 25, 2025
    date_display: Oct 2025
    date_iso: '2025-10-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.036
    true_std: null
    value_gap_source_arxiv: '2510.22123'
    value_gap_source_title: Learning 3D Anisotropic Noise Distributions Improves Molecular
      Force Field Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.036
    sort_std: null
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
  - model: DeNS (Lmax=3)
    model_key: dens (lmax=3)
    model_plain: DeNS (Lmax=3)
    value: 0.037
    std: null
    paper_value: 0.037
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
    source_ref: liao2024generalizing
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 test set split
    date: Oct 25, 2025
    date_display: Oct 2025
    date_iso: '2025-10-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.037
    true_std: null
    value_gap_source_arxiv: '2510.22123'
    value_gap_source_title: Learning 3D Anisotropic Noise Distributions Improves Molecular
      Force Field Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.037
    sort_std: null
    global_rank: 33
    paper_rank: 33
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: TorchMD-Net
    model_key: torchmd-net
    model_plain: TorchMD-Net
    value: 0.061
    std: null
    paper_value: 0.061
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
    source_ref: torchmd
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 test set split
    date: Oct 25, 2025
    date_display: Oct 2025
    date_iso: '2025-10-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.039
    at_pub_std: null
    at_pub_source_arxiv: '2510.16780'
    at_pub_source_title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective
      Re-mask Decoding'
    at_pub_source_date_iso: '2025-10-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.022
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.039
    true_std: null
    value_gap_source_arxiv: '2510.16780'
    value_gap_source_title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective
      Re-mask Decoding'
    value_gap_source_is_current_paper: false
    value_gap: 0.022
    has_value_note: false
    value_note: ''
    sort_value: 0.039
    sort_std: null
    global_rank: 35
    paper_rank: 63
    rank_delta: 28
    rank_delta_abs: 28
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective
      Re-mask Decoding'
    comparison_source_arxiv: '2510.16780'
    is_best: false
    is_std_outlier: false
  - model: NequIP (Lmax=3)
    model_key: nequip (lmax=3)
    model_plain: NequIP (Lmax=3)
    value: 0.039
    std: null
    paper_value: 0.039
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
    source_ref: batzner20223
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 test set split
    date: Oct 25, 2025
    date_display: Oct 2025
    date_iso: '2025-10-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2025-10-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.039
    true_std: null
    value_gap_source_arxiv: '2510.22123'
    value_gap_source_title: Learning 3D Anisotropic Noise Distributions Improves Molecular
      Force Field Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.039
    sort_std: null
    global_rank: 38
    paper_rank: 38
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Frad
    model_key: frad
    model_plain: Frad
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
    source_ref: feng2023fractional
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 test set split
    date: Oct 25, 2025
    date_display: Oct 2025
    date_iso: '2025-10-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.0431
    at_pub_std: null
    at_pub_source_arxiv: '2510.16780'
    at_pub_source_title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective
      Re-mask Decoding'
    at_pub_source_date_iso: '2025-10-19'
    at_pub_source_date_label: '2025'
    value_gap_source_date_iso: '2025-10-19'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.009899999999999999
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.0431
    true_std: null
    value_gap_source_arxiv: '2510.16780'
    value_gap_source_title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective
      Re-mask Decoding'
    value_gap_source_is_current_paper: false
    value_gap: 0.009899999999999999
    has_value_note: false
    value_note: ''
    sort_value: 0.0431
    sort_std: null
    global_rank: 42
    paper_rank: 58
    rank_delta: 16
    rank_delta_abs: 16
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: '3D-GSRD: 3D Molecular Graph Auto-Encoder with Selective
      Re-mask Decoding'
    comparison_source_arxiv: '2510.16780'
    is_best: false
    is_std_outlier: false
  - model: SliDe
    model_key: slide
    model_plain: SliDe
    value: 0.048
    std: null
    paper_value: 0.048
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
    source_ref: ni2023sliced
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 test set split
    date: Oct 25, 2025
    date_display: Oct 2025
    date_iso: '2025-10-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.0483
    at_pub_std: null
    at_pub_source_arxiv: '2311.02124'
    at_pub_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    at_pub_source_date_iso: '2023-11-03'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2025-10-25'
    value_gap_source_date_label: '2025'
    gap_vs_at_pub: 0.00030000000000000165
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: true
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.048
    true_std: null
    value_gap_source_arxiv: '2510.22123'
    value_gap_source_title: Learning 3D Anisotropic Noise Distributions Improves Molecular
      Force Field Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.048
    sort_std: null
    global_rank: 45
    paper_rank: 45
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: true
    comparison_type: improved
    comparison_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    comparison_source_arxiv: '2311.02124'
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
    source_ref: schutt2018schnet
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 test set split
    date: Oct 25, 2025
    date_display: Oct 2025
    date_iso: '2025-10-25'
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
    gap_vs_at_pub: 0.26
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
    value_gap: 0.26
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
    source_ref: zaidi2022pre
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 test set split
    date: Oct 25, 2025
    date_display: Oct 2025
    date_iso: '2025-10-25'
    published_venue: ''
    published_conference: ''
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
    global_rank: 58
    paper_rank: 58
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
    source_ref: gasteiger2020fast
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 test set split
    date: Oct 25, 2025
    date_display: Oct 2025
    date_iso: '2025-10-25'
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
    gap_vs_at_pub: 0.123
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
    value_gap: 0.123
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
    source_ref: liu2023molecular
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: graph_regression
    protocol_decision: standard
    protocol_note: MD17 test set split
    date: Oct 25, 2025
    date_display: Oct 2025
    date_iso: '2025-10-25'
    published_venue: ''
    published_conference: ''
    at_pub_value: 0.122
    at_pub_std: null
    at_pub_source_arxiv: '2311.02124'
    at_pub_source_title: 'Sliced Denoising: A Physics-Informed Molecular Pre-Training
      Method'
    at_pub_source_date_iso: '2023-11-03'
    at_pub_source_date_label: ICLR 2023
    value_gap_source_date_iso: '2025-10-25'
    value_gap_source_date_label: '2025'
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
    value_gap_source_arxiv: '2510.22123'
    value_gap_source_title: Learning 3D Anisotropic Noise Distributions Improves Molecular
      Force Field Modeling
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.122
    sort_std: null
    global_rank: 87
    paper_rank: 87
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
single_proposed_model: AniDS
main_figure: /figures/2510.22123/main_figure.jpegoptim.jpg
---

