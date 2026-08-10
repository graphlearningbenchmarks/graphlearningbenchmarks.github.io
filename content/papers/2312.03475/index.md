---
title: 'Molecule Joint Auto-Encoding: Trajectory Pretraining with 2D and 3D Diffusion'
arxiv_id: '2312.03475'
source_url: ''
authors:
- name: Weitao Du
  orcid: null
  s2_author_id: '2270356923'
  s2_url: null
- name: Jiujiu Chen
  orcid: null
  s2_author_id: '2155427925'
  s2_url: null
- name: Xuecang Zhang
  orcid: null
  s2_author_id: '2271467311'
  s2_url: null
- name: Zhiming Ma
  orcid: null
  s2_author_id: '2116415767'
  s2_url: null
- name: Shengchao Liu
  orcid: null
  s2_author_id: '2271820535'
  s2_url: null
published_date: Dec 6, 2023
published_date_iso: '2023-12-06'
published_venue: NeurIPS 2023
published_conference: NeurIPS 2023
published_conference_short: NeurIPS
published_conference_slug: neurips
abstract: Recently, artificial intelligence for drug discovery has raised increasing
  interest in both machine learning and chemistry domains. The fundamental building
  block for drug discovery is molecule geometry and thus, the molecule's geometrical
  representation is the main bottleneck to better utilize machine learning techniques
  for drug discovery. In this work, we propose a pretraining method for molecule joint
  auto-encoding (MoleculeJAE). MoleculeJAE can learn both the 2D bond (topology) and
  3D conformation (geometry) information, and a diffusion process model is applied
  to mimic the augmented trajectories of such two modalities, based on which, MoleculeJAE
  will learn the inherent chemical structure in a self-supervised manner. Thus, the
  pretrained geometrical representation in MoleculeJAE is expected to benefit downstream
  geometry-related tasks. Empirically, MoleculeJAE proves its effectiveness by reaching
  state-of-the-art performance on 15 out of 20 tasks by comparing it with 12 competitive
  baselines.
codebase_url: ''
extraction_model: cyankiwi/gemma-4-26B-A4B-it-AWQ-4bit
has_results: true
paper_type: method
proposed_models:
- MoleculeJAE
mrr: 0.0094
adjusted_mrr: 0.0031
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
  - model: GeoSSL-DDM
    model_key: geossl-ddm
    model_plain: GeoSSL-DDM
    value: 0.357
    std: null
    paper_value: 0.357
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.051
    at_pub_std: null
    at_pub_source_arxiv: '2206.13602'
    at_pub_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    at_pub_source_date_iso: '2022-06-27'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-06-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.306
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.051
    true_std: null
    value_gap_source_arxiv: '2206.13602'
    value_gap_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    value_gap_source_is_current_paper: false
    value_gap: 0.306
    has_value_note: false
    value_note: ''
    sort_value: 0.051
    sort_std: null
    global_rank: 50
    paper_rank: 107
    rank_delta: 57
    rank_delta_abs: 57
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    comparison_source_arxiv: '2206.13602'
    is_best: false
    is_std_outlier: false
  - model: GeoSSL-RR
    model_key: geossl-rr
    model_plain: GeoSSL-RR
    value: 0.393
    std: null
    paper_value: 0.393
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.052
    at_pub_std: null
    at_pub_source_arxiv: '2206.13602'
    at_pub_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    at_pub_source_date_iso: '2022-06-27'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-06-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.341
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.052
    true_std: null
    value_gap_source_arxiv: '2206.13602'
    value_gap_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    value_gap_source_is_current_paper: false
    value_gap: 0.341
    has_value_note: false
    value_note: ''
    sort_value: 0.052
    sort_std: null
    global_rank: 57
    paper_rank: 109
    rank_delta: 52
    rank_delta_abs: 52
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    comparison_source_arxiv: '2206.13602'
    is_best: false
    is_std_outlier: false
  - model: GeoSSL-InfoNCE
    model_key: geossl-infonce
    model_plain: GeoSSL-InfoNCE
    value: 0.395
    std: null
    paper_value: 0.395
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.066
    at_pub_std: null
    at_pub_source_arxiv: '2206.13602'
    at_pub_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    at_pub_source_date_iso: '2022-06-27'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-06-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.329
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.066
    true_std: null
    value_gap_source_arxiv: '2206.13602'
    value_gap_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    value_gap_source_is_current_paper: false
    value_gap: 0.329
    has_value_note: false
    value_note: ''
    sort_value: 0.066
    sort_std: null
    global_rank: 65
    paper_rank: 109
    rank_delta: 44
    rank_delta_abs: 44
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    comparison_source_arxiv: '2206.13602'
    is_best: false
    is_std_outlier: false
  - model: GeoSSL-EBM-NCE
    model_key: geossl-ebm-nce
    model_plain: GeoSSL-EBM-NCE
    value: 0.373
    std: null
    paper_value: 0.373
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.073
    at_pub_std: null
    at_pub_source_arxiv: '2206.13602'
    at_pub_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    at_pub_source_date_iso: '2022-06-27'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-06-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.3
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.073
    true_std: null
    value_gap_source_arxiv: '2206.13602'
    value_gap_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    value_gap_source_is_current_paper: false
    value_gap: 0.3
    has_value_note: false
    value_note: ''
    sort_value: 0.073
    sort_std: null
    global_rank: 66
    paper_rank: 107
    rank_delta: 41
    rank_delta_abs: 41
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    comparison_source_arxiv: '2206.13602'
    is_best: false
    is_std_outlier: false
  - model: Distance Prediction
    model_key: distance prediction
    model_plain: Distance Prediction
    value: 0.396
    std: null
    paper_value: 0.396
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.09
    at_pub_std: null
    at_pub_source_arxiv: '2206.13602'
    at_pub_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    at_pub_source_date_iso: '2022-06-27'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-06-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.30600000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.09
    true_std: null
    value_gap_source_arxiv: '2206.13602'
    value_gap_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    value_gap_source_is_current_paper: false
    value_gap: 0.30600000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.09
    sort_std: null
    global_rank: 71
    paper_rank: 109
    rank_delta: 38
    rank_delta_abs: 38
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    comparison_source_arxiv: '2206.13602'
    is_best: false
    is_std_outlier: false
  - model: Angle Prediction
    model_key: angle prediction
    model_plain: Angle Prediction
    value: 0.447
    std: null
    paper_value: 0.447
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.105
    at_pub_std: null
    at_pub_source_arxiv: '2206.13602'
    at_pub_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    at_pub_source_date_iso: '2022-06-27'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-06-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.342
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.105
    true_std: null
    value_gap_source_arxiv: '2206.13602'
    value_gap_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    value_gap_source_is_current_paper: false
    value_gap: 0.342
    has_value_note: false
    value_note: ''
    sort_value: 0.105
    sort_std: null
    global_rank: 78
    paper_rank: 109
    rank_delta: 31
    rank_delta_abs: 31
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    comparison_source_arxiv: '2206.13602'
    is_best: false
    is_std_outlier: false
  - model: 3D InfoGraph
    model_key: 3d infograph
    model_plain: 3D InfoGraph
    value: 0.415
    std: null
    paper_value: 0.415
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.114
    at_pub_std: null
    at_pub_source_arxiv: '2206.13602'
    at_pub_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    at_pub_source_date_iso: '2022-06-27'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-06-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.301
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.114
    true_std: null
    value_gap_source_arxiv: '2206.13602'
    value_gap_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    value_gap_source_is_current_paper: false
    value_gap: 0.301
    has_value_note: false
    value_note: ''
    sort_value: 0.114
    sort_std: null
    global_rank: 82
    paper_rank: 109
    rank_delta: 27
    rank_delta_abs: 27
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    comparison_source_arxiv: '2206.13602'
    is_best: false
    is_std_outlier: false
  - model: GraphMVP
    model_key: graphmvp
    model_plain: GraphMVP
    value: 0.377
    std: null
    paper_value: 0.377
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.1166
    at_pub_std: null
    at_pub_source_arxiv: '2207.08824'
    at_pub_source_title: Energy-Motivated Equivariant Pretraining for 3D Molecular
      Graphs
    at_pub_source_date_iso: '2022-07-18'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-07-18'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.2604
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.1166
    true_std: null
    value_gap_source_arxiv: '2207.08824'
    value_gap_source_title: Energy-Motivated Equivariant Pretraining for 3D Molecular
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.2604
    has_value_note: false
    value_note: ''
    sort_value: 0.1166
    sort_std: null
    global_rank: 83
    paper_rank: 107
    rank_delta: 24
    rank_delta_abs: 24
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Energy-Motivated Equivariant Pretraining for 3D Molecular
      Graphs
    comparison_source_arxiv: '2207.08824'
    is_best: false
    is_std_outlier: false
  - model: 3D Infomax
    model_key: 3d infomax
    model_plain: 3D Infomax
    value: 0.388
    std: null
    paper_value: 0.388
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.1296
    at_pub_std: null
    at_pub_source_arxiv: '2207.08824'
    at_pub_source_title: Energy-Motivated Equivariant Pretraining for 3D Molecular
      Graphs
    at_pub_source_date_iso: '2022-07-18'
    at_pub_source_date_label: AAAI 2022
    value_gap_source_date_iso: '2022-07-18'
    value_gap_source_date_label: AAAI 2022
    gap_vs_at_pub: 0.2584
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.1296
    true_std: null
    value_gap_source_arxiv: '2207.08824'
    value_gap_source_title: Energy-Motivated Equivariant Pretraining for 3D Molecular
      Graphs
    value_gap_source_is_current_paper: false
    value_gap: 0.2584
    has_value_note: false
    value_note: ''
    sort_value: 0.1296
    sort_std: null
    global_rank: 88
    paper_rank: 108
    rank_delta: 20
    rank_delta_abs: 20
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Energy-Motivated Equivariant Pretraining for 3D Molecular
      Graphs
    comparison_source_arxiv: '2207.08824'
    is_best: false
    is_std_outlier: false
  - model: MoleculeJAE
    model_key: moleculejae
    model_plain: MoleculeJAE
    value: 0.345
    std: null
    paper_value: 0.345
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
    uses_external_data: 0
    input_feature_source: null
    feature_source_evidence: ''
    table_ref: Table 1
    source_ref: this paper
    variant_inference_reason: 'dataset: exact match'
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
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
    true_value: 0.345
    true_std: null
    value_gap_source_arxiv: '2405.10343'
    value_gap_source_title: 'UniCorn: A Unified Contrastive Learning Approach for
      Multi-view Molecular Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.345
    sort_std: null
    global_rank: 106
    paper_rank: 106
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: Type Prediction
    model_key: type prediction
    model_plain: Type Prediction
    value: 0.402
    std: null
    paper_value: 0.402
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.349
    at_pub_std: null
    at_pub_source_arxiv: '2206.13602'
    at_pub_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    at_pub_source_date_iso: '2022-06-27'
    at_pub_source_date_label: ICLR 2022
    value_gap_source_date_iso: '2022-06-27'
    value_gap_source_date_label: ICLR 2022
    gap_vs_at_pub: 0.05300000000000005
    worse_than_at_pub: true
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: true
    true_value: 0.349
    true_std: null
    value_gap_source_arxiv: '2206.13602'
    value_gap_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    value_gap_source_is_current_paper: false
    value_gap: 0.05300000000000005
    has_value_note: false
    value_note: ''
    sort_value: 0.349
    sort_std: null
    global_rank: 107
    paper_rank: 109
    rank_delta: 2
    rank_delta_abs: 2
    rank_delta_direction: worse
    has_value_gap: true
    comparison_type: behind
    comparison_source_title: Molecular Geometry Pretraining with SE(3)-Invariant Denoising
      Distance Matching
    comparison_source_arxiv: '2206.13602'
    is_best: false
    is_std_outlier: false
  - model: random init
    model_key: random init
    model_plain: random init
    value: 0.38
    std: null
    paper_value: 0.38
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: 0.38
    at_pub_std: null
    at_pub_source_arxiv: '2305.18407'
    at_pub_source_title: A Group Symmetric Stochastic Differential Equation Model
      for Molecule Multi-modal Pretraining
    at_pub_source_date_iso: '2023-05-28'
    at_pub_source_date_label: ICML 2023
    value_gap_source_date_iso: '2024-05-09'
    value_gap_source_date_label: NeurIPS 2024
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.38
    true_std: null
    value_gap_source_arxiv: '2405.05665'
    value_gap_source_title: 'SubGDiff: A Subgraph Diffusion Model to Improve Molecular
      Representation Learning'
    value_gap_source_is_current_paper: false
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.38
    sort_std: null
    global_rank: 108
    paper_rank: 108
    rank_delta: 0
    rank_delta_abs: 0
    rank_delta_direction: same
    has_value_gap: false
    comparison_type: null
    comparison_source_title: ''
    comparison_source_arxiv: ''
    is_best: false
    is_std_outlier: false
  - model: GeoSSL-DDM-1L
    model_key: geossl-ddm-1l
    model_plain: GeoSSL-DDM-1L
    value: 0.391
    std: null
    paper_value: 0.391
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
    evaluation_task: ''
    protocol_decision: uncertain
    protocol_note: ''
    date: Dec 6, 2023
    date_display: Dec 2023
    date_iso: '2023-12-06'
    published_venue: NeurIPS 2023
    published_conference: NeurIPS 2023
    at_pub_value: null
    at_pub_std: null
    at_pub_source_arxiv: ''
    at_pub_source_title: ''
    at_pub_source_date_iso: ''
    at_pub_source_date_label: ''
    value_gap_source_date_iso: '2023-12-06'
    value_gap_source_date_label: NeurIPS 2023
    gap_vs_at_pub: null
    worse_than_at_pub: false
    surpassed_since_pub: false
    better_than_at_pub: false
    insignificant_improvement_at_pub: false
    improvement_surpassed_since_pub: false
    insignificant_value_gap: false
    today_delta_significant: false
    true_value: 0.391
    true_std: null
    value_gap_source_arxiv: '2312.03475'
    value_gap_source_title: 'Molecule Joint Auto-Encoding: Trajectory Pretraining
      with 2D and 3D Diffusion'
    value_gap_source_is_current_paper: true
    value_gap: null
    has_value_note: false
    value_note: ''
    sort_value: 0.391
    sort_std: null
    global_rank: 109
    paper_rank: 109
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
single_proposed_model: MoleculeJAE
main_figure: /figures/2312.03475/main_figure.jpegoptim.jpg
---

